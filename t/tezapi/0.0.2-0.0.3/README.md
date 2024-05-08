# Comparing `tmp/tezapi-0.0.2.tar.gz` & `tmp/tezapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tezapi-0.0.2.tar", last modified: Wed May  8 08:22:37 2024, max compression
+gzip compressed data, was "tezapi-0.0.3.tar", last modified: Wed May  8 08:47:09 2024, max compression
```

## Comparing `tezapi-0.0.2.tar` & `tezapi-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/
--rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4809 2024-05-08 08:22:37.637879 tezapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4192 2024-05-08 08:06:39.000000 tezapi-0.0.2/README.md
--rw-rw-rw-   0        0        0      782 2024-05-08 08:22:26.000000 tezapi-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 08:22:37.637879 tezapi-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.590159 tezapi-0.0.2/tezapi/
--rw-rw-rw-   0        0        0       68 2024-05-07 15:49:43.000000 tezapi-0.0.2/tezapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/tezapi/exceptions/
--rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.2/tezapi/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.2/tezapi/exceptions/apiexception.py
--rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/exceptions/base_exceptions.py
--rw-rw-rw-   0        0        0     1927 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/handle.py
--rw-rw-rw-   0        0        0     1394 2024-05-07 19:17:10.000000 tezapi-0.0.2/tezapi/responses.py
--rw-rw-rw-   0        0        0     2029 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/routes.py
--rw-rw-rw-   0        0        0     1482 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/schemas.py
--rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.2/tezapi/templating.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:22:37.637879 tezapi-0.0.2/tezapi.egg-info/
--rw-rw-rw-   0        0        0     4809 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 08:22:37.000000 tezapi-0.0.2/tezapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:47:09.706714 tezapi-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4809 2024-05-08 08:47:09.706714 tezapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4192 2024-05-08 08:46:11.000000 tezapi-0.0.3/README.md
+-rw-rw-rw-   0        0        0      782 2024-05-08 08:46:50.000000 tezapi-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:47:09.706714 tezapi-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:47:09.657848 tezapi-0.0.3/tezapi/
+-rw-rw-rw-   0        0        0       68 2024-05-08 08:43:10.000000 tezapi-0.0.3/tezapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:47:09.706714 tezapi-0.0.3/tezapi/exceptions/
+-rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.3/tezapi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.3/tezapi/exceptions/apiexception.py
+-rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.3/tezapi/exceptions/base_exceptions.py
+-rw-rw-rw-   0        0        0     1927 2024-05-08 08:43:10.000000 tezapi-0.0.3/tezapi/handle.py
+-rw-rw-rw-   0        0        0     1394 2024-05-07 19:17:10.000000 tezapi-0.0.3/tezapi/responses.py
+-rw-rw-rw-   0        0        0     2029 2024-05-08 08:00:45.000000 tezapi-0.0.3/tezapi/routes.py
+-rw-rw-rw-   0        0        0     1482 2024-05-08 08:00:45.000000 tezapi-0.0.3/tezapi/schemas.py
+-rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.3/tezapi/templating.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:47:09.706714 tezapi-0.0.3/tezapi.egg-info/
+-rw-rw-rw-   0        0        0     4809 2024-05-08 08:47:09.000000 tezapi-0.0.3/tezapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-08 08:47:09.000000 tezapi-0.0.3/tezapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:47:09.000000 tezapi-0.0.3/tezapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 08:47:09.000000 tezapi-0.0.3/tezapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 08:47:09.000000 tezapi-0.0.3/tezapi.egg-info/top_level.txt
```

### Comparing `tezapi-0.0.2/LICENSE` & `tezapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.2/PKG-INFO` & `tezapi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,20 @@
 
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
-from tezapi import AioAPI, Request
+from tezapi import TezAPI, Request
 from tezapi.exceptions import APIError, ClassBaseError
 from tezapi.schemas import SchemaModel
 from tezapi.templating import Jinja2Template
 
-app = AioAPI()
+app = TezAPI()
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return "Hello, aiohttp-api!"
```

### Comparing `tezapi-0.0.2/README.md` & `tezapi-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
-from tezapi import AioAPI, Request
+from tezapi import TezAPI, Request
 from tezapi.exceptions import APIError, ClassBaseError
 from tezapi.schemas import SchemaModel
 from tezapi.templating import Jinja2Template
 
-app = AioAPI()
+app = TezAPI()
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return "Hello, aiohttp-api!"
```

### Comparing `tezapi-0.0.2/pyproject.toml` & `tezapi-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 [project]
 dependencies = [
     "aiohttp~=3.9.5",
     "jinja2~=3.1.4"
 ]
 name = "tezapi"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "dev-au", email = "devaubusiness@gmail.com" },
 ]
 description = "Asynchronous web framework for building powerful web APIs and applications with Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tezapi-0.0.2/tezapi/exceptions/apiexception.py` & `tezapi-0.0.3/tezapi/exceptions/apiexception.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.2/tezapi/handle.py` & `tezapi-0.0.3/tezapi/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aiohttp import web
 from aiohttp.web_request import Request
 
 from .routes import Route
 
 
-class AioAPI(web.Application):
+class TezAPI(web.Application):
     def __init__(self, host: str = '127.0.0.1', port: int = 8000, **kwargs):
         self.host = host
         self.port = port
         self.routes = []
         super().__init__(**kwargs)
 
     def _add_route(self, path, handler, method: str, **kwargs):
```

### Comparing `tezapi-0.0.2/tezapi/responses.py` & `tezapi-0.0.3/tezapi/responses.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.2/tezapi/routes.py` & `tezapi-0.0.3/tezapi/routes.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.2/tezapi/schemas.py` & `tezapi-0.0.3/tezapi/schemas.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.2/tezapi.egg-info/PKG-INFO` & `tezapi-0.0.3/tezapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,20 @@
 
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
-from tezapi import AioAPI, Request
+from tezapi import TezAPI, Request
 from tezapi.exceptions import APIError, ClassBaseError
 from tezapi.schemas import SchemaModel
 from tezapi.templating import Jinja2Template
 
-app = AioAPI()
+app = TezAPI()
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return "Hello, aiohttp-api!"
```

