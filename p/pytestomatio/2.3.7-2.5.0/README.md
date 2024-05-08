# Comparing `tmp/pytestomatio-2.3.7.tar.gz` & `tmp/pytestomatio-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.3.7.tar", last modified: Fri May  3 11:29:22 2024, max compression
+gzip compressed data, was "pytestomatio-2.5.0.tar", last modified: Wed May  8 15:53:08 2024, max compression
```

## Comparing `pytestomatio-2.3.7.tar` & `pytestomatio-2.5.0.tar`

### file list

```diff
@@ -1,41 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.356450 pytestomatio-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-03 11:29:22.356450 pytestomatio-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.352450 pytestomatio-2.3.7/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.352450 pytestomatio-2.3.7/pytestomatio/decor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/decor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/decor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/decor/pep8.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.356450 pytestomatio-2.3.7/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 11:29:22.000000 pytestomatio-2.3.7/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:29:22.356450 pytestomatio-2.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.352450 pytestomatio-2.3.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.352450 pytestomatio-2.3.7/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:22.356450 pytestomatio-2.3.7/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-03 11:29:17.000000 pytestomatio-2.3.7/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.669726 pytestomatio-2.5.0/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/s3_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/testItem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/testomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/pytestomatio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/parser_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/worker_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_root.py
```

### Comparing `pytestomatio-2.3.7/LICENSE` & `pytestomatio-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/PKG-INFO` & `pytestomatio-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.7
+Version: 2.5.0
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,24 @@
 TESTOMATIO=<key>
 ```
 Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
 If you are not sure, don't set this variable. Default value is 'default'
 ```bash
 TESTOMATIO_CODE_STYLE=pep8
 ```
+Set test run name in Testomat.io
+```bash
+TESTOMATIO_RUN=test_run_name
+```
+Set test run environment in Testomat.io
+```bash
+TESTOMATIO_ENV=linux,chrome,1920x1080
+```
+Set test run labels in Testomat.io
+TESTOMATIO_LABELS=smoke,regression
 
 ```bash
 
 
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
```

### Comparing `pytestomatio-2.3.7/README.md` & `pytestomatio-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,24 @@
 TESTOMATIO=<key>
 ```
 Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
 If you are not sure, don't set this variable. Default value is 'default'
 ```bash
 TESTOMATIO_CODE_STYLE=pep8
 ```
+Set test run name in Testomat.io
+```bash
+TESTOMATIO_RUN=test_run_name
+```
+Set test run environment in Testomat.io
+```bash
+TESTOMATIO_ENV=linux,chrome,1920x1080
+```
+Set test run labels in Testomat.io
+TESTOMATIO_LABELS=smoke,regression
 
 ```bash
 
 
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
```

### Comparing `pytestomatio-2.3.7/pyproject.toml` & `pytestomatio-2.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=65.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-exclude = [".github", "tests"]
+exclude = [".github", "tests", "build", "dist", ".venv", "pytestomatio.egg-info", ".env", ".gitignore", "CHANGELOG.md"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.3.7"
+version = "2.5.0"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>7.2.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
@@ -35,16 +35,14 @@
 classifiers = [
     "Framework :: Pytest",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[tool.pytest.ini_options]
-
 [project.urls]
 "Testomat.io" = "https://testomat.io/"
 "Homepage" = "https://github.com/testomatio/pytestomatio"
 "Bug Tracker" = "https://github.com/testomatio/pytestomatio/issues"
 
 [project.entry-points.pytest11]
 pytestomatio = "pytestomatio.main"
```

### Comparing `pytestomatio-2.3.7/pytestomatio/code_collector.py` & `pytestomatio-2.5.0/pytestomatio/testing/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/pytestomatio/connector.py` & `pytestomatio-2.5.0/pytestomatio/connect/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import requests
 from requests.exceptions import HTTPError, ConnectionError
 import logging
 from os.path import join, normpath
-from os import getenv
 
-from .testItem import TestItem
+from pytestomatio.testing.testItem import TestItem
 
 log = logging.getLogger('pytestomatio')
 
 
 class Connector:
     def __init__(self, base_url: str = 'https://app.testomat.io', api_key: str = None):
         self.base_url = base_url
@@ -21,15 +20,15 @@
             self,
             tests: list[TestItem],
             no_empty: bool = False,
             no_detach: bool = False,
             structure: bool = False,
             create: bool = False,
             directory: str = None
-        ):
+    ):
         request = {
             "framework": "pytest",
             "language": "python",
             "noempty": no_empty,
             "no-detach": no_detach,
             "structure": structure if not no_empty else False,
             "create": create,
@@ -39,15 +38,16 @@
         for test in tests:
             request['tests'].append({
                 "name": test.sync_title,
                 "suites": [
                     test.class_name
                 ],
                 "code": test.source_code,
-                "file": test.file_path if structure else (test.file_name if directory is None else normpath(join(directory, test.file_name))),
+                "file": test.file_path if structure else (
+                    test.file_name if directory is None else normpath(join(directory, test.file_name))),
             })
 
         try:
             response = self.session.post(f'{self.base_url}/api/load?api_key={self.api_key}', json=request)
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
             return
@@ -72,15 +72,14 @@
         request = {
             "api_key": self.api_key,
             "title": title,
             "group_title": group_title,
             "env": env,
             "label": label,
             "parallel": True,
-            "shared_run": True,
         }
         filtered_request = {k: v for k, v in request.items() if v is not None}
         print('create_test_run', filtered_request)
         try:
             response = self.session.post(f'{self.base_url}/api/reporter', json=filtered_request)
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
@@ -91,27 +90,27 @@
         except Exception as e:
             log.error(f'Generic exception happened. Please report an issue. {e}')
             return
 
         if response.status_code == 200:
             log.info(f'Test run created {response.json()["uid"]}')
             return response.json()
-        
-    def update_test_run(self, id: str, title: str, group_title, env: str, label: str, shared_run: bool, parallel) -> dict | None:
+
+    def update_test_run(self, id: str, title: str, group_title, env: str, label: str, shared_run: bool,
+                        parallel) -> dict | None:
         request = {
             "api_key": self.api_key,
             "title": title,
             "group_title": group_title,
-            #"env": env, TODO: enabled when bug with 500 response fixed
-            #"label": label, TODO: enabled when bug with 500 response fixed
+            # "env": env, TODO: enabled when bug with 500 response fixed
+            # "label": label, TODO: enabled when bug with 500 response fixed
             "parallel": True,
-            "shared_run": True
         }
         filtered_request = {k: v for k, v in request.items() if v is not None}
-        
+
         try:
             response = self.session.put(f'{self.base_url}/api/reporter/{id}', json=filtered_request)
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
             return
         except HTTPError:
             log.error(f'Failed to connect to {self.base_url}')
@@ -165,17 +164,16 @@
         except Exception as e:
             log.error(f'Generic exception happened. Please report an issue. {e}')
             return
         if response.status_code == 200:
             log.info('Test status updated')
 
     # TODO: I guess this class should be just an API client and used within testRun (testRunConfig)
-    def finish_test_run(self, run_id: str) -> None:
-        is_parallel = getenv('TESTOMATIO_SHARED_RUN', 'false').lower() in ['true', '1']
-        status_event = "finish_parallel" if is_parallel else 'finish'
+    def finish_test_run(self, run_id: str, is_final=False) -> None:
+        status_event = 'finish_parallel' if is_final else 'finish'
         try:
             self.session.put(f'{self.base_url}/api/reporter/{run_id}?api_key={self.api_key}',
                              json={"status_event": status_event})
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
             return
         except HTTPError:
```

### Comparing `pytestomatio-2.3.7/pytestomatio/decor/default.py` & `pytestomatio-2.5.0/pytestomatio/decor/default.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/pytestomatio/decor/pep8.py` & `pytestomatio-2.5.0/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/pytestomatio/decorator_updater.py` & `pytestomatio-2.5.0/pytestomatio/decor/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/pytestomatio/s3_connector.py` & `pytestomatio-2.5.0/pytestomatio/connect/s3_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 import logging
 from io import BytesIO
 
 log = logging.getLogger(__name__)
 log.setLevel('INFO')
 
 
+def parse_endpoint(endpoint: str or None) -> str or None:
+    if endpoint is None:
+        return
+    if endpoint.startswith('https://'):
+        return endpoint[8:]
+    elif endpoint.startswith('http://'):
+        return endpoint[7:]
+    return endpoint
+
+
 class S3Connector:
-    def __init__(self, aws_access_key_id: str, aws_secret_access_key: str,
-                 endpoint: str, bucket_name: str = None):
-        if endpoint.startswith('https://'):
-            self.endpoint = endpoint[8:]
-        elif endpoint.startswith('http://'):
-            self.endpoint = endpoint[7:]
-        else:
-            self.endpoint = endpoint
+    def __init__(self, aws_access_key_id: str or None = None,
+                 aws_secret_access_key: str or None = None,
+                 endpoint: str or None = None,
+                 bucket_name: str or None = None):
+
+        self.endpoint = parse_endpoint(endpoint)
         self.bucket_name = bucket_name
         self.client = None
         self._is_logged_in = False
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
 
     def login(self):
```

### Comparing `pytestomatio-2.3.7/pytestomatio/testItem.py` & `pytestomatio-2.5.0/pytestomatio/testing/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.7/pytestomatio/testRunConfig.py` & `pytestomatio-2.5.0/pytestomatio/testomatio/testRunConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import datetime as dt
+import uuid
 from re import sub
+from pytestomatio.utils.worker_sync import SyncLock
 
 
 class TestRunConfig:
     def __init__(
             self,
             id: str = None,
             title: str = None,
             group_title: str = None,
             environment: str = None,
             label: str = None,
             parallel: bool = True,
             shared_run: bool = True
-        ):
+    ):
         self.test_run_id = id
         self.title = title if title else 'test run at ' + dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.environment = self.safe_string_list(environment)
         self.label = self.safe_string_list(label)
         self.group_title = group_title
         self.parallel = parallel
