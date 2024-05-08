# Comparing `tmp/anydi-0.25.0a1.tar.gz` & `tmp/anydi-0.25.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.25.0a1.tar", max compression
+gzip compressed data, was "anydi-0.25.0a2.tar", max compression
```

## Comparing `anydi-0.25.0a1.tar` & `anydi-0.25.0a2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a1/LICENSE
--rw-r--r--   0        0        0     2625 2024-05-06 12:48:30.095334 anydi-0.25.0a1/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.0a1/anydi/__init__.py
--rw-r--r--   0        0        0    28341 2024-05-06 12:48:30.096342 anydi-0.25.0a1/anydi/_container.py
--rw-r--r--   0        0        0    10258 2024-02-28 07:17:37.315755 anydi-0.25.0a1/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a1/anydi/_logger.py
--rw-r--r--   0        0        0     3712 2024-03-04 13:20:12.098039 anydi-0.25.0a1/anydi/_module.py
--rw-r--r--   0        0        0     6775 2024-05-06 12:48:30.096926 anydi-0.25.0a1/anydi/_scanner.py
--rw-r--r--   0        0        0     3412 2024-05-06 12:48:30.097344 anydi-0.25.0a1/anydi/_types.py
--rw-r--r--   0        0        0     3152 2024-03-04 13:20:12.098746 anydi-0.25.0a1/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a1/anydi/ext/__init__.py
--rw-r--r--   0        0        0       59 2024-05-06 12:48:26.500021 anydi-0.25.0a1/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-06 12:48:26.500416 anydi-0.25.0a1/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      430 2024-05-06 12:48:26.500759 anydi-0.25.0a1/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     6326 2024-05-07 16:36:00.772662 anydi-0.25.0a1/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      540 2024-05-06 17:06:30.923058 anydi-0.25.0a1/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2660 2024-05-06 12:48:26.501627 anydi-0.25.0a1/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2177 2024-05-06 12:48:26.501823 anydi-0.25.0a1/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5311 2024-04-20 17:59:50.473425 anydi-0.25.0a1/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     3976 2024-03-20 12:47:26.894485 anydi-0.25.0a1/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a1/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a1/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a1/anydi/py.typed
--rw-r--r--   0        0        0     3103 2024-05-07 16:39:52.000899 anydi-0.25.0a1/pyproject.toml
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 anydi-0.25.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a2/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 08:47:53.359541 anydi-0.25.0a2/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.0a2/anydi/__init__.py
+-rw-r--r--   0        0        0    27978 2024-05-08 08:36:20.511875 anydi-0.25.0a2/anydi/_container.py
+-rw-r--r--   0        0        0    10215 2024-05-08 08:36:20.512415 anydi-0.25.0a2/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a2/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-08 08:27:43.981700 anydi-0.25.0a2/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.0a2/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.0a2/anydi/_types.py
+-rw-r--r--   0        0        0     3439 2024-05-08 08:36:20.513338 anydi-0.25.0a2/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a2/anydi/ext/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-08 08:36:17.250672 anydi-0.25.0a2/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 08:36:17.250922 anydi-0.25.0a2/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      828 2024-05-08 08:36:17.251228 anydi-0.25.0a2/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3491 2024-05-08 08:36:17.251589 anydi-0.25.0a2/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2760 2024-05-08 08:36:17.251795 anydi-0.25.0a2/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 08:36:17.252105 anydi-0.25.0a2/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 08:36:17.252306 anydi-0.25.0a2/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 08:36:17.252503 anydi-0.25.0a2/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2213 2024-05-08 08:36:17.252796 anydi-0.25.0a2/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.0a2/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     3999 2024-05-08 06:51:25.864651 anydi-0.25.0a2/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a2/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a2/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a2/anydi/py.typed
+-rw-r--r--   0        0        0     3109 2024-05-08 08:48:33.072752 anydi-0.25.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 anydi-0.25.0a2/PKG-INFO
```

### Comparing `anydi-0.25.0a1/LICENSE` & `anydi-0.25.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a1/README.md` & `anydi-0.25.0a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -94,7 +94,63 @@
 def say_hello(message: str = Inject()) -> dict[str, str]:
     return {"message": message}
 
 
 # Install the container into the FastAPI app
 anydi.ext.fastapi.install(app, container)
 ```
+
+
+
+## Django Ninja Example
+
+*container.py*
+
+```python
+from anydi import Container
+
+
+def get_container() -> Container:
+    container = Container()
+
+    @container.provider(scope="singleton")
+    def message() -> str:
+        return "Hello, World!"
+
+    return container
+```
+
+*settings.py*
+
+```python
+INSTALLED_APPS = [
+    ...
+    "anydi.ext.django",
+]
+
+ANYDI = {
+    "CONTAINER_FACTORY": "myapp.container.get_container",
+    "PATCH_NINJA": True,
+}
+```
+
+*urls.py*
+
+```python
+from django.http import HttpRequest
+from django.urls import path
+from ninja import NinjaAPI
+
+from anydi import auto
+
+api = NinjaAPI()
+
+
+@api.get("/hello")
+def say_hello(request: HttpRequest, message: str = auto) -> dict[str, str]:
+    return {"message": message}
+
+
+urlpatterns = [
+    path("api/", api.urls),
+]
+```
```

