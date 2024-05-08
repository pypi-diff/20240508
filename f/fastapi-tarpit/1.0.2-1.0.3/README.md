# Comparing `tmp/fastapi_tarpit-1.0.2.tar.gz` & `tmp/fastapi_tarpit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_tarpit-1.0.2.tar", last modified: Sat May  4 21:00:15 2024, max compression
+gzip compressed data, was "fastapi_tarpit-1.0.3.tar", last modified: Wed May  8 19:19:37 2024, max compression
```

## Comparing `fastapi_tarpit-1.0.2.tar` & `fastapi_tarpit-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/
--rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/LICENSE
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/README.md
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/fastapi_tarpit/
--rw-rw-r--   0 mats      (1000) mats      (1000)      106 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/fastapi_tarpit/__init__.py
--rw-rw-r--   0 mats      (1000) mats      (1000)     5711 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/fastapi_tarpit/tarpit.py
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)      273 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/SOURCES.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/dependency_links.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/requires.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/top_level.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)      693 2024-05-04 21:00:05.000000 fastapi_tarpit-1.0.2/pyproject.toml
--rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/setup.cfg
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-04-16 21:29:58.000000 fastapi_tarpit-1.0.3/LICENSE
+-rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-04-25 19:23:39.000000 fastapi_tarpit-1.0.3/README.md
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/fastapi_tarpit/
+-rw-rw-r--   0 mats      (1000) mats      (1000)       87 2024-05-08 19:09:42.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/__init__.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)     3300 2024-05-08 19:15:16.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/client.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)      519 2024-05-08 19:02:19.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/config.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)     2221 2024-05-08 19:14:04.000000 fastapi_tarpit-1.0.3/fastapi_tarpit/middleware.py
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/
+-rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)      327 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/requires.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-05-08 19:19:37.000000 fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/top_level.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)      693 2024-05-08 19:17:04.000000 fastapi_tarpit-1.0.3/pyproject.toml
+-rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-05-08 19:19:37.276832 fastapi_tarpit-1.0.3/setup.cfg
```

### Comparing `fastapi_tarpit-1.0.2/LICENSE` & `fastapi_tarpit-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.2/PKG-INFO` & `fastapi_tarpit-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.2
+Version: 1.0.3
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_tarpit-1.0.2/README.md` & `fastapi_tarpit-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/PKG-INFO` & `fastapi_tarpit-1.0.3/fastapi_tarpit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.2
+Version: 1.0.3
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_tarpit-1.0.2/pyproject.toml` & `fastapi_tarpit-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi-tarpit"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Mats Klepsland", email="mats.klepsland@gmail.com" },
 ]
 dependencies = [
   "fastapi",
 ]
 description = "FastAPI middleware that purposely delays incoming connections on unused routes"
```

