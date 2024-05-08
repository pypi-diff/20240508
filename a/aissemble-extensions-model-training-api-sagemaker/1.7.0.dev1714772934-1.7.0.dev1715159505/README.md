# Comparing `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934.tar.gz` & `tmp/aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934.tar", max compression
+gzip compressed data, was "aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar", max compression
```

## Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934.tar` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9580 2024-05-03 21:48:15.829891 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/LICENSE
--rw-r--r--   0        0        0        0 2024-05-03 20:59:00.548692 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/README.md
--rw-r--r--   0        0        0      791 2024-05-03 21:48:54.848847 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/pyproject.toml
--rw-r--r--   0        0        0     8837 2024-05-03 20:59:00.548692 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/src/model_training_api_sagemaker/model_training_api_sagemaker.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 09:11:05.300400 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-08 08:12:12.864270 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/README.md
+-rw-r--r--   0        0        0      781 2024-05-08 09:11:46.146405 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/pyproject.toml
+-rw-r--r--   0        0        0     8837 2024-05-08 08:12:12.864270 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/src/model_training_api_sagemaker/model_training_api_sagemaker.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/PKG-INFO
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/LICENSE` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/pyproject.toml` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-model-training-api-sagemaker"
-version = "1.7.0.dev1714772934"
+version = "1.7.0.dev1715159505"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_training_api_sagemaker", from = "src"},
 ]
 
@@ -12,15 +12,15 @@
 python = ">=3.11.4, <3.12"
 fastapi = ">=0.95.0"
 uvicorn = {version = "^0.18.0", extras = ["standard"]}
 pydantic = ">=1.8.0,<2.0.0"
 kubernetes = ">=26.1.0"
 urllib3 = "^1.26.18"
 krausening = ">=19"
-sagemaker = ">2.173.0, <=2.182.0"
+sagemaker = ">=2.218.0"
 mlflow = "^2.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.1.0"
 behave = ">=1.2.6"
 nose = ">=1.3.7"
 setuptools = "^69.0.3"
```

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/src/model_training_api_sagemaker/model_training_api_sagemaker.py` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/src/model_training_api_sagemaker/model_training_api_sagemaker.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1714772934/PKG-INFO` & `aissemble_extensions_model_training_api_sagemaker-1.7.0.dev1715159505/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-model-training-api-sagemaker
-Version: 1.7.0.dev1714772934
+Version: 1.7.0.dev1715159505
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: krausening (>=19)
 Requires-Dist: kubernetes (>=26.1.0)
 Requires-Dist: mlflow (>=2.3.1,<3.0.0)
 Requires-Dist: pydantic (>=1.8.0,<2.0.0)
-Requires-Dist: sagemaker (>2.173.0,<=2.182.0)
+Requires-Dist: sagemaker (>=2.218.0)
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Requires-Dist: uvicorn[standard] (>=0.18.0,<0.19.0)
 Description-Content-Type: text/markdown
```

