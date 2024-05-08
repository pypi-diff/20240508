# Comparing `tmp/mypy_boto3_cognito_idp-1.34.91.tar.gz` & `tmp/mypy_boto3_cognito_idp-1.34.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_cognito_idp-1.34.91.tar", last modified: Thu Apr 25 00:48:23 2024, max compression
+gzip compressed data, was "mypy_boto3_cognito_idp-1.34.93.tar", last modified: Fri Apr 26 19:32:22 2024, max compression
```

## Comparing `mypy_boto3_cognito_idp-1.34.91.tar` & `mypy_boto3_cognito_idp-1.34.93.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14243 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12660 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2396 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2396 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    80829 2024-04-24 23:43:40.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    80826 2024-04-24 23:43:39.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14776 2024-04-24 23:43:42.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14776 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11049 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11039 2024-04-24 23:43:41.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    83482 2024-04-24 23:43:47.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    83482 2024-04-24 23:43:45.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-24 23:43:37.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14243 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2024-04-25 00:48:22.000000 mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 00:48:23.058523 mypy_boto3_cognito_idp-1.34.91/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2014 2024-04-24 23:43:36.000000 mypy_boto3_cognito_idp-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.179536 mypy_boto3_cognito_idp-1.34.93/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-04-26 19:32:22.179536 mypy_boto3_cognito_idp-1.34.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.175536 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80829 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80826 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-04-26 19:31:55.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    83482 2024-04-26 19:31:57.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83482 2024-04-26 19:31:56.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:32:22.179536 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 19:32:22.000000 mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:32:22.179536 mypy_boto3_cognito_idp-1.34.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-26 19:31:54.000000 mypy_boto3_cognito_idp-1.34.93/setup.py
```

### Comparing `mypy_boto3_cognito_idp-1.34.91/LICENSE` & `mypy_boto3_cognito_idp-1.34.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/PKG-INFO` & `mypy_boto3_cognito_idp-1.34.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.34.91
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.93
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_cognito_idp-1.34.91/README.md` & `mypy_boto3_cognito_idp-1.34.93/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__init__.pyi` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/__main__.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentityProvider 1.34.91\n"
-        "Version:         1.34.91\n"
+        "Type annotations for boto3.CognitoIdentityProvider 1.34.93\n"
+        "Version:         1.34.93\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.91")
+    print("1.34.93")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/client.pyi` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/literals.pyi` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/paginator.pyi` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.py` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.34.91
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.93
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.34.93 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-idp)](https://pepy.tech/project/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.34.93](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_cognito_idp-1.34.91/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy_boto3_cognito_idp-1.34.93/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_cognito_idp-1.34.91/setup.py` & `mypy_boto3_cognito_idp-1.34.93/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.34.91",
+    version="1.34.93",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CognitoIdentityProvider 1.34.91 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.CognitoIdentityProvider 1.34.93 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

