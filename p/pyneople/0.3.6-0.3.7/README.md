# Comparing `tmp/pyneople-0.3.6.tar.gz` & `tmp/pyneople-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.3.6.tar", last modified: Wed May  8 08:56:52 2024, max compression
+gzip compressed data, was "pyneople-0.3.7.tar", last modified: Wed May  8 09:05:34 2024, max compression
```

## Comparing `pyneople-0.3.6.tar` & `pyneople-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:56:52.590759 pyneople-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 08:56:41.000000 pyneople-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:56:52.590759 pyneople-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 08:56:41.000000 pyneople-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 08:56:41.000000 pyneople-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:56:52.590759 pyneople-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 08:56:41.000000 pyneople-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:56:52.586759 pyneople-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:56:52.586759 pyneople-0.3.6/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 08:56:41.000000 pyneople-0.3.6/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 08:56:41.000000 pyneople-0.3.6/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37543 2024-05-08 08:56:41.000000 pyneople-0.3.6/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-08 08:56:41.000000 pyneople-0.3.6/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-08 08:56:41.000000 pyneople-0.3.6/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:56:52.590759 pyneople-0.3.6/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:56:52.000000 pyneople-0.3.6/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:56:52.000000 pyneople-0.3.6/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:56:52.000000 pyneople-0.3.6/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 08:56:52.000000 pyneople-0.3.6/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:34.359842 pyneople-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 09:05:19.000000 pyneople-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 09:05:34.359842 pyneople-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 09:05:19.000000 pyneople-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 09:05:19.000000 pyneople-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:05:34.359842 pyneople-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 09:05:19.000000 pyneople-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:34.355842 pyneople-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:34.359842 pyneople-0.3.7/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 09:05:19.000000 pyneople-0.3.7/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 09:05:19.000000 pyneople-0.3.7/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37562 2024-05-08 09:05:19.000000 pyneople-0.3.7/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-08 09:05:19.000000 pyneople-0.3.7/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-08 09:05:19.000000 pyneople-0.3.7/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:05:34.359842 pyneople-0.3.7/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 09:05:34.000000 pyneople-0.3.7/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 09:05:34.000000 pyneople-0.3.7/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:05:34.000000 pyneople-0.3.7/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 09:05:34.000000 pyneople-0.3.7/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.3.6/LICENSE` & `pyneople-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.6/PKG-INFO` & `pyneople-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.6
+Version: 0.3.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.3.6/setup.py` & `pyneople-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.3.6",
+    version="0.3.7",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.3.6/src/pyneople/METADATA.py` & `pyneople-0.3.7/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.6/src/pyneople/character.py` & `pyneople-0.3.7/src/pyneople/character.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+character
+"""
+
 import datetime
 import urllib.parse
 from typing import Iterable, Union
 from .functions import get_request, explain_enchant
 from .METADATA import SERVER_NAME_2_ID, CHARACTER_SEARCH_NAME, \
                     CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST, \
                     BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME, GROWINFO_NAME
```

### Comparing `pyneople-0.3.6/src/pyneople/database_connecter.py` & `pyneople-0.3.7/src/pyneople/database_connecter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+database connecter
+"""
+
 from .functions import get_request, ServerMaintenanceError, attr_flatten
 from .character import CharacterFame, CharacterSearch, Timeline
 from multiprocessing import Process, Queue, Value
 from pymongo import MongoClient
 from typing import Callable
 from psycopg2 import sql
 from typing import Union
```

### Comparing `pyneople-0.3.6/src/pyneople/functions.py` & `pyneople-0.3.7/src/pyneople/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+functions
+"""
+
 import time
 import json
 import requests
 from .METADATA import JOBCLASS
 from .METADATA import SETTINGS
 
 __all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'system_maintenance', 'NeopleOpenAPIError', 'ServerMaintenanceError', 'value_flatten', 'attr_flatten']
```

### Comparing `pyneople-0.3.6/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.3.7/src/pyneople.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.6
+Version: 0.3.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

