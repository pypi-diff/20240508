# Comparing `tmp/modelmerge-0.1.8.tar.gz` & `tmp/modelmerge-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.1.8.tar", last modified: Wed May  8 18:50:16 2024, max compression
+gzip compressed data, was "modelmerge-0.1.9.tar", last modified: Wed May  8 18:54:53 2024, max compression
```

## Comparing `modelmerge-0.1.8.tar` & `modelmerge-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.745784 modelmerge-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:50:08.000000 modelmerge-0.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.745784 modelmerge-0.1.8/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:50:16.000000 modelmerge-0.1.8/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-08 18:50:16.000000 modelmerge-0.1.8/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:50:16.000000 modelmerge-0.1.8/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:50:16.000000 modelmerge-0.1.8/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:50:16.000000 modelmerge-0.1.8/ModelMerge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:50:16.745784 modelmerge-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:50:08.000000 modelmerge-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.741784 modelmerge-0.1.8/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 18:50:08.000000 modelmerge-0.1.8/models/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:50:16.745784 modelmerge-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 18:50:08.000000 modelmerge-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.741784 modelmerge-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 18:50:08.000000 modelmerge-0.1.8/test/test_google_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.745784 modelmerge-0.1.8/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:08.000000 modelmerge-0.1.8/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 18:50:08.000000 modelmerge-0.1.8/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:16.745784 modelmerge-0.1.8/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:08.000000 modelmerge-0.1.8/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 18:50:08.000000 modelmerge-0.1.8/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 18:50:08.000000 modelmerge-0.1.8/utils/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:54:45.000000 modelmerge-0.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.548281 modelmerge-0.1.9/ModelMerge/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:54:53.000000 modelmerge-0.1.9/ModelMerge/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:53.552281 modelmerge-0.1.9/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 18:54:45.000000 modelmerge-0.1.9/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:54:53.552281 modelmerge-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:54:45.000000 modelmerge-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:54:53.552281 modelmerge-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 18:54:45.000000 modelmerge-0.1.9/setup.py
```

### Comparing `modelmerge-0.1.8/LICENSE` & `modelmerge-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/chatgpt.py` & `modelmerge-0.1.9/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/claude.py` & `modelmerge-0.1.9/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/config.py` & `modelmerge-0.1.9/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/dalle.py` & `modelmerge-0.1.9/ModelMerge/models/dalle.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/genimi.py` & `modelmerge-0.1.9/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/models/groq.py` & `modelmerge-0.1.9/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/setup.py` & `modelmerge-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 setup(
     name="ModelMerge",
-    version="0.1.8",
+    version="0.1.9",
     description="ModelMerge is a multi-large language model API aggregator.",
     long_description=Path.open(Path("README.md"), encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    packages=find_packages(),
-    # package_dir={"": "."},
+    packages=find_packages("ModelMerge"),
+    package_dir={"": "ModelMerge"},
     install_requires=Path.open(Path("requirements.txt"), encoding="utf-8").read().splitlines(),
     # py_modules=["LLM-Hub"]
 )
```

### Comparing `modelmerge-0.1.8/tools/function_call.py` & `modelmerge-0.1.9/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/utils/plugins.py` & `modelmerge-0.1.9/ModelMerge/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.8/utils/prompt.py` & `modelmerge-0.1.9/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

