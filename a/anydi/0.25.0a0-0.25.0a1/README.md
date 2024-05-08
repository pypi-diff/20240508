# Comparing `tmp/anydi-0.25.0a0.tar.gz` & `tmp/anydi-0.25.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.25.0a0.tar", max compression
+gzip compressed data, was "anydi-0.25.0a1.tar", max compression
```

## Comparing `anydi-0.25.0a0.tar` & `anydi-0.25.0a1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a0/LICENSE
--rw-r--r--   0        0        0     2625 2024-03-11 08:19:19.508853 anydi-0.25.0a0/README.md
--rw-r--r--   0        0        0      562 2024-03-04 13:20:12.097070 anydi-0.25.0a0/anydi/__init__.py
--rw-r--r--   0        0        0    28347 2024-04-07 18:01:12.996941 anydi-0.25.0a0/anydi/_container.py
--rw-r--r--   0        0        0    10258 2024-02-28 07:17:37.315755 anydi-0.25.0a0/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a0/anydi/_logger.py
--rw-r--r--   0        0        0     3712 2024-03-04 13:20:12.098039 anydi-0.25.0a0/anydi/_module.py
--rw-r--r--   0        0        0     6781 2024-03-04 13:20:12.098430 anydi-0.25.0a0/anydi/_scanner.py
--rw-r--r--   0        0        0     3240 2024-02-28 07:17:37.316974 anydi-0.25.0a0/anydi/_types.py
--rw-r--r--   0        0        0     3152 2024-03-04 13:20:12.098746 anydi-0.25.0a0/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a0/anydi/ext/__init__.py
--rw-r--r--   0        0        0       59 2024-05-05 18:26:46.598768 anydi-0.25.0a0/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-05 18:26:47.962644 anydi-0.25.0a0/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      430 2024-05-05 18:27:49.545197 anydi-0.25.0a0/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     4739 2024-05-05 18:50:18.088878 anydi-0.25.0a0/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      520 2024-05-05 18:27:26.714331 anydi-0.25.0a0/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2660 2024-05-05 18:27:49.545197 anydi-0.25.0a0/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2177 2024-05-05 18:27:47.544088 anydi-0.25.0a0/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5311 2024-04-20 17:59:50.473425 anydi-0.25.0a0/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     3976 2024-03-20 12:47:26.894485 anydi-0.25.0a0/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a0/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a0/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a0/anydi/py.typed
--rw-r--r--   0        0        0     2905 2024-05-05 18:49:20.165988 anydi-0.25.0a0/pyproject.toml
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 anydi-0.25.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a1/LICENSE
+-rw-r--r--   0        0        0     2625 2024-05-06 12:48:30.095334 anydi-0.25.0a1/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.0a1/anydi/__init__.py
+-rw-r--r--   0        0        0    28341 2024-05-06 12:48:30.096342 anydi-0.25.0a1/anydi/_container.py
+-rw-r--r--   0        0        0    10258 2024-02-28 07:17:37.315755 anydi-0.25.0a1/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a1/anydi/_logger.py
+-rw-r--r--   0        0        0     3712 2024-03-04 13:20:12.098039 anydi-0.25.0a1/anydi/_module.py
+-rw-r--r--   0        0        0     6775 2024-05-06 12:48:30.096926 anydi-0.25.0a1/anydi/_scanner.py
+-rw-r--r--   0        0        0     3412 2024-05-06 12:48:30.097344 anydi-0.25.0a1/anydi/_types.py
+-rw-r--r--   0        0        0     3152 2024-03-04 13:20:12.098746 anydi-0.25.0a1/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a1/anydi/ext/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-06 12:48:26.500021 anydi-0.25.0a1/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-06 12:48:26.500416 anydi-0.25.0a1/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      430 2024-05-06 12:48:26.500759 anydi-0.25.0a1/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     6326 2024-05-07 16:36:00.772662 anydi-0.25.0a1/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      540 2024-05-06 17:06:30.923058 anydi-0.25.0a1/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-06 12:48:26.501627 anydi-0.25.0a1/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2177 2024-05-06 12:48:26.501823 anydi-0.25.0a1/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5311 2024-04-20 17:59:50.473425 anydi-0.25.0a1/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     3976 2024-03-20 12:47:26.894485 anydi-0.25.0a1/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a1/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a1/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a1/anydi/py.typed
+-rw-r--r--   0        0        0     3103 2024-05-07 16:39:52.000899 anydi-0.25.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 anydi-0.25.0a1/PKG-INFO
```

### Comparing `anydi-0.25.0a0/LICENSE` & `anydi-0.25.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/README.md` & `anydi-0.25.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 ```
 
 ## Quick Example
 
 *app.py*
 
 ```python
