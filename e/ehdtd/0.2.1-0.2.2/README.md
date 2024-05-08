# Comparing `tmp/ehdtd-0.2.1.tar.gz` & `tmp/ehdtd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.2.1.tar", max compression
+gzip compressed data, was "ehdtd-0.2.2.tar", max compression
```

## Comparing `ehdtd-0.2.1.tar` & `ehdtd-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.1/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.1/README.md
--rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.1/ehdtd/__init__.py
--rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.1/ehdtd/binance.py
--rw-r--r--   0        0        0   121687 2024-05-08 04:30:39.346014 ehdtd-0.2.1/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.1/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      705 2024-05-08 04:32:31.702555 ehdtd-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.2/README.md
+-rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.2/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.2/ehdtd/binance.py
+-rw-r--r--   0        0        0   121756 2024-05-08 13:26:24.819355 ehdtd-0.2.2/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.2/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      705 2024-05-08 13:20:15.782470 ehdtd-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.2/PKG-INFO
```

### Comparing `ehdtd-0.2.1/LICENSE` & `ehdtd-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.1/README.md` & `ehdtd-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.1/ehdtd/__init__.py` & `ehdtd-0.2.2/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.1/ehdtd/binance.py` & `ehdtd-0.2.2/ehdtd/binance.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.1/ehdtd/ehdtd.py` & `ehdtd-0.2.2/ehdtd/ehdtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1474,15 +1474,16 @@
 
                             __delta_seconds = (
                                 Ehdtd.get_delta_seconds_for_interval('1mo',__year, __month)
                             )
 
                         if (int(__get_data[0]['close_time']) - int(__get_data[0]['open_time']))\
                             == __delta_seconds\
-                            and int(__get_data[0]['close_time']) == int(__get_data[1]['open_time']):
+                            and int(__get_data[0]['close_time']) == int(__get_data[1]['open_time'])\
+                            and float(__get_data[0]['volume']) != 0:
 
                             if self.__exec_db_upsert_stmt(symbol, interval, __get_data, db_conn):
 
                                 str_out += ' -> YES'
 
                                 __next_open_time = None
```

### Comparing `ehdtd-0.2.1/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.2.2/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.1/pyproject.toml` & `ehdtd-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.2.1"
+version = "0.2.2"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.2.1/PKG-INFO` & `ehdtd-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

