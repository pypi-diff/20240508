# Comparing `tmp/RFL.settings-1.0.0.tar.gz` & `tmp/rfl_settings-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.settings-1.0.0.tar", last modified: Mon Apr  8 13:15:47 2024, max compression
+gzip compressed data, was "rfl_settings-1.0.1.tar", last modified: Wed May  8 08:33:33 2024, max compression
```

## Comparing `RFL.settings-1.0.0.tar` & `rfl_settings-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:47.146272 RFL.settings-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      827 2024-04-08 13:15:47.146272 RFL.settings-1.0.0/PKG-INFO
--rw-r--r--   0 remi      (1000) remi      (1000)       62 2023-10-20 06:38:04.000000 RFL.settings-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:47.142272 RFL.settings-1.0.0/RFL.settings.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      827 2024-04-08 13:15:47.000000 RFL.settings-1.0.0/RFL.settings.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      351 2024-04-08 13:15:47.000000 RFL.settings-1.0.0/RFL.settings.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:15:47.000000 RFL.settings-1.0.0/RFL.settings.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       16 2024-04-08 13:15:47.000000 RFL.settings-1.0.0/RFL.settings.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:15:47.000000 RFL.settings-1.0.0/RFL.settings.egg-info/top_level.txt
--rw-r--r--   0 remi      (1000) remi      (1000)      929 2024-04-08 09:21:12.000000 RFL.settings-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:47.134272 RFL.settings-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:47.142272 RFL.settings-1.0.0/rfl/settings/
--rw-rw-r--   0 remi      (1000) remi      (1000)     6074 2023-12-11 10:43:33.000000 RFL.settings-1.0.0/rfl/settings/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     7077 2023-12-11 10:37:31.000000 RFL.settings-1.0.0/rfl/settings/definition.py
--rw-r--r--   0 remi      (1000) remi      (1000)      355 2023-10-19 09:59:49.000000 RFL.settings-1.0.0/rfl/settings/errors.py
--rw-r--r--   0 remi      (1000) remi      (1000)     1152 2023-09-08 08:36:43.000000 RFL.settings-1.0.0/rfl/settings/loaders.py
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:47.142272 RFL.settings-1.0.0/rfl/tests/
--rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-10-19 09:16:01.000000 RFL.settings-1.0.0/rfl/tests/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)    14720 2023-12-11 11:10:59.000000 RFL.settings-1.0.0/rfl/tests/test_settings.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:15:47.146272 RFL.settings-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      827 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)       62 2023-10-20 06:38:04.000000 rfl_settings-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/RFL.settings.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      827 2024-05-08 08:33:33.000000 rfl_settings-1.0.1/RFL.settings.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      351 2024-05-08 08:33:33.000000 rfl_settings-1.0.1/RFL.settings.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:33:33.000000 rfl_settings-1.0.1/RFL.settings.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       16 2024-05-08 08:33:33.000000 rfl_settings-1.0.1/RFL.settings.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:33:33.000000 rfl_settings-1.0.1/RFL.settings.egg-info/top_level.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)      929 2024-05-08 07:35:14.000000 rfl_settings-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:33:33.699545 rfl_settings-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/rfl/settings/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6074 2023-12-11 10:43:33.000000 rfl_settings-1.0.1/rfl/settings/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7077 2023-12-11 10:37:31.000000 rfl_settings-1.0.1/rfl/settings/definition.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      355 2023-10-19 09:59:49.000000 rfl_settings-1.0.1/rfl/settings/errors.py
+-rw-r--r--   0 remi      (1000) remi      (1000)     1152 2023-09-08 08:36:43.000000 rfl_settings-1.0.1/rfl/settings/loaders.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/rfl/tests/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-10-19 09:16:01.000000 rfl_settings-1.0.1/rfl/tests/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    14720 2023-12-11 11:10:59.000000 rfl_settings-1.0.1/rfl/tests/test_settings.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:33:33.703545 rfl_settings-1.0.1/setup.cfg
```

### Comparing `RFL.settings-1.0.0/PKG-INFO` & `rfl_settings-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.settings
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: settings package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.settings-1.0.0/RFL.settings.egg-info/PKG-INFO` & `rfl_settings-1.0.1/RFL.settings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.settings
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: settings package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.settings-1.0.0/pyproject.toml` & `rfl_settings-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.settings"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: settings package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.settings-1.0.0/rfl/settings/__init__.py` & `rfl_settings-1.0.1/rfl/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `RFL.settings-1.0.0/rfl/settings/definition.py` & `rfl_settings-1.0.1/rfl/settings/definition.py`

 * *Files identical despite different names*

### Comparing `RFL.settings-1.0.0/rfl/settings/loaders.py` & `rfl_settings-1.0.1/rfl/settings/loaders.py`

 * *Files identical despite different names*

### Comparing `RFL.settings-1.0.0/rfl/tests/test_settings.py` & `rfl_settings-1.0.1/rfl/tests/test_settings.py`

 * *Files identical despite different names*

