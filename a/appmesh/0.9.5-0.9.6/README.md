# Comparing `tmp/appmesh-0.9.5-py3-none-any.whl.zip` & `tmp/appmesh-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15969 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-07 12:04 appmesh/__init__.py
--rw-r--r--  2.0 unx    58539 b- defN 24-May-07 12:04 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-07 12:05 appmesh-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 12:05 appmesh-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-07 12:05 appmesh-0.9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-07 12:05 appmesh-0.9.5.dist-info/RECORD
-6 files, 69891 bytes uncompressed, 15147 bytes compressed:  78.3%
+Zip file size: 15945 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-08 05:31 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58043 b- defN 24-May-08 05:31 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-08 05:31 appmesh-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 05:31 appmesh-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-08 05:31 appmesh-0.9.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-08 05:31 appmesh-0.9.6.dist-info/RECORD
+6 files, 69395 bytes uncompressed, 15123 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.9.5.dist-info/METADATA
+Filename: appmesh-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.9.5.dist-info/WHEEL
+Filename: appmesh-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.9.5.dist-info/top_level.txt
+Filename: appmesh-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.9.5.dist-info/RECORD
+Filename: appmesh-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -322,15 +322,15 @@
     ########################################
     def login(self, user_name: str, user_pwd: str, totp_code="", timeout_seconds=DEFAULT_TOKEN_EXPIRE_SECONDS) -> str:
         """Login with user name and password
 
         Args:
             user_name (str): the name of the user.
             user_pwd (str): the password of the user.
-            totp_code (str, optional): the TOTP key if enabled for the user.
+            totp_code (str, optional): the TOTP code if enabled for the user.
             timeout_seconds (int | str, optional): token expire timeout of seconds. support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P1W').
 
         Returns:
             str: JWT token if verify success, otherwise return None.
         """
         self.jwt_token = None
         resp = self._request_http(
@@ -446,42 +446,26 @@
             # resp.raise_for_status()
         return None
 
     def totp_setup(self, totp_code: str) -> bool:
         """Setup 2FA for current login user
 
         Args:
-            totp_code (str): TOTP key
+            totp_code (str): TOTP code
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path=f"/appmesh/totp/setup",
             header={"Totp": base64.b64encode(totp_code.encode())},
         )
         return resp.status_code == HTTPStatus.OK
 
-    def totp_validate(self, totp_code: str) -> bool:
-        """Validate TOTP key
-
-        Args:
-            totp_code (str): TOTP key
-
-        Returns:
-            bool: success or failure.
-        """
-        resp = self._request_http(
-            method=AppMeshClient.Method.POST,
-            path=f"/appmesh/totp/validate",
-            header={"Totp": base64.b64encode(totp_code.encode())},
-        )
-        return (resp.status_code == HTTPStatus.OK), resp.json()[REST_TEXT_MESSAGE_JSON_KEY]
-
     def totp_disable(self, user="self") -> bool:
         """Disable 2FA for current user
 
         Args:
             user (str, optional): user name for disable TOTP.
 
         Returns:
```

## Comparing `appmesh-0.9.5.dist-info/METADATA` & `appmesh-0.9.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.9.5
+Version: 0.9.6
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.9.5 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.9.6 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

