# Comparing `tmp/niklibpy-0.1.2.tar.gz` & `tmp/niklibpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niklibpy-0.1.2.tar", max compression
+gzip compressed data, was "niklibpy-0.1.3.tar", max compression
```

## Comparing `niklibpy-0.1.2.tar` & `niklibpy-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       22 2023-04-09 10:26:08.644963 niklibpy-0.1.2/niklibpy/__init__.py
--rw-r--r--   0        0        0     3885 2024-01-18 13:55:24.317304 niklibpy-0.1.2/niklibpy/niklib.py
--rw-r--r--   0        0        0      554 2024-02-05 10:38:22.269721 niklibpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 niklibpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1268 2024-05-07 16:19:08.704395 niklibpy-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-09 10:26:08.644963 niklibpy-0.1.3/niklibpy/__init__.py
+-rw-r--r--   0        0        0     5252 2024-05-07 16:17:33.254541 niklibpy-0.1.3/niklibpy/niklib.py
+-rw-r--r--   0        0        0      552 2024-05-08 11:27:27.234733 niklibpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 niklibpy-0.1.3/PKG-INFO
```

### Comparing `niklibpy-0.1.2/niklibpy/niklib.py` & `niklibpy-0.1.3/niklibpy/niklib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import asyncio
 import concurrent.futures
+import copy
 import warnings
-from functools import reduce
+from functools import reduce, partial
 from typing import Any, Callable, List, Union
-import copy
 
 
 def pmap(funcs: List[Callable], max_workers: int = 2) -> List[Any]:
     """Simple parallel map construction, using a thread pool executor.
 
     Feed it an array of functions, and it will execute them in parallel, returning
     the results in the same order as the input functions"""
@@ -20,29 +21,69 @@
                 warnings.warn(f"Function {i} raised an exception: {e}")
                 result = None
             results.append((i, result))
         results.sort()
         return [result for i, result in results]
 
 
-def pipe(inp: Any, *fns: Callable[..., Any]) -> Any:
-    """
-       Applies a series of functions to an input value, with the output of each function
-       being passed as the input to the next function in the series. Returns the final
-       output value after all functions have been applied.
-
-       :param inp: The initial input value
-       :param fns: A variable-length list of functions to apply to the input value
-    poetry config pypi-token.pypi
-       :return: The final output value after all functions have been applied
-    """
+async def apmap(funcs: List[Callable]) -> List[Any]:
+    """Asynchronous parallel map construction, using asyncio.
+
+    Feed it an array of async functions, and it will execute them in parallel, returning the results
+    in the same order as the input functions"""
+
+    async def run_func(i, func):
+        try:
+            return i, await func()
+        except Exception as e:
+            warnings.warn(f"Function {i} raised an exception: {e}")
+            return i, None
+
+    tasks = [asyncio.create_task(run_func(i, func)) for i, func in enumerate(funcs)]
+    results = await asyncio.gather(*tasks)
+    results.sort()
+    return [result for i, result in results]
+
+
+def pipe(
+    inp: Any,
+    *fns: Callable[..., Any],
+    debug: bool = False,
+    debug_print_fn: Callable = print,
+) -> Any:
+    """
+    Applies a series of functions to an input value, with the output of each function
+    being passed as the input to the next function in the series. Returns the final
+    output value after all functions have been applied. If debug is True, uses
+    debug_print_fn to print the input and output of each function.
+
+    :param inp: The initial input value
+    :param fns: A variable-length list of functions to apply to the input value
+    :param debug: If True, prints the input and output of each function using debug_print_fn
+    :param debug_print_fn: The function used for printing debug information (default is print)
+    :return: The final output value after all functions have been applied
+    """
+
+    def debug_wrapper(fn, input_value):
+        output_value = fn(input_value)
+        try:
+            debug_print_fn(
+                f"<pipe> Function: {fn.__name__}, Input: '{input_value}', Output: '{output_value}'"
+            )
+        except:
+            pass
+        return output_value
+
     for fn in fns:
         if inp is None:
             return None
-        inp = fn(inp)
+        if debug:
+            inp = debug_wrapper(fn, inp)
+        else:
+            inp = fn(inp)
     return inp
 
 
 def dig(data: Union[dict, list], *keys: Any) -> Any:
     """
     Attempts to retrieve a value from a nested data structure (dictionary or list)
     using a sequence of keys. If no key is found, it returns None.
@@ -96,8 +137,8 @@
                     current.append({})
                 current = current[key]
             else:
                 raise TypeError(
                     "Cannot bury value in non-dictionary or non-list object"
                 )
 
-    return data
+    return data
```

### Comparing `niklibpy-0.1.2/pyproject.toml` & `niklibpy-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "niklibpy"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Nik V <github@nikvdp.com>"]
-# readme = "README.md"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
 
 [tool.pdm.build]
@@ -26,9 +26,9 @@
     {name = "Nik V", email = "github@nikvdp.com"},
 ]
 requires-python = ">=3.9,<4.0"
 dependencies = [
     "pytest>=7.4.4",
 ]
 name = "niklibpy"
-version = "0.1.1"
+version = "0.1.3"
 description = ""
```