### Comparing `anydi-0.25.0a1/anydi/__init__.py` & `anydi-0.25.0a2/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a1/anydi/_container.py` & `anydi-0.25.0a2/anydi/_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,24 @@
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
     Awaitable,
     Callable,
     ContextManager,
-    Dict,
     Iterable,
     Iterator,
-    List,
     Mapping,
-    Optional,
     Sequence,
-    Type,
     TypeVar,
-    Union,
     cast,
     overload,
 )
 
-from typing_extensions import Annotated, ParamSpec, final, get_args, get_origin
+from typing_extensions import ParamSpec, final, get_args, get_origin
 
 try:
     from types import NoneType
 except ImportError:
     NoneType = type(None)  # type: ignore[misc]
 
 
@@ -44,20 +39,25 @@
     SingletonContext,
     TransientContext,
 )
 from ._logger import logger
 from ._module import Module, ModuleRegistry
 from ._scanner import Scanner
 from ._types import AnyInterface, Interface, Provider, Scope, is_marker
-from ._utils import get_full_qualname, get_signature, is_builtin_type
+from ._utils import (
+    get_full_qualname,
+    get_typed_parameters,
+    get_typed_return_annotation,
+    is_builtin_type,
+)
 
 T = TypeVar("T", bound=Any)
 P = ParamSpec("P")
 
