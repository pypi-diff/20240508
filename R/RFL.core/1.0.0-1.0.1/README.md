# Comparing `tmp/RFL.core-1.0.0.tar.gz` & `tmp/rfl_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.core-1.0.0.tar", last modified: Mon Apr  8 13:14:44 2024, max compression
+gzip compressed data, was "rfl_core-1.0.1.tar", last modified: Wed May  8 08:32:01 2024, max compression
```

## Comparing `RFL.core-1.0.0.tar` & `rfl_core-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:44.666191 RFL.core-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      769 2024-04-08 13:14:44.666191 RFL.core-1.0.0/PKG-INFO
--rw-r--r--   0 remi      (1000) remi      (1000)       58 2023-10-20 06:36:52.000000 RFL.core-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:44.666191 RFL.core-1.0.0/RFL.core.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      769 2024-04-08 13:14:44.000000 RFL.core-1.0.0/RFL.core.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      192 2024-04-08 13:14:44.000000 RFL.core-1.0.0/RFL.core.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:14:44.000000 RFL.core-1.0.0/RFL.core.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:14:44.000000 RFL.core-1.0.0/RFL.core.egg-info/top_level.txt
--rw-r--r--   0 remi      (1000) remi      (1000)      885 2024-04-08 09:20:45.000000 RFL.core-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:44.666191 RFL.core-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:44.666191 RFL.core-1.0.0/rfl/core/
--rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-07-24 14:07:08.000000 RFL.core-1.0.0/rfl/core/__init__.py
--rw-r--r--   0 remi      (1000) remi      (1000)      144 2023-09-08 08:36:20.000000 RFL.core-1.0.0/rfl/core/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:14:44.666191 RFL.core-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:01.919368 rfl_core-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      769 2024-05-08 08:32:01.919368 rfl_core-1.0.1/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)       58 2023-10-20 06:36:52.000000 rfl_core-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:01.919368 rfl_core-1.0.1/RFL.core.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      769 2024-05-08 08:32:01.000000 rfl_core-1.0.1/RFL.core.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      192 2024-05-08 08:32:01.000000 rfl_core-1.0.1/RFL.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:32:01.000000 rfl_core-1.0.1/RFL.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:32:01.000000 rfl_core-1.0.1/RFL.core.egg-info/top_level.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)      885 2024-05-08 07:35:28.000000 rfl_core-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:01.919368 rfl_core-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:01.919368 rfl_core-1.0.1/rfl/core/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-07-24 14:07:08.000000 rfl_core-1.0.1/rfl/core/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      144 2023-09-08 08:36:20.000000 rfl_core-1.0.1/rfl/core/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:32:01.919368 rfl_core-1.0.1/setup.cfg
```

### Comparing `RFL.core-1.0.0/PKG-INFO` & `rfl_core-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: core package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.core-1.0.0/RFL.core.egg-info/PKG-INFO` & `rfl_core-1.0.1/RFL.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: core package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.core-1.0.0/pyproject.toml` & `rfl_core-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.core"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: core package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

