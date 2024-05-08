# Comparing `tmp/hxm_refuel-0.2.7.tar.gz` & `tmp/hxm_refuel-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hxm_refuel-0.2.7.tar", max compression
+gzip compressed data, was "hxm_refuel-0.2.8.tar", max compression
```

## Comparing `hxm_refuel-0.2.7.tar` & `hxm_refuel-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-12-01 11:06:34.970622 hxm_refuel-0.2.7/hxm_refuel/__init__.py
--rw-r--r--   0        0        0      105 2023-09-24 14:23:26.541224 hxm_refuel-0.2.7/hxm_refuel/bloomberg/__init__.py
--rw-r--r--   0        0        0    14713 2024-02-28 12:16:07.522424 hxm_refuel-0.2.7/hxm_refuel/bloomberg/bloomberg_api.py
--rw-r--r--   0        0        0     2910 2023-09-24 12:17:44.083265 hxm_refuel-0.2.7/hxm_refuel/bloomberg/bloomberg_recipies.py
--rw-r--r--   0        0        0     5958 2024-02-28 12:48:30.731267 hxm_refuel-0.2.7/hxm_refuel/jeeves.py
--rw-r--r--   0        0        0      148 2024-02-09 07:15:41.900434 hxm_refuel-0.2.7/hxm_refuel/snowflake/__init__.py
--rw-r--r--   0        0        0     4389 2023-11-16 09:53:55.341194 hxm_refuel-0.2.7/hxm_refuel/snowflake/connector.py
--rw-r--r--   0        0        0     1431 2024-02-09 07:24:40.724467 hxm_refuel-0.2.7/hxm_refuel/snowflake/snowflake_recipes.py
--rw-r--r--   0        0        0     6627 2023-11-20 18:51:50.473891 hxm_refuel-0.2.7/hxm_refuel/snowflake/sql_recipes.py
--rw-r--r--   0        0        0     6649 2023-02-08 07:39:46.066344 hxm_refuel-0.2.7/hxm_refuel/validation.py
--rw-r--r--   0        0        0     1085 2023-09-24 11:04:20.427375 hxm_refuel-0.2.7/LICENSE
--rw-r--r--   0        0        0      860 2024-02-28 12:48:39.205681 hxm_refuel-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4021 2023-11-16 10:18:45.692284 hxm_refuel-0.2.7/README.md
--rw-r--r--   0        0        0     4582 1970-01-01 00:00:00.000000 hxm_refuel-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 11:06:34.970622 hxm_refuel-0.2.8/hxm_refuel/__init__.py
+-rw-r--r--   0        0        0      105 2023-09-24 14:23:26.541224 hxm_refuel-0.2.8/hxm_refuel/bloomberg/__init__.py
+-rw-r--r--   0        0        0    14912 2024-03-19 17:19:40.062775 hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_api.py
+-rw-r--r--   0        0        0     2910 2023-09-24 12:17:44.083265 hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_recipies.py
+-rw-r--r--   0        0        0     5958 2024-02-28 12:48:30.731267 hxm_refuel-0.2.8/hxm_refuel/jeeves.py
+-rw-r--r--   0        0        0      148 2024-02-09 07:15:41.900434 hxm_refuel-0.2.8/hxm_refuel/snowflake/__init__.py
+-rw-r--r--   0        0        0     4389 2023-11-16 09:53:55.341194 hxm_refuel-0.2.8/hxm_refuel/snowflake/connector.py
+-rw-r--r--   0        0        0     1431 2024-02-09 07:24:40.724467 hxm_refuel-0.2.8/hxm_refuel/snowflake/snowflake_recipes.py
+-rw-r--r--   0        0        0     6627 2023-11-20 18:51:50.473891 hxm_refuel-0.2.8/hxm_refuel/snowflake/sql_recipes.py
+-rw-r--r--   0        0        0     6649 2023-02-08 07:39:46.066344 hxm_refuel-0.2.8/hxm_refuel/validation.py
+-rw-r--r--   0        0        0     1085 2023-09-24 11:04:20.427375 hxm_refuel-0.2.8/LICENSE
+-rw-r--r--   0        0        0      766 2024-05-08 15:58:18.041334 hxm_refuel-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4021 2023-11-16 10:18:45.692284 hxm_refuel-0.2.8/README.md
+-rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 hxm_refuel-0.2.8/PKG-INFO
```

### Comparing `hxm_refuel-0.2.7/hxm_refuel/bloomberg/bloomberg_api.py` & `hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,24 +266,28 @@
     # pdblp requires dates in string format of form YYYYMMDD
     # if no date provided use today and -12M
     t0 = flex_date_solver(t0).strftime("%Y-%m-%d")
     t1 = flex_date_solver(t1).strftime("%Y-%m-%d")
 
     try:
         call = blp.bdh(clean_tickers, clean_fields, t0, t1, **kwargs)       # Run bdh call