-        if shared_run and not title:
-            raise ValueError('TESTOMATIO_SHARED_RUN can only be used together with TESTOMATIO_TITLE')
         self.shared_run = shared_run
         self.status_request = {}
+        self.lock = SyncLock()
 
     def to_dict(self) -> dict:
         result = dict()
         if self.test_run_id:
             result['id'] = self.test_run_id
         result['title'] = self.title
         result['group_title'] = self.group_title
         result['env'] = self.environment
         result['label'] = self.label
         result['parallel'] = self.parallel
         result['shared_run'] = self.shared_run
         return result
-    
-    def set_run_id(self, run_id: str) -> None:
-        self.test_run_id = run_id
 
     def set_env(self, env: str) -> None:
         self.environment = self.safe_string_list(env)
-    
+
     def safe_string_list(self, param: str):
         if not param:
             return None
         return ",".join([sub(r"\s", "", part) for part in param.split(',')])
```

### Comparing `pytestomatio-2.3.7/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.5.0/pytestomatio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.7
+Version: 2.5.0
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,24 @@
 TESTOMATIO=<key>
 ```
 Select code style by set environment variable `TESTOMATIO_CODE_STYLE`. Available options are 'default' and 'pep8'  
 If you are not sure, don't set this variable. Default value is 'default'
 ```bash
 TESTOMATIO_CODE_STYLE=pep8
 ```
+Set test run name in Testomat.io
+```bash
+TESTOMATIO_RUN=test_run_name
+```
+Set test run environment in Testomat.io
+```bash
+TESTOMATIO_ENV=linux,chrome,1920x1080
+```
+Set test run labels in Testomat.io
+TESTOMATIO_LABELS=smoke,regression
 
 ```bash
 
 
 ### Run groups parameter
 There is environment variable `TESTOMATIO_RUNGROUP_TITLE` that can be used to specify run tests with specific group title.
```

### Comparing `pytestomatio-2.3.7/tests/test_root.py` & `pytestomatio-2.5.0/tests/test_root.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 
 
 @mark.testomatio('@T4e2f8df1')
 def test_pass_fix(dummy_fixture):
     assert 3 + 3 == 6
 
 
+#  -------------------------------------------
 @mark.testomatio('@Tefe6c6a2')
 def test_fail():
     assert 2 + 2 == 11
 
 
+#  -------------------------------------------
+
 @mark.testomatio('@Tca8a4366')
 @mark.parametrize('data', [8, 1, 2, 3, 4, 5, 'a', b'123', b'asdasd', {'hello': 'world'}, [1, 2, 3]])
 def test_ddt_parametrized(data):
     assert str(data).isnumeric()
 
 
 @mark.testomatio('@Tc5045fa6')
```

