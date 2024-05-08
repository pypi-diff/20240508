# Comparing `tmp/utilsforecast-0.1.7.tar.gz` & `tmp/utilsforecast-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsforecast-0.1.7.tar", last modified: Mon Apr 22 22:14:50 2024, max compression
+gzip compressed data, was "utilsforecast-0.1.8.tar", last modified: Wed May  8 17:14:52 2024, max compression
```

## Comparing `utilsforecast-0.1.7.tar` & `utilsforecast-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:50.882763 utilsforecast-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-22 22:14:50.882763 utilsforecast-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:14:50.882763 utilsforecast-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:50.878762 utilsforecast-0.1.7/utilsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-22 22:14:46.000000 utilsforecast-0.1.7/utilsforecast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:14:50.882763 utilsforecast-0.1.7/utilsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 22:14:50.000000 utilsforecast-0.1.7/utilsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:52.890080 utilsforecast-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-08 17:14:52.890080 utilsforecast-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:14:52.890080 utilsforecast-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:52.890080 utilsforecast-0.1.8/utilsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28143 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-08 17:14:49.000000 utilsforecast-0.1.8/utilsforecast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:52.890080 utilsforecast-0.1.8/utilsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 17:14:52.000000 utilsforecast-0.1.8/utilsforecast.egg-info/top_level.txt
```

### Comparing `utilsforecast-0.1.7/CONTRIBUTING.md` & `utilsforecast-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/LICENSE` & `utilsforecast-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/PKG-INFO` & `utilsforecast-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.7
+Version: 0.1.8
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: polars; extra == "dev"
 Requires-Dist: numba; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
 Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.7/README.md` & `utilsforecast-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/settings.ini` & `utilsforecast-0.1.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utilsforecast
 lib_name = utilsforecast
-version = 0.1.7
+version = 0.1.8
 min_python = 3.8
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = utilsforecast
 nbs_path = nbs
 recursive = True
```

### Comparing `utilsforecast-0.1.7/setup.py` & `utilsforecast-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/_modidx.py` & `utilsforecast-0.1.8/utilsforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/compat.py` & `utilsforecast-0.1.8/utilsforecast/compat.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/data.py` & `utilsforecast-0.1.8/utilsforecast/data.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/evaluation.py` & `utilsforecast-0.1.8/utilsforecast/evaluation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/feature_engineering.py` & `utilsforecast-0.1.8/utilsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/grouped_array.py` & `utilsforecast-0.1.8/utilsforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/losses.py` & `utilsforecast-0.1.8/utilsforecast/losses.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/plotting.py` & `utilsforecast-0.1.8/utilsforecast/plotting.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/preprocessing.py` & `utilsforecast-0.1.8/utilsforecast/preprocessing.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/processing.py` & `utilsforecast-0.1.8/utilsforecast/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,18 @@
         df = df.select(expr).to_numpy(order="c")
     return df
 
 # %% ../nbs/processing.ipynb 7
 def counts_by_id(df: DataFrame, id_col: str) -> DataFrame:
     if isinstance(df, pd.DataFrame):
         id_counts = df.groupby(id_col, observed=True).size().reset_index()
-        # sort using numpy to prevent pandas from sorting categoricals by their codes
-        # and ensuring a consistent sorting
-        sort_idxs = id_counts[id_col].to_numpy().argsort()
+        ids = id_counts[id_col]
+        if isinstance(ids.dtype, pd.CategoricalDtype):
+            ids = ids.cat.codes
+        sort_idxs = ids.to_numpy().argsort()
         id_counts = id_counts.iloc[sort_idxs].reset_index(drop=True)
     else:
         id_counts = df[id_col].value_counts().sort(id_col)
     id_counts.columns = [id_col, "counts"]
     return id_counts
 
 # %% ../nbs/processing.ipynb 8
@@ -82,26 +83,34 @@
     -------
     numpy array or None
         Array with indices to sort the dataframe or None if it's already sorted.
     """
     ids = df[id_col]
     times = df[time_col]
     if isinstance(df, pd.DataFrame):
+        if isinstance(ids.dtype, pd.CategoricalDtype):
+            # we sort categoricals by their codes, this is also done in counts_by_id
+            ids = ids.cat.codes
         # pandas series alignment makes this slow, cast to numpy
         ids = ids.to_numpy()
         times = times.to_numpy()
     ids_are_sorted = (ids[:-1] <= ids[1:]).all()
-    times_are_sorted = (
-        (times[:-1] < times[1:])  # times are ascending
-        | (ids[:-1] != ids[1:])  # except when the id changes
-    ).all()
-    if ids_are_sorted and times_are_sorted:
-        return None
+    if ids_are_sorted:
+        times_are_sorted = (
+            (times[:-1] < times[1:])  # times are ascending
+            | (ids[:-1] != ids[1:])  # except when the id changes
+        ).all()
+        if times_are_sorted:
+            return None
     if isinstance(df, pd.DataFrame):
-        sort_idxs = np.lexsort((times, ids))
+        if pd.api.types.is_object_dtype(df.dtypes[id_col]):
+            # MultiIndex.argsort is faster than lexsort for strings
+            sort_idxs = pd.MultiIndex.from_frame(df[[id_col, time_col]]).argsort()
+        else:
+            sort_idxs = np.lexsort((times, ids))
     else:
         sort_idxs = (
             df.select(pl.arg_sort_by([id_col, time_col])).to_series(0).to_numpy()
         )
     return sort_idxs
 
 # %% ../nbs/processing.ipynb 9
```

### Comparing `utilsforecast-0.1.7/utilsforecast/target_transforms.py` & `utilsforecast-0.1.8/utilsforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast/validation.py` & `utilsforecast-0.1.8/utilsforecast/validation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.7/utilsforecast.egg-info/PKG-INFO` & `utilsforecast-0.1.8/utilsforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.7
+Version: 0.1.8
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: polars; extra == "dev"
 Requires-Dist: numba; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: polars; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
 Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.7/utilsforecast.egg-info/SOURCES.txt` & `utilsforecast-0.1.8/utilsforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

