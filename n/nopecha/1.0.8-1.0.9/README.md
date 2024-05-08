# Comparing `tmp/nopecha-1.0.8.tar.gz` & `tmp/nopecha-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopecha-1.0.8.tar", last modified: Fri Mar 24 19:09:53 2023, max compression
+gzip compressed data, was "nopecha-1.0.9.tar", last modified: Wed May  8 13:16:41 2024, max compression
```

## Comparing `nopecha-1.0.8.tar` & `nopecha-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jae       (1000) users      (985)        0 2023-03-24 19:09:53.818298 nopecha-1.0.8/
--rw-r--r--   0 jae       (1000) users      (985)     1064 2022-12-02 18:19:51.000000 nopecha-1.0.8/LICENSE
--rw-r--r--   0 jae       (1000) users      (985)     2465 2023-03-24 19:09:53.818298 nopecha-1.0.8/PKG-INFO
--rw-r--r--   0 jae       (1000) users      (985)     1921 2022-12-02 23:14:22.000000 nopecha-1.0.8/README.md
--rw-r--r--   0 jae       (1000) users      (985)      610 2023-03-24 18:56:44.000000 nopecha-1.0.8/pyproject.toml
--rw-r--r--   0 jae       (1000) users      (985)       38 2023-03-24 19:09:53.818298 nopecha-1.0.8/setup.cfg
-drwxr-xr-x   0 jae       (1000) users      (985)        0 2023-03-24 19:09:53.818298 nopecha-1.0.8/src/
-drwxr-xr-x   0 jae       (1000) users      (985)        0 2023-03-24 19:09:53.818298 nopecha-1.0.8/src/nopecha/
--rw-r--r--   0 jae       (1000) users      (985)      758 2022-12-02 23:13:36.000000 nopecha-1.0.8/src/nopecha/__init__.py
--rw-r--r--   0 jae       (1000) users      (985)     6010 2022-12-02 20:02:57.000000 nopecha-1.0.8/src/nopecha/api_requestor.py
--rw-r--r--   0 jae       (1000) users      (985)      906 2022-12-02 19:53:54.000000 nopecha-1.0.8/src/nopecha/error.py
--rw-r--r--   0 jae       (1000) users      (985)     1867 2022-12-03 00:21:32.000000 nopecha-1.0.8/src/nopecha/nopecha.py
--rw-r--r--   0 jae       (1000) users      (985)     3210 2022-12-02 19:24:17.000000 nopecha-1.0.8/src/nopecha/nopecha_object.py
-drwxr-xr-x   0 jae       (1000) users      (985)        0 2023-03-24 19:09:53.818298 nopecha-1.0.8/src/nopecha.egg-info/
--rw-r--r--   0 jae       (1000) users      (985)     2465 2023-03-24 19:09:53.000000 nopecha-1.0.8/src/nopecha.egg-info/PKG-INFO
--rw-r--r--   0 jae       (1000) users      (985)      299 2023-03-24 19:09:53.000000 nopecha-1.0.8/src/nopecha.egg-info/SOURCES.txt
--rw-r--r--   0 jae       (1000) users      (985)        1 2023-03-24 19:09:53.000000 nopecha-1.0.8/src/nopecha.egg-info/dependency_links.txt
--rw-r--r--   0 jae       (1000) users      (985)        8 2023-03-24 19:09:53.000000 nopecha-1.0.8/src/nopecha.egg-info/top_level.txt
+drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.132273 nopecha-1.0.9/
+-rw-r--r--   0 jae       (1000) jae       (1000)     1064 2023-10-25 05:59:14.000000 nopecha-1.0.9/LICENSE
+-rw-r--r--   0 jae       (1000) jae       (1000)     2465 2024-05-08 13:16:41.132273 nopecha-1.0.9/PKG-INFO
+-rw-r--r--   0 jae       (1000) jae       (1000)     1921 2023-10-25 05:59:14.000000 nopecha-1.0.9/README.md
+-rw-r--r--   0 jae       (1000) jae       (1000)      610 2024-05-08 12:19:04.000000 nopecha-1.0.9/pyproject.toml
+-rw-r--r--   0 jae       (1000) jae       (1000)       38 2024-05-08 13:16:41.135606 nopecha-1.0.9/setup.cfg
+drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.115606 nopecha-1.0.9/src/
+drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.125606 nopecha-1.0.9/src/nopecha/
+-rw-r--r--   0 jae       (1000) jae       (1000)      814 2024-05-08 11:19:46.000000 nopecha-1.0.9/src/nopecha/__init__.py
+-rw-r--r--   0 jae       (1000) jae       (1000)     6128 2024-05-08 11:19:15.000000 nopecha-1.0.9/src/nopecha/api_requestor.py
+-rw-r--r--   0 jae       (1000) jae       (1000)      962 2024-05-08 11:19:59.000000 nopecha-1.0.9/src/nopecha/error.py
+-rw-r--r--   0 jae       (1000) jae       (1000)     1857 2024-05-08 12:19:35.000000 nopecha-1.0.9/src/nopecha/nopecha.py
+-rw-r--r--   0 jae       (1000) jae       (1000)     3210 2023-10-25 05:59:14.000000 nopecha-1.0.9/src/nopecha/nopecha_object.py
+drwxr-xr-x   0 jae       (1000) jae       (1000)        0 2024-05-08 13:16:41.132273 nopecha-1.0.9/src/nopecha.egg-info/
+-rw-r--r--   0 jae       (1000) jae       (1000)     2465 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/PKG-INFO
+-rw-r--r--   0 jae       (1000) jae       (1000)      299 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/SOURCES.txt
+-rw-r--r--   0 jae       (1000) jae       (1000)        1 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/dependency_links.txt
+-rw-r--r--   0 jae       (1000) jae       (1000)        8 2024-05-08 13:16:41.000000 nopecha-1.0.9/src/nopecha.egg-info/top_level.txt
```

### Comparing `nopecha-1.0.8/LICENSE` & `nopecha-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nopecha-1.0.8/PKG-INFO` & `nopecha-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopecha
-Version: 1.0.8
+Version: 1.0.9
 Summary: NopeCHA Python Library
 Author-email: NopeCHA <nopechasolver@gmail.com>
 Project-URL: Homepage, https://nopecha.com
 Project-URL: Documentation, https://developers.nopecha.com
 Project-URL: GitHub Repository, https://github.com/NopeCHALLC/nopecha-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nopecha-1.0.8/README.md` & `nopecha-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nopecha-1.0.8/pyproject.toml` & `nopecha-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nopecha"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     {name="NopeCHA", email="nopechasolver@gmail.com"},
 ]
 description = "NopeCHA Python Library"
 readme = "README.md"
 requires-python = ">=3.7.1"
 classifiers = [
```

### Comparing `nopecha-1.0.8/src/nopecha/__init__.py` & `nopecha-1.0.9/src/nopecha/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from nopecha.nopecha import (
     Recognition,
     Token,
     Balance,
 )
-from nopecha.error import NopeCHAError, InvalidRequestError, IncompleteJobError, RateLimitError, AuthenticationError, InsufficientCreditError, UnknownError, Timeout, APIError, ServiceUnavailableError
+from nopecha.error import NopeCHAError, InvalidRequestError, IncompleteJobError, RateLimitError, AuthenticationError, UnavailableFeatureError, InsufficientCreditError, UnknownError, Timeout, APIError, ServiceUnavailableError
 
 api_base = os.environ.get("NOPECHA_API_BASE", "https://api.nopecha.com")
 api_key = os.environ.get("NOPECHA_API_KEY")
 proxy = None
 
 __all__ = [
     "Recognition",
@@ -17,14 +17,15 @@
     "Balance",
 
     "NopeCHAError",
     "InvalidRequestError",
     "IncompleteJobError",
     "RateLimitError",
     "AuthenticationError",
+    "UnavailableFeatureError",
     "InsufficientCreditError",
     "UnknownError",
     "Timeout",
     "APIError",
     "ServiceUnavailableError",
 
     "api_base",
```

### Comparing `nopecha-1.0.8/src/nopecha/api_requestor.py` & `nopecha-1.0.9/src/nopecha/api_requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         error_data = f"{resp['message']}" if "message" in resp else f"{resp['error']}"
         if rcode == 429:
             return error.RateLimitError(error_data, rbody, rcode, resp, rheaders)
         elif rcode == 400:
             return error.InvalidRequestError(error_data, rbody, rcode, resp, rheaders)
         elif rcode == 401:
             return error.AuthenticationError(error_data, rbody, rcode, resp, rheaders)
+        elif rcode == 402:
+            return error.UnavailableFeatureError(error_data, rbody, rcode, resp, rheaders)
         elif rcode == 403:
             return error.InsufficientCreditError(error_data, rbody, rcode, resp, rheaders)
         elif rcode == 409:
             return error.IncompleteJobError(error_data, rbody, rcode, resp, rheaders)
         else:
             return error.UnknownError(error_data, rbody, rcode, resp, rheaders)
```

### Comparing `nopecha-1.0.8/src/nopecha/error.py` & `nopecha-1.0.9/src/nopecha/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     pass
 
 
 class AuthenticationError(NopeCHAError):
     pass
 
 
+class UnavailableFeatureError(NopeCHAError):
+    pass
+
+
 class InsufficientCreditError(NopeCHAError):
     pass
 
 
 class UnknownError(NopeCHAError):
     pass
```

### Comparing `nopecha-1.0.8/src/nopecha/nopecha.py` & `nopecha-1.0.9/src/nopecha/nopecha.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import nopecha.error
 from nopecha.nopecha_object import NopeCHAObject
 
 
 class NopeCHARequest(NopeCHAObject):
     @classmethod
-    def get_url(self):
+    def get_url(cls):
         raise NotImplementedError()
 
     @classmethod
-    def get_retries(self):
+    def get_retries(cls):
         raise NotImplementedError()
 
     @classmethod
-    def get_interval(self):
+    def get_interval(cls):
         raise NotImplementedError()
 
     @classmethod
     def post(cls, **params):
         return cls().request("post", cls.get_url(), params)
 
     @classmethod
@@ -40,43 +40,43 @@
         if isinstance(r, nopecha.error.NopeCHAError):
             raise r
         return r['data']
 
 
 class Recognition(NopeCHARequest):
     @classmethod
-    def get_url(self):
+    def get_url(cls):
         return "/"
 
     @classmethod
-    def get_retries(self):
+    def get_retries(cls):
         return 120
 
     @classmethod
-    def get_interval(self):
+    def get_interval(cls):
         return 1
 
 
 class Token(NopeCHARequest):
     @classmethod
-    def get_url(self):
+    def get_url(cls):
         return "/token"
 
     @classmethod
-    def get_retries(self):
+    def get_retries(cls):
         return 180
 
     @classmethod
-    def get_interval(self):
+    def get_interval(cls):
         return 1
 
 
 class Balance(NopeCHAObject):
     @classmethod
-    def get_url(self):
+    def get_url(cls):
         return "/status"
 
     @classmethod
     def get(cls, **params):
         r = cls().request("get", cls.get_url(), params)
         if isinstance(r, nopecha.error.NopeCHAError):
             raise r
```

### Comparing `nopecha-1.0.8/src/nopecha/nopecha_object.py` & `nopecha-1.0.9/src/nopecha/nopecha_object.py`

 * *Files identical despite different names*

### Comparing `nopecha-1.0.8/src/nopecha.egg-info/PKG-INFO` & `nopecha-1.0.9/src/nopecha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopecha
-Version: 1.0.8
+Version: 1.0.9
 Summary: NopeCHA Python Library
 Author-email: NopeCHA <nopechasolver@gmail.com>
 Project-URL: Homepage, https://nopecha.com
 Project-URL: Documentation, https://developers.nopecha.com
 Project-URL: GitHub Repository, https://github.com/NopeCHALLC/nopecha-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

