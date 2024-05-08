# Comparing `tmp/RFL.authentication-1.0.0.tar.gz` & `tmp/rfl_authentication-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFL.authentication-1.0.0.tar", last modified: Mon Apr  8 13:13:03 2024, max compression
+gzip compressed data, was "rfl_authentication-1.0.1.tar", last modified: Wed May  8 08:31:01 2024, max compression
```

## Comparing `RFL.authentication-1.0.0.tar` & `rfl_authentication-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:13:03.790203 RFL.authentication-1.0.0/
--rw-r--r--   0 remi      (1000) remi      (1000)      868 2024-04-08 13:13:03.790203 RFL.authentication-1.0.0/PKG-INFO
--rw-r--r--   0 remi      (1000) remi      (1000)       65 2023-12-05 11:16:07.000000 RFL.authentication-1.0.0/README.md
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:13:03.790203 RFL.authentication-1.0.0/RFL.authentication.egg-info/
--rw-r--r--   0 remi      (1000) remi      (1000)      868 2024-04-08 13:13:03.000000 RFL.authentication-1.0.0/RFL.authentication.egg-info/PKG-INFO
--rw-rw-r--   0 remi      (1000) remi      (1000)      373 2024-04-08 13:13:03.000000 RFL.authentication-1.0.0/RFL.authentication.egg-info/SOURCES.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-04-08 13:13:03.000000 RFL.authentication-1.0.0/RFL.authentication.egg-info/dependency_links.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)       27 2024-04-08 13:13:03.000000 RFL.authentication-1.0.0/RFL.authentication.egg-info/requires.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-04-08 13:13:03.000000 RFL.authentication-1.0.0/RFL.authentication.egg-info/top_level.txt
--rw-rw-r--   0 remi      (1000) remi      (1000)      964 2024-04-08 09:20:29.000000 RFL.authentication-1.0.0/pyproject.toml
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:13:03.786203 RFL.authentication-1.0.0/rfl/
-drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-04-08 13:13:03.790203 RFL.authentication-1.0.0/rfl/authentication/
--rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-08 08:34:23.000000 RFL.authentication-1.0.0/rfl/authentication/__init__.py
--rw-r--r--   0 remi      (1000) remi      (1000)      498 2024-03-14 09:24:27.000000 RFL.authentication-1.0.0/rfl/authentication/errors.py
--rw-rw-r--   0 remi      (1000) remi      (1000)     6173 2024-03-26 21:55:38.000000 RFL.authentication-1.0.0/rfl/authentication/jwt.py
--rw-rw-r--   0 remi      (1000) remi      (1000)    12827 2024-04-03 11:48:36.000000 RFL.authentication-1.0.0/rfl/authentication/ldap.py
--rw-r--r--   0 remi      (1000) remi      (1000)      479 2024-03-25 10:19:46.000000 RFL.authentication-1.0.0/rfl/authentication/user.py
--rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-04-08 13:13:03.790203 RFL.authentication-1.0.0/setup.cfg
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/
+-rw-r--r--   0 remi      (1000) remi      (1000)      868 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)       65 2023-12-05 11:16:07.000000 rfl_authentication-1.0.1/README.md
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/RFL.authentication.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      868 2024-05-08 08:31:01.000000 rfl_authentication-1.0.1/RFL.authentication.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)      373 2024-05-08 08:31:01.000000 rfl_authentication-1.0.1/RFL.authentication.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-05-08 08:31:01.000000 rfl_authentication-1.0.1/RFL.authentication.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       27 2024-05-08 08:31:01.000000 rfl_authentication-1.0.1/RFL.authentication.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        4 2024-05-08 08:31:01.000000 rfl_authentication-1.0.1/RFL.authentication.egg-info/top_level.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      964 2024-05-08 07:35:37.000000 rfl_authentication-1.0.1/pyproject.toml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/rfl/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/rfl/authentication/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-09-08 08:34:23.000000 rfl_authentication-1.0.1/rfl/authentication/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      498 2024-03-14 09:24:27.000000 rfl_authentication-1.0.1/rfl/authentication/errors.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6173 2024-03-26 21:55:38.000000 rfl_authentication-1.0.1/rfl/authentication/jwt.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    12827 2024-04-03 11:48:36.000000 rfl_authentication-1.0.1/rfl/authentication/ldap.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      479 2024-03-25 10:19:46.000000 rfl_authentication-1.0.1/rfl/authentication/user.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       38 2024-05-08 08:31:01.343538 rfl_authentication-1.0.1/setup.cfg
```

### Comparing `RFL.authentication-1.0.0/PKG-INFO` & `rfl_authentication-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.authentication
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: authentication package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.authentication-1.0.0/RFL.authentication.egg-info/PKG-INFO` & `rfl_authentication-1.0.1/RFL.authentication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RFL.authentication
-Version: 1.0.0
+Version: 1.0.1
 Summary: Rackslab Foundation Library: authentication package
 Author-email: Rémi Palancher <remi@rackslab.io>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/rackslab/RFL
 Project-URL: Bug Tracker, https://github.com/rackslab/RFL/issues
 Keywords: utility,basic
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RFL.authentication-1.0.0/pyproject.toml` & `rfl_authentication-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RFL.authentication"
-version = "1.0.0"
+version = "1.0.1"
 description = "Rackslab Foundation Library: authentication package"
 license = {text = "GPLv3+"}
 requires-python = ">=3.6"
 keywords = ["utility", "basic"]
 authors = [
     {name = "Rémi Palancher", email = "remi@rackslab.io"},
 ]
```

### Comparing `RFL.authentication-1.0.0/rfl/authentication/jwt.py` & `rfl_authentication-1.0.1/rfl/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `RFL.authentication-1.0.0/rfl/authentication/ldap.py` & `rfl_authentication-1.0.1/rfl/authentication/ldap.py`

 * *Files identical despite different names*

