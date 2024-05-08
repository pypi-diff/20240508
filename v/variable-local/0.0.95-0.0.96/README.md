# Comparing `tmp/variable_local-0.0.95.tar.gz` & `tmp/variable_local-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.95.tar", last modified: Sun Apr 28 04:42:34 2024, max compression
+gzip compressed data, was "variable_local-0.0.96.tar", last modified: Wed May  8 01:15:37 2024, max compression
```

## Comparing `variable_local-0.0.95.tar` & `variable_local-0.0.96.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:42:34.638240 variable_local-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-28 04:42:34.638240 variable_local-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-28 04:42:05.000000 variable_local-0.0.95/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-28 04:42:05.000000 variable_local-0.0.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:42:34.638240 variable_local-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-28 04:42:05.000000 variable_local-0.0.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:42:34.634240 variable_local-0.0.95/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:42:34.634240 variable_local-0.0.95/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:42:05.000000 variable_local-0.0.95/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-28 04:42:05.000000 variable_local-0.0.95/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-28 04:42:05.000000 variable_local-0.0.95/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-28 04:42:05.000000 variable_local-0.0.95/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-28 04:42:05.000000 variable_local-0.0.95/variable_local/src/variables_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:42:34.634240 variable_local-0.0.95/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-28 04:42:34.000000 variable_local-0.0.95/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-28 04:42:34.000000 variable_local-0.0.95/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:42:34.000000 variable_local-0.0.95/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 04:42:34.000000 variable_local-0.0.95/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 04:42:34.000000 variable_local-0.0.95/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.173658 variable_local-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:15:37.173658 variable_local-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 01:15:00.000000 variable_local-0.0.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 01:15:00.000000 variable_local-0.0.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:15:37.173658 variable_local-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 01:15:00.000000 variable_local-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/variables_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.95/PKG-INFO` & `variable_local-0.0.96/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.95
+Version: 0.0.96
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Dist: logger-local>=0.0.118
-Requires-Dist: language-local
-Requires-Dist: database-mysql-local>=0.0.261
-Requires-Dist: smartlink-local
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: language-remote>=0.0.20
+Requires-Dist: database-mysql-local>=0.0.290
+Requires-Dist: smartlink-local>=0.0.34
 
 PyPI Package for Circles variable Local/Remote Python
```

### Comparing `variable_local-0.0.95/README.md` & `variable_local-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.95/pyproject.toml` & `variable_local-0.0.96/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.95/setup.py` & `variable_local-0.0.96/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.95',  # https://pypi.org/project/variable-local
+    version='0.0.96',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'logger-local>=0.0.118',
-        'language-local',
-        'database-mysql-local>=0.0.261',
-        'smartlink-local'
+        'logger-local>=0.0.135',
+        'language-remote>=0.0.20',
+        'database-mysql-local>=0.0.290',
+        'smartlink-local>=0.0.34'
     ],
 )
```

### Comparing `variable_local-0.0.95/variable_local/src/constants.py` & `variable_local-0.0.96/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.95/variable_local/src/template.py` & `variable_local-0.0.96/variable_local/src/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import re
 from datetime import datetime
 
-from language_local.lang_code import LangCode
+from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from smartlink_local.smartlink import SmartlinkLocal
 
 from .constants import variable_local_logger_init_object
 from .variables_local import VariablesLocal
 
 logger = Logger.create_logger(object=variable_local_logger_init_object)
```

### Comparing `variable_local-0.0.95/variable_local/src/variables_local.py` & `variable_local-0.0.96/variable_local/src/variables_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 
 from database_mysql_local.generic_crud import GenericCRUD
-from language_local.lang_code import LangCode
+from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from user_context_remote.user_context import UserContext
 
 from .constants import variable_local_logger_init_object, VARIABLE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID
 
 logger = Logger.create_logger(object=variable_local_logger_init_object)
 cache_with_timeout = {}
```

### Comparing `variable_local-0.0.95/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.96/variable_local.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.95
+Version: 0.0.96
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Dist: logger-local>=0.0.118
-Requires-Dist: language-local
-Requires-Dist: database-mysql-local>=0.0.261
-Requires-Dist: smartlink-local
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: language-remote>=0.0.20
+Requires-Dist: database-mysql-local>=0.0.290
+Requires-Dist: smartlink-local>=0.0.34
 
 PyPI Package for Circles variable Local/Remote Python
```

