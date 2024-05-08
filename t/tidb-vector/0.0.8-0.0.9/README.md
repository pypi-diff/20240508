# Comparing `tmp/tidb_vector-0.0.8.tar.gz` & `tmp/tidb_vector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidb_vector-0.0.8.tar", max compression
+gzip compressed data, was "tidb_vector-0.0.9.tar", max compression
```

## Comparing `tidb_vector-0.0.8.tar` & `tidb_vector-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.8/LICENSE
--rw-r--r--   0        0        0     6872 2024-04-22 13:07:11.269379 tidb_vector-0.0.8/README.md
--rw-r--r--   0        0        0      852 2024-04-01 08:18:14.580905 tidb_vector-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-23 11:11:43.858106 tidb_vector-0.0.8/tidb_vector/__init__.py
--rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.8/tidb_vector/constants.py
--rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.8/tidb_vector/integrations/__init__.py
--rw-r--r--   0        0        0     3666 2024-04-23 03:30:37.756240 tidb_vector-0.0.8/tidb_vector/integrations/utils.py
--rw-r--r--   0        0        0    18701 2024-04-23 03:30:37.757294 tidb_vector-0.0.8/tidb_vector/integrations/vector_client.py
--rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.8/tidb_vector/peewee/__init__.py
--rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.8/tidb_vector/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      863 2024-03-14 03:59:19.126501 tidb_vector-0.0.8/tidb_vector/utils.py
--rw-r--r--   0        0        0     7540 1970-01-01 00:00:00.000000 tidb_vector-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11294 2024-03-04 08:01:44.610607 tidb_vector-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6872 2024-04-22 13:07:11.269379 tidb_vector-0.0.9/README.md
+-rw-r--r--   0        0        0      852 2024-05-08 07:52:40.919837 tidb_vector-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-08 07:53:03.287067 tidb_vector-0.0.9/tidb_vector/__init__.py
+-rw-r--r--   0        0        0      109 2024-03-14 03:53:20.150919 tidb_vector-0.0.9/tidb_vector/constants.py
+-rw-r--r--   0        0        0      356 2024-03-05 22:28:11.819145 tidb_vector-0.0.9/tidb_vector/integrations/__init__.py
+-rw-r--r--   0        0        0     3666 2024-04-23 03:30:37.756240 tidb_vector-0.0.9/tidb_vector/integrations/utils.py
+-rw-r--r--   0        0        0    18701 2024-04-23 03:30:37.757294 tidb_vector-0.0.9/tidb_vector/integrations/vector_client.py
+-rw-r--r--   0        0        0      962 2024-03-14 03:59:19.124632 tidb_vector-0.0.9/tidb_vector/peewee/__init__.py
+-rw-r--r--   0        0        0     2775 2024-03-16 06:37:36.615096 tidb_vector-0.0.9/tidb_vector/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      932 2024-05-08 07:52:53.774576 tidb_vector-0.0.9/tidb_vector/utils.py
+-rw-r--r--   0        0        0     7540 1970-01-01 00:00:00.000000 tidb_vector-0.0.9/PKG-INFO
```

### Comparing `tidb_vector-0.0.8/LICENSE` & `tidb_vector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/README.md` & `tidb_vector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/pyproject.toml` & `tidb_vector-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/tidb_vector/integrations/utils.py` & `tidb_vector-0.0.9/tidb_vector/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/tidb_vector/integrations/vector_client.py` & `tidb_vector-0.0.9/tidb_vector/integrations/vector_client.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/tidb_vector/peewee/__init__.py` & `tidb_vector-0.0.9/tidb_vector/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/tidb_vector/sqlalchemy/__init__.py` & `tidb_vector-0.0.9/tidb_vector/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `tidb_vector-0.0.8/tidb_vector/utils.py` & `tidb_vector-0.0.9/tidb_vector/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,8 +25,11 @@
 def decode_vector(value):
     if value is None or isinstance(value, np.ndarray):
         return value
 
     if isinstance(value, bytes):
         value = value.decode("utf-8")
 
+    if value == "[]":
+        return np.array([], dtype=np.float32)
+
     return np.array(value[1:-1].split(","), dtype=np.float32)
```

### Comparing `tidb_vector-0.0.8/PKG-INFO` & `tidb_vector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidb-vector
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python client for TiDB Vector
 License: Apache-2.0
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

