# Comparing `tmp/core_ct-1.3.1.tar.gz` & `tmp/core_ct-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_ct-1.3.1.tar", max compression
+gzip compressed data, was "core_ct-1.4.0.tar", max compression
```

## Comparing `core_ct-1.3.1.tar` & `core_ct-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2024-05-08 20:48:03.329829 core_ct-1.3.1/LICENSE
--rw-r--r--   0        0        0     2593 2024-05-08 20:48:03.329829 core_ct-1.3.1/README.md
--rw-r--r--   0        0        0      976 2024-05-08 20:48:03.761836 core_ct-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/__init__.py
--rw-r--r--   0        0        0      747 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/analysis.py
--rw-r--r--   0        0        0    22841 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/core.py
--rw-r--r--   0        0        0     6274 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/importers.py
--rw-r--r--   0        0        0     4647 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/slice.py
--rw-r--r--   0        0        0     7286 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/visualize.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-08 21:22:30.617143 core_ct-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2593 2024-05-08 21:22:30.617143 core_ct-1.4.0/README.md
+-rw-r--r--   0        0        0      976 2024-05-08 21:22:31.045143 core_ct-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-08 21:22:31.045143 core_ct-1.4.0/src/core_ct/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-08 21:22:31.045143 core_ct-1.4.0/src/core_ct/analysis.py
+-rw-r--r--   0        0        0    31462 2024-05-08 21:22:31.045143 core_ct-1.4.0/src/core_ct/core.py
+-rw-r--r--   0        0        0     6274 2024-05-08 21:22:31.045143 core_ct-1.4.0/src/core_ct/importers.py
+-rw-r--r--   0        0        0    11655 2024-05-08 21:22:31.049143 core_ct-1.4.0/src/core_ct/slice.py
+-rw-r--r--   0        0        0     7286 2024-05-08 21:22:31.049143 core_ct-1.4.0/src/core_ct/visualize.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.4.0/PKG-INFO
```

### Comparing `core_ct-1.3.1/LICENSE` & `core_ct-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `core_ct-1.3.1/README.md` & `core_ct-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `core_ct-1.3.1/pyproject.toml` & `core_ct-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-ct"
-version = "1.3.1"
+version = "1.4.0"
 description = "A Python library to assist geologists with the analysis of rock core CT scans"
 authors = [
     "Kira Hanson <khanson@mines.edu>",
     "Carla Ellefsen <cellefsen@mines.edu>",
     "Connor Sparks <csparks@mines.edu>",
     "Asa Sprow <arsprow@mines.edu>",
 ]
```

### Comparing `core_ct-1.3.1/src/core_ct/analysis.py` & `core_ct-1.4.0/src/core_ct/analysis.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.3.1/src/core_ct/importers.py` & `core_ct-1.4.0/src/core_ct/importers.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.3.1/src/core_ct/visualize.py` & `core_ct-1.4.0/src/core_ct/visualize.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.3.1/PKG-INFO` & `core_ct-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-ct
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Python library to assist geologists with the analysis of rock core CT scans
 License: MIT
 Author: Kira Hanson
 Author-email: khanson@mines.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

