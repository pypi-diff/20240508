# Comparing `tmp/poetry_plugin_dotenv-2.1.1.tar.gz` & `tmp/poetry_plugin_dotenv-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-2.1.1.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-2.1.2.tar", max compression
```

## Comparing `poetry_plugin_dotenv-2.1.1.tar` & `poetry_plugin_dotenv-2.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-05-07 08:49:20.403439 poetry_plugin_dotenv-2.1.1/LICENSE
--rw-r--r--   0        0        0     9687 2024-05-07 08:49:20.403439 poetry_plugin_dotenv-2.1.1/README.md
--rw-r--r--   0        0        0     6955 2024-05-07 08:49:41.539426 poetry_plugin_dotenv-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      778 2024-05-07 08:49:41.539426 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/config.py
--rw-r--r--   0        0        0      335 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5421 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6005 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1572 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     1558 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/logger.py
--rw-r--r--   0        0        0     1999 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-05-07 08:49:20.419439 poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-08 20:07:23.245219 poetry_plugin_dotenv-2.1.2/LICENSE
+-rw-r--r--   0        0        0     9687 2024-05-08 20:07:23.245219 poetry_plugin_dotenv-2.1.2/README.md
+-rw-r--r--   0        0        0     6955 2024-05-08 20:07:43.821416 poetry_plugin_dotenv-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-05-08 20:07:43.825416 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     1558 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.2/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-2.1.1/LICENSE` & `poetry_plugin_dotenv-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/README.md` & `poetry_plugin_dotenv-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-    <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=200>
+    <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=300>
 </div>
 
 <p align="center">
     <a href="https://opensource.org/licenses/MIT">
         <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
```

### Comparing `poetry_plugin_dotenv-2.1.1/pyproject.toml` & `poetry_plugin_dotenv-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "2.1.1"
+version = "2.1.2"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
```

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/config.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/config.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/logger.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/logger.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.1/PKG-INFO` & `poetry_plugin_dotenv-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 2.1.1
+Version: 2.1.2
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -33,15 +33,15 @@
 Project-URL: Issues, https://github.com/pivoshenko/poetry-plugin-dotenv/issues
 Project-URL: Repository, https://github.com/pivoshenko/poetry-plugin-dotenv
 Project-URL: Releases, https://github.com/pivoshenko/poetry-plugin-dotenv/releases
 Project-URL: Say Thanks!, https://www.buymeacoffee.com/pivoshenko
 Description-Content-Type: text/markdown
 
 <div align="center">
-    <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=200>
+    <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=300>
 </div>
 
 <p align="center">
     <a href="https://opensource.org/licenses/MIT">
         <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.1 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.2 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
```