-ALLOWED_SCOPES: Dict[Scope, List[Scope]] = {
+ALLOWED_SCOPES: dict[Scope, list[Scope]] = {
     "singleton": ["singleton"],
     "request": ["request", "singleton"],
     "transient": ["transient", "singleton", "request"],
 }
 
 
 @final
@@ -67,34 +67,33 @@
     Args:
         modules: Optional sequence of modules to register during initialization.
     """
 
     def __init__(
         self,
         *,
-        providers: Optional[Mapping[Type[Any], Provider]] = None,
-        modules: Optional[
-            Sequence[Union[Module, Type[Module], Callable[[Container], None]]]
-        ] = None,
+        providers: Mapping[type[Any], Provider] | None = None,
+        modules: Sequence[Module | type[Module] | Callable[[Container], None]]
+        | None = None,
         strict: bool = False,
     ) -> None:
         """Initialize the AnyDI instance.
 
         Args:
             providers: Optional mapping of providers to register during initialization.
             modules: Optional sequence of modules to register during initialization.
             strict: Whether to enable strict mode. Defaults to False.
         """
-        self._providers: Dict[Type[Any], Provider] = {}
+        self._providers: dict[type[Any], Provider] = {}
         self._singleton_context = SingletonContext(self)
         self._transient_context = TransientContext(self)
-        self._request_context_var: ContextVar[Optional[RequestContext]] = ContextVar(
+        self._request_context_var: ContextVar[RequestContext | None] = ContextVar(
             "request_context", default=None
         )
-        self._override_instances: Dict[Type[Any], Any] = {}
+        self._override_instances: dict[type[Any], Any] = {}
         self._strict = strict
 
         # Components
         self._modules = ModuleRegistry(self)
         self._scanner = Scanner(self)
 
         # Register providers
@@ -113,15 +112,15 @@
 
         Returns:
             True if strict mode is enabled, False otherwise.
         """
         return self._strict
 
     @property
-    def providers(self) -> Dict[Type[Any], Provider]:
+    def providers(self) -> dict[type[Any], Provider]:
         """Get the registered providers.
 
         Returns:
             A dictionary containing the registered providers.
         """
         return self._providers
 
@@ -329,15 +328,15 @@
 
         Raises:
             ValueError: If the provider and its dependencies have mismatched scopes.
             TypeError: If a dependency is missing an annotation.
         """
         related_providers = []
 
-        for parameter in provider.parameters.values():
+        for parameter in provider.parameters:
             if parameter.annotation is inspect._empty:  # noqa
                 raise TypeError(
                     f"Missing provider `{provider}` "
                     f"dependency `{parameter.name}` annotation."
                 )
             try:
                 sub_provider = self._get_or_register_provider(parameter.annotation)
@@ -359,24 +358,24 @@
                     f"The provider `{provider}` with a {provider.scope} scope was "
                     "attempted to be registered with the provider "
                     f"`{related_provider}` with a `{related_provider.scope}` scope, "
                     "which is not allowed. Please ensure that all providers are "
                     "registered with matching scopes."
                 )
 
-    def _detect_scope(self, obj: Callable[..., Any]) -> Optional[Scope]:
+    def _detect_scope(self, obj: Callable[..., Any]) -> Scope | None:
         """Detect the scope for a provider.
 
         Args:
             obj: The provider to detect the auto scope for.
         Returns:
             The auto scope, or None if the auto scope cannot be detected.
         """
         has_transient, has_request, has_singleton = False, False, False
-        for parameter in get_signature(obj).parameters.values():
+        for parameter in get_typed_parameters(obj):
             sub_provider = self._get_or_register_provider(parameter.annotation)
             if not has_transient and sub_provider.scope == "transient":
                 has_transient = True
             if not has_request and sub_provider.scope == "request":
                 has_request = True
             if not has_singleton and sub_provider.scope == "singleton":
                 has_singleton = True
@@ -385,15 +384,15 @@
         if has_request:
             return "request"
         if has_singleton:
             return "singleton"
         return None
 
     def register_module(
-        self, module: Union[Module, Type[Module], Callable[[Container], None]]
+        self, module: Module | type[Module] | Callable[[Container], None]
     ) -> None:
         """Register a module as a callable, module type, or module instance.
 
         Args:
             module: The module to register.
         """
         self._modules.register(module)
@@ -629,35 +628,32 @@
     @overload
     def inject(self, obj: Callable[P, T]) -> Callable[P, T]: ...
 
     @overload
     def inject(self) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
     def inject(
-        self, obj: Union[Callable[P, Union[T, Awaitable[T]]], None] = None
-    ) -> Union[
-        Callable[
-            [Callable[P, Union[T, Awaitable[T]]]],
-            Callable[P, Union[T, Awaitable[T]]],
-        ],
-        Callable[P, Union[T, Awaitable[T]]],
-    ]:
+        self, obj: Callable[P, T | Awaitable[T]] | None = None
+    ) -> (
+        Callable[[Callable[P, T | Awaitable[T]]], Callable[P, T | Awaitable[T]]]
+        | Callable[P, T | Awaitable[T]]
+    ):
         """Decorator to inject dependencies into a callable.
 
         Args:
             obj: The callable object to be decorated. If None, returns
                 the decorator itself.
 
         Returns:
             The decorated callable object or decorator function.
         """
 
         def decorator(
-            obj: Callable[P, Union[T, Awaitable[T]]],
-        ) -> Callable[P, Union[T, Awaitable[T]]]:
+            obj: Callable[P, T | Awaitable[T]],
+        ) -> Callable[P, T | Awaitable[T]]:
             injected_params = self._get_injected_params(obj)
 
             if inspect.iscoroutinefunction(obj):
 
                 @wraps(obj)
                 async def awrapped(*args: P.args, **kwargs: P.kwargs) -> T:
                     for name, annotation in injected_params.items():
@@ -690,20 +686,17 @@
             The result of the callable object.
         """
         return self.inject(obj)(*args, **kwargs)
 
     def scan(
         self,
         /,
-        packages: Union[
-            Union[types.ModuleType, str],
-            Iterable[Union[types.ModuleType, str]],
-        ],
+        packages: types.ModuleType | str | Iterable[types.ModuleType | str],
         *,
-        tags: Optional[Iterable[str]] = None,
+        tags: Iterable[str] | None = None,
     ) -> None:
         """Scan packages or modules for decorated members and inject dependencies.
 
         Args:
             packages: A single package or module to scan,
                 or an iterable of packages or modules to scan.
             tags: Optional list of tags to filter the scanned members. Only members
@@ -719,51 +712,45 @@
 
         Returns:
             The provider return annotation.
 
         Raises:
             TypeError: If the provider return annotation is missing or invalid.
         """
-        annotation = get_signature(obj).return_annotation
+        annotation = get_typed_return_annotation(obj)
 
-        if annotation is inspect._empty:  # noqa
+        if annotation is None:
             raise TypeError(
                 f"Missing `{get_full_qualname(obj)}` provider return annotation."
             )
 
-        origin = get_origin(annotation) or annotation
-        args = get_args(annotation)
-
-        # Supported generic types
-        if origin in (list, dict, tuple, Annotated):
+        if get_origin(annotation) in (get_origin(Iterator), get_origin(AsyncIterator)):
+            args = get_args(annotation)
             if args:
-                return annotation
+                return args[0]
             else:
                 raise TypeError(
-                    f"Cannot use `{get_full_qualname(obj)}` generic type annotation "
+                    f"Cannot use `{get_full_qualname(obj)}` resource type annotation "
                     "without actual type."
                 )
 
-        try:
-            return args[0]
-        except IndexError:
-            return annotation
+        return annotation
 
-    def _get_injected_params(self, obj: Callable[..., Any]) -> Dict[str, Any]:
+    def _get_injected_params(self, obj: Callable[..., Any]) -> dict[str, Any]:
         """Get the injected parameters of a callable object.
 
         Args:
             obj: The callable object.
 
         Returns:
             A dictionary containing the names and annotations
                 of the injected parameters.
         """
         injected_params = {}
-        for parameter in get_signature(obj).parameters.values():
+        for parameter in get_typed_parameters(obj):
             if not is_marker(parameter.default):
                 continue
             try:
                 self._validate_injected_parameter(obj, parameter)
             except LookupError as exc:
                 if not self.strict:
                     logger.debug(
```

### Comparing `anydi-0.25.0a1/anydi/_context.py` & `anydi-0.25.0a2/anydi/_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import abc
 import contextlib
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Type, TypeVar, cast
+from typing import TYPE_CHECKING, Any, TypeVar, cast
 
 from typing_extensions import Self, final
 
 from ._types import AnyInterface, Interface, Provider
 from ._utils import run_async
 
 if TYPE_CHECKING:
@@ -83,60 +83,60 @@
         args, kwargs = await self._aget_provider_arguments(provider)
         if provider.is_coroutine:
             return await provider.obj(*args, **kwargs)
         return await run_async(provider.obj, *args, **kwargs)
 
     def _get_provider_arguments(
         self, provider: Provider
-    ) -> Tuple[List[Any], Dict[str, Any]]:
+    ) -> tuple[list[Any], dict[str, Any]]:
         """Retrieve the arguments for a provider.
 
         Args:
             provider: The provider object.
 
         Returns:
             The arguments for the provider.
         """
         args, kwargs = [], {}
-        for parameter in provider.parameters.values():
+        for parameter in provider.parameters:
             instance = self.container.resolve(parameter.annotation)
             if parameter.kind == parameter.POSITIONAL_ONLY:
                 args.append(instance)
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
     async def _aget_provider_arguments(
         self, provider: Provider
-    ) -> Tuple[List[Any], Dict[str, Any]]:
+    ) -> tuple[list[Any], dict[str, Any]]:
         """Asynchronously retrieve the arguments for a provider.
 
         Args:
             provider: The provider object.
 
         Returns:
             The arguments for the provider.
         """
         args, kwargs = [], {}
