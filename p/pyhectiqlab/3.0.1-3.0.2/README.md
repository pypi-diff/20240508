# Comparing `tmp/pyhectiqlab-3.0.1.tar.gz` & `tmp/pyhectiqlab-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhectiqlab-3.0.1.tar", last modified: Mon May  6 17:56:07 2024, max compression
+gzip compressed data, was "pyhectiqlab-3.0.2.tar", last modified: Wed May  8 15:24:53 2024, max compression
```

## Comparing `pyhectiqlab-3.0.1.tar` & `pyhectiqlab-3.0.2.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:56:07.114186 pyhectiqlab-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-06 17:56:07.114186 pyhectiqlab-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:56:07.110186 pyhectiqlab-3.0.1/pyhectiqlab/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    24825 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyhectiqlab/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:56:07.114186 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 17:56:07.000000 pyhectiqlab-3.0.1/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:56:07.114186 pyhectiqlab-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:56:07.114186 pyhectiqlab-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-06 17:55:49.000000 pyhectiqlab-3.0.1/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:24:53.071185 pyhectiqlab-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 15:24:53.067185 pyhectiqlab-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:24:53.063185 pyhectiqlab-3.0.2/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:24:53.067185 pyhectiqlab-3.0.2/pyhectiqlab/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/functional/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24825 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:24:53.067185 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:24:53.000000 pyhectiqlab-3.0.2/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:24:53.071185 pyhectiqlab-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:24:53.067185 pyhectiqlab-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-08 15:24:34.000000 pyhectiqlab-3.0.2/tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.1/PKG-INFO` & `pyhectiqlab-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/__init__.py` & `pyhectiqlab-3.0.2/pyhectiqlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 from pyhectiqlab.settings import getenv
 
 API_URL = getenv("PYHECTIQLAB_API_URL", "https://api.lab.hectiq.ai")
 
 from pyhectiqlab.config import Config
 from pyhectiqlab.dataset import Dataset
@@ -13,15 +13,14 @@
 
 def debug_mode():
     from pyhectiqlab.client import Client
 
     Client.online(False)
 
 
-
 __all__ = [
     "API_URL",
     "Artifact",
     "Dataset",
     "Model",
     "Run",
     "Config",
```

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/artifact.py` & `pyhectiqlab-3.0.2/pyhectiqlab/artifact.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/auth.py` & `pyhectiqlab-3.0.2/pyhectiqlab/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/block.py` & `pyhectiqlab-3.0.2/pyhectiqlab/block.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/client.py` & `pyhectiqlab-3.0.2/pyhectiqlab/client.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/dataset.py` & `pyhectiqlab-3.0.2/pyhectiqlab/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from pyhectiqlab.tag import Tag
 from pyhectiqlab.project import Project
 from pyhectiqlab.block import Block
 from pyhectiqlab.block import Block
 from pyhectiqlab.client import Client
 from pyhectiqlab.decorators import functional_alias, online_method
-from pyhectiqlab.utils.path import list_all_files_in_dir, extract_host_from_source
-from pyhectiqlab.utils.itertools import batched
+from .utils import batched, list_all_files_in_dir, extract_host_from_source
 
 
 class Dataset:
     _client: Client = Client
 
     @staticmethod
     @online_method
```

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/decorators.py` & `pyhectiqlab-3.0.2/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/logging.py` & `pyhectiqlab-3.0.2/pyhectiqlab/logging.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.2/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/model.py` & `pyhectiqlab-3.0.2/pyhectiqlab/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from typing import Optional, List, Union
 
 from pyhectiqlab.tag import Tag
 from pyhectiqlab.block import Block
 from pyhectiqlab.project import Project
 from pyhectiqlab.client import Client
 from pyhectiqlab.decorators import functional_alias, online_method
-from pyhectiqlab.utils.path import list_all_files_in_dir
-from pyhectiqlab.utils.itertools import batched
+from pyhectiqlab.utils import batched, list_all_files_in_dir
 
 
 class Model:
     _client: Client = Client
 
     @staticmethod
     @online_method
```

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/project.py` & `pyhectiqlab-3.0.2/pyhectiqlab/project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/run.py` & `pyhectiqlab-3.0.2/pyhectiqlab/run.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/step.py` & `pyhectiqlab-3.0.2/pyhectiqlab/step.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/tag.py` & `pyhectiqlab-3.0.2/pyhectiqlab/tag.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab/versions.py` & `pyhectiqlab-3.0.2/pyhectiqlab/versions.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-3.0.2/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.1/pyproject.toml` & `pyhectiqlab-3.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0"]
 
 [tool.setuptools]
-packages = ["pyhectiqlab"]
+packages = ["pyhectiqlab", "pyhectiqlab.functional"]
 
 [project]
 authors = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 dependencies = [
@@ -21,24 +21,24 @@
   "hectiq-config==1.1.0",
   "tqdm",
   "packaging>=21.0",
   "click",
   "toml",
   "pydantic",
   "python-dotenv",
-  "google-cloud-storage"
+  "google-cloud-storage",
 ]
 description = "Python client for the Hectiq Lab plateform."
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 name = "pyhectiqlab"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "3.0.1"
+version = "3.0.2"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-lab-revision.git"
 
 [project.entry-points.console_scripts]
 hectiq-lab = "pyhectiqlab.cli:main"
```

### Comparing `pyhectiqlab-3.0.1/tests/test_dataset.py` & `pyhectiqlab-3.0.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/tests/test_model.py` & `pyhectiqlab-3.0.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/tests/test_project.py` & `pyhectiqlab-3.0.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.1/tests/test_run.py` & `pyhectiqlab-3.0.2/tests/test_run.py`

 * *Files identical despite different names*

