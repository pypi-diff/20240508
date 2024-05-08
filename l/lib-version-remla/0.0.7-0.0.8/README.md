# Comparing `tmp/lib_version_remla-0.0.7.tar.gz` & `tmp/lib_version_remla-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla-0.0.7.tar", max compression
+gzip compressed data, was "lib_version_remla-0.0.8.tar", max compression
```

## Comparing `lib_version_remla-0.0.7.tar` & `lib_version_remla-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-08 13:46:14.633782 lib_version_remla-0.0.7/LICENSE
--rw-r--r--   0        0        0      625 2024-05-08 13:46:14.633782 lib_version_remla-0.0.7/README.md
--rw-r--r--   0        0        0     1152 2024-05-08 13:46:33.697858 lib_version_remla-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      235 2024-05-08 13:46:14.637782 lib_version_remla-0.0.7/src/lib_version_remla/return_version.py
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 lib_version_remla-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 13:52:47.621232 lib_version_remla-0.0.8/LICENSE
+-rw-r--r--   0        0        0      686 2024-05-08 13:52:47.621232 lib_version_remla-0.0.8/README.md
+-rw-r--r--   0        0        0     1152 2024-05-08 13:53:06.877432 lib_version_remla-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      283 2024-05-08 13:52:47.621232 lib_version_remla-0.0.8/src/lib_version_remla/return_version.py
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 lib_version_remla-0.0.8/PKG-INFO
```

### Comparing `lib_version_remla-0.0.7/LICENSE` & `lib_version_remla-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_version_remla-0.0.7/README.md` & `lib_version_remla-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 3. ```poetry build```
 <!-- 3. ```python3 -m build```
 To upload to PyPi you need to have access to the API key, which is stored in the team channel -->
 1. ```python3 -m twine upload --repository pypi dist/*``` 
 
 ### Updating the package via workflow
 After pushing an update you can tag it with the following command to trigger the workflow.
-1. ```git tag v0.0.n```
+1. ```git tag version``, where version is the version number. E.g. ```git tag 0.0.1`
 2. ```git push origin --tags ```
 
 ### Importing the package
 1. Install with: ```pip install lib-version-remla```
```

### Comparing `lib_version_remla-0.0.7/pyproject.toml` & `lib_version_remla-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib_version_remla"
-version = "0.0.7"
+version = "0.0.8"
 description = "A small package which returns its own version."
 authors = ["Jan <j2000.vdm@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lib_version_remla-0.0.7/PKG-INFO` & `lib_version_remla-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_version_remla
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small package which returns its own version.
 Author: Jan
 Author-email: j2000.vdm@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,12 +22,12 @@
 3. ```poetry build```
 <!-- 3. ```python3 -m build```
 To upload to PyPi you need to have access to the API key, which is stored in the team channel -->
 1. ```python3 -m twine upload --repository pypi dist/*``` 
 
 ### Updating the package via workflow
 After pushing an update you can tag it with the following command to trigger the workflow.
-1. ```git tag v0.0.n```
+1. ```git tag version``, where version is the version number. E.g. ```git tag 0.0.1`
 2. ```git push origin --tags ```
 
 ### Importing the package
 1. Install with: ```pip install lib-version-remla```
```

