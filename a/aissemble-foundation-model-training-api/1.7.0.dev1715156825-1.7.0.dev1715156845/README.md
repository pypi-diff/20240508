# Comparing `tmp/aissemble_foundation_model_training_api-1.7.0.dev1715156825.tar.gz` & `tmp/aissemble_foundation_model_training_api-1.7.0.dev1715156845.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1715156825.tar", max compression
+gzip compressed data, was "aissemble_foundation_model_training_api-1.7.0.dev1715156845.tar", max compression
```

## Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825.tar` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-05-08 08:26:48.240067 aissemble_foundation_model_training_api-1.7.0.dev1715156825/LICENSE
--rw-r--r--   0        0        0      318 2024-05-08 08:12:08.903494 aissemble_foundation_model_training_api-1.7.0.dev1715156825/LICENSE.txt
--rw-r--r--   0        0        0     1796 2024-05-08 08:12:08.903494 aissemble_foundation_model_training_api-1.7.0.dev1715156825/README.md
--rw-r--r--   0        0        0      859 2024-05-08 08:27:05.869597 aissemble_foundation_model_training_api-1.7.0.dev1715156825/pyproject.toml
--rw-r--r--   0        0        0     6779 2024-05-08 08:12:08.903494 aissemble_foundation_model_training_api-1.7.0.dev1715156825/src/model_training_api/model_training_api.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1715156825/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 08:27:04.604872 aissemble_foundation_model_training_api-1.7.0.dev1715156845/LICENSE
+-rw-r--r--   0        0        0      318 2024-05-08 08:12:12.930270 aissemble_foundation_model_training_api-1.7.0.dev1715156845/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2024-05-08 08:12:12.930270 aissemble_foundation_model_training_api-1.7.0.dev1715156845/README.md
+-rw-r--r--   0        0        0      859 2024-05-08 08:27:25.472862 aissemble_foundation_model_training_api-1.7.0.dev1715156845/pyproject.toml
+-rw-r--r--   0        0        0     6779 2024-05-08 08:12:12.931270 aissemble_foundation_model_training_api-1.7.0.dev1715156845/src/model_training_api/model_training_api.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 aissemble_foundation_model_training_api-1.7.0.dev1715156845/PKG-INFO
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825/LICENSE` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825/README.md` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825/pyproject.toml` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-model-training-api"
-version = "1.7.0.dev1715156825"
+version = "1.7.0.dev1715156845"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api", from = "src"},
 ]
```

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825/src/model_training_api/model_training_api.py` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845/src/model_training_api/model_training_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_training_api-1.7.0.dev1715156825/PKG-INFO` & `aissemble_foundation_model_training_api-1.7.0.dev1715156845/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-model-training-api
-Version: 1.7.0.dev1715156825
+Version: 1.7.0.dev1715156845
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: aissemble-foundation-messaging-python (==1.7.0.*)
 Requires-Dist: fastapi (>=0.95.0)
```

