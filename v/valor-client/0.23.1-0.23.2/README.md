# Comparing `tmp/valor_client-0.23.1.tar.gz` & `tmp/valor_client-0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.23.1.tar", last modified: Mon May  6 17:30:47 2024, max compression
+gzip compressed data, was "valor_client-0.23.2.tar", last modified: Wed May  8 20:34:21 2024, max compression
```

## Comparing `valor_client-0.23.1.tar` & `valor_client-0.23.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.534159 valor_client-0.23.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 17:30:41.000000 valor_client-0.23.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-06 17:30:47.534159 valor_client-0.23.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 17:30:41.000000 valor_client-0.23.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:30:47.534159 valor_client-0.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 17:30:41.000000 valor_client-0.23.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.526158 valor_client-0.23.1/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.526158 valor_client-0.23.1/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-06 17:30:41.000000 valor_client-0.23.1/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53919 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.530158 valor_client-0.23.1/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.534159 valor_client-0.23.1/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-06 17:30:41.000000 valor_client-0.23.1/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:30:47.534159 valor_client-0.23.1/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-06 17:30:47.000000 valor_client-0.23.1/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 17:30:47.000000 valor_client-0.23.1/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:30:47.000000 valor_client-0.23.1/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 17:30:47.000000 valor_client-0.23.1/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 17:30:47.000000 valor_client-0.23.1/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 20:34:17.000000 valor_client-0.23.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 20:34:21.736180 valor_client-0.23.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 20:34:17.000000 valor_client-0.23.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:34:21.736180 valor_client-0.23.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 20:34:17.000000 valor_client-0.23.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.732180 valor_client-0.23.2/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-08 20:34:17.000000 valor_client-0.23.2/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-08 20:34:17.000000 valor_client-0.23.2/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:34:21.736180 valor_client-0.23.2/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 20:34:21.000000 valor_client-0.23.2/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.23.1/LICENSE` & `valor_client-0.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/PKG-INFO` & `valor_client-0.23.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.23.1
+Version: 0.23.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.23.1/pyproject.toml` & `valor_client-0.23.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/conftest.py` & `valor_client-0.23.2/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/coretypes/test_core.py` & `valor_client-0.23.2/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.23.2/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/coretypes/test_filtering.py` & `valor_client-0.23.2/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/schemas/test_filters.py` & `valor_client-0.23.2/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/schemas/test_geojson.py` & `valor_client-0.23.2/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/schemas/test_label.py` & `valor_client-0.23.2/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.23.2/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.23.2/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.23.2/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/test_operators.py` & `valor_client-0.23.2/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.23.2/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.23.2/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/test_client.py` & `valor_client-0.23.2/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/unit-tests/test_viz.py` & `valor_client-0.23.2/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/__init__.py` & `valor_client-0.23.2/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/client.py` & `valor_client-0.23.2/valor/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import math
 import os
 import time
 from dataclasses import asdict, dataclass
-from typing import Callable, List, Optional, TypeVar, Union
+from typing import Callable, Dict, List, Optional, TypeVar, Union
 from urllib.parse import urlencode, urljoin
 
 import requests
 from packaging import version
 
 from valor import __version__ as client_version
 from valor.enums import TableStatus
@@ -823,28 +823,33 @@
 
     def get_evaluations(
         self,
         *,
         evaluation_ids: Optional[List[int]] = None,
         models: Optional[List[str]] = None,
         datasets: Optional[List[str]] = None,
+        metrics_to_sort_by: Optional[
+            Dict[str, Union[Dict[str, str], str]]
+        ] = None,
     ) -> List[dict]:
         """
         Returns all evaluations associated with user-supplied dataset and/or model names.
 
         `GET` endpoint.
 
         Parameters
         ----------
         evaluation_ids : List[int], optional
             A list of job IDs to return metrics for.
         models : List[str], optional
             A list of model names that we want to return metrics for.
         datasets : List[str], optional
             A list of dataset names that we want to return metrics for.
+        metrics_to_sort_by: dict[str, str | dict[str, str]], optional
+            An optional dict of metric types to sort the evaluations by.
 
         Returns
         -------
         List[dict]
             List of dictionaries describing the returned evaluations.
         """
 
@@ -861,14 +866,17 @@
                 element = [element]
             return {param_name: ",".join(map(str, element))}
 
         params = {
             **_build_query_param("evaluation_ids", evaluation_ids, int),
             **_build_query_param("models", models, str),
             **_build_query_param("datasets", datasets, str),
+            **_build_query_param(
+                "metrics_to_sort_by", json.dumps(metrics_to_sort_by), str
+            ),
         }
 
         query_str = urlencode(params)
         endpoint = f"evaluations?{query_str}"
 
         return self._requests_get_rel_host(endpoint).json()
