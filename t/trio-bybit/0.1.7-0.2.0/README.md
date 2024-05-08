# Comparing `tmp/trio_bybit-0.1.7.tar.gz` & `tmp/trio_bybit-0.2.0.tar.gz`

## Comparing `trio_bybit-0.1.7.tar` & `trio_bybit-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/pytest.ini
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/test_async_client.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/__init__.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/enums.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/README.md
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/keypair.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pkcs8.key
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pytest.ini
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_async_client.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_rsa.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/PKG-INFO
```

### Comparing `trio_bybit-0.1.7/tests/test_async_client.py` & `trio_bybit-0.2.0/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/tests/test_streams.py` & `trio_bybit-0.2.0/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/trio_bybit/client.py` & `trio_bybit-0.2.0/trio_bybit/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import base64
 import hmac
 import os
 
 import httpx
 import hashlib
 import time
 
 import orjson
+from Crypto.Hash import SHA256
+from Crypto.Signature import PKCS1_v1_5
+from Crypto.PublicKey import RSA
 
 from .exceptions import BybitAPIException, BybitRequestException
 
 
 class BaseClient:
     API_URL = "https://api.bybit.com/"
     # SECONDARY_API_URL = "https://api.bytick.com/"
@@ -27,22 +31,24 @@
         sign_style: str = "HMAC",
         alternative_net: str = "",
     ):
         """API Client constructor
         :param api_key: Api Key
         :param api_secret: Api Secret
         :param receive_window: Receive Window
-        :param sign_style: Sign Style. Default HMAC. RSA not implemented yet.
+        :param sign_style: Sign Style. Default HMAC. Choices: ["HMAC", "RSA"]
         :param alternative_net: Alternative network. Default empty to use mainnet. Choices: "test", "demo"
         """
         self.API_KEY = api_key
         self.API_SECRET = api_secret
         self.response = None
         self.receive_window = receive_window
-        self.sign_style = sign_style  # RSA not implemented yet
+        if sign_style != "HMAC" and sign_style != "RSA":
+            raise ValueError("Invalid sign style. Must be HMAC or RSA")
+        self.sign_style = sign_style
         self.timestamp_offset = 0
         if alternative_net == "test":
             self.base = self.TEST_NET_API_URL
         elif alternative_net == "demo":
             self.base = self.DEMO_NET_API_URL
         else:
             self.base = self.API_URL
@@ -64,15 +70,22 @@
     def _generate_signature(self, request: httpx.Request, timestamp_milli: int) -> str:
         if request.method == "GET":
             prepared_str = str(timestamp_milli) + self.API_KEY + str(self.receive_window) + str(request.url.params)
         else:
             prepared_str = (
                 str(timestamp_milli) + self.API_KEY + str(self.receive_window) + request.content.decode("utf-8")
             )
-        return hmac.new(self.API_SECRET.encode("utf-8"), prepared_str.encode("utf-8"), hashlib.sha256).hexdigest()
+        prepared_bytes = prepared_str.encode("utf-8")
+        if self.sign_style == "HMAC":
+            return hmac.new(self.API_SECRET.encode("utf-8"), prepared_bytes, hashlib.sha256).hexdigest()
+        else:  # RSA
+            encoded_param = SHA256.new(prepared_bytes)
+            signature = PKCS1_v1_5.new(RSA.importKey(self.API_SECRET)).sign(encoded_param)
+
+            return base64.b64encode(signature).decode()
 
     def _get_request(self, method, uri, signed: bool, **kwargs) -> httpx.Request:
         timestamp = int(time.time() * 1000 + self.timestamp_offset)
         headers = self._get_headers(timestamp, signed)
         if method.lower() == "get":
             req = self.session.build_request(method, uri, headers=headers, params=kwargs)
         else:
```

### Comparing `trio_bybit-0.1.7/trio_bybit/exceptions.py` & `trio_bybit-0.2.0/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/trio_bybit/helpers.py` & `trio_bybit-0.2.0/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/trio_bybit/streams.py` & `trio_bybit-0.2.0/trio_bybit/streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/.gitignore` & `trio_bybit-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/LICENSE` & `trio_bybit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/README.md` & `trio_bybit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.7/pyproject.toml` & `trio_bybit-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "trio-bybit"
-version = "0.1.7"
+version = "0.2.0"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
     "orjson>=3.10.0",
     "dateparser>=1.2.0",
     "pytz>=2024.1",
     "trio-websocket>=0.11.1",
+    "pycryptodome>=3.20.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries",
```

### Comparing `trio_bybit-0.1.7/PKG-INFO` & `trio_bybit-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
         
@@ -32,14 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.12
 Requires-Dist: dateparser>=1.2.0
 Requires-Dist: httpx[http2]>=0.27.0
 Requires-Dist: orjson>=3.10.0
+Requires-Dist: pycryptodome>=3.20.0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: trio-websocket>=0.11.1
 Requires-Dist: trio>=0.25.0
 Description-Content-Type: text/markdown
 
 # Welcome to trio-bybit
```