-        for parameter in provider.parameters.values():
+        for parameter in provider.parameters:
             instance = await self.container.aresolve(parameter.annotation)
             if parameter.kind == parameter.POSITIONAL_ONLY:
                 args.append(instance)
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
 
 class ResourceScopedContext(ScopedContext):
     """ScopedContext with closable resources support."""
 
     def __init__(self, container: Container) -> None:
         """Initialize the ScopedContext."""
         super().__init__(container)
-        self._instances: Dict[Type[Any], Any] = {}
+        self._instances: dict[type[Any], Any] = {}
         self._stack = contextlib.ExitStack()
         self._async_stack = contextlib.AsyncExitStack()
 
     def get(self, interface: Interface[T], provider: Provider) -> T:
         """Get an instance of a dependency from the scoped context.
 
         Args:
@@ -233,15 +233,15 @@
         Returns:
             The scoped context.
         """
         return self
 
     def __exit__(
         self,
-        exc_type: Type[BaseException] | None,
+        exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Exit the context.
 
         Args:
             exc_type: The type of the exception, if any.
@@ -261,15 +261,15 @@
         Returns:
             The scoped context.
         """
         return self
 
     async def __aexit__(
         self,
-        exc_type: Type[BaseException] | None,
+        exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Exit the context asynchronously.
 
         Args:
             exc_type: The type of the exception, if any.
```

### Comparing `anydi-0.25.0a1/anydi/_module.py` & `anydi-0.25.0a2/anydi/_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """AnyDI decorators module."""
 
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Tuple, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 from typing_extensions import Concatenate, NamedTuple, ParamSpec
 
 from ._types import Scope
 
 if TYPE_CHECKING:
     from ._container import Container
@@ -20,15 +20,15 @@
 class ModuleMeta(type):
     """A metaclass used for the Module base class.
 
     This metaclass extracts provider information from the class attributes
     and stores it in the `providers` attribute.
     """
 
-    def __new__(cls, name: str, bases: Tuple[type, ...], attrs: Dict[str, Any]) -> Any:
+    def __new__(cls, name: str, bases: tuple[type, ...], attrs: dict[str, Any]) -> Any:
         """Create a new instance of the ModuleMeta class.
 
         This method extracts provider information from the class attributes and
         stores it in the `providers` attribute.
 
         Args:
             name: The name of the class.
@@ -45,15 +45,15 @@
         ]
         return super().__new__(cls, name, bases, attrs)
 
 
 class Module(metaclass=ModuleMeta):
     """A base class for defining AnyDI modules."""
 
