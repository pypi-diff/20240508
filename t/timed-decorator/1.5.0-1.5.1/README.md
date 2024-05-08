# Comparing `tmp/timed_decorator-1.5.0.tar.gz` & `tmp/timed_decorator-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_decorator-1.5.0.tar", last modified: Thu May  2 19:41:25 2024, max compression
+gzip compressed data, was "timed_decorator-1.5.1.tar", last modified: Wed May  8 08:50:28 2024, max compression
```

## Comparing `timed_decorator-1.5.0.tar` & `timed_decorator-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.029379 timed_decorator-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/tests/test_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.029379 timed_decorator-1.5.0/timed_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/nested_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/simple_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/timed_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18163 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/timed_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/timed_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/timed_decorator/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/timed_decorator/nested_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/timed_decorator/simple_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-08 08:50:19.000000 timed_decorator-1.5.1/timed_decorator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:50:28.298469 timed_decorator-1.5.1/timed_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18163 2024-05-08 08:50:28.000000 timed_decorator-1.5.1/timed_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-08 08:50:28.000000 timed_decorator-1.5.1/timed_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:50:28.000000 timed_decorator-1.5.1/timed_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 08:50:28.000000 timed_decorator-1.5.1/timed_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 08:50:28.000000 timed_decorator-1.5.1/timed_decorator.egg-info/top_level.txt
```

### Comparing `timed_decorator-1.5.0/LICENSE` & `timed_decorator-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.5.0/PKG-INFO` & `timed_decorator-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.5.0
+Version: 1.5.1
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -92,20 +92,22 @@
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
     * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
-3. `create_timed_decorator` registers a timed decorator with a given name.
+3. `create_timed_decorator` registers a timed decorator with a given name. Can be enabled or disabled during creation.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
+   * `enabled` (`bool`): If `True`, the timed decorator is enabled and used for timing decorated functions. Otherwise, functions decorated with `name` will not be timed. Default: `True`.
    * Also receives all the other arguments accepted by `timed` and `nested_timed`.
 
-4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call.
+4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call. If the timer is disabled, the elapsed time will not be measured.
+
    * `name` (`str`): The name of the timed decorator registered using `timed_decorator.builder.create_timed_decorator`.
 
 
 ### Examples
 
 Simple usage.
 ```py
```

### Comparing `timed_decorator-1.5.0/README.md` & `timed_decorator-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,22 @@
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
     * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
-3. `create_timed_decorator` registers a timed decorator with a given name.
+3. `create_timed_decorator` registers a timed decorator with a given name. Can be enabled or disabled during creation.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
+   * `enabled` (`bool`): If `True`, the timed decorator is enabled and used for timing decorated functions. Otherwise, functions decorated with `name` will not be timed. Default: `True`.
    * Also receives all the other arguments accepted by `timed` and `nested_timed`.
 
-4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call.
+4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call. If the timer is disabled, the elapsed time will not be measured.
+
    * `name` (`str`): The name of the timed decorator registered using `timed_decorator.builder.create_timed_decorator`.
 
 
 ### Examples
 
 Simple usage.
 ```py
```

### Comparing `timed_decorator-1.5.0/pyproject.toml` & `timed_decorator-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timed-decorator"
-version = "1.5.0"
+version = "1.5.1"
 #requires-python = ">=3.10"
 requires-python = ">=3.7"
 description = "A timing decorator for python functions."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "George Stoica", email = "george.stoica@senticlab.com" },
```

### Comparing `timed_decorator-1.5.0/tests/test_usage.py` & `timed_decorator-1.5.1/tests/test_usage.py`

 * *Files 14% similar despite different names*

```diff
@@ -183,10 +183,21 @@
         self.assertRaises(KeyError, fn, 10000)
 
         # Defer instantiation
         fn = get_timed_decorator('lazy name')(fibonacci)
         create_timed_decorator('lazy name')
         fn(10000)
 
