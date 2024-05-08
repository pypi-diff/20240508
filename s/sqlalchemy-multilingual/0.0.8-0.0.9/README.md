# Comparing `tmp/sqlalchemy_multilingual-0.0.8.tar.gz` & `tmp/sqlalchemy_multilingual-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_multilingual-0.0.8.tar", last modified: Mon May  6 10:48:42 2024, max compression
+gzip compressed data, was "sqlalchemy_multilingual-0.0.9.tar", last modified: Mon May  6 10:50:27 2024, max compression
```

## Comparing `sqlalchemy_multilingual-0.0.8.tar` & `sqlalchemy_multilingual-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-06 10:48:42.287529 sqlalchemy_multilingual-0.0.8/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy_multilingual-0.0.8/LICENSE.txt
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy_multilingual-0.0.8/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-06 10:48:42.287591 sqlalchemy_multilingual-0.0.8/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy_multilingual-0.0.8/README.md
--rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-06 10:48:41.000000 sqlalchemy_multilingual-0.0.8/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-06 10:48:42.287825 sqlalchemy_multilingual-0.0.8/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:29:38.000000 sqlalchemy_multilingual-0.0.8/setup.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-06 10:48:42.287434 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-06 10:48:42.000000 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-06 10:48:42.000000 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-06 10:48:42.000000 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-06 10:48:42.000000 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-06 10:48:42.000000 sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-06 10:50:27.983353 sqlalchemy_multilingual-0.0.9/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy_multilingual-0.0.9/LICENSE.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy_multilingual-0.0.9/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-06 10:50:27.983430 sqlalchemy_multilingual-0.0.9/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy_multilingual-0.0.9/README.md
+-rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-06 10:50:24.000000 sqlalchemy_multilingual-0.0.9/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-06 10:50:27.983710 sqlalchemy_multilingual-0.0.9/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      161 2024-05-06 10:50:17.000000 sqlalchemy_multilingual-0.0.9/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-06 10:50:27.983257 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-06 10:50:27.000000 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-06 10:50:27.000000 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-06 10:50:27.000000 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-06 10:50:27.000000 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-06 10:50:27.000000 sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/top_level.txt
```

### Comparing `sqlalchemy_multilingual-0.0.8/LICENSE.txt` & `sqlalchemy_multilingual-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_multilingual-0.0.8/PKG-INFO` & `sqlalchemy_multilingual-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_multilingual
-Version: 0.0.8
+Version: 0.0.9
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqlalchemy_multilingual-0.0.8/pyproject.toml` & `sqlalchemy_multilingual-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy_multilingual"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sqlalchemy_multilingual-0.0.8/setup.cfg` & `sqlalchemy_multilingual-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy_multilingual
-version = 0.0.8
+version = 0.0.9
 description = ""
 long_description = file: README.md
 author = Kosenko Viktor
 author_email = kosenkoviktor11@gmail.com
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
```

### Comparing `sqlalchemy_multilingual-0.0.8/sqlalchemy_multilingual.egg-info/PKG-INFO` & `sqlalchemy_multilingual-0.0.9/sqlalchemy_multilingual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-multilingual
-Version: 0.0.8
+Version: 0.0.9
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

