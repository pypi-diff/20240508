# Comparing `tmp/lib_version_remla-0.0.3.tar.gz` & `tmp/lib_version_remla-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla-0.0.3.tar", last modified: Wed May  8 12:39:20 2024, max compression
+gzip compressed data, was "lib_version_remla-0.0.4.tar", last modified: Wed May  8 12:47:37 2024, max compression
```

## Comparing `lib_version_remla-0.0.3.tar` & `lib_version_remla-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.640267 lib_version_remla-0.0.3/
--rw-r--r--   0 jan       (1000) jan       (1000)      765 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      328 2024-05-08 12:32:45.000000 lib_version_remla-0.0.3/README.md
--rw-r--r--   0 jan       (1000) jan       (1000)     1031 2024-05-08 12:39:05.000000 lib_version_remla-0.0.3/pyproject.toml
--rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-08 12:39:20.640267 lib_version_remla-0.0.3/setup.cfg
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/lib_version_remla/
--rw-r--r--   0 jan       (1000) jan       (1000)      134 2024-05-08 12:20:57.000000 lib_version_remla-0.0.3/src/lib_version_remla/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)      129 2024-05-08 12:00:25.000000 lib_version_remla-0.0.3/src/lib_version_remla/return_version.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)      765 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      278 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       18 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/top_level.txt
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.336959 lib_version_remla-0.0.4/
+-rw-r--r--   0 jan       (1000) jan       (1000)      897 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      459 2024-05-08 12:40:53.000000 lib_version_remla-0.0.4/README.md
+-rw-r--r--   0 jan       (1000) jan       (1000)     1031 2024-05-08 12:47:26.000000 lib_version_remla-0.0.4/pyproject.toml
+-rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-08 12:47:37.336959 lib_version_remla-0.0.4/setup.cfg
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/lib_version_remla/
+-rw-r--r--   0 jan       (1000) jan       (1000)       87 2024-05-08 12:46:45.000000 lib_version_remla-0.0.4/src/lib_version_remla/return_version.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)      897 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      244 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)       18 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/top_level.txt
```

### Comparing `lib_version_remla-0.0.3/PKG-INFO` & `lib_version_remla-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_version_remla
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package which returns its own version.
 Author-email: Jan <j2000.vdm@gmail.com>
 Project-URL: Homepage, https://github.com/remla24-team10/lib-version
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -15,7 +15,11 @@
 
 ### Building the package locally
 1. ```poetry install```
 2. ```poetry shell```
 3. ```python3 -m build```
 To upload to PyPi you need to have access to the API key, which is stored in the team channel.
 4. ```python3 -m twine upload --repository pypi dist/*```
+
+### Importing the package
+1. Install with: ```pip install --index-url https://pypi.org/project/ --no-deps lib-version-remla```
+2.
```

### Comparing `lib_version_remla-0.0.3/pyproject.toml` & `lib_version_remla-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lib_version_remla"
-version = "0.0.3"
+version = "0.0.4"
 description = "A small package which returns its own version."
 authors = ["Jan <j2000.vdm@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project]
 name = "lib_version_remla"
-version = "0.0.3"
+version = "0.0.4"
 description = "A small package which returns its own version."
 authors = [
     { name = "Jan", email="j2000.vdm@gmail.com" },
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `lib_version_remla-0.0.3/src/lib_version_remla.egg-info/PKG-INFO` & `lib_version_remla-0.0.4/src/lib_version_remla.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_version_remla
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package which returns its own version.
 Author-email: Jan <j2000.vdm@gmail.com>
 Project-URL: Homepage, https://github.com/remla24-team10/lib-version
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -15,7 +15,11 @@
 
 ### Building the package locally
 1. ```poetry install```
 2. ```poetry shell```
 3. ```python3 -m build```
 To upload to PyPi you need to have access to the API key, which is stored in the team channel.
 4. ```python3 -m twine upload --repository pypi dist/*```
+
+### Importing the package
+1. Install with: ```pip install --index-url https://pypi.org/project/ --no-deps lib-version-remla```
+2.
```