-from anydi import Container, dep
+from anydi import auto, Container
 
 container = Container()
 
 
 @container.provider(scope="singleton")
 def message() -> str:
     return "Hello, world!"
 
 
 @container.inject
-def say_hello(message: str = dep()) -> None:
+def say_hello(message: str = auto) -> None:
     print(message)
 
 
 if __name__ == "__main__":
     say_hello()
 ```
```

### Comparing `anydi-0.25.0a0/anydi/__init__.py` & `anydi-0.25.0a1/anydi/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """AnyDI public objects and functions."""
 
-from typing import Any
+from typing import Any, cast
 
 from ._container import Container, request, singleton, transient
 from ._module import Module, provider
 from ._scanner import injectable
 from ._types import Marker, Provider, Scope
 
 
 def dep() -> Any:
     """A marker for dependency injection."""
     return Marker()
 
 
 # Alias for dependency auto marker
-auto = dep
+auto = cast(Any, Marker())
 
 
 __all__ = [
     "Container",
     "Module",
     "Provider",
     "Scope",
```

### Comparing `anydi-0.25.0a0/anydi/_container.py` & `anydi-0.25.0a1/anydi/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ScopedContext,
     SingletonContext,
     TransientContext,
 )
 from ._logger import logger
 from ._module import Module, ModuleRegistry
 from ._scanner import Scanner
