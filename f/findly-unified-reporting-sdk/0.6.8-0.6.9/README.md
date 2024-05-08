# Comparing `tmp/findly_unified_reporting_sdk-0.6.8.tar.gz` & `tmp/findly_unified_reporting_sdk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findly_unified_reporting_sdk-0.6.8.tar", max compression
+gzip compressed data, was "findly_unified_reporting_sdk-0.6.9.tar", max compression
```

## Comparing `findly_unified_reporting_sdk-0.6.8.tar` & `findly_unified_reporting_sdk-0.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.8/LICENSE
--rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.8/README.md
--rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.8/findly/__init__.py
--rw-r--r--   0        0        0      342 2024-04-25 14:35:17.466011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/__init__.py
--rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/common_parser.py
--rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
--rw-r--r--   0        0        0     3647 2024-04-25 14:35:17.494011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/reports_client.py
--rw-r--r--   0        0        0     5671 2024-04-25 14:35:17.526011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
--rw-r--r--   0        0        0    20517 2024-04-25 14:29:11.890413 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
--rw-r--r--   0        0        0    30965 2024-04-25 14:29:43.918010 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
--rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
--rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
--rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
--rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
--rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
--rw-r--r--   0        0        0    38179 2024-04-25 14:29:11.890413 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
--rw-r--r--   0        0        0    30064 2024-04-25 14:35:17.658009 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
--rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
--rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
--rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/.gitignore
--rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/__init__.py
--rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
--rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
--rw-r--r--   0        0        0     2915 2024-04-25 14:35:17.490011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/urs.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/util/__init__.py
--rw-r--r--   0        0        0      457 2024-04-25 14:35:17.470011 findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/util/create_numeric_string_series.py
--rw-r--r--   0        0        0     1237 2024-04-25 14:32:46.123787 findly_unified_reporting_sdk-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 19:37:41.412820 findly_unified_reporting_sdk-0.6.9/LICENSE
+-rw-r--r--   0        0        0     2182 2024-04-02 19:37:41.412956 findly_unified_reporting_sdk-0.6.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.413191 findly_unified_reporting_sdk-0.6.9/findly/__init__.py
+-rw-r--r--   0        0        0      342 2024-05-08 15:01:52.878122 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.413425 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.413525 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/__init__.py
+-rw-r--r--   0        0        0     7897 2024-04-02 19:37:41.413652 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/common_parser.py
+-rw-r--r--   0        0        0      971 2024-04-02 19:37:41.413724 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
+-rw-r--r--   0        0        0     3647 2024-05-08 15:01:52.878346 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/reports_client.py
+-rw-r--r--   0        0        0     5671 2024-05-08 15:01:52.878672 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.413992 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
+-rw-r--r--   0        0        0    20517 2024-05-08 15:01:52.879200 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
+-rw-r--r--   0        0        0    32194 2024-05-08 15:18:10.912238 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
+-rw-r--r--   0        0        0     1492 2024-04-02 19:37:41.414407 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
+-rw-r--r--   0        0        0     5778 2024-04-02 19:37:41.414507 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
+-rw-r--r--   0        0        0    16489 2024-04-02 19:37:41.414627 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0    17708 2024-04-02 19:37:41.414762 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
+-rw-r--r--   0        0        0    20146 2024-04-02 19:37:41.414903 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.415259 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
+-rw-r--r--   0        0        0    38179 2024-05-08 15:01:52.880455 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
+-rw-r--r--   0        0        0    30064 2024-05-08 15:01:52.880996 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
+-rw-r--r--   0        0        0    33511 2024-04-02 19:37:41.415779 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.415875 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.415931 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
+-rw-r--r--   0        0        0     1038 2024-04-02 19:37:41.416183 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
+-rw-r--r--   0        0        0       27 2024-04-02 19:37:41.416316 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/.gitignore
+-rw-r--r--   0        0        0      137 2024-04-02 19:37:41.416398 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/__init__.py
+-rw-r--r--   0        0        0     6568 2024-04-02 20:07:23.839442 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
+-rw-r--r--   0        0        0    29515 2024-04-02 20:07:23.839558 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
+-rw-r--r--   0        0        0     2915 2024-05-08 15:01:52.881208 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/urs.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:37:41.416537 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/util/__init__.py
+-rw-r--r--   0        0        0      457 2024-05-08 15:01:52.881385 findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/util/create_numeric_string_series.py
+-rw-r--r--   0        0        0     1237 2024-05-08 15:02:30.438538 findly_unified_reporting_sdk-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.9/PKG-INFO
```

### Comparing `findly_unified_reporting_sdk-0.6.8/LICENSE` & `findly_unified_reporting_sdk-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/README.md` & `findly_unified_reporting_sdk-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/common_parser.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/common_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/reports_client.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/reports_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,29 @@
                     # action breakdowns won't show as they are nested in the response
                     # But we should check them later if they are really nested
                     if "action" in col:
                         missing_action.append(col)
                     else:
                         df[col] = np.nan
 
