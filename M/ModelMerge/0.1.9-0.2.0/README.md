# Comparing `tmp/modelmerge-0.1.9.tar.gz` & `tmp/modelmerge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.1.9.tar", last modified: Wed May  8 18:54:53 2024, max compression
+gzip compressed data, was "modelmerge-0.2.0.tar", last modified: Wed May  8 19:06:28 2024, max compression
```

## Comparing `modelmerge-0.1.9.tar` & `modelmerge-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:54:45.000000 modelmerge-0.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.548281 modelmerge-0.1.9/ModelMerge/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:54:53.552281 modelmerge-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:54:45.000000 modelmerge-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:54:53.552281 modelmerge-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 18:54:45.000000 modelmerge-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 19:06:20.000000 modelmerge-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:06:28.552159 modelmerge-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 19:06:20.000000 modelmerge-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:06:28.552159 modelmerge-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 19:06:20.000000 modelmerge-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.548159 modelmerge-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.548159 modelmerge-0.2.0/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.1.9/LICENSE` & `modelmerge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.0/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from .config import BaseLLM, ENGINES, CUSTOM_MODELS, PLUGINS, LANGUAGE
 
 import httpx
 import requests
 import tiktoken
 
 # import config
-from utils.plugins import check_json, Web_crawler, cut_message
-from tools.function_call import function_call_list
+from ..utils.plugins import check_json, Web_crawler, cut_message
+from ..tools.function_call import function_call_list
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
     """
```

### Comparing `modelmerge-0.1.9/ModelMerge/models/claude.py` & `modelmerge-0.2.0/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/models/config.py` & `modelmerge-0.2.0/src/ModelMerge/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import httpx
 import requests
 from pathlib import Path
 
-from utils import prompt
+from ..utils import prompt
 
 
 
 # if config.CUSTOM_MODELS_LIST:
 #     ENGINES.extend(config.CUSTOM_MODELS_LIST)
 
 ENGINES = [
```

### Comparing `modelmerge-0.1.9/ModelMerge/models/dalle.py` & `modelmerge-0.2.0/src/ModelMerge/models/dalle.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/models/genimi.py` & `modelmerge-0.2.0/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/models/groq.py` & `modelmerge-0.2.0/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/tools/function_call.py` & `modelmerge-0.2.0/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/utils/plugins.py` & `modelmerge-0.2.0/src/ModelMerge/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/ModelMerge/utils/prompt.py` & `modelmerge-0.2.0/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.9/setup.py` & `modelmerge-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 setup(
     name="ModelMerge",
-    version="0.1.9",
+    version="0.2.0",
     description="ModelMerge is a multi-large language model API aggregator.",
     long_description=Path.open(Path("README.md"), encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    packages=find_packages("ModelMerge"),
-    package_dir={"": "ModelMerge"},
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     install_requires=Path.open(Path("requirements.txt"), encoding="utf-8").read().splitlines(),
     # py_modules=["LLM-Hub"]
 )
```

