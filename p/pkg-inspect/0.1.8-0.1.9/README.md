# Comparing `tmp/pkg_inspect-0.1.8.tar.gz` & `tmp/pkg_inspect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.1.8.tar", last modified: Tue May  7 01:58:06 2024, max compression
+gzip compressed data, was "pkg_inspect-0.1.9.tar", last modified: Wed May  8 04:02:05 2024, max compression
```

## Comparing `pkg_inspect-0.1.8.tar` & `pkg_inspect-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.360261 pkg_inspect-0.1.8/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.8/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.8/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-07 01:58:06.360021 pkg_inspect-0.1.8/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.8/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-07 01:58:06.360922 pkg_inspect-0.1.8/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.8/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.347678 pkg_inspect-0.1.8/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.1.8/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.348244 pkg_inspect-0.1.8/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       55 2024-05-07 01:45:28.000000 pkg_inspect-0.1.8/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.352460 pkg_inspect-0.1.8/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13476 2024-05-07 01:40:20.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.354784 pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47562 2024-05-07 00:47:21.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47635 2024-05-07 00:49:28.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.358026 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:47:07.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5538 2024-05-07 01:12:45.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/cli.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-07 01:55:50.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/metadata.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-07 01:31:43.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49692 2024-05-07 01:38:33.000000 pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.351159 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-07 01:58:06.000000 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-07 01:58:06.000000 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-07 01:58:06.000000 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-07 01:58:06.000000 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/entry_points.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-07 01:58:06.000000 pkg_inspect-0.1.8/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:58:06.359112 pkg_inspect-0.1.8/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.8/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.1.8/tests/test_pkg_inspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.230388 pkg_inspect-0.1.9/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.9/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.9/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-08 04:02:05.230091 pkg_inspect-0.1.9/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.9/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-08 04:02:05.231377 pkg_inspect-0.1.9/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.9/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.218783 pkg_inspect-0.1.9/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.1.9/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.219126 pkg_inspect-0.1.9/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       56 2024-05-08 03:30:25.000000 pkg_inspect-0.1.9/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.222457 pkg_inspect-0.1.9/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13925 2024-05-08 03:55:26.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.224637 pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47596 2024-05-08 03:30:25.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47492 2024-05-08 03:57:52.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.228284 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-07 01:47:07.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5847 2024-05-08 03:56:31.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/cli.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-08 03:58:23.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/metadata.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-07 01:31:43.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49570 2024-05-08 03:40:17.000000 pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.221548 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-08 04:02:05.000000 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-08 04:02:05.000000 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-08 04:02:05.000000 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-08 04:02:05.000000 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/entry_points.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-08 04:02:05.000000 pkg_inspect-0.1.9/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:02:05.229173 pkg_inspect-0.1.9/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.9/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.1.9/tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.1.8/LICENSE.md` & `pkg_inspect-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/PKG-INFO` & `pkg_inspect-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.8/README.md` & `pkg_inspect-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/setup.cfg` & `pkg_inspect-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.1.8
+version = 0.1.9
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A package for inspecting Python packages and their versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_functions/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,56 +24,47 @@
 
 
 from ..pkg_modules import PkgInspect, PkgVersions
 from ..pkg_utils.exception import PkgException, RedPkgE
 from ..pkg_utils.util_types import (
     DateTimeAndVersion,
     Iterable,
+    Literal,
+    Optional,
     PyPIOptionsT,
     TupleOfPkgVersions,
     Union,
 )
 from ..pkg_utils.utils import (
     BASE_EXCEPTIONS,
     alter_if_string,
+    equal_,
     filter_empty,
     find_best_match,
     get_properties,
     has_decorators,
     is_class,
     is_function,
     partial,
     wraps,
 )
 
 
+# region Constants
+# - PkgInspect partial function to disable the 'generator' attribute
 _PkgI: PkgInspect = partial(PkgInspect, generator=False)
-_PKGV_PROPS: tuple[str] = (*get_properties(PkgVersions),)
-
 
-# Constants - Tuple of available fieldnames for inspection
+# - Tuple of available fieldnames for inspection
 INSPECTION_FIELDS: tuple[str] = _PkgI().get_fieldnames
 
