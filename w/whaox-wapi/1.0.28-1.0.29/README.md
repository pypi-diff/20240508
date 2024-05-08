# Comparing `tmp/whaox-wapi-1.0.28.tar.gz` & `tmp/whaox-wapi-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.28.tar", last modified: Mon Apr 15 09:37:41 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.29.tar", last modified: Wed May  8 17:41:34 2024, max compression
```

## Comparing `whaox-wapi-1.0.28.tar` & `whaox-wapi-1.0.29.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.200803 whaox-wapi-1.0.28/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.28/LICENSE
--rw-rw-rw-   0        0        0     2931 2024-04-15 09:37:41.199941 whaox-wapi-1.0.28/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2024-04-15 09:18:10.000000 whaox-wapi-1.0.28/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 09:37:41.200803 whaox-wapi-1.0.28/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-15 09:37:37.000000 whaox-wapi-1.0.28/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.161563 whaox-wapi-1.0.28/wapi/
--rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.28/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.164871 whaox-wapi-1.0.28/wapi/features/
--rw-rw-rw-   0        0        0     1001 2024-04-15 09:36:06.000000 whaox-wapi-1.0.28/wapi/features/GET.py
--rw-rw-rw-   0        0        0      847 2024-04-15 09:37:37.000000 whaox-wapi-1.0.28/wapi/features/POST.py
--rw-rw-rw-   0        0        0      939 2024-04-11 20:45:55.000000 whaox-wapi-1.0.28/wapi/features/Route.py
--rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.28/wapi/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.169898 whaox-wapi-1.0.28/wapi/static/
--rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.28/wapi/static/T.py
--rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.28/wapi/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.173048 whaox-wapi-1.0.28/wapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.28/wapi/utils/__init__.py
--rw-rw-rw-   0        0        0      307 2024-04-11 20:01:35.000000 whaox-wapi-1.0.28/wapi/utils/get_path.py
--rw-rw-rw-   0        0        0       56 2024-04-11 20:01:35.000000 whaox-wapi-1.0.28/wapi/utils/is_class.py
--rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.28/wapi/utils/is_dataclass.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:37:41.195689 whaox-wapi-1.0.28/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2931 2024-04-15 09:37:41.000000 whaox-wapi-1.0.28/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-04-15 09:37:41.000000 whaox-wapi-1.0.28/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:37:41.000000 whaox-wapi-1.0.28/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 09:37:41.000000 whaox-wapi-1.0.28/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 09:37:41.000000 whaox-wapi-1.0.28/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.457036 whaox-wapi-1.0.29/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.29/LICENSE
+-rw-rw-rw-   0        0        0     3020 2024-05-08 17:41:34.455539 whaox-wapi-1.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0     2632 2024-04-15 10:27:15.000000 whaox-wapi-1.0.29/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 17:41:34.458047 whaox-wapi-1.0.29/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-05-08 17:41:06.000000 whaox-wapi-1.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.371553 whaox-wapi-1.0.29/wapi/
+-rw-rw-rw-   0        0        0       27 2024-04-15 09:31:56.000000 whaox-wapi-1.0.29/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.381885 whaox-wapi-1.0.29/wapi/features/
+-rw-rw-rw-   0        0        0     1001 2024-04-15 09:36:06.000000 whaox-wapi-1.0.29/wapi/features/GET.py
+-rw-rw-rw-   0        0        0      797 2024-05-08 17:41:06.000000 whaox-wapi-1.0.29/wapi/features/POST.py
+-rw-rw-rw-   0        0        0      941 2024-04-15 11:14:57.000000 whaox-wapi-1.0.29/wapi/features/Route.py
+-rw-rw-rw-   0        0        0       72 2024-04-12 10:19:11.000000 whaox-wapi-1.0.29/wapi/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.384340 whaox-wapi-1.0.29/wapi/static/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/static/T.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:20:58.000000 whaox-wapi-1.0.29/wapi/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.413298 whaox-wapi-1.0.29/wapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 09:21:14.000000 whaox-wapi-1.0.29/wapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      307 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/get_path.py
+-rw-rw-rw-   0        0        0       56 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/is_class.py
+-rw-rw-rw-   0        0        0      124 2024-04-11 20:01:35.000000 whaox-wapi-1.0.29/wapi/utils/is_dataclass.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:41:34.454537 whaox-wapi-1.0.29/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     3020 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 17:41:34.000000 whaox-wapi-1.0.29/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.28/LICENSE` & `whaox-wapi-1.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.28/PKG-INFO` & `whaox-wapi-1.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.28
+Version: 1.0.29
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
+
 # WApi: Web-Library for Python
 
 [![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
+## Features
 
+* Routes
+* Serialization
+* Params
+	* Auto-Complete
+	* Unpaking
 ## Installation
 
  You can install the latest version with the command:
  
 ```commandline
 pip install whaox-wapi
 ```
 
-## • Routes 
+## • Routes #routes
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
 
 @Route("https://example.com")
 class WApi:
@@ -53,15 +60,15 @@
 ```python 
 wapi = WApi()
 wapi.service.get()
 # eq
 requests.get("https://example.com/wapi/path/")
 ```
 
-## • Serialization 
+## • Serialization
 
 > The library deserializes the received data according to the type that you specify in the \_T parameter of the decorator. 
 > 
 > NOTE: The specified type must be json serializable - these are the base types and classes marked with the @dataclass annotation
 
 ```python
```

### Comparing `whaox-wapi-1.0.28/README.md` & `whaox-wapi-1.0.29/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+
 # WApi: Web-Library for Python
 
 [![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
+## Features
 
+* Routes
+* Serialization
+* Params
+	* Auto-Complete
+	* Unpaking
 ## Installation
 
  You can install the latest version with the command:
  
 ```commandline
 pip install whaox-wapi
 ```
 
-## • Routes 
+## • Routes #routes
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
 
 @Route("https://example.com")
 class WApi:
@@ -39,15 +46,15 @@
 ```python 
 wapi = WApi()
 wapi.service.get()
 # eq
 requests.get("https://example.com/wapi/path/")
 ```
 
-## • Serialization 
+## • Serialization
 
 > The library deserializes the received data according to the type that you specify in the \_T parameter of the decorator. 
 > 
 > NOTE: The specified type must be json serializable - these are the base types and classes marked with the @dataclass annotation
 
 ```python
```

### Comparing `whaox-wapi-1.0.28/setup.py` & `whaox-wapi-1.0.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.28'
+version = '1.0.29'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.28/wapi/features/GET.py` & `whaox-wapi-1.0.29/wapi/features/GET.py`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.28/wapi/features/POST.py` & `whaox-wapi-1.0.29/wapi/features/POST.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         def wrapper(self, **kwargs):
             headers = kwargs.pop('headers', None)
             data = dict()
 
             if body := dump(kwargs.pop('body', None)):
                 data.update(body)
 
-            if not kwargs:
-                data.update(kwargs)
-
-            url = get_path(self, func, path)
+            url = get_path(self, func, path).format(**kwargs)
             response = post(url, json=data, headers=headers)
 
             if _T is None:
                 return response
             return load(response.json(), _T)
 
         return wrapper
```

### Comparing `whaox-wapi-1.0.28/wapi/features/Route.py` & `whaox-wapi-1.0.29/wapi/features/Route.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
             return obj(self, *args, **kwargs)
 
         if is_class(obj):
             return class_wrapper()
         return func_wrapper
 
-    return decorator
+    return decorator
```

### Comparing `whaox-wapi-1.0.28/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.29/whaox_wapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.28
+Version: 1.0.29
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Keywords: python,web,api,requests,post,get
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
+
 # WApi: Web-Library for Python
 
 [![PyPI version](https://badge.fury.io/py/whaox-wapi.svg)](https://badge.fury.io/py/whaox-wapi)
 
 ## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
+## Features
 
+* Routes
+* Serialization
+* Params
+	* Auto-Complete
+	* Unpaking
 ## Installation
 
  You can install the latest version with the command:
  
 ```commandline
 pip install whaox-wapi
 ```
 
-## • Routes 
+## • Routes #routes
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
 
 @Route("https://example.com")
 class WApi:
@@ -53,15 +60,15 @@
 ```python 
 wapi = WApi()
 wapi.service.get()
 # eq
 requests.get("https://example.com/wapi/path/")
 ```
 
-## • Serialization 
+## • Serialization
 
 > The library deserializes the received data according to the type that you specify in the \_T parameter of the decorator. 
 > 
 > NOTE: The specified type must be json serializable - these are the base types and classes marked with the @dataclass annotation
 
 ```python
```

