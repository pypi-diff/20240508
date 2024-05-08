# Comparing `tmp/RFL.log-1.0.0.tar.gz` & `tmp/rfl_log-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.log-1.0.0.tar", last modified: Mon Apr  8 13:15:05 2024, max compression
+gzip compressed data, was "rfl_log-1.0.1.tar", last modified: Wed May  8 08:32:24 2024, max compression
```

## Comparing `RFL.log-1.0.0.tar` & `rfl_log-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:05.486220 RFL.log-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      746 2024-04-08 13:15:05.486220 RFL.log-1.0.0/PKG-INFO
--rw-r--r--   0 remi      (1000) remi      (1000)       37 2024-03-15 10:33:25.000000 RFL.log-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:05.486220 RFL.log-1.0.0/RFL.log.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      746 2024-04-08 13:15:05.000000 RFL.log-1.0.0/RFL.log.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      190 2024-04-08 13:15:05.000000 RFL.log-1.0.0/RFL.log.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:15:05.000000 RFL.log-1.0.0/RFL.log.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:15:05.000000 RFL.log-1.0.0/RFL.log.egg-info/top_level.txt
--rw-r--r--   0 remi      (1000) remi      (1000)      882 2024-04-08 09:20:54.000000 RFL.log-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:05.478220 RFL.log-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:05.486220 RFL.log-1.0.0/rfl/log/
--rw-rw-r--   0 remi      (1000) remi      (1000)     2505 2024-03-12 19:51:35.000000 RFL.log-1.0.0/rfl/log/__init__.py
--rw-r--r--   0 remi      (1000) remi      (1000)     2034 2024-03-11 09:18:24.000000 RFL.log-1.0.0/rfl/log/formatters.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:15:05.486220 RFL.log-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:24.787304 rfl_log-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      746 2024-05-08 08:32:24.787304 rfl_log-1.0.1/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)       37 2024-03-15 10:33:25.000000 rfl_log-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:24.787304 rfl_log-1.0.1/RFL.log.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      746 2024-05-08 08:32:24.000000 rfl_log-1.0.1/RFL.log.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      190 2024-05-08 08:32:24.000000 rfl_log-1.0.1/RFL.log.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:32:24.000000 rfl_log-1.0.1/RFL.log.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:32:24.000000 rfl_log-1.0.1/RFL.log.egg-info/top_level.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)      882 2024-05-08 07:35:23.000000 rfl_log-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:24.787304 rfl_log-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:24.787304 rfl_log-1.0.1/rfl/log/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2505 2024-03-12 19:51:35.000000 rfl_log-1.0.1/rfl/log/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)     2034 2024-03-11 09:18:24.000000 rfl_log-1.0.1/rfl/log/formatters.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:32:24.787304 rfl_log-1.0.1/setup.cfg
```

### Comparing `RFL.log-1.0.0/PKG-INFO` & `rfl_log-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.log
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: log package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.log-1.0.0/RFL.log.egg-info/PKG-INFO` & `rfl_log-1.0.1/RFL.log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.log
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: log package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.log-1.0.0/pyproject.toml` & `rfl_log-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.log"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: log package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.log-1.0.0/rfl/log/__init__.py` & `rfl_log-1.0.1/rfl/log/__init__.py`

 * *Files identical despite different names*

### Comparing `RFL.log-1.0.0/rfl/log/formatters.py` & `rfl_log-1.0.1/rfl/log/formatters.py`

 * *Files identical despite different names*

