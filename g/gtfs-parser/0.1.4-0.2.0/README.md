# Comparing `tmp/gtfs_parser-0.1.4.tar.gz` & `tmp/gtfs_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtfs_parser-0.1.4.tar", max compression
+gzip compressed data, was "gtfs_parser-0.2.0.tar", max compression
```

## Comparing `gtfs_parser-0.1.4.tar` & `gtfs_parser-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1051 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/LICENSE
--rw-r--r--   0        0        0     1143 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/README.md
--rw-r--r--   0        0        0       54 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/__init__.py
--rw-r--r--   0        0        0     4198 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/__main__.py
--rw-r--r--   0        0        0    17228 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/aggregate.py
--rw-r--r--   0        0        0     1178 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/gtfs.py
--rw-r--r--   0        0        0     6135 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/gtfs_parser/parse.py
--rw-r--r--   0        0        0      529 2023-07-04 15:17:51.833881 gtfs_parser-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 gtfs_parser-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1051 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1143 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/README.md
+-rw-r--r--   0        0        0       67 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/gtfs_parser/__init__.py
+-rw-r--r--   0        0        0     3747 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/gtfs_parser/__main__.py
+-rw-r--r--   0        0        0    15464 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/gtfs_parser/aggregate.py
+-rw-r--r--   0        0        0     3780 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/gtfs_parser/gtfs.py
+-rw-r--r--   0        0        0     6046 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/gtfs_parser/parse.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:46:39.801985 gtfs_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 gtfs_parser-0.2.0/PKG-INFO
```

### Comparing `gtfs_parser-0.1.4/LICENSE` & `gtfs_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.4/README.md` & `gtfs_parser-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gtfs_parser-0.1.4/gtfs_parser/__main__.py` & `gtfs_parser-0.2.0/gtfs_parser/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import json
 import os
-import zipfile
-import tempfile
 import argparse
-import shutil
 
-from .gtfs import GTFS
+from .gtfs import GTFSFactory
 from .parse import read_routes, read_stops
 from .aggregate import Aggregator
 
 
 def load_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("mode")
@@ -51,27 +48,15 @@
             raise RuntimeError("begintime is not set.")
 
 
 def main():
     args = load_args()
     validate_args(args)
 
