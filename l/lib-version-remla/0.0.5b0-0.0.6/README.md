# Comparing `tmp/lib_version_remla-0.0.5b0.tar.gz` & `tmp/lib_version_remla-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla-0.0.5b0.tar", max compression
+gzip compressed data, was "lib_version_remla-0.0.6.tar", max compression
```

## Comparing `lib_version_remla-0.0.5b0.tar` & `lib_version_remla-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-08 13:25:05.200175 lib_version_remla-0.0.5b0/LICENSE
--rw-r--r--   0        0        0      486 2024-05-08 13:25:05.200175 lib_version_remla-0.0.5b0/README.md
--rw-r--r--   0        0        0     1154 2024-05-08 13:25:22.988188 lib_version_remla-0.0.5b0/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-08 13:25:05.204175 lib_version_remla-0.0.5b0/src/lib_version_remla/return_version.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 lib_version_remla-0.0.5b0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 13:31:16.811270 lib_version_remla-0.0.6/LICENSE
+-rw-r--r--   0        0        0      495 2024-05-08 13:31:16.811270 lib_version_remla-0.0.6/README.md
+-rw-r--r--   0        0        0     1152 2024-05-08 13:31:39.175380 lib_version_remla-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      247 2024-05-08 13:31:16.811270 lib_version_remla-0.0.6/src/lib_version_remla/return_version.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 lib_version_remla-0.0.6/PKG-INFO
```

### Comparing `lib_version_remla-0.0.5b0/LICENSE` & `lib_version_remla-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_version_remla-0.0.5b0/pyproject.toml` & `lib_version_remla-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib_version_remla"
-version = "0.0.5b0"
+version = "0.0.6"
 description = "A small package which returns its own version."
 authors = ["Jan <j2000.vdm@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lib_version_remla-0.0.5b0/PKG-INFO` & `lib_version_remla-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_version_remla
-Version: 0.0.5b0
+Version: 0.0.6
 Summary: A small package which returns its own version.
 Author: Jan
 Author-email: j2000.vdm@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -18,11 +18,11 @@
 
 ### Building the package locally
 1. ```poetry install```
 2. ```poetry shell```
 3. ```poetry build```
 <!-- 3. ```python3 -m build```
 To upload to PyPi you need to have access to the API key, which is stored in the team channel -->
-4. ```python3 -m twine upload --repository pypi dist/*``` 
+<!-- 4. ```python3 -m twine upload --repository pypi dist/*```  -->
 
 ### Importing the package
 1. Install with: ```pip install --index-url https://pypi.org/project/ --no-deps lib-version-remla```
```

