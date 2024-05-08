# Comparing `tmp/synfras-0.2.0.tar.gz` & `tmp/synfras-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synfras-0.2.0.tar", max compression
+gzip compressed data, was "synfras-0.3.0.tar", max compression
```

## Comparing `synfras-0.2.0.tar` & `synfras-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      653 2024-05-07 02:30:14.772273 synfras-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-0.2.0/synfras/__init__.py
--rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-0.2.0/synfras/config.py
--rw-r--r--   0        0        0     1126 2024-05-07 02:18:48.800446 synfras-0.2.0/synfras/database.py
--rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-0.2.0/synfras/parallel.py
--rw-r--r--   0        0        0      447 2024-05-07 02:29:05.584450 synfras-0.2.0/synfras/utils.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 synfras-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2024-05-08 08:38:21.921743 synfras-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      542 2024-05-07 03:29:24.028213 synfras-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-13 06:43:19.642186 synfras-0.3.0/synfras/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-07 02:18:48.798900 synfras-0.3.0/synfras/config.py
+-rw-r--r--   0        0        0     1126 2024-05-07 02:18:48.800446 synfras-0.3.0/synfras/database.py
+-rw-r--r--   0        0        0     1189 2024-05-07 02:18:48.801460 synfras-0.3.0/synfras/parallel.py
+-rw-r--r--   0        0        0      816 2024-05-08 08:38:21.923774 synfras-0.3.0/synfras/utils.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 synfras-0.3.0/PKG-INFO
```

### Comparing `synfras-0.2.0/pyproject.toml` & `synfras-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synfras"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Trung Dang <dangtrung96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 dynaconf = "^3.2.4"
```

### Comparing `synfras-0.2.0/README.md` & `synfras-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `synfras-0.2.0/synfras/database.py` & `synfras-0.3.0/synfras/database.py`

 * *Files identical despite different names*

### Comparing `synfras-0.2.0/synfras/parallel.py` & `synfras-0.3.0/synfras/parallel.py`

 * *Files identical despite different names*

### Comparing `synfras-0.2.0/PKG-INFO` & `synfras-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: synfras
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Trung Dang
 Author-email: dangtrung96@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dynaconf (>=3.2.4,<4.0.0)
 Requires-Dist: oracledb (>=2.0.1,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pymssql (==2.2.7)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
```

