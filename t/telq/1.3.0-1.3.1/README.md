# Comparing `tmp/telq-1.3.0.tar.gz` & `tmp/telq-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telq-1.3.0.tar", max compression
+gzip compressed data, was "telq-1.3.1.tar", max compression
```

## Comparing `telq-1.3.0.tar` & `telq-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11345 2024-04-11 08:27:49.459812 telq-1.3.0/LICENSE
--rwxr-xr-x   0        0        0      461 2024-04-11 08:27:49.459812 telq-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-11 08:27:49.459812 telq-1.3.0/telq/.DS_Store
--rwxr-xr-x   0        0        0     6325 2024-04-11 08:27:49.459812 telq-1.3.0/telq/__init__.py
--rwxr-xr-x   0        0        0     3490 2024-04-11 08:27:49.463812 telq-1.3.0/telq/authentication/__init__.py
--rwxr-xr-x   0        0        0     4481 2024-04-11 08:27:49.463812 telq-1.3.0/telq/endpoints/__init__.py
--rwxr-xr-x   0        0        0     2004 2024-04-11 08:27:49.463812 telq-1.3.0/telq/networks/__init__.py
--rwxr-xr-x   0        0        0     5066 2024-04-11 08:27:49.463812 telq-1.3.0/telq/session/__init__.py
--rw-r--r--   0        0        0     1685 2024-04-11 08:27:49.463812 telq-1.3.0/telq/session/session_data.py
--rwxr-xr-x   0        0        0     6376 2024-04-11 08:27:49.463812 telq-1.3.0/telq/supplier/__init__.py
--rw-r--r--   0        0        0     1514 2024-04-11 08:27:49.463812 telq-1.3.0/telq/supplier/supplier_data.py
--rwxr-xr-x   0        0        0       94 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/__init__.py
--rwxr-xr-x   0        0        0     7267 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/lnt.py
--rw-r--r--   0        0        0      277 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/model.py
--rwxr-xr-x   0        0        0     5051 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/mt.py
--rw-r--r--   0        0        0     1876 2024-04-11 08:27:49.463812 telq-1.3.0/telq/util/rest.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 telq-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-08 12:17:51.315054 telq-1.3.1/LICENSE
+-rwxr-xr-x   0        0        0      461 2024-05-08 12:17:51.315054 telq-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-08 12:17:51.315054 telq-1.3.1/telq/.DS_Store
+-rwxr-xr-x   0        0        0     6325 2024-05-08 12:17:51.315054 telq-1.3.1/telq/__init__.py
+-rwxr-xr-x   0        0        0     3026 2024-05-08 12:17:51.315054 telq-1.3.1/telq/authentication/__init__.py
+-rwxr-xr-x   0        0        0     4481 2024-05-08 12:17:51.315054 telq-1.3.1/telq/endpoints/__init__.py
+-rwxr-xr-x   0        0        0     2004 2024-05-08 12:17:51.315054 telq-1.3.1/telq/networks/__init__.py
+-rwxr-xr-x   0        0        0     5066 2024-05-08 12:17:51.319054 telq-1.3.1/telq/session/__init__.py
+-rw-r--r--   0        0        0     1685 2024-05-08 12:17:51.319054 telq-1.3.1/telq/session/session_data.py
+-rwxr-xr-x   0        0        0     6376 2024-05-08 12:17:51.319054 telq-1.3.1/telq/supplier/__init__.py
+-rw-r--r--   0        0        0     1514 2024-05-08 12:17:51.319054 telq-1.3.1/telq/supplier/supplier_data.py
+-rwxr-xr-x   0        0        0       94 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/__init__.py
+-rwxr-xr-x   0        0        0     7267 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/lnt.py
+-rw-r--r--   0        0        0      277 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/model.py
+-rwxr-xr-x   0        0        0     5051 2024-05-08 12:17:51.319054 telq-1.3.1/telq/tests/mt.py
+-rw-r--r--   0        0        0     1369 2024-05-08 12:17:51.319054 telq-1.3.1/telq/util/rest.py
+-rw-r--r--   0        0        0       20 2024-05-08 12:17:51.319054 telq-1.3.1/telq/util/version.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 telq-1.3.1/PKG-INFO
```

### Comparing `telq-1.3.0/LICENSE` & `telq-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/.DS_Store` & `telq-1.3.1/telq/.DS_Store`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/__init__.py` & `telq-1.3.1/telq/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/authentication/__init__.py` & `telq-1.3.1/telq/authentication/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from dataclasses import dataclass
 import warnings
 import toml
 import requests
 import telq.endpoints as endpoints
+from telq.util.version import SDK_VERSION
 
 
 @dataclass
 class Authentication:
     """Performs authentication with the App Id and App Key
     The App Id and App Key is validated with the token endpoint
 
@@ -38,34 +39,20 @@
     base_url: str
     api_version: str = "v3"
 
     def __post_init__(self) -> None:
         self.headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
-            "User-Agent": f"python-sdk/{self.__get_sdk_version__()}"
+            "User-Agent": f"python-sdk/{SDK_VERSION}"
         }
         self.data = {"appId": self.api_id, "appKey": self.api_key, "baseUrl": self.base_url}
         self._validate_api_version()
         self._authenticate_user()
 
-    def __get_sdk_version__(self):
-        pyproject_toml_path = os.path.abspath(
-            os.path.join(os.path.dirname(__file__), "..", "..", "pyproject.toml")
-        )
-        with open(pyproject_toml_path, "r") as file:
-            content = file.read()
-
-        # Parse the content using the toml library
-        data = toml.loads(content)
-
-        # Extract the version (assuming it's under [tool.poetry])
-        version = data["tool"]["poetry"]["version"]
-        return version
-
     def _validate_api_version(self) -> None:
         _deprecated_versions = ["v1.0", "v1.1", "v1.2", "v1.3", "v1.4"]
         _currently_supported_versions = ["v1.5", "v2.1", "v3"]
 
         if self.api_version in _deprecated_versions:
             warnings.warn(
                 "Versions 1.0 through 1.4 are deprecated and will not longer be supported in the future",
```

### Comparing `telq-1.3.0/telq/endpoints/__init__.py` & `telq-1.3.1/telq/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/networks/__init__.py` & `telq-1.3.1/telq/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/session/__init__.py` & `telq-1.3.1/telq/session/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/session/session_data.py` & `telq-1.3.1/telq/session/session_data.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/supplier/__init__.py` & `telq-1.3.1/telq/supplier/__init__.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/supplier/supplier_data.py` & `telq-1.3.1/telq/supplier/supplier_data.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/tests/lnt.py` & `telq-1.3.1/telq/tests/lnt.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/telq/tests/mt.py` & `telq-1.3.1/telq/tests/mt.py`

 * *Files identical despite different names*

### Comparing `telq-1.3.0/PKG-INFO` & `telq-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telq
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for TelQ Telecom API
 Author: Tuvshinbayar Davaa
 Author-email: tuvshinbayar.davaa@telqtele.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

