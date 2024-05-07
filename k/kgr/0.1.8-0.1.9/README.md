# Comparing `tmp/kgr-0.1.8.tar.gz` & `tmp/kgr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.8.tar", last modified: Tue May  7 22:07:09 2024, max compression
+gzip compressed data, was "kgr-0.1.9.tar", last modified: Tue May  7 22:43:42 2024, max compression
```

## Comparing `kgr-0.1.8.tar` & `kgr-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.1.8/LICENSE
--rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.1.8/README.md
--rw-r--r--   0        0        0      880 2024-05-07 22:07:09.558441 kgr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 20:46:37.221089 kgr-0.1.8/src/__init__.py
--rw-r--r--   0        0        0       30 2024-04-13 20:46:37.221251 kgr-0.1.8/src/__main__.py
--rw-r--r--   0        0        0     9024 2024-05-07 22:02:45.239020 kgr-0.1.8/src/lib.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 kgr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.1.9/LICENSE
+-rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.1.9/README.md
+-rw-r--r--   0        0        0      880 2024-05-07 22:43:42.480206 kgr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 20:46:37.221089 kgr-0.1.9/src/kgr/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-13 20:46:37.221251 kgr-0.1.9/src/kgr/__main__.py
+-rw-r--r--   0        0        0     9024 2024-05-07 22:02:45.239020 kgr-0.1.9/src/kgr/lib.py
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 kgr-0.1.9/PKG-INFO
```

### Comparing `kgr-0.1.8/LICENSE` & `kgr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.8/pyproject.toml` & `kgr-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
```

### Comparing `kgr-0.1.8/src/lib.py` & `kgr-0.1.9/src/kgr/lib.py`

 * *Files identical despite different names*

### Comparing `kgr-0.1.8/PKG-INFO` & `kgr-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Dmitry Luschan
```

