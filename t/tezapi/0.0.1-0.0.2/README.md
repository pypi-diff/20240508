# Comparing `tmp/tezapi-0.0.1.tar.gz` & `tmp/tezapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tezapi-0.0.1.tar", last modified: Wed May  8 08:06:59 2024, max compression
+gzip compressed data, was "tezapi-0.0.2.tar", last modified: Wed May  8 08:22:37 2024, max compression
```

## Comparing `tezapi-0.0.1.tar` & `tezapi-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:06:59.316676 tezapi-0.0.1/
--rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4809 2024-05-08 08:06:59.314715 tezapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4192 2024-05-08 08:06:39.000000 tezapi-0.0.1/README.md
--rw-rw-rw-   0        0        0      710 2024-05-08 08:06:39.000000 tezapi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 08:06:59.316676 tezapi-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 08:06:59.225888 tezapi-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 08:06:59.251903 tezapi-0.0.1/src/tezapi/
--rw-rw-rw-   0        0        0       68 2024-05-07 15:49:43.000000 tezapi-0.0.1/src/tezapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:06:59.311188 tezapi-0.0.1/src/tezapi/exceptions/
--rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.1/src/tezapi/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.1/src/tezapi/exceptions/apiexception.py
--rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.1/src/tezapi/exceptions/base_exceptions.py
--rw-rw-rw-   0        0        0     1927 2024-05-08 08:00:45.000000 tezapi-0.0.1/src/tezapi/handle.py
--rw-rw-rw-   0        0        0     1394 2024-05-07 19:17:10.000000 tezapi-0.0.1/src/tezapi/responses.py
--rw-rw-rw-   0        0        0     2029 2024-05-08 08:00:45.000000 tezapi-0.0.1/src/tezapi/routes.py
--rw-rw-rw-   0        0        0     1482 2024-05-08 08:00:45.000000 tezapi-0.0.1/src/tezapi/schemas.py
--rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.1/src/tezapi/templating.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:06:59.311188 tezapi-0.0.1/src/tezapi.egg-info/
--rw-rw-rw-   0        0        0     4809 2024-05-08 08:06:59.000000 tezapi-0.0.1/src/tezapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2024-05-08 08:06:59.000000 tezapi-0.0.1/src/tezapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:06:59.000000 tezapi-0.0.1/src/tezapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 08:06:59.000000 tezapi-0.0.1/src/tezapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 08:06:59.000000 tezapi-0.0.1/src/tezapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4809 2024-05-08 08:22:37.637879 tezapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4192 2024-05-08 08:06:39.000000 tezapi-0.0.2/README.md
+-rw-rw-rw-   0        0        0      782 2024-05-08 08:22:26.000000 tezapi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:22:37.637879 tezapi-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.590159 tezapi-0.0.2/tezapi/
+-rw-rw-rw-   0        0        0       68 2024-05-07 15:49:43.000000 tezapi-0.0.2/tezapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/tezapi/exceptions/
+-rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.2/tezapi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.2/tezapi/exceptions/apiexception.py
+-rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/exceptions/base_exceptions.py
+-rw-rw-rw-   0        0        0     1927 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/handle.py
+-rw-rw-rw-   0        0        0     1394 2024-05-07 19:17:10.000000 tezapi-0.0.2/tezapi/responses.py
+-rw-rw-rw-   0        0        0     2029 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/routes.py
+-rw-rw-rw-   0        0        0     1482 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/schemas.py
+-rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/templating.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/tezapi.egg-info/
+-rw-rw-rw-   0        0        0     4809 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/top_level.txt
```

### Comparing `tezapi-0.0.1/LICENSE` & `tezapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/PKG-INFO` & `tezapi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tezapi-0.0.1/README.md` & `tezapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi/exceptions/apiexception.py` & `tezapi-0.0.2/tezapi/exceptions/apiexception.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi/handle.py` & `tezapi-0.0.2/tezapi/handle.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi/responses.py` & `tezapi-0.0.2/tezapi/responses.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi/routes.py` & `tezapi-0.0.2/tezapi/routes.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi/schemas.py` & `tezapi-0.0.2/tezapi/schemas.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.1/src/tezapi.egg-info/PKG-INFO` & `tezapi-0.0.2/tezapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

