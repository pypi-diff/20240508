# Comparing `tmp/trio_binance-0.3.3.tar.gz` & `tmp/trio_binance-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio_binance-0.3.3.tar", max compression
+gzip compressed data, was "trio_binance-0.3.4.tar", max compression
```

## Comparing `trio_binance-0.3.3.tar` & `trio_binance-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.3/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.3/README.rst
--rw-r--r--   0        0        0     1055 2024-05-03 01:53:52.093160 trio_binance-0.3.3/pyproject.toml
--rwxr-xr-x   0        0        0       67 2024-05-03 01:53:47.150389 trio_binance-0.3.3/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    78460 2024-05-03 01:52:58.369872 trio_binance-0.3.3/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.3/trio_binance/enums.py
--rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.3/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.3/trio_binance/helpers.py
--rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.3/trio_binance/streams.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.3.4/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.3.4/README.rst
+-rw-r--r--   0        0        0     1055 2024-05-08 02:33:11.981014 trio_binance-0.3.4/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-05-08 02:33:06.051918 trio_binance-0.3.4/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    78460 2024-05-08 02:32:01.001696 trio_binance-0.3.4/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.3.4/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.3.4/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.3.4/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.3.4/trio_binance/streams.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 trio_binance-0.3.4/PKG-INFO
```

### Comparing `trio_binance-0.3.3/LICENSE` & `trio_binance-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/README.rst` & `trio_binance-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/pyproject.toml` & `trio_binance-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trio-binance"
-version = "0.3.3"
+version = "0.3.4"
 description = "trio based asynchronous binance SDK"
 authors = ["Shu Wang <halfelf.ronin@gmail.com>"]
 keywords = ["binance", "python-trio"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/halfelf/trio-binance"
 repository = "https://github.com/halfelf/trio-binance"
```

### Comparing `trio_binance-0.3.3/trio_binance/client.py` & `trio_binance-0.3.4/trio_binance/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
     async def _request(self, method, uri: str, signed: bool, force_params: bool = False, **kwargs):
         kwargs = self._get_request_kwargs(method, signed, force_params, **kwargs)
         if method.lower() == "get":
             req = self.session.build_request(method, uri, params=kwargs.get("params", ""), timeout=self.REQUEST_TIMEOUT)
         else:
             req = self.session.build_request(
-                method, uri, data=dict(kwargs.get("data", {})), timeout=self.REQUEST_TIMEOUT
+                method, uri, json=dict(kwargs.get("data", {})), timeout=self.REQUEST_TIMEOUT
             )
         self.response = await self.session.send(req)
         return await self._handle_response(self.response)
 
     @staticmethod
     async def _handle_response(response: httpx.Response):
         """Internal helper for handling API responses from the Binance server.
```

### Comparing `trio_binance-0.3.3/trio_binance/enums.py` & `trio_binance-0.3.4/trio_binance/enums.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/trio_binance/exceptions.py` & `trio_binance-0.3.4/trio_binance/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/trio_binance/helpers.py` & `trio_binance-0.3.4/trio_binance/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/trio_binance/streams.py` & `trio_binance-0.3.4/trio_binance/streams.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.3.3/PKG-INFO` & `trio_binance-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-binance
-Version: 0.3.3
+Version: 0.3.4
 Summary: trio based asynchronous binance SDK
 Home-page: https://github.com/halfelf/trio-binance
 License: MIT
 Keywords: binance,python-trio
 Author: Shu Wang
 Author-email: halfelf.ronin@gmail.com
 Requires-Python: >=3.11,<4.0
```

