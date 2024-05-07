# Comparing `tmp/fastapi_restful-0.5.0.tar.gz` & `tmp/fastapi_restful-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_restful-0.5.0.tar", max compression
+gzip compressed data, was "fastapi_restful-0.6.0.tar", max compression
```

## Comparing `fastapi_restful-0.5.0.tar` & `fastapi_restful-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-08-13 17:15:36.375865 fastapi_restful-0.5.0/LICENSE
--rw-r--r--   0        0        0     3597 2023-08-13 17:15:36.375865 fastapi_restful-0.5.0/README.md
--rw-r--r--   0        0        0      196 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/__init__.py
--rw-r--r--   0        0        0     1251 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/api_model.py
--rw-r--r--   0        0        0     2851 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/api_settings.py
--rw-r--r--   0        0        0      882 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/camelcase.py
--rw-r--r--   0        0        0     7159 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/cbv.py
--rw-r--r--   0        0        0     1045 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/cbv_base.py
--rw-r--r--   0        0        0     1226 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/enums.py
--rw-r--r--   0        0        0     2251 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/guid_type.py
--rw-r--r--   0        0        0      245 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/inferring_router.py
--rw-r--r--   0        0        0      367 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/openapi.py
--rw-r--r--   0        0        0        0 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/py.typed
--rw-r--r--   0        0        0     5205 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/session.py
--rw-r--r--   0        0        0     3519 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/tasks.py
--rw-r--r--   0        0        0     7113 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/fastapi_restful/timing.py
--rw-r--r--   0        0        0     3434 2023-08-13 17:15:36.379865 fastapi_restful-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 fastapi_restful-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-07 22:45:24.674872 fastapi_restful-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3473 2024-05-07 22:45:24.674872 fastapi_restful-0.6.0/README.md
+-rw-r--r--   0        0        0      892 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/api_model.py
+-rw-r--r--   0        0        0     2851 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/api_settings.py
+-rw-r--r--   0        0        0      882 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/camelcase.py
+-rw-r--r--   0        0        0     7261 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/cbv.py
+-rw-r--r--   0        0        0     1045 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/cbv_base.py
+-rw-r--r--   0        0        0     1226 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/enums.py
+-rw-r--r--   0        0        0     2251 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/guid_type.py
+-rw-r--r--   0        0        0      245 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/inferring_router.py
+-rw-r--r--   0        0        0      367 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/openapi.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/py.typed
+-rw-r--r--   0        0        0     5205 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/session.py
+-rw-r--r--   0        0        0     3472 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/tasks.py
+-rw-r--r--   0        0        0     7117 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/fastapi_restful/timing.py
+-rw-r--r--   0        0        0     3577 2024-05-07 22:45:24.678871 fastapi_restful-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 fastapi_restful-0.6.0/PKG-INFO
```

### Comparing `fastapi_restful-0.5.0/LICENSE` & `fastapi_restful-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/README.md` & `fastapi_restful-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 </a>
 <br />
 <a href="https://pypi.org/project/FastApi-RESTful" target="_blank">
     <img src="https://badge.fury.io/py/fastapi-restful.svg" alt="Package version">
 </a>
 <a href="https://github.com/yuval9313/fastapi-restful" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/FastApi-RESTful.svg" alt="Python versions">
-    <img src="https://img.shields.io/github/license/yuval9313/fastapi-utils.svg" alt="License">
+    <img src="https://img.shields.io/github/license/yuval9313/FastApi-RESTful.svg" alt="License">
 </a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-restful.netlify.app" target="_blank">https://fastapi-restful.netlify.app</a>
 
@@ -37,31 +37,30 @@
 
 ## Features
 
 This package includes a number of utilities to help reduce boilerplate and reuse common functionality across projects:
 
 * **Resource Class**: Create CRUD with ease the OOP way with `Resource` base class that lets you implement methods quick.
 * **Class Based Views**: Stop repeating the same dependencies over and over in the signature of related endpoints.