-    providers: List[Tuple[str, ProviderDecoratorArgs]]
+    providers: list[tuple[str, ProviderDecoratorArgs]]
 
     def configure(self, container: Container) -> None:
         """Configure the AnyDI container with providers and their dependencies.
 
         This method can be overridden in derived classes to provide the
         configuration logic.
 
@@ -63,15 +63,15 @@
 
 
 class ModuleRegistry:
     def __init__(self, container: Container) -> None:
         self.container = container
 
     def register(
-        self, module: Union[Module, Type[Module], Callable[[Container], None]]
+        self, module: Module | type[Module] | Callable[[Container], None]
     ) -> None:
         """Register a module as a callable, module type, or module instance.
 
         Args:
             module: The module to register.
         """
         # Callable Module
```

### Comparing `anydi-0.25.0a1/anydi/_scanner.py` & `anydi-0.25.0a2/anydi/_scanner.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from dataclasses import dataclass
 from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
-    List,
-    Optional,
     TypeVar,
     Union,
     cast,
     final,
     overload,
 )
 
 from typing_extensions import NamedTuple, ParamSpec
 
 from ._types import is_marker
-from ._utils import get_signature
+from ._utils import get_typed_parameters
 
 if TYPE_CHECKING:
     from ._container import Container
 
 
 T = TypeVar("T")
 P = ParamSpec("P")
@@ -52,46 +50,46 @@
 
     def __init__(self, container: Container) -> None:
         self.container = container
 
     def scan(
         self,
         /,
-        packages: Union[Union[ModuleType, str], Iterable[Union[ModuleType, str]]],
+        packages: ModuleType | str | Iterable[ModuleType | str],
         *,
-        tags: Optional[Iterable[str]] = None,
+        tags: Iterable[str] | None = None,
     ) -> None:
         """Scan packages or modules for decorated members and inject dependencies.
 
         Args:
             packages: A single package or module to scan,
                 or an iterable of packages or modules to scan.
             tags: Optional list of tags to filter the scanned members. Only members
                 with at least one matching tag will be scanned. Defaults to None.
         """
-        dependencies: List[Dependency] = []
+        dependencies: list[Dependency] = []
 
         if isinstance(packages, Iterable) and not isinstance(packages, str):
-            scan_packages: Iterable[Union[ModuleType, str]] = packages
+            scan_packages: Iterable[ModuleType | str] = packages
         else:
             scan_packages = cast(Iterable[Union[ModuleType, str]], [packages])
 
         for package in scan_packages:
             dependencies.extend(self._scan_package(package, tags=tags))
 
         for dependency in dependencies:
             decorator = self.container.inject()(dependency.member)
             setattr(dependency.module, dependency.member.__name__, decorator)
 
     def _scan_package(
         self,
-        package: Union[ModuleType, str],
+        package: ModuleType | str,
         *,
-        tags: Optional[Iterable[str]] = None,
-    ) -> List[Dependency]:
+        tags: Iterable[str] | None = None,
+    ) -> list[Dependency]:
         """Scan a package or module for decorated members.
 
         Args:
             package: The package or module to scan.
             tags: Optional list of tags to filter the scanned members. Only members
                 with at least one matching tag will be scanned. Defaults to None.
 
@@ -103,38 +101,38 @@
             package = importlib.import_module(package)
 
         package_path = getattr(package, "__path__", None)
 
         if not package_path:
             return self._scan_module(package, tags=tags)
 
-        dependencies: List[Dependency] = []
+        dependencies: list[Dependency] = []
 
         for module_info in pkgutil.walk_packages(
             path=package_path, prefix=package.__name__ + "."
         ):
             module = importlib.import_module(module_info.name)
             dependencies.extend(self._scan_module(module, tags=tags))
 
         return dependencies
 
     def _scan_module(
         self, module: ModuleType, *, tags: Iterable[str]
-    ) -> List[Dependency]:
+    ) -> list[Dependency]:
         """Scan a module for decorated members.
 
         Args:
             module: The module to scan.
             tags: List of tags to filter the scanned members. Only members with at
                 least one matching tag will be scanned.
 
         Returns:
             A list of scanned dependencies.
         """
-        dependencies: List[Dependency] = []
+        dependencies: list[Dependency] = []
 
         for _, member in inspect.getmembers(module):
             if getattr(member, "__module__", None) != module.__name__ or not callable(
                 member
             ):
                 continue
 
@@ -155,18 +153,18 @@
                 dependencies.append(
                     self._create_dependency(member=member, module=module)
                 )
                 continue
 
             # Get by Marker
             if inspect.isclass(member):
-                signature = get_signature(member.__init__)
+                parameters = get_typed_parameters(member.__init__)
             else:
-                signature = get_signature(member)
-            for parameter in signature.parameters.values():
+                parameters = get_typed_parameters(member)
+            for parameter in parameters:
                 if is_marker(parameter.default):
                     dependencies.append(
                         self._create_dependency(member=member, module=module)
                     )
                     continue
 
         return dependencies
@@ -184,37 +182,31 @@
         if hasattr(member, "__wrapped__"):
             member = member.__wrapped__
         return Dependency(member=member, module=module)
 
 
 class InjectDecoratorArgs(NamedTuple):
     wrapped: bool