+    def test_create_disabled_timed_decorator(self):
+        out = {}
+        create_timed_decorator('disabled', enabled=False, out=out)
+        get_timed_decorator('disabled')(fibonacci)(10000)
+
+        create_timed_decorator('enabled', enabled=True, out=out)
+        get_timed_decorator('enabled')(recursive_fibonacci)(30)
+
+        self.assertNotIn(fibonacci.__qualname__, out)
+        self.assertIn(recursive_fibonacci.__qualname__, out)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timed_decorator-1.5.0/timed_decorator/builder.py` & `timed_decorator-1.5.1/timed_decorator/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .simple_timed import timed
 
 _timed_decorators = {}
 
 
 def create_timed_decorator(name: str,
                            nested: bool = False,
+                           enabled: bool = True,
                            collect_gc: bool = True,
                            disable_gc: bool = False,
                            use_seconds: bool = False,
                            precision: int = 9,
                            show_args: bool = False,
                            show_kwargs: bool = False,
                            display_level: int = 1,
@@ -21,67 +22,76 @@
                            file_path: Union[str, None] = None,
                            logger_name: Union[str, None] = None,
                            return_time: bool = False,
                            out: dict = None,
                            use_qualname: bool = False):
     """
     Registers a timed decorator with a given name. Once instantiated, the timed decorator can be retrieved with
-    :class:`timed_decorator.builder.get_timed_decorator` and used for measuring the runtime of decorated functions.
+    :class:`timed_decorator.builder.get_timed_decorator` and used for measuring the runtime of decorated functions if
+    enabled.
 
     Args:
         name (str): The name of the timed decorator which will be instantiated using the provided arguments. Use this
             name for retrieving the timed decorator with :class:`timed_decorator.builder.get_timed_decorator`.
         nested (bool): If `True`, uses the :class:`timed_decorator.nested_timed.nested_timed` as decorator, otherwise
             uses :class:`timed_decorator.simple_timed.timed`. Default: `False`.
+        enabled (bool): If `True`, the timed decorator is enabled and used for timing decorated functions. Otherwise,
+            functions decorated with `name` will not be timed. Default: `True`.
 
     See Also:
         :class:`timed_decorator.simple_timed.timed` for the remaining parameters' documentation.
 
     """
     global _timed_decorators
     if name in _timed_decorators:
         raise KeyError(f'Timed decorator {name} already registered.')
 
     decorator = nested_timed if nested else timed
-    _timed_decorators[name] = decorator(collect_gc=collect_gc,
-                                        disable_gc=disable_gc,
-                                        use_seconds=use_seconds,
-                                        precision=precision,
-                                        show_args=show_args,
-                                        show_kwargs=show_kwargs,
-                                        display_level=display_level,
-                                        sep=sep,
-                                        stdout=stdout,
-                                        file_path=file_path,
-                                        logger_name=logger_name,
-                                        return_time=return_time,
-                                        out=out,
-                                        use_qualname=use_qualname)
+    timer = decorator(collect_gc=collect_gc,
+                      disable_gc=disable_gc,
+                      use_seconds=use_seconds,
+                      precision=precision,
+                      show_args=show_args,
+                      show_kwargs=show_kwargs,
+                      display_level=display_level,
+                      sep=sep,
+                      stdout=stdout,
+                      file_path=file_path,
+                      logger_name=logger_name,
+                      return_time=return_time,
+                      out=out,
+                      use_qualname=use_qualname)
+    _timed_decorators[name] = (timer, enabled)
 
 
 def _get_timed_decorator(name: str):
     global _timed_decorators
     if name not in _timed_decorators:
         raise KeyError(f'Timed decorator {name} not registered. Please register it first using '
                        f'timed_decorator.builder.create_timed_decorator')
 
     return _timed_decorators[name]
 
 
 def get_timed_decorator(name: str):
     """
     Wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer
-    can be registered after the function definition, but must be registered before the first function call.
+    can be registered after the function definition, but must be registered before the first function call. If the timer
+    is disabled, the elapsed time will not be measured.
 
     Args:
         name (str): The name of the timed decorator registered using
             :class:`timed_decorator.builder.create_timed_decorator`.
 
     """
+
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
-            return _get_timed_decorator(name)(fn)(*args, **kwargs)
+            timer, enabled = _get_timed_decorator(name)
+            if enabled:
+                return timer(fn)(*args, **kwargs)
+            return fn(*args, **kwargs)
 
         return wrap
 
     return decorator
```

### Comparing `timed_decorator-1.5.0/timed_decorator/nested_timed.py` & `timed_decorator-1.5.1/timed_decorator/nested_timed.py`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.5.0/timed_decorator/simple_timed.py` & `timed_decorator-1.5.1/timed_decorator/simple_timed.py`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.5.0/timed_decorator/utils.py` & `timed_decorator-1.5.1/timed_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.5.0/timed_decorator.egg-info/PKG-INFO` & `timed_decorator-1.5.1/timed_decorator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.5.0
+Version: 1.5.1
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -92,20 +92,22 @@
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
     * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
-3. `create_timed_decorator` registers a timed decorator with a given name.
+3. `create_timed_decorator` registers a timed decorator with a given name. Can be enabled or disabled during creation.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
+   * `enabled` (`bool`): If `True`, the timed decorator is enabled and used for timing decorated functions. Otherwise, functions decorated with `name` will not be timed. Default: `True`.
    * Also receives all the other arguments accepted by `timed` and `nested_timed`.
 
-4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call.
+4. `get_timed_decorator` wraps the decorated function and lazily measures its elapsed time using the registered timed decorator. The timer can be registered after the function definition, but must be registered before the first function call. If the timer is disabled, the elapsed time will not be measured.
+
    * `name` (`str`): The name of the timed decorator registered using `timed_decorator.builder.create_timed_decorator`.
 
 
 ### Examples
 
 Simple usage.
 ```py
```

