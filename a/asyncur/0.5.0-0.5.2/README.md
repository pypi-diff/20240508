# Comparing `tmp/asyncur-0.5.0.tar.gz` & `tmp/asyncur-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncur-0.5.0.tar", max compression
+gzip compressed data, was "asyncur-0.5.2.tar", max compression
```

## Comparing `asyncur-0.5.0.tar` & `asyncur-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.5.0/LICENSE
--rw-r--r--   0        0        0     1870 2024-04-25 08:31:01.627968 asyncur-0.5.0/README.md
--rw-r--r--   0        0        0      380 2024-04-25 03:15:51.639066 asyncur-0.5.0/asyncur/__init__.py
--rw-r--r--   0        0        0     4438 2024-04-18 07:08:46.175588 asyncur-0.5.0/asyncur/aio.py
--rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.5.0/asyncur/py.typed
--rw-r--r--   0        0        0     4084 2024-04-05 15:00:30.881587 asyncur-0.5.0/asyncur/timing.py
--rw-r--r--   0        0        0      859 2024-04-18 09:24:22.041437 asyncur-0.5.0/asyncur/utils.py
--rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.5.0/asyncur/xls.py
--rw-r--r--   0        0        0      976 2024-04-25 03:22:46.699512 asyncur-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 asyncur-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-07 09:10:14.471122 asyncur-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2442 2024-05-08 07:03:10.336085 asyncur-0.5.2/README.md
+-rw-r--r--   0        0        0      429 2024-05-08 06:30:39.462306 asyncur-0.5.2/asyncur/__init__.py
+-rw-r--r--   0        0        0     4438 2024-04-18 07:08:46.175588 asyncur-0.5.2/asyncur/aio.py
+-rw-r--r--   0        0        0     1984 2024-05-08 07:01:52.496219 asyncur-0.5.2/asyncur/client.py
+-rw-r--r--   0        0        0        0 2023-09-19 11:58:47.096600 asyncur-0.5.2/asyncur/py.typed
+-rw-r--r--   0        0        0     4104 2024-05-06 08:27:26.590055 asyncur-0.5.2/asyncur/timing.py
+-rw-r--r--   0        0        0      859 2024-04-18 09:24:22.041437 asyncur-0.5.2/asyncur/utils.py
+-rw-r--r--   0        0        0      927 2023-10-26 09:32:47.265695 asyncur-0.5.2/asyncur/xls.py
+-rw-r--r--   0        0        0     1226 2024-05-08 07:03:42.049934 asyncur-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 asyncur-0.5.2/PKG-INFO
```

### Comparing `asyncur-0.5.0/LICENSE` & `asyncur-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncur-0.5.0/README.md` & `asyncur-0.5.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -52,14 +52,40 @@
 >>> @timeit
 ... def sleep_test2():
 ...     time.sleep(3.1)
 ...
 >>> sleep_test2()
 sleep_test2 Cost: 3.1 seconds
 ```
+- AsyncRedis
+```py
+from contextlib import asynccontextmanager
+
+from asyncur import AsyncRedis
+from fastapi import FastAPI, Request
+
+@asynccontextmanager
+async def lifespan(app):
+    async with AsyncRedis(app):
+        yield
+
+app = FastAPI(lifespan=lifespan)
+
+@app.get('/')
+async def root(request: Request) -> list[str]:
+    return await AsyncRedis(request).keys()
+
+@app.get('/redis')
+async def get_value_from_redis_by_key(request: Request, key: str) -> str:
+    value = await AsyncRedis(request).get(key)
+    if not value:
+        return ''
+    return value.decode()
+```
+
 
 - Read Excel File(need to install with xls extra: `pip install "asyncur[xls]"`)
 ```py
 >>> from asycur.xls import load_xls
 >>> await load_xls('tests/demo.xlsx')
 [{'Column1': 'row1-\\t%c', 'Column2\nMultiLines': 0, 'Column 3': 1, 4: ''}, {'Column1': 'r2c1\n00', 'Column2\nMultiLines': 'r2 c2', 'Column 3': 2, 4: ''}]
 ```
```