```

### Comparing `valor_client-0.23.1/valor/coretypes.py` & `valor_client-0.23.2/valor/coretypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,24 +592,34 @@
                 "Cannot filter by dataset_names when calling `Dataset.get_datums`."
             )
         filter_["dataset_names"] = [self.get_name()]
         return Client(self.conn).get_datums(filter_by=filter_)
 
     def get_evaluations(
         self,
+        metrics_to_sort_by: Optional[
+            Dict[str, Union[Dict[str, str], str]]
+        ] = None,
     ) -> List[Evaluation]:
         """
         Get all evaluations associated with a given dataset.
 
+        Parameters
+        ----------
+        metrics_to_sort_by: dict[str, str | dict[str, str]], optional
+            An optional dict of metric types to sort the evaluations by.
+
         Returns
         ----------
         List[Evaluation]
             A list of `Evaluations` associated with the dataset.
         """
-        return Client(self.conn).get_evaluations(datasets=[self])
+        return Client(self.conn).get_evaluations(
+            datasets=[self], metrics_to_sort_by=metrics_to_sort_by
+        )
 
     def get_summary(self) -> DatasetSummary:
         """
         Get the summary of a given dataset.
 
         Returns
         -------
@@ -1100,24 +1110,35 @@
         List[Label]
             A list of `Labels` associated with the model.
         """
         return Client(self.conn).get_labels_from_model(self)
 
     def get_evaluations(
         self,
+        metrics_to_sort_by: Optional[
+            Dict[str, Union[Dict[str, str], str]]
+        ] = None,
     ) -> List[Evaluation]:
         """
         Get all evaluations associated with a given model.
 
+        Parameters
+        ----------
+        metrics_to_sort_by: dict[str, str | dict[str, str]], optional
+            An optional dict of metric types to sort the evaluations by.
+
+
         Returns
         ----------
         List[Evaluation]
             A list of `Evaluations` associated with the model.
         """
-        return Client(self.conn).get_evaluations(models=[self])
+        return Client(self.conn).get_evaluations(
+            models=[self], metrics_to_sort_by=metrics_to_sort_by
+        )
 
 
 class Client:
     """
     Valor client object for interacting with the api.
 
     Parameters
@@ -1705,26 +1726,31 @@
 
     def get_evaluations(
         self,
         *,
         evaluation_ids: Optional[List[int]] = None,
         models: Union[List[Model], List[str], None] = None,
         datasets: Union[List[Dataset], List[str], None] = None,
+        metrics_to_sort_by: Optional[
+            Dict[str, Union[Dict[str, str], str]]
+        ] = None,
     ) -> List[Evaluation]:
         """
         Returns all evaluations associated with user-supplied dataset and/or model names.
 
         Parameters
         ----------
         evaluation_ids : List[int], optional.
             A list of job IDs to return metrics for.
         models : Union[List[valor.Model], List[str]], optional
             A list of model names that we want to return metrics for.
         datasets : Union[List[valor.Dataset], List[str]], optional
             A list of dataset names that we want to return metrics for.
+        metrics_to_sort_by: dict[str, str | dict[str, str]], optional
+            An optional dict of metric types to sort the evaluations by.
 
         Returns
         -------
         List[valor.Evaluation]
             A list of evaluations.
         """
         if isinstance(datasets, list):
@@ -1739,14 +1765,15 @@
             ]
         return [
             Evaluation(connection=self.conn, **evaluation)
             for evaluation in self.conn.get_evaluations(
                 evaluation_ids=evaluation_ids,
                 models=models,
                 datasets=datasets,
+                metrics_to_sort_by=metrics_to_sort_by,
             )
         ]
 
     def evaluate(
         self, request: EvaluationRequest, allow_retries: bool = False
     ) -> List[Evaluation]:
         """
```

### Comparing `valor_client-0.23.1/valor/enums.py` & `valor_client-0.23.2/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/exceptions.py` & `valor_client-0.23.2/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/metatypes.py` & `valor_client-0.23.2/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/__init__.py` & `valor_client-0.23.2/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/evaluation.py` & `valor_client-0.23.2/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/filters.py` & `valor_client-0.23.2/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/symbolic/collections.py` & `valor_client-0.23.2/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/symbolic/operators.py` & `valor_client-0.23.2/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/schemas/symbolic/types.py` & `valor_client-0.23.2/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/type_checks.py` & `valor_client-0.23.2/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor/viz.py` & `valor_client-0.23.2/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.23.1/valor_client.egg-info/PKG-INFO` & `valor_client-0.23.2/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.23.1
+Version: 0.23.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.23.1/valor_client.egg-info/SOURCES.txt` & `valor_client-0.23.2/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

