# Comparing `tmp/RFL.web-1.0.0.tar.gz` & `tmp/rfl_web-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.web-1.0.0.tar", last modified: Mon Apr  8 13:16:04 2024, max compression
+gzip compressed data, was "rfl_web-1.0.1.tar", last modified: Wed May  8 08:34:04 2024, max compression
```

## Comparing `RFL.web-1.0.0.tar` & `rfl_web-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:16:04.518292 RFL.web-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      834 2024-04-08 13:16:04.518292 RFL.web-1.0.0/PKG-INFO
--rw-r--r--   0 remi      (1000) remi      (1000)       60 2023-10-20 06:39:29.000000 RFL.web-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:16:04.518292 RFL.web-1.0.0/RFL.web.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      834 2024-04-08 13:16:04.000000 RFL.web-1.0.0/RFL.web.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      216 2024-04-08 13:16:04.000000 RFL.web-1.0.0/RFL.web.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:16:04.000000 RFL.web-1.0.0/RFL.web.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       35 2024-04-08 13:16:04.000000 RFL.web-1.0.0/RFL.web.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:16:04.000000 RFL.web-1.0.0/RFL.web.egg-info/top_level.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)      931 2024-04-08 09:21:19.000000 RFL.web-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:16:04.514292 RFL.web-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:16:04.514292 RFL.web-1.0.0/rfl/web/
--rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-11 08:10:30.000000 RFL.web-1.0.0/rfl/web/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     4493 2024-03-13 15:55:17.000000 RFL.web-1.0.0/rfl/web/tokens.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:16:04.518292 RFL.web-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:34:04.107856 rfl_web-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      834 2024-05-08 08:34:04.107856 rfl_web-1.0.1/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)       60 2023-10-20 06:39:29.000000 rfl_web-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:34:04.107856 rfl_web-1.0.1/RFL.web.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      834 2024-05-08 08:34:04.000000 rfl_web-1.0.1/RFL.web.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      216 2024-05-08 08:34:04.000000 rfl_web-1.0.1/RFL.web.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:34:04.000000 rfl_web-1.0.1/RFL.web.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       35 2024-05-08 08:34:04.000000 rfl_web-1.0.1/RFL.web.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:34:04.000000 rfl_web-1.0.1/RFL.web.egg-info/top_level.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      931 2024-05-08 07:35:07.000000 rfl_web-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:34:04.103856 rfl_web-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:34:04.107856 rfl_web-1.0.1/rfl/web/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-11 08:10:30.000000 rfl_web-1.0.1/rfl/web/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4493 2024-03-13 15:55:17.000000 rfl_web-1.0.1/rfl/web/tokens.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:34:04.107856 rfl_web-1.0.1/setup.cfg
```

### Comparing `RFL.web-1.0.0/PKG-INFO` & `rfl_web-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.web
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: web package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.web-1.0.0/RFL.web.egg-info/PKG-INFO` & `rfl_web-1.0.1/RFL.web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.web
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: web package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.web-1.0.0/pyproject.toml` & `rfl_web-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.web"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: web package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.web-1.0.0/rfl/web/tokens.py` & `rfl_web-1.0.1/rfl/web/tokens.py`

 * *Files identical despite different names*