-    tags: Optional[Iterable[str]]
+    tags: Iterable[str] | None
 
 
 @overload
 def injectable(obj: Callable[P, T]) -> Callable[P, T]: ...
 
 
 @overload
 def injectable(
-    *, tags: Optional[Iterable[str]] = None
+    *, tags: Iterable[str] | None = None
 ) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
 
 def injectable(
-    obj: Optional[Callable[P, T]] = None,
-    tags: Optional[Iterable[str]] = None,
-) -> Union[
-    Callable[
-        [Callable[P, T]],
-        Callable[P, T],
-    ],
-    Callable[P, T],
-]:
+    obj: Callable[P, T] | None = None,
+    tags: Iterable[str] | None = None,
+) -> Callable[[Callable[P, T]], Callable[P, T]] | Callable[P, T]:
     """Decorator for marking a function or method as requiring dependency injection.
 
     Args:
         obj: The target function or method to be decorated.
         tags: Optional tags to associate with the injection point.
 
     Returns:
```

### Comparing `anydi-0.25.0a1/anydi/_types.py` & `anydi-0.25.0a2/anydi/_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import inspect
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Any, Callable, Type, TypeVar, Union
 
-from typing_extensions import Annotated, Literal, Mapping, Self, TypeAlias
+from typing_extensions import Annotated, Literal, Self, TypeAlias
 
-from ._utils import get_full_qualname, get_signature
+from ._utils import get_full_qualname, get_typed_parameters
 
 Scope = Literal["transient", "singleton", "request"]
 
 T = TypeVar("T")
 AnyInterface: TypeAlias = Union[Type[Any], Annotated[Any, ...]]
 Interface: TypeAlias = Type[T]
 
@@ -54,21 +56,21 @@
 
         Returns:
             The full qualified name of the provider object.
         """
         return get_full_qualname(self.obj)
 
     @cached_property
-    def parameters(self) -> Mapping[str, inspect.Parameter]:
+    def parameters(self) -> list[inspect.Parameter]:
         """Returns the parameters of the provider as a mapping.
 
         Returns:
             The parameters of the provider.
         """
-        return get_signature(self.obj).parameters
+        return get_typed_parameters(self.obj)
 
     @cached_property
     def is_class(self) -> bool:
         """Checks if the provider object is a class.
 
         Returns:
             True if the provider object is a class, False otherwise.
```

### Comparing `anydi-0.25.0a1/anydi/_utils.py` & `anydi-0.25.0a2/anydi/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """Shared AnyDI utils module."""
 
+from __future__ import annotations
+
 import builtins
 import functools
 import inspect
 import sys
-from typing import Any, Callable, Dict, Type, TypeVar
+from typing import Any, Callable, ForwardRef, TypeVar, cast
 
 from typing_extensions import Annotated, ParamSpec, get_origin
 
 try:
     import anyio  # noqa
 except ImportError:
     anyio = None  # type: ignore[assignment]
 
 
-T = TypeVar("T")
-P = ParamSpec("P")
+if sys.version_info < (3, 9):  # pragma: nocover
 
+    def evaluate_forwardref(type_: ForwardRef, globalns: Any, localns: Any) -> Any:
+        return type_._evaluate(globalns, localns)  # noqa
 
-def get_full_qualname(obj: Any) -> str:
-    """Get the fully qualified name of an object.
+else:
 
-    This function returns the fully qualified name of the given object,
-    which includes both the module name and the object's qualname.
+    def evaluate_forwardref(type_: ForwardRef, globalns: Any, localns: Any) -> Any:
+        return cast(Any, type_)._evaluate(globalns, localns, set())  # noqa
 
-    Args:
-        obj: The object for which to retrieve the fully qualified name.
 
