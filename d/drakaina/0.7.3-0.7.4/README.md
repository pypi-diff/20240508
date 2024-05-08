# Comparing `tmp/drakaina-0.7.3.tar.gz` & `tmp/drakaina-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.3.tar", max compression
+gzip compressed data, was "drakaina-0.7.4.tar", max compression
```

## Comparing `drakaina-0.7.3.tar` & `drakaina-0.7.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     9452 2024-05-06 22:36:55.277641 drakaina-0.7.3/drakaina/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.3/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.3/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.3/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.3/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.3/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      351 2024-05-06 19:02:29.664147 drakaina-0.7.3/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     8995 2024-05-06 20:03:49.435550 drakaina-0.7.3/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.3/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18281 2024-05-06 22:36:55.277641 drakaina-0.7.3/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.3/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.3/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.3/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7749 2024-05-06 22:36:55.277641 drakaina-0.7.3/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     1991 2024-05-06 22:36:55.277641 drakaina-0.7.3/drakaina/middleware/exception.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.3/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12943 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.3/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     8028 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    14864 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.3/drakaina/serializers.py
--rw-r--r--   0        0        0    34083 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/types.py
--rw-r--r--   0        0        0     6193 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/utils.py
--rw-r--r--   0        0        0     8073 2024-05-06 22:36:55.278641 drakaina-0.7.3/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.3/LICENSE
--rw-r--r--   0        0        0     2684 2024-05-06 22:36:19.843905 drakaina-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     6992 2024-05-06 22:36:55.277641 drakaina-0.7.3/README.md
--rw-r--r--   0        0        0     8462 1970-01-01 00:00:00.000000 drakaina-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     9452 2024-05-08 01:44:52.693913 drakaina-0.7.4/drakaina/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.4/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.4/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.4/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.4/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.4/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-06 19:02:29.664147 drakaina-0.7.4/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     9046 2024-05-08 00:40:36.187403 drakaina-0.7.4/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.4/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18281 2024-05-08 01:44:52.694912 drakaina-0.7.4/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.4/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.4/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.4/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7473 2024-05-08 01:44:52.694912 drakaina-0.7.4/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1991 2024-05-08 01:44:52.694912 drakaina-0.7.4/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.4/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12943 2024-05-08 01:44:52.694912 drakaina-0.7.4/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.4/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     8028 2024-05-08 01:44:52.694912 drakaina-0.7.4/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    14864 2024-05-08 01:44:52.695912 drakaina-0.7.4/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.4/drakaina/serializers.py
+-rw-r--r--   0        0        0    34083 2024-05-08 01:44:52.695912 drakaina-0.7.4/drakaina/types.py
+-rw-r--r--   0        0        0     5544 2024-05-08 01:44:52.695912 drakaina-0.7.4/drakaina/utils.py
+-rw-r--r--   0        0        0     7804 2024-05-08 01:44:52.696381 drakaina-0.7.4/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.4/LICENSE
+-rw-r--r--   0        0        0     2684 2024-05-08 01:40:14.817404 drakaina-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     6992 2024-05-08 01:44:52.693913 drakaina-0.7.4/README.md
+-rw-r--r--   0        0        0     8462 1970-01-01 00:00:00.000000 drakaina-0.7.4/PKG-INFO
```

### Comparing `drakaina-0.7.3/drakaina/__init__.py` & `drakaina-0.7.4/drakaina/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/contrib/django/__init__.py` & `drakaina-0.7.4/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/contrib/django/middleware.py` & `drakaina-0.7.4/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/contrib/django/views.py` & `drakaina-0.7.4/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.4/drakaina/contrib/jwt/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def __init__(
         self,
         app: WSGIApplication,
         algorithms: str | Iterable[str] = SUPPORTED_ALGORITHMS,
         secret_key: str = None,
         public_key: str = None,
         credentials_required: bool = True,
-        prefix: str = "Bearer",
+        prefix: str | Iterable[str] = "Bearer",
         use_cookies: bool = False,
         cookie_key: str = "jwt",
         decode_options: dict[str, bool | list[str]] | None = None,
         verify_values: (
             dict[str, str | Iterable[str] | re.Pattern] | None
         ) = None,
         leeway_value: int | float = 0,
@@ -110,15 +110,15 @@
         **kwargs,
     ):
         super().__init__(app, **kwargs)
 
         self._algorithms = iterable_str_arg(algorithms)
         self.__verify_key = secret_key or public_key
         self._credentials_required = credentials_required
