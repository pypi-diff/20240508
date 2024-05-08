# Comparing `tmp/RFL.build-1.0.0.tar.gz` & `tmp/rfl_build-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.build-1.0.0.tar", last modified: Mon Apr  8 13:14:09 2024, max compression
+gzip compressed data, was "rfl_build-1.0.1.tar", last modified: Wed May  8 08:31:34 2024, max compression
```

## Comparing `RFL.build-1.0.0.tar` & `rfl_build-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:09.214143 RFL.build-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      835 2024-04-08 13:14:09.210143 RFL.build-1.0.0/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)       77 2023-10-23 20:47:53.000000 RFL.build-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:09.210143 RFL.build-1.0.0/RFL.build.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      835 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      363 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)      128 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/entry_points.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       15 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:14:09.000000 RFL.build-1.0.0/RFL.build.egg-info/top_level.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)     1110 2024-04-08 09:20:37.000000 RFL.build-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:09.210143 RFL.build-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:09.210143 RFL.build-1.0.0/rfl/build/
--rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-23 20:47:53.000000 RFL.build-1.0.0/rfl/build/__init__.py
--rw-r--r--   0 remi      (1000) remi      (1000)      183 2024-04-03 11:37:30.000000 RFL.build-1.0.0/rfl/build/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      496 2024-03-15 09:09:49.000000 RFL.build-1.0.0/rfl/build/installsetup.py
--rw-r--r--   0 remi      (1000) remi      (1000)     7219 2024-04-04 19:23:26.000000 RFL.build-1.0.0/rfl/build/ninja.py
--rw-r--r--   0 remi      (1000) remi      (1000)     1674 2024-03-22 14:58:34.000000 RFL.build-1.0.0/rfl/build/projectversion.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:14:09.210143 RFL.build-1.0.0/rfl/build/scripts/
--rw-rw-r--   0 remi      (1000) remi      (1000)     3326 2024-03-18 20:39:19.000000 RFL.build-1.0.0/rfl/build/scripts/setup
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:14:09.214143 RFL.build-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:34.387446 rfl_build-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      835 2024-05-08 08:31:34.387446 rfl_build-1.0.1/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)       77 2023-10-23 20:47:53.000000 rfl_build-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:34.387446 rfl_build-1.0.1/RFL.build.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      835 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      363 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      128 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/entry_points.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       15 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:31:34.000000 rfl_build-1.0.1/RFL.build.egg-info/top_level.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1110 2024-05-08 07:35:32.000000 rfl_build-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:34.387446 rfl_build-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:34.387446 rfl_build-1.0.1/rfl/build/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-10-23 20:47:53.000000 rfl_build-1.0.1/rfl/build/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      183 2024-04-03 11:37:30.000000 rfl_build-1.0.1/rfl/build/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      496 2024-03-15 09:09:49.000000 rfl_build-1.0.1/rfl/build/installsetup.py
+-rw-r--r--   0 remi      (1000) remi      (1000)     7219 2024-04-04 19:23:26.000000 rfl_build-1.0.1/rfl/build/ninja.py
+-rw-r--r--   0 remi      (1000) remi      (1000)     1674 2024-03-22 14:58:34.000000 rfl_build-1.0.1/rfl/build/projectversion.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:34.387446 rfl_build-1.0.1/rfl/build/scripts/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3326 2024-03-18 20:39:19.000000 rfl_build-1.0.1/rfl/build/scripts/setup
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:31:34.387446 rfl_build-1.0.1/setup.cfg
```

### Comparing `RFL.build-1.0.0/PKG-INFO` & `rfl_build-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.build
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: build package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.build-1.0.0/RFL.build.egg-info/PKG-INFO` & `rfl_build-1.0.1/RFL.build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.build
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: build package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.build-1.0.0/pyproject.toml` & `rfl_build-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.build"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: build package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.build-1.0.0/rfl/build/ninja.py` & `rfl_build-1.0.1/rfl/build/ninja.py`

 * *Files identical despite different names*

### Comparing `RFL.build-1.0.0/rfl/build/projectversion.py` & `rfl_build-1.0.1/rfl/build/projectversion.py`

 * *Files identical despite different names*

### Comparing `RFL.build-1.0.0/rfl/build/scripts/setup` & `rfl_build-1.0.1/rfl/build/scripts/setup`

 * *Files identical despite different names*

