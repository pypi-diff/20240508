# Comparing `tmp/picodi-0.4.2.tar.gz` & `tmp/picodi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.4.2.tar", max compression
+gzip compressed data, was "picodi-0.4.3.tar", max compression
```

## Comparing `picodi-0.4.2.tar` & `picodi-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-05-06 19:02:45.751363 picodi-0.4.2/LICENSE
--rw-r--r--   0        0        0     6787 2024-05-06 19:02:45.751363 picodi-0.4.2/README.md
--rw-r--r--   0        0        0      265 2024-05-06 19:02:45.751363 picodi-0.4.2/picodi/__init__.py
--rw-r--r--   0        0        0     9610 2024-05-06 19:02:45.751363 picodi-0.4.2/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-05-06 19:02:45.751363 picodi-0.4.2/picodi/py.typed
--rw-r--r--   0        0        0     4253 2024-05-06 19:02:45.751363 picodi-0.4.2/picodi/scopes.py
--rw-r--r--   0        0        0     2583 2024-05-06 19:02:45.751363 picodi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 picodi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-08 11:08:11.997047 picodi-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6904 2024-05-08 11:08:11.997047 picodi-0.4.3/README.md
+-rw-r--r--   0        0        0      265 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/__init__.py
+-rw-r--r--   0        0        0     9298 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/py.typed
+-rw-r--r--   0        0        0     4253 2024-05-08 11:08:11.997047 picodi-0.4.3/picodi/scopes.py
+-rw-r--r--   0        0        0     2604 2024-05-08 11:08:12.001047 picodi-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7666 1970-01-01 00:00:00.000000 picodi-0.4.3/PKG-INFO
```

### Comparing `picodi-0.4.2/LICENSE` & `picodi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.4.2/README.md` & `picodi-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -242,23 +242,27 @@
 - **Parameters**:
   - `dependency`: A callable that returns the dependency or a generator for context management.
 
 ### `inject(fn)`
 
 Decorator to automatically inject dependencies declared by `Provide` into a function.
 
+Should be placed first in the decorator chain (on bottom).
+
 - **Parameters**:
   - `fn`: The function into which dependencies will be injected.
 
 ### `resource(fn)`
 
 Decorator to declare a resource,
 which ensures that the provided function is treated as a singleton
 and that its lifecycle is managed across the application.
 
+Should be placed first in the decorator chain (on top).
+
 - **Parameters**:
   - `fn`: A generator function that yields a resource.
 
 ### `init_resources()`
 
 Initializes all declared resources. Typically called at the startup of the application.
```

### Comparing `picodi-0.4.2/picodi/picodi.py` & `picodi-0.4.3/picodi/picodi.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,15 @@
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
 try:
     import fastapi.params
 except ImportError:
-    fastapi = None
-
-
-try:
-    import fastapi.params
-except ImportError:
-    fastapi = None
+    fastapi = None  # type: ignore[assignment]
 
 
 Dependency = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
 TC = TypeVar("TC", bound=Callable)
 
@@ -73,23 +67,22 @@
         print("closing db connection")
 
     @inject
     def my_service(db: str = Provide(get_db)):
         assert db == "db connection"
     ```
     """
-    if not getattr(dependency, "_picodi_scope_", None):
-        dependency._picodi_scope_ = "null"  # type: ignore[attr-defined] # noqa: SF01
     return Depends.from_dependency(dependency)
 
 
 def inject(fn: Callable[P, T]) -> Callable[P, T]:
     """
     Decorator to inject dependencies into a function.
     Use it in combination with `Provide` to declare dependencies.
+    Should be placed first in the decorator chain (on bottom).
 
     Example:
     ```
     from picodi import inject, Provide
 
     @inject
     def my_service(db=Provide(some_dependency_func)):
@@ -140,52 +133,49 @@
 def resource(fn: TC) -> TC:
     """
     Decorator to declare a resource. Resource is a dependency that should be
     called only once, cached and shared across the application.
     On shutdown, all resources will be closed
     (you need to call `shutdown_resources` manually).
     Use it with a dependency generator function to declare a resource.
+    Should be placed last in the decorator chain (on top).
     """
-    if not inspect.isgeneratorfunction(fn) and not inspect.isasyncgenfunction(fn):
-        raise TypeError("Resource should be a generator function")
     fn._picodi_scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
     with _lock:
         _resources.append(Depends.from_dependency(fn))
     return fn
 
 
-def init_resources() -> Awaitable | None:
+def init_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
     async_resources = []
     for depends in _resources:
         if depends.is_async:
             async_resources.append(_resolve_value_async(depends))
         else:
             _resolve_value(depends)
 
-    if _is_async_environment():
-        return asyncio.gather(*async_resources)
-    return None
+    return asyncio.gather(*async_resources)
 
 
-def shutdown_resources() -> Awaitable | None:
+def shutdown_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shut down.
     """
     if _is_async_environment():
         tasks = [scope.exit_stack.close() for scope in _scopes.values()]
         return asyncio.gather(*tasks)  # type: ignore[arg-type]
 
     for scope in _scopes.values():
         scope.exit_stack.close(only_sync=True)
-    return None
+    return asyncio.gather(*[])
 
 
 def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
     signature = inspect.signature(fn)
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
 
@@ -214,17 +204,15 @@
         return cls(
             dependency,
             inspect.iscoroutinefunction(dependency)
             or inspect.isasyncgenfunction(dependency),
         )
 
     def get_scope(self) -> Scope:
-        scope_name = (
-            self.dependency._picodi_scope_  # type: ignore[attr-defined] # noqa: SF01
-        )
+        scope_name = getattr(self.dependency, "_picodi_scope_", "null")
         return _scopes[scope_name]
 
     def resolve_value(self) -> Any:
         scope = self.get_scope()
         value_or_gen = self.dependency()
         if self.is_async:
```

### Comparing `picodi-0.4.2/picodi/scopes.py` & `picodi-0.4.3/picodi/scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.4.2/pyproject.toml` & `picodi-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.4.2"
+version = "0.4.3"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
 
@@ -33,14 +33,15 @@
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-randomly = "^3.12"
+fastapi = "^0.111.0"
 
 [tool.isort]
 # isort configuration:
 # https://github.com/timothycrosley/isort/wiki/isort-Settings
 profile = "black"
 include_trailing_comma = true
 use_parentheses = true
```

### Comparing `picodi-0.4.2/PKG-INFO` & `picodi-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.4.2
+Version: 0.4.3
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -262,23 +262,27 @@
 - **Parameters**:
   - `dependency`: A callable that returns the dependency or a generator for context management.
 
 ### `inject(fn)`
 
 Decorator to automatically inject dependencies declared by `Provide` into a function.
 
+Should be placed first in the decorator chain (on bottom).
+
 - **Parameters**:
   - `fn`: The function into which dependencies will be injected.
 
 ### `resource(fn)`
 
 Decorator to declare a resource,
 which ensures that the provided function is treated as a singleton
 and that its lifecycle is managed across the application.
 
+Should be placed first in the decorator chain (on top).
+
 - **Parameters**:
   - `fn`: A generator function that yields a resource.
 
 ### `init_resources()`
 
 Initializes all declared resources. Typically called at the startup of the application.
```