-* **Response-Model Inferring Router**: Let FastAPI infer the `response_model` to use based on your return type annotation. 
 * **Repeated Tasks**: Easily trigger periodic tasks on server startup
 * **Timing Middleware**: Log basic timing information for every request
 * **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator
 * **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency
 
 ---
 
 It also adds a variety of more basic utilities that are useful across a wide variety of projects:
 
 * **APIModel**: A reusable `pydantic.BaseModel`-derived base class with useful defaults
-* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables 
+* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables
 * **String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to maintain
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
-See the [docs](https://fastapi-restful.netlify.app/) for more details and examples. 
+See the [docs](https://fastapi-restful.netlify.app/) for more details and examples.
 
 ## Requirements
 
 This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
```

#### html2text {}

```diff
@@ -6,30 +6,29 @@
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_v_a_l_9_3_1_3_/_f_a_s_t_a_p_i_-_r_e_s_t_f_u_l Base on: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
 _d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s --- _F_a_s_t_A_P_I is a modern, fast web framework for building
 APIs with Python 3.7+. But if you're here, you probably already knew that! --
 - ## Features This package includes a number of utilities to help reduce
 boilerplate and reuse common functionality across projects: * **Resource
 Class**: Create CRUD with ease the OOP way with `Resource` base class that lets
 you implement methods quick. * **Class Based Views**: Stop repeating the same
-dependencies over and over in the signature of related endpoints. * **Response-
-Model Inferring Router**: Let FastAPI infer the `response_model` to use based
-on your return type annotation. * **Repeated Tasks**: Easily trigger periodic
-tasks on server startup * **Timing Middleware**: Log basic timing information
-for every request * **OpenAPI Spec Simplification**: Simplify your OpenAPI
-Operation IDs for cleaner output from OpenAPI Generator * **SQLAlchemy
-Sessions**: The `FastAPISessionMaker` class provides an easily-customized
-SQLAlchemy Session dependency --- It also adds a variety of more basic
-utilities that are useful across a wide variety of projects: * **APIModel**: A
-reusable `pydantic.BaseModel`-derived base class with useful defaults *
-**APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to
-configure FastAPI through environment variables * **String-Valued Enums**: The
-`StrEnum` and `CamelStrEnum` classes make string-valued enums easier to
-maintain * **CamelCase Conversions**: Convenience functions for converting
-strings from `snake_case` to `camelCase` or `PascalCase` and back * **GUID
-Type**: The provided GUID type makes it easy to use UUIDs as the primary keys
-for your database tables See the [docs](https://fastapi-restful.netlify.app/
-) for more details and examples. ## Requirements This package is intended for
-use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
-Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
-slim package :) pip install fastapi-restful[session] # To add sqlalchemy
-session maker pip install fastapi-restful[all] # For all the packages ``` ##
-License This project is licensed under the terms of the MIT license.
+dependencies over and over in the signature of related endpoints. * **Repeated
+Tasks**: Easily trigger periodic tasks on server startup * **Timing
+Middleware**: Log basic timing information for every request * **OpenAPI Spec
+Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from
+OpenAPI Generator * **SQLAlchemy Sessions**: The `FastAPISessionMaker` class
+provides an easily-customized SQLAlchemy Session dependency --- It also adds a
+variety of more basic utilities that are useful across a wide variety of
+projects: * **APIModel**: A reusable `pydantic.BaseModel`-derived base class
+with useful defaults * **APISettings**: A subclass of `pydantic.BaseSettings`
+that makes it easy to configure FastAPI through environment variables *
+**String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-
+valued enums easier to maintain * **CamelCase Conversions**: Convenience
+functions for converting strings from `snake_case` to `camelCase` or
+`PascalCase` and back * **GUID Type**: The provided GUID type makes it easy to
+use UUIDs as the primary keys for your database tables See the [docs](https://
+fastapi-restful.netlify.app/) for more details and examples. ## Requirements
+This package is intended for use with any recent version of FastAPI (depending
+on `pydantic>=1.0`), and Python 3.7+. ## Installation ```bash pip install
+fastapi-restful # For basic slim package :) pip install fastapi-restful
+[session] # To add sqlalchemy session maker pip install fastapi-restful[all] #
+For all the packages ``` ## License This project is licensed under the terms of
+the MIT license.
```

### Comparing `fastapi_restful-0.5.0/fastapi_restful/api_model.py` & `fastapi_restful-0.6.0/fastapi_restful/api_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/api_settings.py` & `fastapi_restful-0.6.0/fastapi_restful/api_settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/camelcase.py` & `fastapi_restful-0.6.0/fastapi_restful/camelcase.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/cbv.py` & `fastapi_restful-0.6.0/fastapi_restful/cbv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 import inspect
-from typing import Any, Callable, List, Tuple, Type, TypeVar, Union, cast, get_type_hints
+from typing import (
+    Any,
+    Callable,
+    List,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    get_type_hints,
+)
 
 import pydantic
 from fastapi import APIRouter, Depends
 from fastapi.routing import APIRoute
 from starlette.routing import Route, WebSocketRoute
 
 PYDANTIC_VERSION = pydantic.VERSION
@@ -24,15 +34,15 @@
     This function returns a decorator that converts the decorated into a class-based view for the provided router.
 
     Any methods of the decorated class that are decorated as endpoints using the router provided to this function
     will become endpoints in the router. The first positional argument to the methods (typically `self`)
     will be populated with an instance created using FastAPI's dependency-injection.
 
     For more detail, review the documentation at
-    https://fastapi-utils.davidmontague.xyz/user-guide/class-based-views/#the-cbv-decorator
+    https://fastapi-restful.netlify.app/user-guide/class-based-views//#the-cbv-decorator
     """
 
     def decorator(cls: Type[T]) -> Type[T]:
         # Define cls as cbv class exclusively when using the decorator
         return _cbv(router, cls, *urls)
 
     return decorator
@@ -115,14 +125,15 @@
         if isinstance(route, (Route, WebSocketRoute)) and route.endpoint in functions_set
     ]
     prefix_length = len(router.prefix)  # Until 'black' would fix an issue which causes PEP8: E203
     for route in cbv_routes:
         router.routes.remove(route)
         route.path = route.path[prefix_length:]
         _update_cbv_route_endpoint_signature(cls, route)
+        route.name = cls.__name__ + "." + route.name
         cbv_router.routes.append(route)
     router.include_router(cbv_router)
 
 
 def _allocate_routes_by_method_name(router: APIRouter, url: str, function_members: List[Tuple[str, Any]]) -> None:
     existing_routes_endpoints: List[Tuple[Any, str]] = [
         (route.endpoint, route.path) for route in router.routes if isinstance(route, APIRoute)
```

### Comparing `fastapi_restful-0.5.0/fastapi_restful/cbv_base.py` & `fastapi_restful-0.6.0/fastapi_restful/cbv_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/enums.py` & `fastapi_restful-0.6.0/fastapi_restful/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/guid_type.py` & `fastapi_restful-0.6.0/fastapi_restful/guid_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/session.py` & `fastapi_restful-0.6.0/fastapi_restful/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.5.0/fastapi_restful/tasks.py` & `fastapi_restful-0.6.0/fastapi_restful/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import asyncio
 import logging
-from asyncio import ensure_future
 from functools import wraps
 from traceback import format_exception
 from typing import Any, Callable, Coroutine, Union
 
 from starlette.concurrency import run_in_threadpool
 
 NoArgsNoReturnFuncT = Callable[[], None]
@@ -62,21 +61,21 @@
                     await asyncio.sleep(wait_first)
                 while max_repetitions is None or repetitions < max_repetitions:
                     try:
                         if is_coroutine:
                             await func()  # type: ignore
                         else:
                             await run_in_threadpool(func)
-                        repetitions += 1
                     except Exception as exc:
                         if logger is not None:
                             formatted_exception = "".join(format_exception(type(exc), exc, exc.__traceback__))
                             logger.error(formatted_exception)
                         if raise_exceptions:
                             raise exc
+                    repetitions += 1
                     await asyncio.sleep(seconds)
 
-            ensure_future(loop())
+            await loop()
 
         return wrapped
 
     return decorator
```

### Comparing `fastapi_restful-0.5.0/fastapi_restful/timing.py` & `fastapi_restful-0.6.0/fastapi_restful/timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from fastapi import FastAPI
 from starlette.middleware.base import RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.routing import Match, Mount
 from starlette.types import Scope
 
-TIMER_ATTRIBUTE = "__fastapi_utils_timer__"
+TIMER_ATTRIBUTE = "__fastapi_restful_timer__"
 
 
 def add_timing_middleware(
     app: FastAPI, record: Callable[[str], None] | None = None, prefix: str = "", exclude: str | None = None
 ) -> None:
     """
     Adds a middleware to the provided `app` that records timing metrics using the provided `record` callable.
@@ -55,15 +55,15 @@
 def record_timing(request: Request, note: str | None = None) -> None:
     """
     Call this function at any point that you want to display elapsed time during the handling of a single request
 
     This can help profile which piece of a request is causing a performance bottleneck.
 
     Note that for this function to succeed, the request should have been generated by a FastAPI app
-    that has had timing middleware added using the `fastapi_utils.timing.add_timing_middleware` function.
+    that has had timing middleware added using the `fastapi_restful.timing.add_timing_middleware` function.
     """
     timer = getattr(request.state, TIMER_ATTRIBUTE, None)
     if timer is not None:
         if not isinstance(timer, _TimingStats):
             raise ValueError("Timer should be of an instance of TimingStats")
         timer.emit(note)
     else:
```

### Comparing `fastapi_restful-0.5.0/pyproject.toml` & `fastapi_restful-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "fastapi-restful"
-version = "0.5.0"
+version = "0.6.0"
 description = "Quicker FastApi developing tools"
 license = "MIT"
 authors = ["Yuval Levi <yuvall9313@gmail.com>"]
 readme = "README.md"
 homepage = "https://fastapi-restful.netlify.app"
-repository = "https://github.com/yuval9313/fastapi-utils"
+repository = "https://github.com/yuval9313/FastApi-RESTful"
 documentation = "https://fastapi-restful.netlify.app"
 keywords = ["fastapi", "OOP", "RESTful"]
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
@@ -54,21 +54,24 @@
 httpx = "*"  # TestClient
 
 # Testing
 pytest = "^7.0"
 pytest-cov = "*"
 pytest-asyncio = "*"
 coverage = "*"
+mock = { version = "*", python = "<3.8" }
+types-mock = { version = "*", python = "<3.8" }
 
 
 # Static
 ruff = "*"
 black = { version = "*", allow-prereleases = true }
 mypy = "*"
 sqlalchemy-stubs = "*"
+types-setuptools = "*"  # for pkg_resources import
 
 # Documentation
 mkdocs = "*"
 mkdocs-material = "*"
 markdown-include = "*"
 autoflake = "^1.4"
```

### Comparing `fastapi_restful-0.5.0/PKG-INFO` & `fastapi_restful-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-restful
-Version: 0.5.0
+Version: 0.6.0
 Summary: Quicker FastApi developing tools
 Home-page: https://fastapi-restful.netlify.app
 License: MIT
 Keywords: fastapi,OOP,RESTful
 Author: Yuval Levi
 Author-email: yuvall9313@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -38,15 +38,15 @@
 Requires-Dist: fastapi (>=0.89,<1.0)
 Requires-Dist: psutil (>=5,<6)
 Requires-Dist: pydantic (>1.0,<3.0)
 Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0) ; extra == "all"
 Requires-Dist: sqlalchemy (>=1.4,<3.0) ; extra == "all" or extra == "session"
 Requires-Dist: typing-inspect (>=0.9.0,<0.10.0) ; extra == "all"
 Project-URL: Documentation, https://fastapi-restful.netlify.app