+            # if more than the expected columns are in the response, remove them
+            # this happens when we only send breakdowns in the query
+            for col in column_names_list:
+                if col not in expected_columns and col not in [
+                    START_DATE_COLUMN_NAME,
+                    END_DATE_COLUMN_NAME,
+                ]:
+                    LOGGER.info(
+                        {
+                            "msg": "removing_unexpected_column",
+                            "column": col,
+                        }
+                    )
+                    df.drop(columns=[col], inplace=True)
+
             # Now, Check if any of the metrics is of type METRIC_VALUE_TYPE_LIST_ADS_ACTION_STATS
             # If so, we want to explode the values of that column
             try:
                 all_metrics_list = self.parse_metrics()
             except Exception as e:
                 LOGGER.error(
                     {
@@ -427,14 +442,29 @@
         # If any metric is missing, fill it with NaN
         missing_metrics = [
             metric for metric in metrics_headers if metric not in summary_df.columns
         ]
         for missing_metric in missing_metrics:
             summary_df[missing_metric] = np.nan
 
+        # if more than the expected columns are in the response, remove them
+        # this happens when we only send breakdowns in the query
+        for col in summary_df.columns.tolist():
+            if col not in metrics_headers and col not in [
+                START_DATE_COLUMN_NAME,
+                END_DATE_COLUMN_NAME,
+            ]:
+                LOGGER.info(
+                    {
+                        "msg": "removing_unexpected_column",
+                        "column": col,
+                    }
+                )
+                summary_df.drop(columns=[col], inplace=True)
+
         try:
             all_metrics_list = self.parse_metrics()
         except Exception as e:
             LOGGER.error(
                 {
                     "msg": "error_parsing_metrics",
                     "error": str(e),
```

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: findly_semantic_layer.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66indly_semantic_layer.proto\x12\x15\x66indly_semantic_layer\"\x8c\x02\n\tDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x03 \x01(\t\x12\x32\n\x04type\x18\x04 \x01(\x0e\x32$.findly_semantic_layer.DimensionType\x12?\n\x0btype_params\x18\x05 \x01(\x0b\x32*.findly_semantic_layer.DimensionTypeParams\x12\x14\n\x0ctop_n_values\x18\x06 \x03(\t\x12\x12\n\nvalue_type\x18\x07 \x01(\t\x12\x19\n\x11\x64\x61ta_source_names\x18\x08 \x03(\t\x12\x14\n\x0c\x64isplay_name\x18\t \x01(\t\"k\n\x13\x44imensionTypeParams\x12@\n\x10time_granularity\x18\x01 \x01(\x0e\x32&.findly_semantic_layer.DateGranularity\x12\x12\n\nis_primary\x18\x02 \x01(\x08\"\x8b\x03\n\x06Metric\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x12\n\nexpression\x18\x04 \x01(\t\x12\x18\n\x10view_id_of_table\x18\x05 \x01(\t\x12\x12\n\ntable_name\x18\x06 \x01(\t\x12\x10\n\x08measures\x18\x07 \x03(\t\x12\x11\n\tnumerator\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65nominator\x18\t \x01(\t\x12/\n\x04type\x18\n \x01(\x0e\x32!.findly_semantic_layer.MetricType\x12\x10\n\x06window\x18\x0b \x01(\tH\x00\x12\x17\n\rgrain_to_date\x18\x0c \x01(\tH\x00\x12:\n\nvalue_type\x18\r \x01(\x0e\x32&.findly_semantic_layer.MetricValueType\x12\x14\n\x0c\x64isplay_name\x18\x0e \x01(\t\x12\x12\n\nis_numeric\x18\x0f \x01(\x08\x42\x14\n\x12\x63umulative_process\"4\n\x0c\x44\x61teStrRange\x12\x12\n\nstart_date\x18\x01 \x01(\t\x12\x10\n\x08\x65nd_date\x18\x02 \x01(\t\"\xf4\x02\n\tQueryArgs\x12\x14\n\x0cwhere_clause\x18\x01 \x01(\t\x12\x18\n\x10group_by_columns\x18\x02 \x03(\t\x12\x1a\n\x12metrics_expression\x18\x03 \x03(\t\x12\r\n\x05limit\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x03(\t\x12\x19\n\x11\x64\x61te_where_clause\x18\x06 \x01(\t\x12\x0f\n\x07metrics\x18\x07 \x03(\t\x12\x15\n\rhaving_clause\x18\x08 \x01(\t\x12\x1c\n\x14incompatible_metrics\x18\t \x03(\t\x12\x1f\n\x17incompatible_dimensions\x18\n \x03(\t\x12\x38\n\x0b\x64\x61te_ranges\x18\x0b \x03(\x0b\x32#.findly_semantic_layer.DateStrRange\x12\x17\n\x0fsql_explanation\x18\x0c \x01(\t\x12\r\n\x05level\x18\r \x01(\t\x12\x16\n\x0etime_increment\x18\x0e \x01(\t\"\x80\x01\n\x12\x44\x61tasourceMetadata\x12>\n\x08location\x18\x01 \x01(\x0e\x32,.findly_semantic_layer.DataSourceIntegration\x12\x13\n\x0bproperty_id\x18\x02 \x01(\t\x12\x15\n\rproperty_name\x18\x03 \x01(\t*b\n\x15\x44\x61taSourceIntegration\x12 \n\x1c\x44\x41TA_SOURCE_LOCATION_UNKNOWN\x10\x00\x12\x12\n\x0eSEMANTIC_LAYER\x10\x01\x12\x07\n\x03GA4\x10\x02\x12\n\n\x06\x46\x42_ADS\x10\x03*S\n\x0f\x44\x61teGranularity\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x01\x12\x08\n\x04WEEK\x10\x02\x12\t\n\x05MONTH\x10\x03\x12\x0b\n\x07QUARTER\x10\x04\x12\x08\n\x04YEAR\x10\x05*\x7f\n\x0b\x41ggregation\x12\x17\n\x13\x41GGREGATION_UNKNOWN\x10\x00\x12\x07\n\x03SUM\x10\x01\x12\x0f\n\x0bSUM_BOOLEAN\x10\x02\x12\x12\n\x0e\x43OUNT_DISTINCT\x10\x03\x12\x07\n\x03MIN\x10\x04\x12\x07\n\x03MAX\x10\x05\x12\x0b\n\x07\x41VERAGE\x10\x06\x12\n\n\x06MEDIAN\x10\x07*\xab\x01\n\rDimensionType\x12\x15\n\x11\x44IMENSION_UNKNOWN\x10\x00\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x01\x12\x08\n\x04TIME\x10\x02\x12\x10\n\x0c\x46\x42_ADS_FIELD\x10\x03\x12\x14\n\x10\x46\x42_ADS_BREAKDOWN\x10\x04\x12\x1b\n\x17\x46\x42_ADS_ACTION_BREAKDOWN\x10\x05\x12#\n\x1f\x46\x42_ADS_SUMMARY_ACTION_BREAKDOWN\x10\x06*o\n\nMetricType\x12\x12\n\x0eMETRIC_UNKNOWN\x10\x00\x12\x11\n\rMEASURE_PROXY\x10\x01\x12\x0e\n\nCUMULATIVE\x10\x02\x12\t\n\x05RATIO\x10\x03\x12\x0b\n\x07\x44\x45RIVED\x10\x04\x12\x12\n\x0eSQL_EXPRESSION\x10\x05*\xf9\x04\n\x0fMetricValueType\x12\x1d\n\x19METRIC_VALUE_TYPE_UNKNOWN\x10\x00\x12\x1d\n\x19METRIC_VALUE_TYPE_INTEGER\x10\x01\x12\x1b\n\x17METRIC_VALUE_TYPE_FLOAT\x10\x02\x12\x1d\n\x19METRIC_VALUE_TYPE_SECONDS\x10\x03\x12\"\n\x1eMETRIC_VALUE_TYPE_MILLISECONDS\x10\x04\x12\x1d\n\x19METRIC_VALUE_TYPE_MINUTES\x10\x05\x12\x1b\n\x17METRIC_VALUE_TYPE_HOURS\x10\x06\x12\x1e\n\x1aMETRIC_VALUE_TYPE_STANDARD\x10\x07\x12\x1e\n\x1aMETRIC_VALUE_TYPE_CURRENCY\x10\x08\x12\x1a\n\x16METRIC_VALUE_TYPE_FEET\x10\t\x12\x1b\n\x17METRIC_VALUE_TYPE_MILES\x10\n\x12\x1c\n\x18METRIC_VALUE_TYPE_METERS\x10\x0b\x12 \n\x1cMETRIC_VALUE_TYPE_KILOMETERS\x10\x0c\x12\x1c\n\x18METRIC_VALUE_TYPE_STRING\x10\r\x12$\n METRIC_VALUE_TYPE_NUMERIC_STRING\x10\x0e\x12+\n\'METRIC_VALUE_TYPE_LIST_ADS_ACTION_STATS\x10\x0f\x12\x32\n.METRIC_VALUE_TYPE_LIST_ADS_INSIGHTS_DDA_RESULT\x10\x10\x12.\n*METRIC_VALUE_TYPE_LIST_ADS_HISTOGRAM_STATS\x10\x11\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'findly_semantic_layer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_DATASOURCEINTEGRATION']._serialized_start=1392
   _globals['_DATASOURCEINTEGRATION']._serialized_end=1490
   _globals['_DATEGRANULARITY']._serialized_start=1492
   _globals['_DATEGRANULARITY']._serialized_end=1575
   _globals['_AGGREGATION']._serialized_start=1577
   _globals['_AGGREGATION']._serialized_end=1704
```

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/findly/unified_reporting_sdk/urs.py` & `findly_unified_reporting_sdk-0.6.9/findly/unified_reporting_sdk/urs.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.8/pyproject.toml` & `findly_unified_reporting_sdk-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findly.unified-reporting-sdk"
-version = "0.6.8"
+version = "0.6.9"
 license = "GPL-3.0-only"
 description = ""
 authors = []
 readme = "README.md"
 packages = [
     { include = "findly" },
 ]
```

### Comparing `findly_unified_reporting_sdk-0.6.8/PKG-INFO` & `findly_unified_reporting_sdk-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findly-unified-reporting-sdk
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

