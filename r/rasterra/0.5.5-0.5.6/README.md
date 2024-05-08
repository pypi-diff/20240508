# Comparing `tmp/rasterra-0.5.5.tar.gz` & `tmp/rasterra-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterra-0.5.5.tar", max compression
+gzip compressed data, was "rasterra-0.5.6.tar", max compression
```

## Comparing `rasterra-0.5.5.tar` & `rasterra-0.5.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1521 2024-05-07 20:43:35.010338 rasterra-0.5.5/LICENSE
--rw-r--r--   0        0        0     2687 2024-05-07 20:43:35.010338 rasterra-0.5.5/README.md
--rw-r--r--   0        0        0     3548 2024-05-07 20:43:35.014338 rasterra-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      152 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/__init__.py
--rw-r--r--   0        0        0    19220 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_array.py
--rw-r--r--   0        0        0     3267 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_features.py
--rw-r--r--   0        0        0     1657 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_io.py
--rw-r--r--   0        0        0     3795 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_plotting.py
--rw-r--r--   0        0        0      565 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_typing.py
--rw-r--r--   0        0        0        0 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/py.typed
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 rasterra-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-07 21:43:36.420254 rasterra-0.5.6/LICENSE
+-rw-r--r--   0        0        0     2687 2024-05-07 21:43:36.420254 rasterra-0.5.6/README.md
+-rw-r--r--   0        0        0     3548 2024-05-07 21:43:36.424254 rasterra-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/__init__.py
+-rw-r--r--   0        0        0    19220 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/_array.py
+-rw-r--r--   0        0        0     3267 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/_features.py
+-rw-r--r--   0        0        0     1657 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/_io.py
+-rw-r--r--   0        0        0     3795 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/_plotting.py
+-rw-r--r--   0        0        0      755 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:43:36.424254 rasterra-0.5.6/src/rasterra/py.typed
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 rasterra-0.5.6/PKG-INFO
```

### Comparing `rasterra-0.5.5/LICENSE` & `rasterra-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/README.md` & `rasterra-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/pyproject.toml` & `rasterra-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rasterra"
-version = "0.5.5"
+version = "0.5.6"
 description = "A sleek, object-oriented interface designed for intuitive raster data manipulation in Python."
 authors = [
     "James Collins <collijk1@gmail.com>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rasterra-0.5.5/src/rasterra/_array.py` & `rasterra-0.5.6/src/rasterra/_array.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/src/rasterra/_features.py` & `rasterra-0.5.6/src/rasterra/_features.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/src/rasterra/_io.py` & `rasterra-0.5.6/src/rasterra/_io.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/src/rasterra/_plotting.py` & `rasterra-0.5.6/src/rasterra/_plotting.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.5/PKG-INFO` & `rasterra-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterra
-Version: 0.5.5
+Version: 0.5.6
 Summary: A sleek, object-oriented interface designed for intuitive raster data manipulation in Python.
 Home-page: https://collijk.github.io/rasterra
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk1@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