-
-def __valid_option(
-    item: str,
-    choices: Iterable = None,
-    extras: Iterable = None,
-    return_choices: bool = False,
-):
-    """Check if the specified item is a valid option for inspection."""
-    c: Union[None, tuple[str]] = alter_if_string(choices) or _PKGV_PROPS
-    if extras:
-        c += alter_if_string(extras)
-    option = find_best_match(item, c)
-    if return_choices:
-        return c, option
-    return option
+# - Tuple of 'PkgVersions' properties for inspections
+_PKGV_PROPS: tuple[str] = (*get_properties(PkgVersions),)
 
 
+# region FuncDecorators
 def __doc_handler(
     cls: Union[object, str] = None, func_name: str = None, add_doc: bool = True
 ):
     """Decorator to handle docstrings for functions."""
 
     def decorator(func):
         @wraps(func)
@@ -94,21 +85,45 @@
                 # Ensure the function name exists in the class
                 wrapper.__doc__ = getattr(cls_, f_name).__doc__
         return wrapper
 
     return decorator
 
 
+def __prettyprint():
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            pp = kwargs.pop("format", "")
+            f = func(*args, **kwargs)
+            if pp in (True, "pretty"):
+                from pprint import pprint
+
+                pprint(f)
+                f = ""
+            return f
+
+        return wrapper
+
+    return decorator
+
+
+# endregion
+
+
+# region InspectFuncs
 @__doc_handler()
+@__prettyprint()
 def inspect_package(
     package: str = None,
     pyversion: str = None,
     *,
     itemOrfile: str = "",
     package_manager: str = None,
+    format: Optional[Literal["pretty"]] = "",
 ):
     """
     Inspect a local or PyPI package and return the requested `itemOrfile`.
 
     - If the `itemOrfile` is not found in the local system files, the function will attempt to inspect the package on PyPI. \
         Only if the specified `itemOrfile` is a valid option for inspection on PyPI.
 
@@ -130,63 +145,22 @@
         except PkgException as pkg_error:
             raise RedPkgE(
                 f"{_any_e}\n{pkg_error.args[0]}",
                 "If inspecting a package on PyPI, please refer to the 'inspect_pypi' function for more information.",
             )
 
 
-@__doc_handler(func_name="version_compare")
-def pkg_version_compare(
-    package: str,
-    first_pyversion: str,
-    other_pyversion: str,
-    /,
-    *,
-    itemOrfile: str,
-    opmethod: str = None,
-):
-    """
-    Compare the items of a package between two different python versions.
-
-    - If the `opmethod` is not provided, the function will return the items from both versions.
-
-    - Please refer to the `pkg_version_compare.__doc__` for more information on comparing package data between Python versions.
-
-    """
-    return _PkgI(package, first_pyversion).version_compare(
-        other_pyversion, itemOrfile, opmethod=opmethod
-    )
-
-
-@__doc_handler()
-def get_version_packages(pyversion: str) -> DateTimeAndVersion:
-    """
-    Get all the packages installed in a python version.
-
-    - Please refer to the `get_version_packages.__doc__` for more information on retrieving installed packages.
-    """
-    return _PkgI(pyversion=pyversion).get_version_packages()
-
-
-@__doc_handler(func_name="installed_pythons")
-def get_installed_pythons() -> TupleOfPkgVersions:
-    """
-    Get all the installed python versions on the system.
-
-    - Please refer to the `get_installed_pythons.__doc__` for more information on retrieving installed Python versions.
-    """
-    return _PkgI().installed_pythons
-
-
 @__doc_handler(add_doc=False)
+@__prettyprint()
 def inspect_pypi(
     package: str,
     package_manager: str = None,
     *,
     item: PyPIOptionsT = "",
+    format: Optional[Literal["pretty"]] = "",
 ) -> Union[int, DateTimeAndVersion, dict[str, DateTimeAndVersion]]:
     """
     Inspect a package on (`https://pypi.org/`) and (`https://libraries.io/`)
     and return the requested item.
 
     #### Args:
         - `package`: The package name to inspect.
