# Comparing `tmp/RFL.permissions-1.0.0.tar.gz` & `tmp/rfl_permissions-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.permissions-1.0.0.tar", last modified: Mon Apr  8 13:15:29 2024, max compression
+gzip compressed data, was "rfl_permissions-1.0.1.tar", last modified: Wed May  8 08:32:51 2024, max compression
```

## Comparing `RFL.permissions-1.0.0.tar` & `rfl_permissions-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      876 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)       71 2023-12-06 13:26:52.000000 RFL.permissions-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/RFL.permissions.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      876 2024-04-08 13:15:29.000000 RFL.permissions-1.0.0/RFL.permissions.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      296 2024-04-08 13:15:29.000000 RFL.permissions-1.0.0/RFL.permissions.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:15:29.000000 RFL.permissions-1.0.0/RFL.permissions.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       35 2024-04-08 13:15:29.000000 RFL.permissions-1.0.0/RFL.permissions.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:15:29.000000 RFL.permissions-1.0.0/RFL.permissions.egg-info/top_level.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)      963 2024-04-08 09:21:03.000000 RFL.permissions-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/rfl/permissions/
--rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-12-06 13:26:52.000000 RFL.permissions-1.0.0/rfl/permissions/__init__.py
--rw-rw-r--   0 remi      (1000) remi      (1000)      370 2023-12-06 13:26:52.000000 RFL.permissions-1.0.0/rfl/permissions/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     9113 2024-03-25 10:56:49.000000 RFL.permissions-1.0.0/rfl/permissions/rbac.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:15:29.710251 RFL.permissions-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      876 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)       71 2023-12-06 13:26:52.000000 rfl_permissions-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/RFL.permissions.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      876 2024-05-08 08:32:51.000000 rfl_permissions-1.0.1/RFL.permissions.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      296 2024-05-08 08:32:51.000000 rfl_permissions-1.0.1/RFL.permissions.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:32:51.000000 rfl_permissions-1.0.1/RFL.permissions.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       35 2024-05-08 08:32:51.000000 rfl_permissions-1.0.1/RFL.permissions.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:32:51.000000 rfl_permissions-1.0.1/RFL.permissions.egg-info/top_level.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      963 2024-05-08 07:35:18.000000 rfl_permissions-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/rfl/permissions/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2023-12-06 13:26:52.000000 rfl_permissions-1.0.1/rfl/permissions/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      370 2023-12-06 13:26:52.000000 rfl_permissions-1.0.1/rfl/permissions/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     9113 2024-03-25 10:56:49.000000 rfl_permissions-1.0.1/rfl/permissions/rbac.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:32:51.487228 rfl_permissions-1.0.1/setup.cfg
```

### Comparing `RFL.permissions-1.0.0/PKG-INFO` & `rfl_permissions-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.permissions
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: permissions package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.permissions-1.0.0/RFL.permissions.egg-info/PKG-INFO` & `rfl_permissions-1.0.1/RFL.permissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.permissions
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: permissions package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.permissions-1.0.0/pyproject.toml` & `rfl_permissions-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.permissions"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: permissions package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.permissions-1.0.0/rfl/permissions/rbac.py` & `rfl_permissions-1.0.1/rfl/permissions/rbac.py`

 * *Files identical despite different names*