-    if args.src.endswith(".zip"):  # TODO: wiser checking
-        print("extracting zipfile...")
-        temp_dir = os.path.join(tempfile.gettempdir(), "gtfs_parser")
-        if os.path.exists(temp_dir):
-            shutil.rmtree(temp_dir)
-        os.mkdir(temp_dir)
-        with zipfile.ZipFile(args.src) as z:
-            z.extractall(temp_dir)
-        output_dir = temp_dir
-    else:
-        output_dir = args.src
-
-    gtfs = GTFS(output_dir)
+    gtfs = GTFSFactory(args.src)
     print("GTFS loaded.")
 
     os.makedirs(args.dst, exist_ok=True)
 
     if args.mode == "aggregate":
         aggregator = Aggregator(
             gtfs,
```

### Comparing `gtfs_parser-0.1.4/gtfs_parser/aggregate.py` & `gtfs_parser-0.2.0/gtfs_parser/aggregate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,281 +1,240 @@
-from functools import lru_cache
 import datetime
 
 import pandas as pd
 
-
-def latlon_to_str(latlon):
-    return "".join(list(map(lambda coord: str(round(coord, 4)), latlon)))
+from .gtfs import GTFS
 
 
 class Aggregator:
+    """
+    Read stops "interpolated" by parent station or stop_id or stop_name and distance.
+    There are many similar stops that are near to each, has same name, or has same prefix in stop_id.
+    In traffic analyzing, it is good for that similar stops to be grouped as same stop.
+    This method group them by some elements, parent, id, name and distance.
+
+    Args:
+        delimiter (str, optional): stop_id delimiter, sample_A, sample_B, then delimiter is '_'. Defaults to ''.
+        max_distance_degree (float, optional): distance limit in grouping by stop_name. Defaults to 0.003.(approx. 300m)
+
+    Returns:
+        [type]: [description]
+    """
     def __init__(
         self,
-        gtfs: dict,
+        gtfs: GTFS,
         no_unify_stops=False,
         delimiter="",
-        max_distance_degree=0.01,
+        max_distance_degree=0.003,
         yyyymmdd="",
         begin_time="",
         end_time="",
     ):
         self.gtfs = gtfs
-        self.similar_stops_df = None
 
-        self.__aggregate_similar_stops(
-            delimiter,
-            max_distance_degree,
-            no_unify_stops,
-            yyyymmdd=yyyymmdd,
-            begin_time=begin_time,
-            end_time=end_time,
-        )
+        self.stop_times = Aggregator.__filter_stop_times(self.gtfs, yyyymmdd, begin_time, end_time)
 
-    def __aggregate_similar_stops(
-        self,
-        delimiter: str,
-        max_distance_degree: float,
-        no_unify_stops: bool,
-        yyyymmdd="",
-        begin_time="",
-        end_time="",
-    ):
-        """
-        this method occurs side-effect to modify self.gtfs and self.similar_stops_df
-        """
+        if no_unify_stops:
+            similar_results = Aggregator.__get_similar_stop_without_unifying(self.gtfs.stops)
+        else:
+            similar_results = Aggregator.__unify_similar_stops(self.gtfs.stops, delimiter, max_distance_degree)
+        self.similar_stops, self.stop_relations = similar_results
+
+    @staticmethod
+    def __filter_stop_times(gtfs, yyyymmdd, begin_time, end_time):
         # filter stop_times by whether serviced or not
         if yyyymmdd:
-            trips_filtered_by_day = self.__get_trips_on_a_date(yyyymmdd)
-            self.gtfs["stop_times"] = pd.merge(
-                self.gtfs["stop_times"],
-                trips_filtered_by_day,
-                on="trip_id",
-                how="left",
-            )
-            self.gtfs["stop_times"] = self.gtfs["stop_times"][
-                self.gtfs["stop_times"]["service_flag"] == 1
+            trip_ids_filtered_by_day = Aggregator.__get_trips_on_a_date(gtfs, yyyymmdd)
+            filtered_stop_times = gtfs.stop_times[
+                gtfs.stop_times["trip_id"].isin(trip_ids_filtered_by_day)
             ]
-
+        else:
+            filtered_stop_times = gtfs.stop_times.copy()
         # time filter
         if begin_time and end_time:
             # departure_time is nullable and expressed in "hh:mm:ss" or "h:mm:ss" format.
             # Hour can be mor than 24.
             # Therefore, drop null records and convert times to integers.
-            int_dep_times = (
-                self.gtfs["stop_times"].departure_time.str.replace(":", "").astype(int)
-            )
-            self.gtfs["stop_times"] = self.gtfs["stop_times"][
-                self.gtfs["stop_times"].departure_time != ""
-            ][(int_dep_times >= int(begin_time)) & (int_dep_times < int(end_time))]
-
-        if no_unify_stops:
-            # no unifying stops
-            self.gtfs["stops"]["similar_stop_id"] = self.gtfs["stops"]["stop_id"]
-            self.gtfs["stops"]["similar_stop_name"] = self.gtfs["stops"]["stop_name"]
-            self.gtfs["stops"]["similar_stops_centroid"] = self.gtfs["stops"][
-                ["stop_lon", "stop_lat"]
-            ].values.tolist()
-            self.gtfs["stops"]["position_count"] = 1
-            self.similar_stops_df = self.gtfs["stops"][
-                [
-                    "similar_stop_id",
-                    "similar_stop_name",
-                    "similar_stops_centroid",
-                    "position_count",
-                ]
-            ].copy()
+            filtered_stop_times = filtered_stop_times[~filtered_stop_times["departure_time"].isnull()]
+            int_dep_times = filtered_stop_times.departure_time.str.replace(
+                ":", ""
+            ).astype(int)
+            filtered_stop_times = filtered_stop_times[(int_dep_times >= int(begin_time))
+                                                      & (int_dep_times < int(end_time))]
+        return filtered_stop_times
+
+    @staticmethod
+    def __get_similar_stop_without_unifying(stops):
+        if "location_type" in stops:
+            stops = stops[stops["location_type"] == 0]
+        similar_stops_centroid = stops[["stop_lon", "stop_lat"]].values.tolist()
+
+        similar_stops = pd.DataFrame({
+            "similar_stop_id": stops["stop_id"],
+            "similar_stop_name": stops["stop_name"],
+            "similar_stops_centroid": similar_stops_centroid,
+        })
+        similar_relations = pd.concat([
+            stops["stop_id"],
+            similar_stops["similar_stop_id"]
+        ], axis=1)
+        return similar_stops, similar_relations
+
+    @staticmethod
+    def __unify_similar_stops(stops, delimiter, max_distance_degree):
+        child_similar_stop = None
+        child_id_pair = None
+
+        # unify by parent_station
+        if "location_type" in stops.columns:
+            child_similar_stop, child_id_pair = Aggregator.__unify_child_stops(stops)
+
+            solo_stops = stops[
+                ~stops["stop_id"].isin(child_id_pair["stop_id"])
+                & (stops["location_type"] == 0)
+            ]
         else:
-            parent_ids = self.gtfs["stops"]["parent_station"].unique()
-            self.gtfs["stops"]["is_parent"] = self.gtfs["stops"]["stop_id"].map(
-                lambda stop_id: 1 if stop_id in parent_ids else 0
-            )
+            solo_stops = stops
 
-            self.gtfs["stops"][
-                ["similar_stop_id", "similar_stop_name", "similar_stops_centroid"]
-            ] = (
-                self.gtfs["stops"]["stop_id"]
-                .map(
-                    lambda stop_id: self.__get_similar_stop_tuple(
-                        stop_id, delimiter, max_distance_degree
-                    )
-                )
-                .apply(pd.Series)
-            )
-            self.gtfs["stops"]["position_id"] = self.gtfs["stops"][
-                "similar_stops_centroid"
-            ].map(latlon_to_str)
-            self.gtfs["stops"]["unique_id"] = (
-                self.gtfs["stops"]["similar_stop_id"]
-                + self.gtfs["stops"]["position_id"]
-            )
+        # unify solo stops
+        solo_similar_stops, solo_id_pair = Aggregator.__unify_solo_stops(solo_stops, delimiter, max_distance_degree)
 
-            # sometimes stop_name accidently becomes pd.Series instead of str.
-            self.gtfs["stops"]["similar_stop_name"] = self.gtfs["stops"][
-                "similar_stop_name"
-            ].map(lambda val: val if type(val) == str else val.stop_name)
-
-            position_count = (
-                self.gtfs["stop_times"]
-                .merge(self.gtfs["stops"], on="stop_id", how="left")
-                .groupby("position_id")
-                .size()
-                .to_frame()
-                .reset_index()
-            )
-            position_count.columns = ["position_id", "position_count"]
+        # concat similar stops
+        return pd.concat([child_similar_stop, solo_similar_stops]), pd.concat([child_id_pair, solo_id_pair])
 
-            self.similar_stops_df = pd.merge(
-                self.gtfs["stops"].drop_duplicates(subset="position_id")[
-                    [
-                        "position_id",
-                        "similar_stop_id",
-                        "similar_stop_name",
-                        "similar_stops_centroid",
-                    ]
-                ],
-                position_count,
-                on="position_id",
-                how="left",
-            )
+    @staticmethod
+    def __unify_child_stops(stops):
+        child_id_pair = stops[
+            stops["parent_station"].isin(stops["stop_id"])
+            & (stops["location_type"] == 0)
+        ][["stop_id", "parent_station"]]
 
-    @lru_cache(maxsize=None)
-    def __get_similar_stop_tuple(
-        self, stop_id: str, delimiter="", max_distance_degree=0.01
-    ):
-        """
-        With one stop_id, group stops by parent, stop_id, or stop_name and each distance.
-        - parent: if stop has parent_station, the 'centroid' is parent_station lat-lon
-        - stop_id: by delimiter seperate stop_id into prefix and suffix, and group stops having same stop_id-prefix
-        - name and distance: group stops by stop_name, excluding stops are far than max_distance_degree
+        child_id_pair.rename(columns={"parent_station": "similar_stop_id"}, inplace=True)
 
-        Args:
-            stop_id (str): target stop_id
-            max_distance_degree (float, optional): distance limit on grouping, Defaults to 0.01.
-        Returns:
-            str, str, [float, float]: similar_stop_id, similar_stop_name, similar_stops_centroid
-        """
-        stops_df = self.gtfs["stops"].sort_values("stop_id")
-        stop = stops_df[stops_df["stop_id"] == stop_id].iloc[0]
+        similar_ids = child_id_pair["similar_stop_id"].unique()
 
-        if stop["is_parent"] == 1:
-            return (
-                stop["stop_id"],
-                stop["stop_name"],
-                [stop["stop_lon"], stop["stop_lat"]],
-            )
+        similar_stops = stops[stops["stop_id"].isin(similar_ids)][["stop_id", "stop_name", "stop_lon", "stop_lat"]]
 
-        if str(stop["parent_station"]) != "nan":
-            similar_stop_id = stop["parent_station"]
-            similar_stop = stops_df[stops_df["stop_id"] == similar_stop_id]
-            similar_stop_name = similar_stop[["stop_name"]].iloc[0]
-            similar_stop_centroid = (
-                similar_stop[["stop_lon", "stop_lat"]].iloc[0].values.tolist()
-            )
-            return similar_stop_id, similar_stop_name, similar_stop_centroid
+        similar_stops["similar_stops_centroid"] = similar_stops[
+            ["stop_lon", "stop_lat"]
+        ].values.tolist()
+        similar_stops.drop(columns=["stop_lon", "stop_lat"], inplace=True)
+
+        similar_stops.rename(columns={
+            "stop_id": "similar_stop_id",
+            "stop_name": "similar_stop_name",
+        }, inplace=True)
 
+        return similar_stops, child_id_pair
+
+    @staticmethod
+    def __unify_solo_stops(solo_stops, delimiter, max_distance_degree):
+        delimited_id_pair = []
         if delimiter:
-            stops_df_id_delimited = self.__get_stops_id_delimited(delimiter)
-            stop_id_prefix = stop_id.rsplit(delimiter, 1)[0]
-            if stop_id_prefix != stop_id:
-                similar_stop_id = stop_id_prefix
-                seperated_only_stops = stops_df_id_delimited[
-                    stops_df_id_delimited["delimited"]
-                ]
-                similar_stops = seperated_only_stops[
-                    seperated_only_stops["stop_id_prefix"] == stop_id_prefix
-                ][
-                    [
-                        "stop_name",
-                        "similar_stops_centroid_lon",
-                        "similar_stops_centroid_lat",
-                    ]
-                ]
-                similar_stop_name = similar_stops[["stop_name"]].iloc[0]
-                similar_stop_centroid = similar_stops[
-                    ["similar_stops_centroid_lon", "similar_stops_centroid_lat"]
-                ].values.tolist()[0]
-                return similar_stop_id, similar_stop_name, similar_stop_centroid
+            # unify by delimiter
+            stop_id_delimited = solo_stops["stop_id"].str.split(delimiter).str[0].rename("similar_stop_id")
+            delimited_id_pair = pd.concat([solo_stops["stop_id"], stop_id_delimited], axis=1)[
+                solo_stops["stop_id"] != stop_id_delimited
+            ]
+        if len(delimited_id_pair) == len(solo_stops):
+            solo_id_pair = delimited_id_pair
+        else:
+            # unify by distance
+            if len(delimited_id_pair) > 0:
+                undelimited_stops = solo_stops[~solo_stops["stop_id"].isin(delimited_id_pair["stop_id"])]
             else:
-                # when cannot seperate stop_id, grouping by name and distance
-                stops_df = stops_df_id_delimited[~stops_df_id_delimited["delimited"]]
+                undelimited_stops = solo_stops
+            near_id_pair = Aggregator.__calc_near_id_pair(undelimited_stops, max_distance_degree)
 
-        # grouping by name and distance
-        similar_stops = stops_df[stops_df["stop_name"] == stop["stop_name"]][
-            ["stop_id", "stop_name", "stop_lon", "stop_lat"]
-        ]
-        similar_stops = similar_stops.query(
-            f'(stop_lon - {stop["stop_lon"]}) ** 2 + (stop_lat - {stop["stop_lat"]}) ** 2  < {max_distance_degree ** 2}'
-        )
-        similar_stop_centroid = (
-            similar_stops[["stop_lon", "stop_lat"]].mean().values.tolist()
-        )
-        similar_stop_id = similar_stops["stop_id"].iloc[0]
-        similar_stop_name = stop["stop_name"]
-        return similar_stop_id, similar_stop_name, similar_stop_centroid
-
-    @lru_cache(maxsize=None)
-    def __get_stops_id_delimited(self, delimiter: str):
-        stops_df = self.gtfs.get("stops")[
-            ["stop_id", "stop_name", "stop_lon", "stop_lat", "parent_station"]
-        ].copy()
-        stops_df["stop_id_prefix"] = stops_df["stop_id"].map(
-            lambda stop_id: stop_id.rsplit(delimiter, 1)[0]
-        )
-        stops_df["delimited"] = stops_df["stop_id"] != stops_df["stop_id_prefix"]
-        grouped_by_prefix = (
-            stops_df[["stop_id_prefix", "stop_lon", "stop_lat"]]
-            .groupby("stop_id_prefix")
-            .mean()
-            .reset_index()
-        )
-        grouped_by_prefix.columns = [
-            "stop_id_prefix",
-            "similar_stops_centroid_lon",
-            "similar_stops_centroid_lat",
+            if len(delimited_id_pair) == 0:
+                solo_id_pair = near_id_pair
+            else:
+                solo_id_pair = pd.concat([delimited_id_pair, near_id_pair])
+
+        if len(solo_id_pair) == 0:
+            return None, None
+
+        # calc similar stop attributes
+        solo_stops_with_similar = pd.merge(solo_stops, solo_id_pair, on="stop_id")
+        solo_similar_stops = solo_stops_with_similar.groupby("similar_stop_id").agg({
+            'stop_name': 'min',
+            'stop_lon': 'mean',
+            'stop_lat': 'mean'
+        }).reset_index()
+        solo_similar_stops.rename(columns={"stop_name": "similar_stop_name"}, inplace=True)
+        solo_similar_stops["similar_stops_centroid"] = solo_similar_stops[
+            ["stop_lon", "stop_lat"]
+        ].values.tolist()
+        solo_similar_stops.drop(columns=["stop_lon", "stop_lat"], inplace=True)
+        return solo_similar_stops, solo_id_pair
+
+    @staticmethod
+    def __calc_near_id_pair(solo_stops, max_distance_degree):
+        stop_matrix = pd.merge(
+            solo_stops,
+            solo_stops,
+            on="stop_name",
+            suffixes=("", "_r")
+        )
+        near_matrix = stop_matrix[
+            (stop_matrix["stop_lon"] - stop_matrix["stop_lon_r"]) ** 2
+            + (stop_matrix["stop_lat"] - stop_matrix["stop_lat_r"]) ** 2
+            <= max_distance_degree ** 2
         ]
-        stops_df_with_centroid = pd.merge(
-            stops_df, grouped_by_prefix, on="stop_id_prefix", how="left"
-        )
-        return stops_df_with_centroid
 
-    def read_interpolated_stops(self):
-        """
-        Read stops "interpolated" by parent station or stop_id or stop_name and distance.
-        There are many similar stops that are near to each, has same name, or has same prefix in stop_id.
-        In traffic analyzing, it is good for that similar stops to be grouped as same stop.
-        This method group them by some elements, parent, id, name and distance.
+        near_matrix = near_matrix[["stop_id", "stop_id_r"]]
+        # The smallest stop id among the nearest stops is considered as the root id.
+        near_id_pair = near_matrix.groupby("stop_id").min().reset_index()
+
+        near_id_pair = Aggregator.__join_near_group(near_id_pair)
+        return near_id_pair.rename(columns={"stop_id_r": "similar_stop_id"})
+
+    """
+    Join near groups of stops.
+    Trace root stops up to 5 times and modify root id.
+    """
+    @staticmethod
+    def __join_near_group(near_id_pair):
+        for i in range(5):
+            leaf_pair = near_id_pair.query("stop_id != stop_id_r")\
+                .rename(columns={"stop_id": "stop_id_r", "stop_id_r": "stop_id_r2"})
+            sub_pair = pd.merge(near_id_pair, leaf_pair, on="stop_id_r").drop(columns=["stop_id_r"])
+            if len(sub_pair) == 0:
+                break
+            mod_id_trio = pd.merge(near_id_pair, sub_pair, on="stop_id", how="left")
+            mod_id_trio.loc[~mod_id_trio['stop_id_r2'].isna(), 'stop_id_r'] = mod_id_trio['stop_id_r2']
+            near_id_pair = mod_id_trio.drop(columns=["stop_id_r2"])
 
-        Args:
-            delimiter (str, optional): stop_id delimiter, sample_A, sample_B, then delimiter is '_'. Defaults to ''.
-            max_distance_degree (float, optional): distance limit in grouping by stop_name. Defaults to 0.01.
+        return near_id_pair
 
-        Returns:
-            [type]: [description]
-        """
+    def read_interpolated_stops(self):
+        stop_pass_count = self.stop_times.groupby("stop_id").size().rename("count")
+        stop_pass_count = pd.merge(
+            self.stop_relations,
+            stop_pass_count,
+            on="stop_id",
+            how="left"
+        )
+        similar_pass_count = stop_pass_count.groupby("similar_stop_id").sum("count").astype(int)
+        similar_stop_summary = self.similar_stops.merge(similar_pass_count,
+                                                        on="similar_stop_id")
+
+        stop_dicts = similar_stop_summary.to_dict(orient="records")
 
-        stop_dicts = self.similar_stops_df[
-            [
-                "similar_stop_id",
-                "similar_stop_name",
-                "similar_stops_centroid",
-                "position_count",
-            ]
-        ].to_dict(orient="records")
         return [
             {
                 "type": "Feature",
                 "geometry": {
                     "type": "Point",
                     "coordinates": stop["similar_stops_centroid"],
                 },
                 "properties": {
                     "similar_stop_name": stop["similar_stop_name"],
                     "similar_stop_id": stop["similar_stop_id"],
-                    "count": stop["position_count"],
+                    "count": stop["count"],
                 },
             }
             for stop in stop_dicts
         ]
 
     def read_route_frequency(self):
         """
@@ -286,121 +245,90 @@
             yyyymmdd (str, optional): date, like 20210401. Defaults to ''.
             begin_time (str, optional): 'hhmmss' <= departure time, like 030000. Defaults to ''.
             end_time (str, optional): 'hhmmss' > departure time, like 280000. Defaults to ''.
 
         Returns:
             [type]: [description]
         """
-        stop_times_df = (
-            self.gtfs.get("stop_times")[
-                ["stop_id", "trip_id", "stop_sequence", "departure_time"]
-            ]
-            .sort_values(["trip_id", "stop_sequence"])
-            .copy()
-        )
-
-        # join agency info)
+        #
         stop_times_df = pd.merge(
-            stop_times_df,
-            self.gtfs["trips"][["trip_id", "route_id"]],
-            on="trip_id",
-            how="left",
+            self.stop_times[["trip_id", "stop_sequence", "stop_id"]],
+            self.stop_relations,
+            on="stop_id"
+        )
+        # append agency_id
+        trip_agency_df = pd.merge(
+            self.gtfs.trips[["trip_id", "route_id"]],
+            self.gtfs.routes[["route_id", "agency_id"]],
+            on="route_id"
         )
         stop_times_df = pd.merge(
             stop_times_df,
-            self.gtfs["routes"][["route_id", "agency_id"]],
-            on="route_id",
-            how="left",
-        )
-        stop_times_df = pd.merge(
-            stop_times_df,
-            self.gtfs["agency"][["agency_id", "agency_name"]],
-            on="agency_id",
-            how="left",
+            trip_agency_df,
+            on="trip_id"
         )
+        stop_times_df = stop_times_df.sort_values(["trip_id", "stop_sequence"])
 
-        # get prev and next stops_id, stop_name, trip_id
-        stop_times_df = pd.merge(
-            stop_times_df,
-            self.gtfs["stops"][
-                [
-                    "stop_id",
-                    "similar_stop_id",
-                    "similar_stop_name",
-                    "similar_stops_centroid",
-                ]
-            ],
-            on="stop_id",
-            how="left",
-        )
-        stop_times_df["prev_stop_id"] = stop_times_df["similar_stop_id"]
-        stop_times_df["prev_trip_id"] = stop_times_df["trip_id"]
-        stop_times_df["prev_stop_name"] = stop_times_df["similar_stop_name"]
-        stop_times_df["prev_similar_stops_centroid"] = stop_times_df[
-            "similar_stops_centroid"
-        ]
+        # generate path by joining next stop_times
         stop_times_df["next_stop_id"] = stop_times_df["similar_stop_id"].shift(-1)
         stop_times_df["next_trip_id"] = stop_times_df["trip_id"].shift(-1)
-        stop_times_df["next_stop_name"] = stop_times_df["similar_stop_name"].shift(-1)
-        stop_times_df["next_similar_stops_centroid"] = stop_times_df[
-            "similar_stops_centroid"
-        ].shift(-1)
-
-        # drop last stops (-> stops has no next stop)
-        stop_times_df = stop_times_df.drop(
-            index=stop_times_df.query("prev_trip_id != next_trip_id").index
-        )
+        stop_times_df = stop_times_df[stop_times_df["trip_id"] == stop_times_df["next_trip_id"]]
+        path_df = stop_times_df.rename(columns={"similar_stop_id": "prev_stop_id"})
 
-        # define path_id by prev-stops-centroid and next-stops-centroid
-        stop_times_df["path_id"] = (
-            stop_times_df["prev_stop_id"]
-            + stop_times_df["next_stop_id"]
-            + stop_times_df["prev_similar_stops_centroid"].map(latlon_to_str)
-            + stop_times_df["next_similar_stops_centroid"].map(latlon_to_str)
-        )
-
-        # aggregate path-frequency
-        path_frequency = (
-            stop_times_df[["similar_stop_id", "path_id"]]
-            .groupby("path_id")
-            .count()
-            .reset_index()
-        )
-        path_frequency.columns = ["path_id", "path_count"]
-        path_data = pd.merge(
-            path_frequency,
-            stop_times_df.drop_duplicates(subset="path_id"),
-            on="path_id",
+        # count frequency
+        path_freq_sr = path_df.groupby(["agency_id", "prev_stop_id", "next_stop_id"]).size()
+        path_freq_sr.name = "frequency"
+        path_freq_df = path_freq_sr.reset_index()
+
+        # append path attributes
+        for order in ["prev", "next"]:
+            path_freq_df = pd.merge(
+                path_freq_df,
+                self.similar_stops,
+                left_on=f"{order}_stop_id",
+                right_on="similar_stop_id"
+            )
+            path_freq_df.rename(columns={
+                "similar_stop_name": f"{order}_stop_name",
+                "similar_stops_centroid": f"{order}_similar_stops_centroid"
+            }, inplace=True)
+            path_freq_df.drop(columns="similar_stop_id", inplace=True)
+
+        path_freq_df = pd.merge(
+            path_freq_df,
+            self.gtfs.agency[["agency_id", "agency_name"]],
+            on="agency_id"
         )
-        path_data_dict = path_data.to_dict(orient="records")
-
+        # convert to features
+        path_freq_dict = path_freq_df.to_dict(orient="records")
         return [
             {
                 "type": "Feature",
                 "geometry": {
                     "type": "LineString",
                     "coordinates": (
                         path["prev_similar_stops_centroid"],
                         path["next_similar_stops_centroid"],
                     ),
                 },
                 "properties": {
-                    "frequency": path["path_count"],
+                    "frequency": path["frequency"],
                     "prev_stop_id": path["prev_stop_id"],
                     "prev_stop_name": path["prev_stop_name"],
                     "next_stop_id": path["next_stop_id"],
                     "next_stop_name": path["next_stop_name"],
                     "agency_id": path["agency_id"],
                     "agency_name": path["agency_name"],
                 },
             }
-            for path in path_data_dict
+            for path in path_freq_dict
         ]
-
-    def __get_trips_on_a_date(self, yyyymmdd: str):
+    
+    @staticmethod
+    def __get_trips_on_a_date(gtfs, yyyymmdd: str):
         """
         get trips are on service on a date.
 
         Args:
             yyyymmdd (str): [description]
 
         Returns:
@@ -409,44 +337,62 @@
         # sunday, monday, tuesday...
         day_of_week = (
             datetime.date(int(yyyymmdd[0:4]), int(yyyymmdd[4:6]), int(yyyymmdd[6:8]))
             .strftime("%A")
             .lower()
         )
 
-        # filter services by day
-        calendar_df = self.gtfs["calendar"].copy()
-        calendar_df = calendar_df.astype({"start_date": int, "end_date": int})
-        calendar_df = calendar_df[calendar_df[day_of_week] == "1"]
-        calendar_df = calendar_df.query(
-            f"start_date <= {int(yyyymmdd)} and {int(yyyymmdd)} <= end_date",
-            engine="python",
-        )
-
-        services_on_a_day = calendar_df[["service_id"]]
+        # filter services by calendar
+        if gtfs.calendar is None:
+            # generate an empty series if calendar.txt is missing because it is not required.
+            service_ids_on = pd.Series(name="service_id", dtype=str)
+        else:
+            calendar = gtfs.calendar.astype(
+                {"start_date": int, "end_date": int}
+            )
+            calendar = calendar[
+                calendar[day_of_week] == "1"
+            ]
+            calendar = calendar.query(
+                f"start_date <= {int(yyyymmdd)} and {int(yyyymmdd)} <= end_date",
+                engine="python",
+            )
+            service_ids_on = calendar["service_id"]
 
-        calendar_dates_df = self.gtfs.get("calendar_dates")
-        if calendar_dates_df is not None:
-            filtered = calendar_dates_df[calendar_dates_df["date"] == yyyymmdd][
-                ["service_id", "exception_type"]
+        # filter services by dates
+        if gtfs.calendar_dates is not None:
+            filtered = gtfs.calendar_dates[
+                gtfs.calendar_dates["date"] == yyyymmdd
+            ][["service_id", "exception_type"]]
+            to_be_removed_service_ids = filtered[filtered["exception_type"] == "2"][
+                "service_id"
             ]
-            to_be_removed_services = filtered[filtered["exception_type"] == "2"]
-            to_be_appended_services = filtered[filtered["exception_type"] == "1"][
-                ["service_id"]
+            to_be_appended_services_ids = filtered[filtered["exception_type"] == "1"][
+                "service_id"
             ]
 
-            services_on_a_day = pd.merge(
-                services_on_a_day, to_be_removed_services, on="service_id", how="left"
-            )
-            services_on_a_day = services_on_a_day[
-                services_on_a_day["exception_type"] != "2"
+            service_ids_on = service_ids_on[
+                ~service_ids_on.isin(to_be_removed_service_ids)
             ]
-            services_on_a_day = pd.concat([services_on_a_day, to_be_appended_services])
-
-        services_on_a_day["service_flag"] = 1
+            service_ids_on = pd.concat([service_ids_on, to_be_appended_services_ids])
 
         # filter trips
-        trips_df = self.gtfs["trips"].copy()
-        trip_service = pd.merge(trips_df, services_on_a_day, on="service_id")
-        trip_service = trip_service[trip_service["service_flag"] == 1]
+        trips_in_services = gtfs.trips[
+            gtfs.trips["service_id"].isin(service_ids_on)
+        ]
+
+        return trips_in_services["trip_id"]
 
-        return trip_service[["trip_id", "service_flag"]]
+    def read_stop_relations(self) -> list:
+        stop_relation_df = pd.merge(
+            self.stop_relations,
+            self.gtfs.stops[["stop_id", "stop_name"]],
+            on="stop_id"
+        )
+        stop_relation_df = pd.merge(
+            stop_relation_df,
+            self.similar_stops,
+            on="similar_stop_id",
+        )
+        stop_relation_df = stop_relation_df.reindex(columns=["stop_id", "stop_name",
+                                                             "similar_stop_id", "similar_stop_name"])
+        return stop_relation_df.to_dict(orient="records")
```

### Comparing `gtfs_parser-0.1.4/pyproject.toml` & `gtfs_parser-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "gtfs_parser"
-version = "0.1.4"
+version = "0.2.0"
 description = "parse and aggregate GTFS"
 authors = ["MIERUNE Inc.", "Kanahiro IGUCHI"]
 license = "MIT"
 homepage = "https://github.com/MIERUNE"
-repository = "https://github.com/MIERUNE/{project-name}"
+repository = "https://github.com/MIERUNE/gtfs-parser"
 readme = "README.md"
 packages = [{include = "gtfs_parser"}]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1"
+python = "3.9.*"
 pandas = ">=1.3.3"
 
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 gtfs-parser = "gtfs_parser.__main__:main"
```

### Comparing `gtfs_parser-0.1.4/PKG-INFO` & `gtfs_parser-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
-Name: gtfs-parser
-Version: 0.1.4
+Name: gtfs_parser
+Version: 0.2.0
 Summary: parse and aggregate GTFS
 Home-page: https://github.com/MIERUNE
 License: MIT
 Author: MIERUNE Inc.
-Requires-Python: >=3.7.1
+Requires-Python: ==3.9.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1.3.3)
-Project-URL: Repository, https://github.com/MIERUNE/{project-name}
+Project-URL: Repository, https://github.com/MIERUNE/gtfs-parser
 Description-Content-Type: text/markdown
 
 # gtfs_parser
 
 ## LICENSE
 
 MIT License
```