### Comparing `asyncur-0.5.0/asyncur/aio.py` & `asyncur-0.5.2/asyncur/aio.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.5.0/asyncur/timing.py` & `asyncur-0.5.2/asyncur/timing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from __future__ import annotations
 
 import functools
 import inspect
+import sys
 import time
 from contextlib import (
     AbstractAsyncContextManager,
     AbstractContextManager,
-    contextmanager,
 )
 from types import TracebackType
-from typing import Any, Awaitable, Callable, Generator, TypeVar
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, TypeVar, overload
+
+if TYPE_CHECKING:  # pragma: no cover
+    if sys.version_info >= (3, 11):
+        from typing import Self
+    else:
+        from typing_extensions import Self
 
 T_Retval = TypeVar("T_Retval", Awaitable[Any], Any)
 
 
 class Timer(AbstractContextManager, AbstractAsyncContextManager):
     """Print time cost of the function.
 
@@ -56,27 +62,27 @@
 
     async def __aenter__(self) -> "Timer":
         return self.__enter__()
 
     async def __aexit__(self, *args, **kwargs) -> None:
         self.__exit__(*args, **kwargs)
 
-    def __enter__(self) -> "Timer":
+    def __enter__(self) -> "Self":
         self.start = time.time()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         self._echo()
 
-    def _recreate_cm(self) -> "Timer":
+    def _recreate_cm(self) -> "Self":
         return self.__class__(
             getattr(self, "func", None) or self.message, self.decimal_places
         )
 
     def __call__(self, *args, **kwargs) -> Any:
         if (func := getattr(self, "func", None)) is None:
             return None
@@ -89,48 +95,44 @@
 
             return inner(*args, **kwargs)
         else:
             with self._recreate_cm():
                 return func(*args, **kwargs)
 
 
-@contextmanager
-def timer(message: str, decimal_places=1) -> Generator[None, None, None]:
-    """Print time cost of the function.
+@overload
+def timeit(func: str) -> Timer: ...  # pragma: no cover
 
-    Usage::
-        >>> @timer('message')
-        >>> def read_text(filename):
-        ...     return Path(filename).read_text()
 
-        >>> with timer('do sth ...'):
-        ...     # ... sync code ...
-    """
-    start = time.time()
-    try:
-        yield
-    finally:
-        Timer.echo_cost(start, decimal_places, message)
+@overload
+def timeit(
+    func: Callable[..., T_Retval],
+) -> Callable[..., T_Retval]: ...  # pragma: no cover
 
 
-def timeit(func: Callable[..., T_Retval]) -> Callable[..., T_Retval]:
+def timeit(func: str | Callable[..., T_Retval]) -> Timer | Callable[..., T_Retval]:
     """Print time cost of the function.
 
     Usage::
         >>> @timeit
         >>> async def main():
         ...     # ... async code ...
 
         >>> @timeit
         >>> def read_text(filename):
         ...     return Path(filename).read_text()
 
         >>> res = timeit(sync_func)(*args, **kwargs)
         >>> result = await timeit(async_func)(*args, **kwargs)
