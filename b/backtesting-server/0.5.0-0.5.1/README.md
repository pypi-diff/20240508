# Comparing `tmp/backtesting_server-0.5.0.tar.gz` & `tmp/backtesting_server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.5.0.tar", max compression
+gzip compressed data, was "backtesting_server-0.5.1.tar", max compression
```

## Comparing `backtesting_server-0.5.0.tar` & `backtesting_server-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.5.0/LICENSE
--rw-r--r--   0        0        0      628 2024-05-06 23:15:22.309700 backtesting_server-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.5.0/README.md
--rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.5.0/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    27207 2024-05-06 23:14:58.293110 backtesting_server-0.5.0/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.5.1/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-08 20:54:54.193183 backtesting_server-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.5.1/README.md
+-rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.5.1/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    27243 2024-05-08 20:54:36.406102 backtesting_server-0.5.1/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.5.1/PKG-INFO
```

### Comparing `backtesting_server-0.5.0/LICENSE` & `backtesting_server-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.5.0/pyproject.toml` & `backtesting_server-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.5.0"
+version = "0.5.1"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.5.0/README.md` & `backtesting_server-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.5.0/src/backtesting_server/main.py` & `backtesting_server-0.5.1/src/backtesting_server/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,15 +508,15 @@
       for instrument in upload_instruments:
         # Adding previous timestamp.
         if instrument.epic not in previous_timestamps.keys():
           previous_timestamps[instrument.epic] = instrument.ticker.timestamp
         # Checking if timestamp has changed.
         if instrument.ticker.timestamp != previous_timestamps[instrument.epic]:
           # Formatting prices.
-          price_data = [[instrument.ticker.timestamp,instrument.ticker.bid,None,None,instrument.ticker.offer]]
+          price_data = [[instrument.ticker.timestamp,instrument.ticker.bid,instrument.ticker.offer,instrument.ticker.bid,instrument.ticker.offer]]
           # Creating dataframe.
           df = pd.DataFrame(price_data, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
           df.set_index("Datetime",inplace=True)
           # Updating previous timestamp.
           previous_timestamps[instrument.epic] = instrument.ticker.timestamp
 
           # Uploading data.
```

### Comparing `backtesting_server-0.5.0/PKG-INFO` & `backtesting_server-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

