# Comparing `tmp/group_local-0.0.15.tar.gz` & `tmp/group_local-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.15.tar", last modified: Tue May  7 19:45:52 2024, max compression
+gzip compressed data, was "group_local-0.0.16.tar", last modified: Wed May  8 07:01:33 2024, max compression
```

## Comparing `group_local-0.0.15.tar` & `group_local-0.0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:45:52.500985 group_local-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 19:45:52.500985 group_local-0.0.15/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:45:52.496985 group_local-0.0.15/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:45:52.500985 group_local-0.0.15/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:45:29.000000 group_local-0.0.15/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13284 2024-05-07 19:45:29.000000 group_local-0.0.15/group_local/src/groups_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-07 19:45:29.000000 group_local-0.0.15/group_local/src/groups_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:45:52.500985 group_local-0.0.15/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 19:45:52.000000 group_local-0.0.15/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 19:45:52.000000 group_local-0.0.15/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:45:52.000000 group_local-0.0.15/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 19:45:52.000000 group_local-0.0.15/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 19:45:52.000000 group_local-0.0.15/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 19:45:29.000000 group_local-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:45:52.500985 group_local-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-07 19:45:29.000000 group_local-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:01:33.541507 group_local-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 07:01:33.541507 group_local-0.0.16/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:01:33.537507 group_local-0.0.16/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:01:33.541507 group_local-0.0.16/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:01:15.000000 group_local-0.0.16/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-05-08 07:01:15.000000 group_local-0.0.16/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 07:01:15.000000 group_local-0.0.16/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:01:33.541507 group_local-0.0.16/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 07:01:33.000000 group_local-0.0.16/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-08 07:01:33.000000 group_local-0.0.16/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:01:33.000000 group_local-0.0.16/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 07:01:33.000000 group_local-0.0.16/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 07:01:33.000000 group_local-0.0.16/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 07:01:15.000000 group_local-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:01:33.541507 group_local-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 07:01:15.000000 group_local-0.0.16/setup.py
```

### Comparing `group_local-0.0.15/PKG-INFO` & `group_local-0.0.16/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.15
-Summary: PyPI Package for Circles groups-local Python
+Version: 0.0.16
+Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: database-infrastructure-local>=0.0.23
 Requires-Dist: user-context-remote>=0.0.58
 
-PyPI Package for Circles groups-local Python
+PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.15/group_local/src/groups_local.py` & `group_local-0.0.16/group_local/src/group_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Dict
-from .groups_local_constants import GroupsLocalConstants
+from .group_local_constants import GroupLocalConstants
 from database_mysql_local.generic_crud_ml import GenericCRUDML  # noqa: E402
-from database_infrastructure_local.number_generator import NumberGenerator  # noqa: E402
 from user_context_remote.user_context import UserContext  # noqa: E402
 from logger_local.Logger import Logger  # noqa: E402
 from language_remote.lang_code import LangCode  # noqa: E402
 
-logger = Logger.create_logger(object=GroupsLocalConstants.GROUPS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
+logger = Logger.create_logger(object=GroupLocalConstants.GROUP_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 user_context = UserContext()
 
 DEFAULT_SCHEMA_NAME = "group"
 DEFAULT_TABLE_NAME = "group_table"
 DEFAULT_VIEW_TABLE_NAME = "group_view"
 DEFAULT_ID_COLUMN_NAME = "group_id"
 DEFAULT_IS_MAIN_COLUMN_NAME = "is_main_title"
 
 
-class GroupsLocal(GenericCRUDML):
+class GroupLocal(GenericCRUDML):
 
     def __init__(self, is_test_data: bool = False):
         GenericCRUDML.__init__(self, default_schema_name=DEFAULT_SCHEMA_NAME, default_table_name=DEFAULT_TABLE_NAME,
                                default_id_column_name=DEFAULT_ID_COLUMN_NAME,
                                is_main_column_name=DEFAULT_IS_MAIN_COLUMN_NAME,
                                is_test_data=is_test_data)
```

### Comparing `group_local-0.0.15/group_local/src/groups_local_constants.py` & `group_local-0.0.16/group_local/src/group_local_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 
-class GroupsLocalConstants:
+class GroupLocalConstants:
 
     ENGLISH_GROUP_ID = 50001176
     VENTURE_CAPITAL_GROUP_ID = 50001177
     ADVOCATE_GROUP_ID = 50001175
-    GROUPS_LOCAL_PYTHON_COMPONENT_ID = 285
-    GROUPS_LOCAL_PYTHON_COMPONENT_NAME = "groups-local-python-package"
+    GROUP_LOCAL_PYTHON_COMPONENT_ID = 285
+    GROUP_LOCAL_PYTHON_COMPONENT_NAME = "group-local-python-package"
     DEVELOPER_EMAIL = "tal.g@circ.zone"
-    GROUPS_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
-        'component_id': GROUPS_LOCAL_PYTHON_COMPONENT_ID,
-        'component_name': GROUPS_LOCAL_PYTHON_COMPONENT_NAME,
+    GROUP_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
+        'component_id': GROUP_LOCAL_PYTHON_COMPONENT_ID,
+        'component_name': GROUP_LOCAL_PYTHON_COMPONENT_NAME,
         'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
         'developer_email': DEVELOPER_EMAIL
     }
 
-    GROUPS_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
-        'component_id': GROUPS_LOCAL_PYTHON_COMPONENT_ID,
-        'component_name': GROUPS_LOCAL_PYTHON_COMPONENT_NAME,
+    GROUP_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
+        'component_id': GROUP_LOCAL_PYTHON_COMPONENT_ID,
+        'component_name': GROUP_LOCAL_PYTHON_COMPONENT_NAME,
         'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
         'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
         'developer_email': DEVELOPER_EMAIL
     }
```

### Comparing `group_local-0.0.15/group_local.egg-info/PKG-INFO` & `group_local-0.0.16/group_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.15
-Summary: PyPI Package for Circles groups-local Python
+Version: 0.0.16
+Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: database-infrastructure-local>=0.0.23
 Requires-Dist: user-context-remote>=0.0.58
 
-PyPI Package for Circles groups-local Python
+PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.15/setup.py` & `group_local-0.0.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
-    name=PACKAGE_NAME,  # https://pypi.org/project/groups-local
-    version='0.0.15',
+    name=PACKAGE_NAME,  # https://pypi.org/project/group-local
+    version='0.0.16',
     author="Circles",
     author_email="info@circles.life",
-    description="PyPI Package for Circles groups-local Python",
-    long_description="PyPI Package for Circles groups-local Python",
+    description="PyPI Package for Circles group-local Python",
+    long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
```

