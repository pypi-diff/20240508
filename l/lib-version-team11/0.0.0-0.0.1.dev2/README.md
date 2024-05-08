# Comparing `tmp/lib_version_team11-0.0.0.tar.gz` & `tmp/lib_version_team11-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_team11-0.0.0.tar", max compression
+gzip compressed data, was "lib_version_team11-0.0.1.dev2.tar", max compression
```

## Comparing `lib_version_team11-0.0.0.tar` & `lib_version_team11-0.0.1.dev2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       92 2024-05-08 10:27:24.000671 lib_version_team11-0.0.0/README.md
--rw-r--r--   0        0        0      668 2024-05-08 12:35:38.848196 lib_version_team11-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      580 2024-05-08 12:35:21.393089 lib_version_team11-0.0.0/src/lib_version_team11.py
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 lib_version_team11-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2024-05-08 13:20:49.786417 lib_version_team11-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      674 2024-05-08 13:21:14.206431 lib_version_team11-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      580 2024-05-08 13:20:49.786417 lib_version_team11-0.0.1.dev2/src/lib_version_team11.py
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 lib_version_team11-0.0.1.dev2/PKG-INFO
```

### Comparing `lib_version_team11-0.0.0/pyproject.toml` & `lib_version_team11-0.0.1.dev2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.5.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "lib-version-team11"
-version = "0.0.0"
+version = "0.0.1.dev2"
 description = "A version-aware library that can be asked for the version of the library."
 authors = ["team_11 <E.Sipols@student.tudelft.nl>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
@@ -18,10 +18,10 @@
 setuptools_scm = "^6.3.2"
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = 'git'
 style = 'pep440'
```

### Comparing `lib_version_team11-0.0.0/src/lib_version_team11.py` & `lib_version_team11-0.0.1.dev2/src/lib_version_team11.py`

 * *Files identical despite different names*

### Comparing `lib_version_team11-0.0.0/PKG-INFO` & `lib_version_team11-0.0.1.dev2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-team11
-Version: 0.0.0
+Version: 0.0.1.dev2
 Summary: A version-aware library that can be asked for the version of the library.
 Author: team_11
 Author-email: E.Sipols@student.tudelft.nl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