-Project-URL: Repository, https://github.com/yuval9313/fastapi-utils
+Project-URL: Repository, https://github.com/yuval9313/FastApi-RESTful
 Description-Content-Type: text/markdown
 
 <p align="center">
     <em>Quicker FastApi developing tools</em>
 </p>
 <p align="center">
 <a href="https://github.com/yuval9313/fastapi-restful" target="_blank">
@@ -58,15 +58,15 @@
 </a>
 <br />
 <a href="https://pypi.org/project/FastApi-RESTful" target="_blank">
     <img src="https://badge.fury.io/py/fastapi-restful.svg" alt="Package version">
 </a>
 <a href="https://github.com/yuval9313/fastapi-restful" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/FastApi-RESTful.svg" alt="Python versions">
-    <img src="https://img.shields.io/github/license/yuval9313/fastapi-utils.svg" alt="License">
+    <img src="https://img.shields.io/github/license/yuval9313/FastApi-RESTful.svg" alt="License">
 </a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-restful.netlify.app" target="_blank">https://fastapi-restful.netlify.app</a>
 
@@ -84,31 +84,30 @@
 
 ## Features
 
 This package includes a number of utilities to help reduce boilerplate and reuse common functionality across projects:
 
 * **Resource Class**: Create CRUD with ease the OOP way with `Resource` base class that lets you implement methods quick.
 * **Class Based Views**: Stop repeating the same dependencies over and over in the signature of related endpoints.
