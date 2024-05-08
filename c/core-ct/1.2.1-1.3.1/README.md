# Comparing `tmp/core_ct-1.2.1.tar.gz` & `tmp/core_ct-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_ct-1.2.1.tar", max compression
+gzip compressed data, was "core_ct-1.3.1.tar", max compression
```

## Comparing `core_ct-1.2.1.tar` & `core_ct-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2024-05-06 21:29:43.853330 core_ct-1.2.1/LICENSE
--rw-r--r--   0        0        0     2593 2024-05-06 21:29:43.853330 core_ct-1.2.1/README.md
--rw-r--r--   0        0        0      981 2024-05-06 21:29:44.389333 core_ct-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/__init__.py
--rw-r--r--   0        0        0      747 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/analysis.py
--rw-r--r--   0        0        0    22841 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/core.py
--rw-r--r--   0        0        0     6274 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/importers.py
--rw-r--r--   0        0        0     4647 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/slice.py
--rw-r--r--   0        0        0     7286 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/visualize.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-08 20:48:03.329829 core_ct-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2593 2024-05-08 20:48:03.329829 core_ct-1.3.1/README.md
+-rw-r--r--   0        0        0      976 2024-05-08 20:48:03.761836 core_ct-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/analysis.py
+-rw-r--r--   0        0        0    22841 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/core.py
+-rw-r--r--   0        0        0     6274 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/importers.py
+-rw-r--r--   0        0        0     4647 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/slice.py
+-rw-r--r--   0        0        0     7286 2024-05-08 20:48:03.761836 core_ct-1.3.1/src/core_ct/visualize.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.3.1/PKG-INFO
```

### Comparing `core_ct-1.2.1/LICENSE` & `core_ct-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/README.md` & `core_ct-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/pyproject.toml` & `core_ct-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-ct"
-version = "1.2.1"
+version = "1.3.1"
 description = "A Python library to assist geologists with the analysis of rock core CT scans"
 authors = [
     "Kira Hanson <khanson@mines.edu>",
     "Carla Ellefsen <cellefsen@mines.edu>",
     "Connor Sparks <csparks@mines.edu>",
     "Asa Sprow <arsprow@mines.edu>",
 ]
@@ -22,16 +22,16 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 ruff = "^0.0.292"
 black = "^23.9.1"
 pre-commit = "^3.4.0"
 sphinx = "^7.2.6"
 sphinx-copybutton = "^0.5.2"
-myst-parser = "^2.0.0"
-sphinx-wagtail-theme = "^6.1.1"
+myst-nb = "^1.1.0"
+sphinxawesome-theme = "^5.1.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Enable pycodestyle (`E`), Pyflakes (`F`) and pydocstyle (`D`)
```

### Comparing `core_ct-1.2.1/src/core_ct/analysis.py` & `core_ct-1.3.1/src/core_ct/analysis.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/src/core_ct/core.py` & `core_ct-1.3.1/src/core_ct/core.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/src/core_ct/importers.py` & `core_ct-1.3.1/src/core_ct/importers.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/src/core_ct/slice.py` & `core_ct-1.3.1/src/core_ct/slice.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/src/core_ct/visualize.py` & `core_ct-1.3.1/src/core_ct/visualize.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.1/PKG-INFO` & `core_ct-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-ct
-Version: 1.2.1
+Version: 1.3.1
 Summary: A Python library to assist geologists with the analysis of rock core CT scans
 License: MIT
 Author: Kira Hanson
 Author-email: khanson@mines.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