-    Returns:
-        The fully qualified name of the object.
-    """
+T = TypeVar("T")
+P = ParamSpec("P")
+
+
+def get_full_qualname(obj: Any) -> str:
+    """Get the fully qualified name of an object."""
     origin = get_origin(obj)
     if origin is Annotated:
         metadata = ", ".join(
             [
                 f'"{arg}"' if isinstance(arg, str) else str(arg)
                 for arg in obj.__metadata__
             ]
@@ -49,63 +52,60 @@
         module_name = type(obj).__module__
 
     if module_name == builtins.__name__:
         return qualname
     return f"{module_name}.{qualname}"
 
 
-def is_builtin_type(tp: Type[Any]) -> bool:
-    """
-    Check if the given type is a built-in type.
-    Args:
-        tp (type): The type to check.
-    Returns:
-        bool: True if the type is a built-in type, False otherwise.
-    """
+def is_builtin_type(tp: type[Any]) -> bool:
+    """Check if the given type is a built-in type."""
     return tp.__module__ == builtins.__name__
 
 
-@functools.lru_cache(maxsize=None)
-def get_signature(obj: Callable[..., Any]) -> inspect.Signature:
-    """Get the signature of a callable object.
-
-    This function uses the `inspect.signature` function to retrieve the signature
-    of the given callable object. It applies an LRU cache decorator to improve
-    performance by caching the signatures of previously inspected objects.
-
-    Args:
-        obj: The callable object to inspect.
-
-    Returns:
-        The signature of the callable object.
-    """
-    signature_kwargs: Dict[str, Any] = {}
-    if sys.version_info >= (3, 10):
-        signature_kwargs["eval_str"] = True
-    return inspect.signature(obj, **signature_kwargs)
+def make_forwardref(annotation: str, globalns: dict[str, Any]) -> Any:
+    """Create a forward reference from a string annotation."""
+    forward_ref = ForwardRef(annotation)
+    return evaluate_forwardref(forward_ref, globalns, globalns)
+
+
+def get_typed_annotation(annotation: Any, globalns: dict[str, Any]) -> Any:
+    """Get the typed annotation of a parameter."""
+    if isinstance(annotation, str):
+        annotation = ForwardRef(annotation)
+        annotation = evaluate_forwardref(annotation, globalns, globalns)
+    return annotation
+
+
+def get_typed_return_annotation(obj: Callable[..., Any]) -> Any:
+    """Get the typed return annotation of a callable object."""
+    signature = inspect.signature(obj)
+    annotation = signature.return_annotation
+    if annotation is inspect.Signature.empty:
+        return None
+    globalns = getattr(obj, "__globals__", {})
+    return get_typed_annotation(annotation, globalns)
+
+
+def get_typed_parameters(obj: Callable[..., Any]) -> list[inspect.Parameter]:
+    """Get the typed parameters of a callable object."""
+    globalns = getattr(obj, "__globals__", {})
+    return [
+        parameter.replace(
+            annotation=get_typed_annotation(parameter.annotation, globalns)
+        )
+        for name, parameter in inspect.signature(obj).parameters.items()
+    ]
 
 
 async def run_async(
     func: Callable[P, T],
     /,
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> T:
-    """Runs the given function asynchronously using the `anyio` library.
-
-    Args:
-        func: The function to run asynchronously.
-        args: The positional arguments to pass to the function.
-        kwargs: The keyword arguments to pass to the function.
-
-    Returns:
-        The result of the function.
-
-    Raises:
-        ImportError: If the `anyio` library is not installed.
-    """
+    """Runs the given function asynchronously using the `anyio` library."""
     if not anyio:
         raise ImportError(
             "`anyio` library is not currently installed. Please make sure to install "
             "it first, or consider using `anydi[full]` instead."
         )
     return await anyio.to_thread.run_sync(functools.partial(func, *args, **kwargs))
```

### Comparing `anydi-0.25.0a1/anydi/ext/django/ninja/__init__.py` & `anydi-0.25.0a2/anydi/ext/django/ninja/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,11 +6,11 @@
         "Please install it using 'pip install django-ninja'."
     ) from exc
 
 from ._operation import AsyncOperation, Operation
 from ._signature import ViewSignature
 
 
-def patch() -> None:
+def patch_ninja() -> None:
     operation.ViewSignature = ViewSignature  # type: ignore[attr-defined]
     operation.Operation = Operation  # type: ignore[misc]
     operation.AsyncOperation = AsyncOperation  # type: ignore[misc]
```

### Comparing `anydi-0.25.0a1/anydi/ext/django/ninja/_operation.py` & `anydi-0.25.0a2/anydi/ext/django/ninja/_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 from django.http import HttpRequest, HttpResponseBase
 from ninja.operation import (
     AsyncOperation as BaseAsyncOperation,  # noqa
     Operation as BaseOperation,
 )
```

### Comparing `anydi-0.25.0a1/anydi/ext/django/ninja/_signature.py` & `anydi-0.25.0a2/anydi/ext/django/ninja/_signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import inspect
 from collections.abc import Callable
 from typing import Any
 
 from django.http import HttpResponse
 from ninja.signature.details import (
     FuncParam,  # noqa
```

### Comparing `anydi-0.25.0a1/anydi/ext/fastapi.py` & `anydi-0.25.0a2/anydi/ext/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi import Depends, FastAPI, params
 from fastapi.dependencies.models import Dependant
 from fastapi.routing import APIRoute
 from starlette.requests import Request
 from typing_extensions import Annotated, get_args, get_origin
 
 from anydi import Container
-from anydi._utils import get_full_qualname, get_signature
+from anydi._utils import get_full_qualname, get_typed_parameters
 
 from .starlette.middleware import RequestScopedMiddleware
 
 __all__ = ["RequestScopedMiddleware", "install", "get_container", "Inject"]
 
 logger = logging.getLogger(__name__)
 
@@ -43,15 +43,15 @@
         for dependant in _iter_dependencies(route.dependant):
             if dependant.cache_key in patched:
                 continue
             patched.append(dependant.cache_key)
             call, *params = dependant.cache_key
             if not call:
                 continue  # pragma: no cover
-            for parameter in get_signature(call).parameters.values():
+            for parameter in get_typed_parameters(call):
                 _patch_route_parameter(call, parameter, container)
 
 
 def get_container(request: Request) -> Container:
     """Get the AnyDI container from a FastAPI request.
 
     Args:
```

### Comparing `anydi-0.25.0a1/anydi/ext/pytest_plugin.py` & `anydi-0.25.0a2/anydi/ext/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import inspect
-from typing import Any, Callable, Iterator, List, Tuple, cast
+from typing import Any, Callable, Iterator, cast
 
 import pytest
 
 from anydi import Container
 
 
 def pytest_configure(config: pytest.Config) -> None:
@@ -45,26 +47,26 @@
 def _anydi_should_inject(request: pytest.FixtureRequest) -> bool:
     marker = request.node.get_closest_marker("inject")
     inject_all = cast(bool, request.config.getini("anydi_inject_all"))
     return marker is not None or inject_all
 
 
 @pytest.fixture(scope="session")
-def _anydi_unresolved() -> Iterator[List[Any]]:
-    unresolved: List[Any] = []
+def _anydi_unresolved() -> Iterator[list[Any]]:
+    unresolved: list[Any] = []
     yield unresolved
     unresolved.clear()
 
 
 @pytest.fixture
 def _anydi_injected_parameter_iterator(
     request: pytest.FixtureRequest,
-    _anydi_unresolved: List[str],
-) -> Callable[[], Iterator[Tuple[str, Any]]]:
-    def _iterator() -> Iterator[Tuple[str, inspect.Parameter]]:
+    _anydi_unresolved: list[str],
+) -> Callable[[], Iterator[tuple[str, Any]]]:
+    def _iterator() -> Iterator[tuple[str, inspect.Parameter]]:
         for name, parameter in inspect.signature(request.function).parameters.items():
             if (
                 ((interface := parameter.annotation) is parameter.empty)
                 or interface in _anydi_unresolved
                 or name in request.node.funcargs
             ):
                 continue
@@ -73,16 +75,16 @@
     return _iterator
 
 
 @pytest.fixture(autouse=True)
 def _anydi_inject(
     request: pytest.FixtureRequest,
     _anydi_should_inject: bool,
-    _anydi_injected_parameter_iterator: Callable[[], Iterator[Tuple[str, Any]]],
-    _anydi_unresolved: List[str],
+    _anydi_injected_parameter_iterator: Callable[[], Iterator[tuple[str, Any]]],
+    _anydi_unresolved: list[str],
 ) -> None:
     """Inject dependencies into the test function."""
 
     if inspect.iscoroutinefunction(request.function) or not _anydi_should_inject:
         return
 
     # Setup the container
@@ -103,16 +105,16 @@
         request.node.funcargs[argname] = instance
 
 
 @pytest.fixture(autouse=True)
 async def _anydi_ainject(
     request: pytest.FixtureRequest,
     _anydi_should_inject: bool,
-    _anydi_injected_parameter_iterator: Callable[[], Iterator[Tuple[str, Any]]],
-    _anydi_unresolved: List[str],
+    _anydi_injected_parameter_iterator: Callable[[], Iterator[tuple[str, Any]]],
+    _anydi_unresolved: list[str],
 ) -> None:
     """Inject dependencies into the test function."""
     if not inspect.iscoroutinefunction(request.function) or not _anydi_should_inject:
         return
 
     # Setup the container
     container = cast(Container, request.getfixturevalue("anydi_setup_container"))
```

### Comparing `anydi-0.25.0a1/anydi/ext/starlette/middleware.py` & `anydi-0.25.0a2/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.0a1/pyproject.toml` & `anydi-0.25.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.25.0a1"
+version = "0.25.0a2"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -59,15 +59,15 @@
 [tool.poetry.plugins.pytest11]
 anydi = "anydi.ext.pytest_plugin"
 
 [tool.ruff]
 line-length = 88
 
 [tool.ruff.lint]
-select = ["A", "B", "C", "E", "F", "I", "W", "TID252", "T20"]
+select = ["A", "B", "C", "E", "F", "I", "W", "TID252", "T20", "UP"]
 ignore = ["A003", "B008", "B009", "B010", "D104", "D107"]
 
 [tool.ruff.lint.isort]
 combine-as-imports = true
 forced-separate = ["tests", "app"]
 
 [tool.ruff.lint.pydocstyle]
```

### Comparing `anydi-0.25.0a1/PKG-INFO` & `anydi-0.25.0a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.25.0a1
+Version: 0.25.0a2
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -135,7 +135,63 @@
     return {"message": message}
 
 
 # Install the container into the FastAPI app
 anydi.ext.fastapi.install(app, container)
 ```
 
+
+
+## Django Ninja Example
+
+*container.py*
+
+```python
+from anydi import Container
+
+
+def get_container() -> Container:
+    container = Container()
+
+    @container.provider(scope="singleton")
+    def message() -> str:
+        return "Hello, World!"
+
+    return container
+```
+
+*settings.py*
+
+```python
+INSTALLED_APPS = [
+    ...
+    "anydi.ext.django",
+]
+
+ANYDI = {
+    "CONTAINER_FACTORY": "myapp.container.get_container",
+    "PATCH_NINJA": True,
+}
+```
+
+*urls.py*
+
+```python
+from django.http import HttpRequest
+from django.urls import path
+from ninja import NinjaAPI
+
+from anydi import auto
+
+api = NinjaAPI()
+
+
+@api.get("/hello")
+def say_hello(request: HttpRequest, message: str = auto) -> dict[str, str]:
+    return {"message": message}
+
+
+urlpatterns = [
+    path("api/", api.urls),
+]
+```
+
```