-        call.index = pd.to_datetime(call.index)                           # force datetime index
+        call.index = pd.to_datetime(call.index)                             # force datetime index
     except KeyError:
         msg = f"bloomberg error: debug needs work; check valid tickers/fields & timeseries > 3m"
         raise Exception(msg)
 
     # pdblp defaults to outputting daily data (weekdays only)
     # We reindex based on desired frequency
-    # output = _pdblp_freq_hack(call=call, t0=t0, t1=t1, freq=freq)
     output = _pdblp_freq_hack2(df=call, t0=t0, t1=t1, freq=freq)
-    output.index.name = 'date'  # worth renaming the date column while we are at it
+    output.index.name = 'date'                      # worth renaming the date column while we are at it
+
+    # remove data that is beyond t1 date
+    # happens when we resample the date; most recent observation is added to resample freq
+    # ie t1 = 5-March & freq = EOM. Obs from 5th March will be in dataframe labelled 31-March
+    output = output[output.index <= t1]
 
     #
     if interpolate:
         output = output.ffill()
 
     # optional currency translation
     # Bloomberg's FX override is rather unstable, to we have our own
@@ -369,12 +373,11 @@
     tickers = {"MXUS Index": "USA", "MXGB Index": "GB"}
     fields = {"PX_LAST": "Price", "PX_VOLUME": "Volume"}
 
     test_call = bdh(
         tickers="MXUS Index",
         fields=fields,
         t0="20030101",
-        t1="20030601",
-        freq='EOM',
+        freq='D',
     )
 
     print(test_call.tail(12))
```

### Comparing `hxm_refuel-0.2.7/hxm_refuel/bloomberg/bloomberg_recipies.py` & `hxm_refuel-0.2.8/hxm_refuel/bloomberg/bloomberg_recipies.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/hxm_refuel/jeeves.py` & `hxm_refuel-0.2.8/hxm_refuel/jeeves.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/hxm_refuel/snowflake/connector.py` & `hxm_refuel-0.2.8/hxm_refuel/snowflake/connector.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/hxm_refuel/snowflake/snowflake_recipes.py` & `hxm_refuel-0.2.8/hxm_refuel/snowflake/snowflake_recipes.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/hxm_refuel/snowflake/sql_recipes.py` & `hxm_refuel-0.2.8/hxm_refuel/snowflake/sql_recipes.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/hxm_refuel/validation.py` & `hxm_refuel-0.2.8/hxm_refuel/validation.py`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/LICENSE` & `hxm_refuel-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/pyproject.toml` & `hxm_refuel-0.2.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 [tool.poetry]
 name = "hxm-refuel"
-version = "0.2.7"
+version = "0.2.8"
 description = "Wrapper for financial database APIs"
 authors = ["djmcnay <39102979+djmcnay@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 xbbg = "^0.7.7"
-pytest = "^7.4.2"
 snowflake-connector-python = "^3.2.0"
 snowflake-sqlalchemy = "^1.5.0"
 pyarrow = ">=10.0.1, <10.1.0"
 cryptography = "^41.0.5"
+blpapi = {version = "^3.18.0", source = "bloomberg"}
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.8"
 python-dotenv = "^1.0.0"
-
-[tool.poetry.group.optional]
-optional = true
-
-[tool.poetry.group.optional.dependencies]
-blpapi = {version = "^3.18.0", source = "bloomberg"}
+pytest = "^7.4.2"
 
 [[tool.poetry.source]]
 name = "bloomberg"
 url = "https://bcms.bloomberg.com/pip/simple"
 priority = "explicit"
 
 [build-system]
```

### Comparing `hxm_refuel-0.2.7/README.md` & `hxm_refuel-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `hxm_refuel-0.2.7/PKG-INFO` & `hxm_refuel-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hxm-refuel
-Version: 0.2.7
+Version: 0.2.8
 Summary: Wrapper for financial database APIs
 Author: djmcnay
 Author-email: 39102979+djmcnay@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: blpapi (>=3.18.0,<4.0.0)
 Requires-Dist: cryptography (>=41.0.5,<42.0.0)
 Requires-Dist: pyarrow (>=10.0.1,<10.1.0)
-Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: snowflake-connector-python (>=3.2.0,<4.0.0)
 Requires-Dist: snowflake-sqlalchemy (>=1.5.0,<2.0.0)
 Requires-Dist: xbbg (>=0.7.7,<0.8.0)
 Description-Content-Type: text/markdown
 
 # HongXiongMao Refuel
```