-        self._prefix = prefix
+        self._prefix = iterable_str_arg(prefix)
         self._cookie_key = cookie_key
         self._decode_options = (
             decode_options
             if decode_options is not None
             else {
                 "require": [],
                 "verify_iss": False,
@@ -180,21 +180,21 @@
                         verify=False,
                         decode_options=None,
                         verify_values=self._verify_values,
                         leeway=self._leeway,
                     )
                     token_is_valid = environ.get(ENV_IS_AUTHENTICATED, False)
 
-            if callable(self.is_revoked):
+            if callable(self.is_revoked) and token_is_valid:
                 if self.is_revoked(environ, token_payload):
                     raise ForbiddenError("Token is revoked")
 
-            environ[ENV_USER_ID] = token_payload.get(self._user_id_field)
-            environ[ENV_IS_AUTHENTICATED] = token_is_valid
             environ[ENV_AUTH_PAYLOAD] = token_payload
+            environ[ENV_IS_AUTHENTICATED] = token_is_valid
+            environ[ENV_USER_ID] = token_payload.get(self._user_id_field)
 
             if callable(self.get_user):
                 environ[ENV_USER] = self.get_user(environ, token_payload)
             if callable(self.get_scopes):
                 environ[ENV_AUTH_SCOPES] = self.get_scopes(
                     environ,
                     token_payload,
@@ -211,15 +211,14 @@
         await self.app(scope, receive, send)
 
     def _token_from_auth_header(
         self,
         request: ASGIScope | WSGIEnvironment,
     ) -> str | None:
         auth_header = request.get("HTTP_AUTHORIZATION")
-
         if auth_header is None:
             return None
 
         try:
             parts = auth_header.strip().split(" ")
         except ValueError:
             raise AuthenticationFailedError("Invalid `Authorization` header")
@@ -236,14 +235,13 @@
         return parts[1]
 
     def _token_from_cookies(
         self,
         request: ASGIScope | WSGIEnvironment,
     ) -> str | None:
         cookie_header = request.get("HTTP_COOKIE")
-
         if cookie_header is None:
             return None
 
         cookies = get_cookies(cookie_header)
 
         return cookies.get(self._cookie_key)
```

### Comparing `drakaina-0.7.3/drakaina/contrib/jwt/types.py` & `drakaina-0.7.4/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.4/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/exceptions.py` & `drakaina-0.7.4/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/middleware/base.py` & `drakaina-0.7.4/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/middleware/cors.py` & `drakaina-0.7.4/drakaina/middleware/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterable
+from collections.abc import Iterable
 from typing import Optional
 
 from drakaina.middleware.base import BaseMiddleware
 from drakaina.types import ASGIReceive
 from drakaina.types import ASGIScope
 from drakaina.types import ASGISend
 from drakaina.types import WSGIApplication
@@ -26,33 +26,27 @@
 class CORSMiddleware(BaseMiddleware):
     """Middleware for providing CORS headers and handling preflight requests.
 
     See: https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
 
     :param allow_origin:
         The "Access-Control-Allow-Origin" header.
-    :type allow_origin: Union[str, Iterable[str]]
     :param allow_methods:
         The "Access-Control-Allow-Methods" header.
         Default: "GET, POST, OPTIONS".
-    :type allow_methods: Union[str, Iterable[str]]
     :param allow_headers:
         The "Access-Control-Allow-Headers" header.
         Default: "Accept, Accept-Encoding, Authorization,
         Content-Type, DNT, Origin, User-Agent, X-Requested-With".
-    :type allow_headers: Union[str, Iterable[str]]
     :param allow_credentials:
         The "Access-Control-Allow-Credentials" header. Default: None.
-    :type allow_credentials: bool
     :param expose_headers:
         The "Access-Control-Expose-Headers" header. Default: None.
-    :type expose_headers: Union[str, Iterable[str]]
     :param max_age:
         The "Access-Control-Max-Age" header. Default: 3600 sec. (1 hour).
-    :type max_age: Union[int, str]
 
     """
 
     __slots__ = (
         "_cors_headers",
         "_preflight_cors_headers",
         "_allow_origin",
@@ -69,15 +63,15 @@
         allow_credentials: Optional[bool] = None,
         expose_headers: Optional[str | Iterable[str]] = None,
         max_age: int = 3600,
         **kwargs,
     ):
         super().__init__(app, **kwargs)
 
-        self._allow_origin = ", ".join(iterable_str_arg(allow_origin))
+        self._allow_origin = iterable_str_arg(allow_origin)
 
         if allow_methods:
             if "*" in allow_methods:
                 _allow_methods = ALL_METHODS
             else:
                 _allow_methods = ", ".join(iterable_str_arg(allow_methods))
         else:
@@ -195,15 +189,14 @@
         environ: WSGIEnvironment,
         start_response: WSGIStartResponse,
     ) -> WSGIStartResponse:
         """Wraps the start_response method, and includes the CORS header
         for the specified origin.
         """
         request_origin = environ["HTTP_ORIGIN"]
-
         cors_headers = self._cors_headers[:]
 
         if "*" in self._allow_origin:
             if "HTTP_COOKIE" in environ:
                 cors_headers.append(
                     ("Access-Control-Allow-Origin", request_origin),
                 )
```

### Comparing `drakaina-0.7.3/drakaina/middleware/exception.py` & `drakaina-0.7.4/drakaina/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.4/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/registries.py` & `drakaina-0.7.4/drakaina/registries.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/rpc_protocols/base.py` & `drakaina-0.7.4/drakaina/rpc_protocols/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.4/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/serializers.py` & `drakaina-0.7.4/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/types.py` & `drakaina-0.7.4/drakaina/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/drakaina/utils.py` & `drakaina-0.7.4/drakaina/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-""" Utility functions for package."""
 from __future__ import annotations
 
 import inspect
 import re
 from asyncio import iscoroutine
-from decimal import Decimal
-from datetime import date
+from collections.abc import Iterable
 from datetime import datetime
 from datetime import timedelta
 from functools import partial
 from inspect import cleandoc
-from json import JSONEncoder
 from typing import Callable
-from typing import Iterable
 from typing import Literal
 
 
-def iterable_str_arg(s: str | Iterable[str]) -> tuple[str]:
+def iterable_str_arg(s: str | Iterable[str]) -> tuple[str, ...]:
     if isinstance(s, str):
-        s = s.replace(",", " ").strip().replace("  ", " ").split()
+        s = s.replace(",", " ").strip()
+        s = s.replace("  ", " ").split()
     return tuple(map(str, s))
 
 
 def unwrap_func(func: Callable) -> Callable:
     _func = func
     while hasattr(_func, "__wrapped__") or isinstance(_func, partial):
         _func = getattr(_func, "__wrapped__", None) or _func.func
@@ -143,15 +140,14 @@
     :param item_path: URL or regex pattern to match against the request path.
     :param path_info: Request path string.
     """
 
     if item_path is None:
         return True
     if isinstance(item_path, str):
-        # or path_info.startswith(item_path) ?
         return path_info == item_path
     if isinstance(item_path, re.Pattern):
         return bool(item_path.match(path_info))
 
     return False
 
 
@@ -159,37 +155,14 @@
     for pattern in entries:
         if re.match(pattern, path):
             return True
 
     return False
 
 
-class DatetimeDecimalEncoder(JSONEncoder):
-    """Encoder for datetime and decimal serialization.
-
-    Usage: json.dumps(object, cls=DatetimeDecimalEncoder)
-    NOTE: _iterencode does not work
-
-    """
-
-    def default(self, obj) -> str:
-        """Encode JSON.
-
-        :return: A JSON encoded string
-
-        """
-        if isinstance(obj, Decimal):
-            return float(obj)
-
-        if isinstance(obj, (datetime, date)):
-            return obj.isoformat()
-
-        return super().default(self, obj)
-
-
 # validating parameters
 def is_invalid_params(func, *args, **kwargs):
     """
     Method:
         Validate pre-defined criteria, if any is True - function is invalid
         0. func should be callable
         1. kwargs should not have unexpected keywords
```

### Comparing `drakaina-0.7.3/drakaina/wsgi.py` & `drakaina-0.7.4/drakaina/wsgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,29 +41,22 @@
 
 class WSGIHandler:
     """Implementation of WSGI protocol.
 
     # todo: write about urls (route, provide_ args)
 
     :param route:
-    :type route: str | re.Pattern
     :param handler: RPC protocol implementation.
-    :type handler: BaseRPCProtocol
     :param middlewares: List of WSGI middlewares.
-    :type middlewares: Iterable[type[BaseMiddleware] | partial[BaseMiddleware]]
     :param logger: A `logging.Logger` object.
-    :type logger: Logger
     :param max_content_size: Limiting request body size for DoS protection.
-    :type max_content_size: int
     :param openrpc_url: OpenRPC Schema URL.
         The recommended document name is `openrpc.json`.
-    :type openrpc_url: str | re.Pattern
     :param openapi_url: OpenAPI Schema URL.
         The recommended document name is `openapi.json`.
-    :type openapi_url: str | re.Pattern
 
     """
 
     __slots__ = (
         "environ",
         "start_response",
         "handler",
@@ -111,26 +104,27 @@
         self.openrpc_url = openrpc_url
         self.openapi_url = openapi_url
 
         if openrpc_url or openapi_url:
             self._allowed_methods = ", ".join(ALLOWED_METHODS)
         else:
             self._allowed_methods = ", ".join(
-                [m for m in ALLOWED_METHODS if m != "GET"],
+                m for m in ALLOWED_METHODS if m != "GET"
             )
 
         # Build middleware stack
         self._middlewares_chain = self._wsgi_app
         kw = {"is_async": False}
         for mw in reversed(middlewares or ()):
             if (
                 isinstance(mw, partial) and issubclass(mw.func, BaseMiddleware)
             ) or issubclass(mw, BaseMiddleware):
                 self._middlewares_chain = mw(self._middlewares_chain, **kw)
-            self._middlewares_chain = mw(self._middlewares_chain)
+            else:
+                self._middlewares_chain = mw(self._middlewares_chain)
 
         # The middleware for handling exceptions in the middleware according
         #  to the RPC protocol.
         self._middlewares_chain = ExceptionMiddleware(
             RequestWrapperMiddleware(self._middlewares_chain, **kw),  # noqa
             handler=self.handler,
             logger=self.logger,
@@ -150,15 +144,15 @@
         environ: WSGIEnvironment,
         start_response: WSGIStartResponse,
     ) -> WSGIResponse:
         self.environ = environ
         self.start_response = start_response
 
         method = environ["REQUEST_METHOD"]
-        if method in ALLOWED_METHODS:
+        if method in self._allowed_methods:
             return getattr(self, method.lower())()
 
         return self._method_not_allowed()
 
     def get(self) -> WSGIResponse:
         if match_path(self.openrpc_url, self.environ["PATH_INFO"]):
             response_body = self.handler.get_raw_openrpc_schema()
@@ -183,19 +177,19 @@
             return self._not_found()
 
         wsgi_input: WSGIInputStream = self.environ["wsgi.input"]
 
         content_type = self.environ.get("CONTENT_TYPE")
         content_length = int(self.environ.get("CONTENT_LENGTH") or 0)
         if (
-            not (content_type and content_length)
+            not content_type
             or not content_type.startswith(self._rpc_content_type)
             or content_length > self.max_content_size
         ):
-            if content_type != self._rpc_content_type:
+            if not content_type.startswith(self._rpc_content_type):
                 response_status = "415 Unsupported Media Type"
             else:
                 response_status = "400 Bad Request"
             # Return RPC error
             response_body = self.handler.get_raw_error(BadRequestError())
         else:
             response_status = "200 OK"
```

### Comparing `drakaina-0.7.3/LICENSE` & `drakaina-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/pyproject.toml` & `drakaina-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.3"
+version = "0.7.4"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -60,15 +60,15 @@
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 httpx = "^0.27.0"
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 testpaths = "tests"
-addopts = "-vl --cov=drakaina --cov-report term-missing --tb=auto --capture=sys"
+addopts = "-vl --cov=drakaina --cov-report=term-missing --tb=auto --capture=sys"
 
 [tool.ruff]
 # Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F"]
 ignore = []
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
```

### Comparing `drakaina-0.7.3/README.md` & `drakaina-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.3/PKG-INFO` & `drakaina-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.3
+Version: 0.7.4
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.9,<4.0
```