@@ -262,63 +236,91 @@
     """
     if not package:
         # Raise an error if the package argument is not provided
         raise RedPkgE(
             "The 'package' argument is required to inspect a package on PyPI."
         )
 
-    _options, _item = __valid_option(
-        item,
-        extras=(
-            _empty := "",
-            _all_items_str := "all_items",
-            _gh_str := "github_stats",
-            *(gh_stat_keys := PkgVersions.gh_stat_keys()),
-        ),
-        return_choices=True,
+    _options = (
+        *_PKGV_PROPS,
+        (_all_items_str := "all_items"),
+        (_gh_str := "github_stats"),
+        *(gh_stat_keys := PkgVersions.gh_stat_keys()),
     )
+    _item = find_best_match(item, _options)
     options = filter_empty(_options)
 
     if _item is None:
         if find_best_match(item, INSPECTION_FIELDS):
             #! DO NOT REMOVE
             # For 'inspect_package' function purposes
             raise PkgException("")
         raise RedPkgE(
             f"The specified item {item!r} is not a valid option for inspection."
         )
-    elif _item == _empty or not any(filter_empty((item, _item))):
+    elif not any(filter_empty((item, _item))):
         # Return all available options for inspection
         # if no item is specified
         return options
 
     # Return the requested item from the package
     if all((package, _item)):
-        pypi_item = lambda it: getattr(
-            PkgVersions(package, package_manager=package_manager), it
-        )
+        def _get_item(_it):
+            return getattr(PkgVersions(package, package_manager=package_manager), _it)
 
         if _item == _all_items_str:
             # Return all available items in a dictionary format
-            return {k: pypi_item(k) for k in _PKGV_PROPS}
+            return {k: _get_item(k) for k in _PKGV_PROPS}
         elif _item in _PKGV_PROPS:
             # Return the requested item from the package
-            return pypi_item(_item)
+            return _get_item(_item)
         elif _item in (*gh_stat_keys, _gh_str):
-            get_gh_stats = lambda x=_gh_str: pypi_item(x)
+            get_gh_stats = lambda x=_gh_str: _get_item(x)
             if _item == _gh_str:
                 # Return the GitHub statistics for the package
                 return get_gh_stats()
             # Or the specified item from the GitHub statistics
             return get_gh_stats()[_item]
 
 
+# endregion
+
+
+# region GetFunctions
+@__doc_handler()
+@__prettyprint()
+def get_version_packages(
+    pyversion: str, format: Optional[Literal["pretty"]] = ""
+) -> DateTimeAndVersion:
+    """
+    Get all the packages installed in a python version.
+
+    - Please refer to the `get_version_packages.__doc__` for more information on retrieving installed packages.
+    """
+    return _PkgI(pyversion=pyversion).get_version_packages()
+
+
+@__doc_handler(func_name="installed_pythons")
+def get_installed_pythons() -> TupleOfPkgVersions:
+    """
+    Get all the installed python versions on the system.
+
+    - Please refer to the `get_installed_pythons.__doc__` for more information on retrieving installed Python versions.
+    """
+    return _PkgI().installed_pythons
+
+
 @__doc_handler(cls=PkgVersions, func_name="get_updates")
+@__prettyprint()
 def get_available_updates(
-    package: str, current_version: str = None, *, include_betas: bool = False
+    package: str,
+    current_version: str = None,
+    *,
+    format: Optional[Literal["pretty"]] = "",
+    include_betas: bool = False,
 ):
     """
     Fetch the available updates from the specified current version of the package.
 
     - Please refer to the `get_available_updates.__doc__` for more information on fetching updates.
 
     """
@@ -331,14 +333,44 @@
     if current_version is None:
         _pkg_i = partial(_PkgI, package=package)
         i_pythons = _pkg_i().installed_pythons
         current_version = _pkg_i(pyversion=i_pythons[-1]).installed_version
     return PkgVersions(package).get_updates(current_version)
 
 
+# endregion
+
+
+# region OtherFuncs
+@__doc_handler(func_name="version_compare")
+def pkg_version_compare(
+    package: str,
+    first_pyversion: str,
+    other_pyversion: str,
+    /,
+    *,
+    itemOrfile: str,
+    opmethod: str = None,
+):
+    """
+    Compare the items of a package between two different python versions.
+
+    - If the `opmethod` is not provided, the function will return the items from both versions.
+
+    - Please refer to the `pkg_version_compare.__doc__` for more information on comparing package data between Python versions.
+
+    """
+    return _PkgI(package, first_pyversion).version_compare(
+        other_pyversion, itemOrfile, opmethod=opmethod
+    )
+
+
+# endregion
+
+
 __all__ = ("INSPECTION_FIELDS",) + (
     *(
         k
         for k, v in globals().items()
         # All 'pkg_functions.functions' functions
         if all((is_function(v), has_decorators(v)))
     ),
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,14 +801,16 @@
             @exception_handler(
                 msg=f"The 'pypistats' module must be installed to retrieve the {_item!r} item.",
                 exceptions=(AttributeError, ModuleNotFoundError),
                 raise_with=ModuleNotFoundError,
             )
             def _get_pypistat(item_obj):
                 # Return the specified item from the 'pypistats' module into a dictionary.
+                import pypistats
+
                 p_stats_json = json.loads(
                     getattr(pypistats, item_obj)(self._pkg, format="json")
                 )
                 return {p_stats_json["type"]: p_stats_json["data"]}
 
             def _fix_keys(item_obj):
                 if item_obj in map(rm_stats_prefix, mm):
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,15 +962,15 @@
         yield from (
             rd  # release-date
             for i in hsoup.find_all("div", class_="release")
             # Removes all instances of pre-releases
             if search(self.VERSION_PATTERN, rd := i.get_text(strip=True))
         )
 
-    def _get_gh_stats(self, keys_only: bool = False):
+    def _get_gh_stats(self):
         gh_soup = self._main_request(self.github_stats_url)
         stats_chart = [
             _j
             for i in gh_soup.find_all("dl", class_="row detail-card")
             for j in i.text.splitlines()
             if (_j := re.sub(r"\s{2,}", "", j))
         ]
@@ -986,26 +986,24 @@
                     else int(clean(v)) if search(r"[,][^a-zA-Z]", v)
                     # E.g., '12.4 MB' -> Stats NamedTuple
                     else str_to_bytes(*v.split())
                     if v[0].isdigit()
                     and search("|".join(map(re.escape, UNITS)), v, compiler=True)
                     else v
                     for k, v in zip(flat_stats[::2], flat_stats[1::2])
-                    if best_match(k, GH_STATS)
+                    if best_match(k, self.gh_stat_keys())
                 }
             except BASE_EXCEPTIONS:
                 ...
 
-        if all((keys_only, gh_stats)):
-            return (*sorted(gh_stats),)
         return gh_stats
 
-    @classmethod
-    def gh_stat_keys(cls) -> tuple[str]:
-        return cls(package=DUMMY_PKGNAME)._get_gh_stats(keys_only=True) or GH_STATS
+    @staticmethod
+    def gh_stat_keys() -> tuple[str]:
+        return (*sorted(GH_STATS),)
 
     def _version_history(self) -> Generator[DateTimeAndVersion, None, None]:
         @exception_handler(item=f"{self._pkg_path!r}", exceptions=TimeoutError)
         def get_vers(p: Pattern):
             def search_func(i):
                 return search(pattern=p, obj=i, compiler=True).group()
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/cli.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,41 +37,45 @@
     ap_true("--version", help="Display the current version of 'pkg_inspect'.")
     ap_true("--installed-pythons", help="Display all installed python versions.")
 
     # Inspect Package
     i_package = sub_parsers.add_parser("inspect-package", help="Inspect a package.")
     ip_true = _store_true((ip_add := i_package.add_argument))
     ip_true("--ipdoc", help="Display the documentation of 'inspect_package'.")
+    ip_true("--pretty", help="Display the item in 'pretty' format.")
     ip_add("-pkg", help="Choose a package to inspect.")
     ip_add("-pyver", help="Choose a python version to inspect.")
     ip_add("-item", help="Choose an 'itemOrfile' to inspect.")
 
     # Inspect PyPI
     ipypi = sub_parsers.add_parser("inspect-pypi", help="Inspect a package on PyPI.")
     ipypi_true = _store_true((ipypi_add := ipypi.add_argument))
     ipypi_true("--ipdoc", help="Display the documentation of 'inspect_pypi'.")
+    ipypi_true("--pretty", help="Display the item in 'pretty' format.")
     ipypi_add("-pkg", help="Choose a package to inspect.")
     ipypi_add("-pyver", help="Choose a python version to inspect.")
     ipypi_add("-pkgm", help="Choose a package manager to inspect.")
     ipypi_add("-item", help="Choose an 'itemOrfile' to inspect.")
 
     # Retrieve Version Packages
     gvps = sub_parsers.add_parser(
         "get-version-packages", help="Retrieve version packages."
     )
     gvps_true = _store_true((gvps_add := gvps.add_argument))
     gvps_true("--gvpdoc", help="Display the documentation of 'get_version_packages'.")
+    gvps_true("--pretty", help="Display the item in 'pretty' format.")
     gvps_add("-pyver", help="Choose a python version to inspect.")
 
     # Retrieve Available Updates
     gaup = sub_parsers.add_parser(
         "get-available-updates", help="Retrieve available updates."
     )
     gaup_true = _store_true((gaup_add := gaup.add_argument))
     gaup_true("--gaupdoc", help="Display the documentation of 'get_available_updates'.")
+    gaup_true("--pretty", help="Display the item in 'pretty' format.")
     gaup_true("--include-betas", help="A flag to include beta versions.")
     gaup_add("-pkg", help="Choose a package to inspect.")
     gaup_add("-current-version", help="Choose a current version to inspect.")
 
     # Compare Version Packages
     pvc = sub_parsers.add_parser("pkg-version-compare", help="")
     pvc_true = _store_true((pvc_add := pvc.add_argument))
@@ -97,39 +101,35 @@
     elif args.source:
         return _read("src/pkg_inspect/pkg_modules/pkg_inspect.py")
     elif args.version:
         return __current_version
     elif args.command == "inspect-package":
         if args.ipdoc:
             return inspect_package.__doc__
-        return inspect_package(args.pkg, args.pyver, itemOrfile=args.item)
+        return inspect_package(args.pkg, args.pyver, itemOrfile=args.item, format=args.pretty)
     elif args.command == "inspect-py":
         if args.pydoc:
             return inspect_pypi.__doc__
-        return inspect_pypi(args.pkg, args.pkgm, item=args.item)
+        return inspect_pypi(args.pkg, args.pkgm, item=args.item, format=args.pretty)
     elif args.command == "get-version-packages":
         if args.gvpdoc:
             return get_version_packages.__doc__
-        return get_version_packages(args.pyver)
+        return get_version_packages(args.pyver, format=args.pretty)
     elif args.command == "get-available-updates":
         if args.gaupdoc:
             return get_available_updates.__doc__
         return get_available_updates(
-            args.pkg, args.current_version, include_betas=args.include_betas
+            args.pkg, args.current_version, include_betas=args.include_betas, format=args.pretty
         )
     elif args.command == "pkg-version-compare":
         if args.pvcdoc:
             return pkg_version_compare.__doc__
         return pkg_version_compare(
             args.pkg,
             args.fpyver,
             args.opyver,
             itemOrfile=args.item,
             opmethod=args.opmethod,
         )
 
 
-__all__ = "cli_parser"
-
-
-if __name__ == "__main__":
-    print(cli_parser())
+__all__ = "cli_parser"
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/metadata.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .util_types import PackageVersion
 from ..pkg_modules.pkg_versions import PkgVersions
 
 
 # Current Version
-__version__: PackageVersion = PkgVersions.parse_version("0.1.8")
+__version__: PackageVersion = PkgVersions.parse_version("0.1.9")
 
 
 # Package Metadata
 __author__ = "Yousef Abuzahrieh <yousef.zahrieh17@gmail.com"
 __copyright__ = f"Copyright © 2024, {__author__}"
 __license__ = "Apache License, Version 2.0"
 __summary__ = "A package for inspecting Python packages and their versions."
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.1.9/src/pkg_inspect/pkg_utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,28 +63,20 @@
     TupleExceptions,
     TupleOfPkgVersions,
     Union,
     ZeroOrOne,
 )
 
 
-try:
-    import pypistats
-except ModuleNotFoundError:
-    ...
-
-
 # MARK: - Constants, Variables, Functions and Exception Handling
 
-# Default 'DUMMY' values to be used for extracting
+# Default 'DUMMY' object (Main Directory) to be used for extracting
 #   1. package metadata
 #   2. Distribution Information
-#   3. GitHub Statistics
-DUMMY_PATH: Path = Path(__file__).parents[3]  # Main Directory
-DUMMY_PKGNAME: str = "requests"
+DUMMY_PATH: Path = Path(__file__).parents[3]
 
 
 # Field names and custom types to extract
 # from the package's METADATA file or dist-info ('site_path') directory.
 METADATA_FIELDS: tuple[str] = (
     # - 'METADATA' fieldnames
     "Author",
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.1.9/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.8/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.1.9/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.8/tests/test_pkg_inspect.py` & `pkg_inspect-0.1.9/tests/test_pkg_inspect.py`

 * *Files identical despite different names*

