# Comparing `tmp/sema4ai_actions-0.4.0.tar.gz` & `tmp/sema4ai_actions-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.4.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.5.0.tar", max compression
```

## Comparing `sema4ai_actions-0.4.0.tar` & `sema4ai_actions-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2971 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/README.md
--rw-r--r--   0        0        0      971 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5474 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    11619 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11151 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8376 2024-05-02 19:25:06.139425 sema4ai_actions-0.4.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    31250 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      252 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    11986 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     4355 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     4478 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/_secret.py
--rw-r--r--   0        0        0     3134 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/api.py
--rw-r--r--   0        0        0     2277 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-05-02 19:25:06.143425 sema4ai_actions-0.4.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-08 19:14:34.472609 sema4ai_actions-0.5.0/README.md
+-rw-r--r--   0        0        0      971 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5474 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    12093 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11151 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8376 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    31992 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      336 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      252 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    12522 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     5261 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     4478 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/_secret.py
+-rw-r--r--   0        0        0     3134 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:14:34.476609 sema4ai_actions-0.5.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.5.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.4.0/README.md` & `sema4ai_actions-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/pyproject.toml` & `sema4ai_actions-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.4.0"
+version = "0.5.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._secret import Secret
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,41 +108,54 @@
 
     @property
     def managed_params_schema(self) -> Dict[str, Any]:
         from sema4ai.actions._commands import _get_managed_param_type, _is_managed_param
 
         managed_params_schema: Dict[str, Any] = {}
         sig = inspect.signature(self.method)
+
+        param_name_to_description = self._get_param_name_to_description()
         for param in sig.parameters.values():
             if _is_managed_param(self._pm, param.name, param=param):
-                tp = _get_managed_param_type(self._pm, param).__name__
+                tp = _get_managed_param_type(self._pm, param.name, param=param).__name__
+
+                dct = {"type": tp}
 
-                managed_params_schema[param.name] = {"type": tp}
+                desc = param_name_to_description.get(param.name)
+                if desc:
+                    dct["description"] = desc
+                managed_params_schema[param.name] = dct
 
         return managed_params_schema
 
-    @property
-    def input_schema(self) -> Dict[str, Any]:
+    def _get_param_name_to_description(self) -> dict[str, str]:
         import docstring_parser
 
-        from sema4ai.actions._commands import _is_managed_param
-
-        sig = inspect.signature(self.method)
-        method_name = self.method.__code__.co_name
-        type_hints = get_type_hints(self.method)
-
         param_name_to_description: Dict[str, str] = {}
-
         doc = getattr(self.method, "__doc__", "")
         if doc:
             contents = docstring_parser.parse(doc)
             for docparam in contents.params:
                 if docparam.description:
                     param_name_to_description[docparam.arg_name] = docparam.description
 
+        return param_name_to_description
+
+    @property
+    def input_schema(self) -> Dict[str, Any]:
+        from sema4ai.actions._commands import _is_managed_param
+
+        sig = inspect.signature(self.method)
+        method_name = self.method.__code__.co_name
+        type_hints = get_type_hints(self.method)
+
+        param_name_to_description: dict[
+            str, str
+        ] = self._get_param_name_to_description()
+
         properties: Dict[str, Any] = {}
         required: List[str] = []
 
         schema = {
             "properties": properties,
             "type": "object",
         }
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,15 +594,15 @@
     for param_name, param in sig.parameters.items():
         param_type = type_hints.get(param_name)
 
         is_managed_param = _is_managed_param(pm, param.name, param=param)
         if param_type is None:
             # If not given, default to `str`.
             if is_managed_param:
-                param_type = _get_managed_param_type(pm, param)
+                param_type = _get_managed_param_type(pm, param.name, param=param)
             else:
                 param_type = str
 
         if param.default is inspect.Parameter.empty:
             # It's required, so, let's see if it's in the kwargs.
             if not is_managed_param:
                 if param_name not in kwargs:
@@ -724,17 +724,50 @@
         elif param is not None:
             return ep_managed_parameters.is_managed_param(param_name, param=param)
         else:
             raise AssertionError("Not expected to get here.")
     return False
 
 
-def _get_managed_param_type(pm: PluginManager, param: inspect.Parameter) -> type:
+@overload
+def _get_managed_param_type(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    node: FunctionDef,
+) -> str:
+    raise NotImplementedError()
+
+
+@overload
+def _get_managed_param_type(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    param: inspect.Parameter,
+) -> type:
+    raise NotImplementedError()
+
+
+def _get_managed_param_type(
+    pm: PluginManager,
+    param_name: str,
+    *,
+    node: Optional[FunctionDef] = None,
+    param: Optional[inspect.Parameter] = None,
+):
     if pm.has_instance(EPManagedParameters):
         ep_managed_parameters = pm.get_instance(EPManagedParameters)
+        if node is not None:
+            return ep_managed_parameters.get_managed_param_type(param_name, node=node)
+        elif param is not None:
+            return ep_managed_parameters.get_managed_param_type(param_name, param=param)
+        else:
+            raise AssertionError("Not expected to get here.")
+
         managed_param_type = ep_managed_parameters.get_managed_param_type(param)
         assert managed_param_type is not None
         return managed_param_type
     raise RuntimeError(
         "Error: Asked managed param type for a param which is not managed."
     )
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,17 +49,34 @@
         Args:
             sig: The signature of the function being called.
             new_kwargs: The new kwargs (where the parameters should be injected).
             original_kwargs: The original kwargs passed to the function.
         """
         raise NotImplementedError()
 
-    def get_managed_param_type(self, param: inspect.Parameter) -> type:
+    @overload
+    def get_managed_param_type(
+        self, param_name: str, *, param: inspect.Parameter
+    ) -> type:
         """
         Provides the type of the given managed parameter.
 
         Args:
+            param_name: The parameter name for which the type is requested.
             param: The parameter for which the type is requested.
 
         Return: The type of the managed parameter.
         """
         raise NotImplementedError()
+
+    @overload
+    def get_managed_param_type(self, param_name: str, *, node: FunctionDef) -> str:
+        """
+        Provides the type (as a string) of the given managed parameter.
+
+        Args:
+            param_name: The parameter name for which the type is requested.
+            node: The function definition node of the requested parameter
+
+        Return: The type (string) of the managed parameter.
+        """
+        raise NotImplementedError()
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_lint_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast as ast_module
 from dataclasses import dataclass
 from typing import Any, Iterator, List, Optional, Tuple, TypedDict, Union, overload
 
+from sema4ai.actions._commands import _get_managed_param_type
 from sema4ai.actions._customization._plugin_manager import PluginManager
 
 
 def _iter_nodes(
     node, internal_stack: Optional[List[Any]] = None, recursive=True
 ) -> Iterator[Tuple[List[Any], Any]]:
     """
@@ -262,14 +263,23 @@
             severity=DiagnosticSeverity.Warning,
         )
 
     if arguments.args:
         for arg in arguments.args:
             desc = param_name_to_description.pop(arg.arg, None)
             if pm is not None and _is_managed_param(pm, arg.arg, node=node):
+                if not desc:
+                    if _get_managed_param_type(pm, arg.arg, node=node) == "Secret":
+                        yield _make_error(
+                            arg,
+                            f"Parameter: `{arg.arg}` documentation not found in docstring. "
+                            "Please update docstring to add it (as it will be added to the "
+                            "secrets metadata explaining the secret).",
+                        )
+
                 continue
 
             if not desc:
                 yield _make_error(
                     arg,
                     f"Parameter: `{arg.arg}` documentation not found in docstring. "
                     "Please update docstring to add it as an LLM needs this info "
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,51 +27,53 @@
     def is_managed_param(
         self,
         param_name: str,
         *,
         node: Optional[FunctionDef] = None,
         param: Optional[inspect.Parameter] = None,
     ) -> bool:
-        import ast
-
         from sema4ai.actions._secret import Secret
 
         if param_name in self._param_name_to_instance:
             return True
 
         if node is not None:
             assert (
                 param is None
             ), "Either node or param is expected, but not both at the same time."
-            is_managed = False
-            args: ast.arguments = node.args
-            for arg in args.args:
-                if arg.arg == param_name:
-                    if arg.annotation:
-                        unparsed = ast.unparse(arg.annotation)
-                        if unparsed in (
-                            "Secret",
-                            "actions.Secret",
-                            "sema4ai.actions.Secret",
-                        ):
-                            is_managed = True
-
-                    break
-
-            return is_managed
+            return self._is_secret_node(param_name, node)
 
         elif param is not None:
             if param.annotation and issubclass(param.annotation, Secret):
                 return True
 
         else:
             raise AssertionError("Either node or param must be passed.")
 
         return False
 
+    def _is_secret_node(self, param_name: str, node: FunctionDef) -> bool:
+        import ast
+
+        args: ast.arguments = node.args
+        for arg in args.args:
+            if arg.arg == param_name:
+                if arg.annotation:
+                    unparsed = ast.unparse(arg.annotation)
+                    if unparsed in (
+                        "Secret",
+                        "actions.Secret",
+                        "sema4ai.actions.Secret",
+                    ):
+                        return True
+
+                return False
+
+        return False
+
     def inject_managed_params(
         self,
         sig: inspect.Signature,
         new_kwargs: Dict[str, Any],
         original_kwargs: Dict[str, Any],
     ) -> Dict[str, Any]:
         from sema4ai.actions._action_context import ActionContext
@@ -104,26 +106,51 @@
                 elif x_action_context is not None:
                     use_kwargs[param.name] = Secret.from_action_context(
                         x_action_context, f"secrets/{param.name}"
                     )
 
         return use_kwargs
 
+    @overload
     def get_managed_param_type(
-        self,
-        param: inspect.Parameter,
+        self, param_name: str, *, param: inspect.Parameter
     ) -> type:
+        raise NotImplementedError()
+
+    @overload
+    def get_managed_param_type(self, param_name: str, *, node: FunctionDef) -> str:
+        raise NotImplementedError()
+
+    def get_managed_param_type(
+        self,
+        param_name: str,
+        *,
+        param: Optional[inspect.Parameter] = None,
+        node: Optional[FunctionDef] = None,
+    ) -> type | str:
         from sema4ai.actions._request import Request
         from sema4ai.actions._secret import Secret
 
-        if param.name == "request":
+        if param_name == "request":
             return Request
 
-        if param.annotation and issubclass(param.annotation, Secret):
-            return Secret
+        if node is None and param is None:
+            raise ValueError("Either node or param are required.")
+        if node is not None and param is not None:
+            raise ValueError(
+                "Either node or param is expected, but not both at the same time."
+            )
+
+        if param is not None:
+            if param.annotation and issubclass(param.annotation, Secret):
+                return Secret
+        else:
+            assert node is not None
+            if self._is_secret_node(param_name, node):
+                return "Secret"
 
         raise RuntimeError(
             f"Unable to get managed parameter type for parameter: {param}"
         )
 
     def __typecheckself__(self) -> None:
         from sema4ai.actions._protocols import check_implements
```

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/_secret.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/api.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.5.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.4.0/PKG-INFO` & `sema4ai_actions-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.4.0
+Version: 0.5.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