-from ._types import AnyInterface, Interface, Marker, Provider, Scope
+from ._types import AnyInterface, Interface, Provider, Scope, is_marker
 from ._utils import get_full_qualname, get_signature, is_builtin_type
 
 T = TypeVar("T", bound=Any)
 P = ParamSpec("P")
 
 ALLOWED_SCOPES: Dict[Scope, List[Scope]] = {
     "singleton": ["singleton"],
@@ -756,15 +756,15 @@
 
         Returns:
             A dictionary containing the names and annotations
                 of the injected parameters.
         """
         injected_params = {}
         for parameter in get_signature(obj).parameters.values():
-            if not isinstance(parameter.default, Marker):
+            if not is_marker(parameter.default):
                 continue
             try:
                 self._validate_injected_parameter(obj, parameter)
             except LookupError as exc:
                 if not self.strict:
                     logger.debug(
                         f"Cannot validate the `{get_full_qualname(obj)}` parameter "
```

### Comparing `anydi-0.25.0a0/anydi/_context.py` & `anydi-0.25.0a1/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/_module.py` & `anydi-0.25.0a1/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/_scanner.py` & `anydi-0.25.0a1/anydi/_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     cast,
     final,
     overload,
 )
 
 from typing_extensions import NamedTuple, ParamSpec
 
-from ._types import Marker
+from ._types import is_marker
 from ._utils import get_signature
 
 if TYPE_CHECKING:
     from ._container import Container
 
 
 T = TypeVar("T")
@@ -159,15 +159,15 @@
 
             # Get by Marker
             if inspect.isclass(member):
                 signature = get_signature(member.__init__)
             else:
                 signature = get_signature(member)
             for parameter in signature.parameters.values():
-                if isinstance(parameter.default, Marker):
+                if is_marker(parameter.default):
                     dependencies.append(
                         self._create_dependency(member=member, module=module)
                     )
                     continue
 
         return dependencies
```

### Comparing `anydi-0.25.0a0/anydi/_types.py` & `anydi-0.25.0a1/anydi/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Any, Callable, Type, TypeVar, Union
 
-from typing_extensions import Annotated, Literal, Mapping, TypeAlias
+from typing_extensions import Annotated, Literal, Mapping, Self, TypeAlias
 
 from ._utils import get_full_qualname, get_signature
 
 Scope = Literal["transient", "singleton", "request"]
 
 T = TypeVar("T")
 AnyInterface: TypeAlias = Union[Type[Any], Annotated[Any, ...]]
@@ -15,14 +15,22 @@
 
 
 class Marker:
     """A marker class for marking dependencies."""
 
     __slots__ = ()
 
+    def __call__(self) -> Self:
+        return self
+
+
+def is_marker(obj: Any) -> bool:
+    """Checks if an object is a marker."""
+    return isinstance(obj, Marker)
+
 
 @dataclass(frozen=True)
 class Provider:
     """Represents a provider object.
 
     Attributes:
         obj: The callable object that serves as the provider.
```

### Comparing `anydi-0.25.0a0/anydi/_utils.py` & `anydi-0.25.0a1/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/ext/django/apps.py` & `anydi-0.25.0a1/anydi/ext/django/apps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,124 @@
+import logging
 import types
+from asyncio import get_running_loop
 from functools import wraps
-from typing import Annotated, Any, get_origin
+from typing import Any, Callable, cast
 
 from django.apps import AppConfig
 from django.conf import settings
 from django.core.cache import BaseCache, caches
+from django.core.exceptions import ImproperlyConfigured
 from django.db import connections
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.urls import get_resolver
 from django.utils.module_loading import import_string
+from typing_extensions import Annotated, get_origin
 
 import anydi
 
 from ._utils import iter_urlpatterns
 
+logger = logging.getLogger(__name__)
+
 
 class ContainerConfig(AppConfig):  # type: ignore[misc]
     name = "anydi.ext.django"
     label = "anydi_django"
 
     # Prefix for Django settings
-    settings_prefix = "django.conf.settings"
+    settings_prefix = "django.conf.settings."
 
     def __init__(self, app_name: str, app_module: types.ModuleType | None) -> None:
         super().__init__(app_name, app_module)
         # Create a container
-        self.container = anydi.Container(
-            strict=getattr(settings, "ANYDI_STRICT_MODE", False),
-        )
+        container_getter_path = getattr(settings, "ANYDI_CONTAINER_GETTER", None)
+        if container_getter_path:
+            try:
+                container_getter = cast(
+                    Callable[[], anydi.Container], import_string(container_getter_path)
+                )
+            except ImportError as exc:
+                raise ImproperlyConfigured(
+                    f"Cannot import container getter '{container_getter_path}'."
+                ) from exc
+            self.container = container_getter()
+        else:
+            self.container = anydi.Container(
+                strict=getattr(settings, "ANYDI_STRICT_MODE", False),
+            )
 
-    def ready(self) -> None:
+    def ready(self) -> None:  # noqa: C901
         # Register Django settings
         if getattr(settings, "ANYDI_REGISTER_SETTINGS", False):
             self.register_settings()
 
         # Register Django components
         if getattr(settings, "ANYDI_REGISTER_COMPONENTS", False):
             self.register_components()
 
         # Register modules
         for module_path in getattr(settings, "ANYDI_MODULES", []):
-            module_cls = import_string(module_path)
+            try:
+                module_cls = import_string(module_path)
+            except ImportError as exc:
+                raise ImproperlyConfigured(
+                    f"Cannot import module '{module_path}'."
+                ) from exc
             self.container.register_module(module_cls)
 
         # Patching the django-ninja framework if it installed
         if getattr(settings, "ANYDI_PATCH_NINJA", False):
             self.patch_ninja()
 
         # Auto-injecting the container into views
         if urlconf := getattr(settings, "ANYDI_AUTO_INJECT_URLCONF", None):
             self.auto_inject_urlconf(urlconf)
 
+        # Scan packages
+        for scan_package in getattr(settings, "ANYDI_SCAN_PACKAGES", []):
+            self.container.scan(scan_package)
+
+        # Start the container
+        if getattr(settings, "ANYDI_START_CONTAINER", False):
+            try:
+                get_running_loop()
+            except RuntimeError:
+                logger.warning(
+                    "Starting the container is only supported in an async context."
+                )
+            else:
+                self.container.start()
+
     def register_settings(self) -> None:  # noqa: C901
         """Register Django settings into the container."""
 
         def _get_setting_value(value: Any) -> Any:
             return lambda: value
 
-        for setting_name, value in settings.__dict__.items():
+        for setting_name in dir(settings):
+            setting_value = getattr(settings, setting_name)
             if not setting_name.isupper():
                 continue
+
             self.container.register(
-                Annotated[Any, f"{self.settings_prefix}.{setting_name}"],
-                _get_setting_value(value),
+                Annotated[Any, f"{self.settings_prefix}{setting_name}"],
+                _get_setting_value(setting_value),
                 scope="singleton",
             )
 
         def _aware_settings(interface: Any) -> Any:
             origin = get_origin(interface)
             if origin is not Annotated:
-                return interface
+                return interface  # pragma: no cover
             named = interface.__metadata__[-1]
 
-            if isinstance(named, str):
+            if isinstance(named, str) and named.startswith(self.settings_prefix):
                 _, setting_name = named.rsplit(self.settings_prefix, maxsplit=1)
-                return Annotated[Any, f"{self.settings_prefix}.{setting_name}"]
+                return Annotated[Any, f"{self.settings_prefix}{setting_name}"]
             return interface
 
         def _resolve(resolve: Any) -> Any:
             @wraps(resolve)
             def wrapper(interface: Any) -> Any:
                 return resolve(_aware_settings(interface))
 
@@ -106,15 +146,14 @@
             self.container.register(
                 Annotated[BaseCache, cache_name],
                 _get_cache(cache_name),
                 scope="singleton",
             )
 
         # Register database connections
-
         def _get_connection(alias: str) -> Any:
             return lambda: connections[alias]
 
         for alias in connections:
             self.container.register(
                 Annotated[BaseDatabaseWrapper, alias],
                 _get_connection(alias),
@@ -123,15 +162,15 @@
 
     def auto_inject_urlconf(self, urlconf: str) -> None:
         """Auto-inject the container into views."""
         resolver = get_resolver(urlconf)
         for pattern in iter_urlpatterns(resolver.url_patterns):
             # Skip django-ninja views
             if pattern.lookup_str.startswith("ninja."):
-                continue
+                continue  # pragma: no cover
             pattern.callback = self.container.inject(pattern.callback)
 
     @staticmethod
     def patch_ninja() -> None:
         """Patch the django-ninja framework."""
         from .ninja import patch
```

### Comparing `anydi-0.25.0a0/anydi/ext/django/ninja/__init__.py` & `anydi-0.25.0a1/anydi/ext/django/ninja/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 try:
     from ninja import operation
-except ImportError as exc:
+except ImportError as exc:  # pragma: no cover
     raise ImportError(
         "'django-ninja' is not installed. "
         "Please install it using 'pip install django-ninja'."
     ) from exc
 
 from ._operation import AsyncOperation, Operation
 from ._signature import ViewSignature
```

### Comparing `anydi-0.25.0a0/anydi/ext/django/ninja/_operation.py` & `anydi-0.25.0a1/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/ext/django/ninja/_signature.py` & `anydi-0.25.0a1/anydi/ext/django/ninja/_signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from collections.abc import Callable
 from typing import Any
 
 from django.http import HttpResponse
-from ninja.signature.details import (  # noqa
-    FuncParam,
+from ninja.signature.details import (
+    FuncParam,  # noqa
     ViewSignature as BaseViewSignature,
 )
 from ninja.signature.utils import get_path_param_names, get_typed_signature
 
 from anydi._types import Marker  # noqa
```

### Comparing `anydi-0.25.0a0/anydi/ext/fastapi.py` & `anydi-0.25.0a1/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/ext/pytest_plugin.py` & `anydi-0.25.0a1/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/anydi/ext/starlette/middleware.py` & `anydi-0.25.0a1/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a0/pyproject.toml` & `anydi-0.25.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.25.0a0"
+version = "0.25.0a1"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -50,14 +50,15 @@
 ruff = "^0.4.3"
 pytest = "^8.1.0"
 pytest-cov = "^5.0.0"
 fastapi = "^0.100.0"
 httpx = "^0.26.0"
 django = "^4.2"
 django-ninja = "^1.1.0"
+pytest-django = "^4.8.0"
 
 [tool.poetry.plugins.pytest11]
 anydi = "anydi.ext.pytest_plugin"
 
 [tool.ruff]
 line-length = 88
 
@@ -85,14 +86,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 xfail_strict = true
 junit_family = "xunit2"
+DJANGO_SETTINGS_MODULE = "tests.ext.django.settings"
 
 [tool.coverage.report]
 exclude_also = [
     "pragma: no cover",
     "@abstractmethod",
     "@abc.abstractmethod",
     "if TYPE_CHECKING",
@@ -101,10 +103,16 @@
     "@t.overload",
     "raise NotImplementedError",
     "except ImportError:",
     "if has_signature_eval_str_arg",
     "if not anyio:",
 ]
 
+[tool.coverage.run]
+omit = [
+    "anydi/ext/django/ninja/_operation.py",
+    "anydi/ext/django/ninja/_signature.py",
+]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `anydi-0.25.0a0/PKG-INFO` & `anydi-0.25.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.25.0a0
+Version: 0.25.0a1
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -85,26 +85,26 @@
 ```
 
 ## Quick Example
 
 *app.py*
 
 ```python
-from anydi import Container, dep
+from anydi import auto, Container
 
 container = Container()
 
 
 @container.provider(scope="singleton")
 def message() -> str:
     return "Hello, world!"
 
 
 @container.inject
-def say_hello(message: str = dep()) -> None:
+def say_hello(message: str = auto) -> None:
     print(message)
 
 
 if __name__ == "__main__":
     say_hello()
 ```
```