+        >>> with timeit('message'):
+        ...     await main()
+
     """
+    if isinstance(func, str):
+        return Timer(func)
     func_name = getattr(func, "__name__", str(func))
     if inspect.iscoroutinefunction(func):
 
         @functools.wraps(func)
         async def deco(*args, **kwargs) -> T_Retval:
             async with Timer(func_name):
                 return await func(*args, **kwargs)
```

### Comparing `asyncur-0.5.0/asyncur/utils.py` & `asyncur-0.5.2/asyncur/utils.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.5.0/asyncur/xls.py` & `asyncur-0.5.2/asyncur/xls.py`

 * *Files identical despite different names*

### Comparing `asyncur-0.5.0/pyproject.toml` & `asyncur-0.5.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 [tool.poetry]
 name = "asyncur"
-version = "0.5.0"
+version = "0.5.2"
 description = "Async functions to compare with anyio and asyncio, and toolkit to read excel with async/await."
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = ">=3.7.1"
 pandas = {version = "^2.2.2", optional = true}
 openpyxl = {version = "^3.1.2", optional = true}
-exceptiongroup = { version = ">=1.2.0", python = "<3.11" }
-typing-extensions = { version = "^4.11.0", python = "<3.11" }
+exceptiongroup = "^1.2.1"
+typing-extensions = "^4.11.0"
+redis = "^5.0.4"
 
 [tool.poetry.extras]
 xls = ["pandas", "openpyxl"]
 
 
 [tool.poetry.group.dev.dependencies]
 fast-dev-cli = {version = ">=0.7.0", python = ">=3.11", extras = ["all"]}
 pandas-stubs = "^2.2.1.240316"
-coveralls = "^3.3.1"
-ruff = ">=0.3"
-pandas = "*"
-openpyxl = "*"
-mypy = "*"
-pytest = "*"
-coverage = "*"
+coveralls = {version = ">=3.3.1", python = ">=3.10,<3.13"}
+ruff = "^0.4.3"
+pandas = "^2.2.2"
+openpyxl = "^3.1.2"
+mypy = "^1.10.0"
+pytest = "^8.2.0"
+types-redis = "^4.6.0.20240425"
+fastapi = "^0.111.0"
+asgi-lifespan = "^2.1.0"
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 check_untyped_defs = true
 
+[tool.coverage.report]
+omit = ["*/tests/*", "test_*"]
+exclude_lines = [
+    "pragma: no cover",
+    "@overload",
+    'if __name__ == "__main__":',
+    "if TYPE_CHECKING:",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asyncur-0.5.0/PKG-INFO` & `asyncur-0.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: asyncur
-Version: 0.5.0
+Version: 0.5.2
 Summary: Async functions to compare with anyio and asyncio, and toolkit to read excel with async/await.
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: xls
 Requires-Dist: anyio (>=3.7.1)
-Requires-Dist: exceptiongroup (>=1.2.0) ; python_version < "3.11"
+Requires-Dist: exceptiongroup (>=1.2.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "xls"
 Requires-Dist: pandas (>=2.2.2,<3.0.0) ; extra == "xls"
-Requires-Dist: typing-extensions (>=4.11.0,<5.0.0) ; python_version < "3.11"
+Requires-Dist: redis (>=5.0.4,<6.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # asyncur
 ![Python Versions](https://img.shields.io/pypi/pyversions/asyncur)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/asyncur.svg?style=flat)](https://pypi.python.org/pypi/asyncur)
 [![GithubActionResult](https://github.com/waketzheng/asyncur/workflows/ci/badge.svg)](https://github.com/waketzheng/asyncur/actions?query=workflow:ci)
 [![Coverage Status](https://coveralls.io/repos/github/waketzheng/asyncur/badge.svg?branch=main)](https://coveralls.io/github/waketzheng/asyncur?branch=main)
@@ -71,14 +72,40 @@
 >>> @timeit
 ... def sleep_test2():
 ...     time.sleep(3.1)
 ...
 >>> sleep_test2()
 sleep_test2 Cost: 3.1 seconds
 ```
+- AsyncRedis
+```py
+from contextlib import asynccontextmanager
+
+from asyncur import AsyncRedis
+from fastapi import FastAPI, Request
+
+@asynccontextmanager
+async def lifespan(app):
+    async with AsyncRedis(app):
+        yield
+
+app = FastAPI(lifespan=lifespan)
+
+@app.get('/')
+async def root(request: Request) -> list[str]:
+    return await AsyncRedis(request).keys()
+
+@app.get('/redis')
+async def get_value_from_redis_by_key(request: Request, key: str) -> str:
+    value = await AsyncRedis(request).get(key)
+    if not value:
+        return ''
+    return value.decode()
+```
+
 
 - Read Excel File(need to install with xls extra: `pip install "asyncur[xls]"`)
 ```py
 >>> from asycur.xls import load_xls
 >>> await load_xls('tests/demo.xlsx')
 [{'Column1': 'row1-\\t%c', 'Column2\nMultiLines': 0, 'Column 3': 1, 4: ''}, {'Column1': 'r2c1\n00', 'Column2\nMultiLines': 'r2 c2', 'Column 3': 2, 4: ''}]
 ```
```

