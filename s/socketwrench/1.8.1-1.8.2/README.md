# Comparing `tmp/socketwrench-1.8.1.tar.gz` & `tmp/socketwrench-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.1.tar", last modified: Tue May  7 19:02:27 2024, max compression
+gzip compressed data, was "socketwrench-1.8.2.tar", last modified: Wed May  8 16:00:55 2024, max compression
```

## Comparing `socketwrench-1.8.1.tar` & `socketwrench-1.8.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-07 19:02:22.000000 socketwrench-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 19:02:22.000000 socketwrench-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-07 19:02:27.365853 socketwrench-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-07 19:02:22.000000 socketwrench-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 19:02:22.000000 socketwrench-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:02:27.365853 socketwrench-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.357853 socketwrench-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.361853 socketwrench-1.8.1/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-07 19:02:22.000000 socketwrench-1.8.1/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:27.365853 socketwrench-1.8.1/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 19:02:27.000000 socketwrench-1.8.1/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-08 16:00:49.000000 socketwrench-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:00:49.000000 socketwrench-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-08 16:00:55.440589 socketwrench-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-08 16:00:49.000000 socketwrench-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 16:00:49.000000 socketwrench-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:00:55.440589 socketwrench-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.432589 socketwrench-1.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.1/LICENSE` & `socketwrench-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/PKG-INFO` & `socketwrench-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.1/README.md` & `socketwrench-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/pyproject.toml` & `socketwrench-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.1"
+version = "1.8.2"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.1/src/socketwrench/__init__.py` & `socketwrench-1.8.2/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/__main__.py` & `socketwrench-1.8.2/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/connection.py` & `socketwrench-1.8.2/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/handlers.py` & `socketwrench-1.8.2/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/openapi.py` & `socketwrench-1.8.2/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.2/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.2/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.2/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.2/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.2/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.2/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/samples/sample.py` & `socketwrench-1.8.2/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/server.py` & `socketwrench-1.8.2/src/socketwrench/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     default_port = 8080
     default_host = ''
     default_backlog = 1
     default_chunk_size = Connection.default_chunk_size
     default_num_connection_threads = 1
     default_socket_options = None
     default_pause_sleep = 0.1
-    default_accept_sleep = 0.1
+    default_accept_sleep = 0
     default_favicon = RouteHandler.default_favicon
 
     def __init__(self,
                  routes: dict | None = None,
                  port: int = default_port,
                  host: str = default_host,
                  backlog: int = default_backlog,
```

### Comparing `socketwrench-1.8.1/src/socketwrench/tags.py` & `socketwrench-1.8.2/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench/types.py` & `socketwrench-1.8.2/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.1/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.2/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.1/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.2/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