-* **Response-Model Inferring Router**: Let FastAPI infer the `response_model` to use based on your return type annotation. 
 * **Repeated Tasks**: Easily trigger periodic tasks on server startup
 * **Timing Middleware**: Log basic timing information for every request
 * **OpenAPI Spec Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from OpenAPI Generator
 * **SQLAlchemy Sessions**: The `FastAPISessionMaker` class provides an easily-customized SQLAlchemy Session dependency
 
 ---
 
 It also adds a variety of more basic utilities that are useful across a wide variety of projects:
 
 * **APIModel**: A reusable `pydantic.BaseModel`-derived base class with useful defaults
-* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables 
+* **APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to configure FastAPI through environment variables
 * **String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-valued enums easier to maintain
 * **CamelCase Conversions**: Convenience functions for converting strings from `snake_case` to `camelCase` or `PascalCase` and back
 * **GUID Type**: The provided GUID type makes it easy to use UUIDs as the primary keys for your database tables
 
-See the [docs](https://fastapi-restful.netlify.app/) for more details and examples. 
+See the [docs](https://fastapi-restful.netlify.app/) for more details and examples.
 
 ## Requirements
 
 This package is intended for use with any recent version of FastAPI (depending on `pydantic>=1.0`), and Python 3.7+.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-restful Version: 0.5.0 Summary: Quicker
+Metadata-Version: 2.1 Name: fastapi-restful Version: 0.6.0 Summary: Quicker
 FastApi developing tools Home-page: https://fastapi-restful.netlify.app
 License: MIT Keywords: fastapi,OOP,RESTful Author: Yuval Levi Author-email:
 yuvall9313@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
 AsyncIO Classifier: Framework :: FastAPI Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
@@ -19,43 +19,42 @@
 Classifier: Topic :: Utilities Classifier: Typing :: Typed Provides-Extra: all
 Provides-Extra: session Requires-Dist: fastapi (>=0.89,<1.0) Requires-Dist:
 psutil (>=5,<6) Requires-Dist: pydantic (>1.0,<3.0) Requires-Dist: pydantic-
 settings (>=2.0.1,<3.0.0) ; extra == "all" Requires-Dist: sqlalchemy
 (>=1.4,<3.0) ; extra == "all" or extra == "session" Requires-Dist: typing-
 inspect (>=0.9.0,<0.10.0) ; extra == "all" Project-URL: Documentation, https://
 fastapi-restful.netlify.app Project-URL: Repository, https://github.com/
-yuval9313/fastapi-utils Description-Content-Type: text/markdown
+yuval9313/FastApi-RESTful Description-Content-Type: text/markdown
                        QQuuiicckkeerr FFaassttAAppii ddeevveellooppiinngg ttoooollss
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_y_u_v_a_l_9_3_1_3_/_f_a_s_t_a_p_i_-_r_e_s_t_f_u_l_._s_v_g_]_[_B_u_i_l_d
                               _C_I_]_[_N_e_t_l_i_f_y_ _s_t_a_t_u_s_]
                   _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_f_a_s_t_a_p_i_-_r_e_s_t_f_u_l_._n_e_t_l_i_f_y_._a_p_p **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_v_a_l_9_3_1_3_/_f_a_s_t_a_p_i_-_r_e_s_t_f_u_l Base on: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
 _d_m_o_n_t_a_g_u_/_f_a_s_t_a_p_i_-_u_t_i_l_s --- _F_a_s_t_A_P_I is a modern, fast web framework for building
 APIs with Python 3.7+. But if you're here, you probably already knew that! --
 - ## Features This package includes a number of utilities to help reduce
 boilerplate and reuse common functionality across projects: * **Resource
 Class**: Create CRUD with ease the OOP way with `Resource` base class that lets
 you implement methods quick. * **Class Based Views**: Stop repeating the same
-dependencies over and over in the signature of related endpoints. * **Response-
-Model Inferring Router**: Let FastAPI infer the `response_model` to use based
-on your return type annotation. * **Repeated Tasks**: Easily trigger periodic
-tasks on server startup * **Timing Middleware**: Log basic timing information
-for every request * **OpenAPI Spec Simplification**: Simplify your OpenAPI
-Operation IDs for cleaner output from OpenAPI Generator * **SQLAlchemy
-Sessions**: The `FastAPISessionMaker` class provides an easily-customized
-SQLAlchemy Session dependency --- It also adds a variety of more basic
-utilities that are useful across a wide variety of projects: * **APIModel**: A
-reusable `pydantic.BaseModel`-derived base class with useful defaults *
-**APISettings**: A subclass of `pydantic.BaseSettings` that makes it easy to
-configure FastAPI through environment variables * **String-Valued Enums**: The
-`StrEnum` and `CamelStrEnum` classes make string-valued enums easier to
-maintain * **CamelCase Conversions**: Convenience functions for converting
-strings from `snake_case` to `camelCase` or `PascalCase` and back * **GUID
-Type**: The provided GUID type makes it easy to use UUIDs as the primary keys
-for your database tables See the [docs](https://fastapi-restful.netlify.app/
-) for more details and examples. ## Requirements This package is intended for
-use with any recent version of FastAPI (depending on `pydantic>=1.0`), and
-Python 3.7+. ## Installation ```bash pip install fastapi-restful # For basic
-slim package :) pip install fastapi-restful[session] # To add sqlalchemy
-session maker pip install fastapi-restful[all] # For all the packages ``` ##
-License This project is licensed under the terms of the MIT license.
+dependencies over and over in the signature of related endpoints. * **Repeated
+Tasks**: Easily trigger periodic tasks on server startup * **Timing
+Middleware**: Log basic timing information for every request * **OpenAPI Spec
+Simplification**: Simplify your OpenAPI Operation IDs for cleaner output from
+OpenAPI Generator * **SQLAlchemy Sessions**: The `FastAPISessionMaker` class
+provides an easily-customized SQLAlchemy Session dependency --- It also adds a
+variety of more basic utilities that are useful across a wide variety of
+projects: * **APIModel**: A reusable `pydantic.BaseModel`-derived base class
+with useful defaults * **APISettings**: A subclass of `pydantic.BaseSettings`
+that makes it easy to configure FastAPI through environment variables *
+**String-Valued Enums**: The `StrEnum` and `CamelStrEnum` classes make string-
+valued enums easier to maintain * **CamelCase Conversions**: Convenience
+functions for converting strings from `snake_case` to `camelCase` or
+`PascalCase` and back * **GUID Type**: The provided GUID type makes it easy to
+use UUIDs as the primary keys for your database tables See the [docs](https://
+fastapi-restful.netlify.app/) for more details and examples. ## Requirements
+This package is intended for use with any recent version of FastAPI (depending
+on `pydantic>=1.0`), and Python 3.7+. ## Installation ```bash pip install
+fastapi-restful # For basic slim package :) pip install fastapi-restful
+[session] # To add sqlalchemy session maker pip install fastapi-restful[all] #
+For all the packages ``` ## License This project is licensed under the terms of
+the MIT license.
```

