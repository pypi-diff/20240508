# Comparing `tmp/aissemble_machine_learning_training-1.7.0.dev1715160270.tar.gz` & `tmp/aissemble_machine_learning_training-1.7.0.dev1715160290.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_machine_learning_training-1.7.0.dev1715160270.tar", max compression
+gzip compressed data, was "aissemble_machine_learning_training-1.7.0.dev1715160290.tar", max compression
```

## Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270.tar` & `aissemble_machine_learning_training-1.7.0.dev1715160290.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     9580 2024-05-08 09:24:04.778344 aissemble_machine_learning_training-1.7.0.dev1715160270/LICENSE
--rw-r--r--   0        0        0     1725 2024-05-08 09:24:31.097645 aissemble_machine_learning_training-1.7.0.dev1715160270/pyproject.toml
--rw-r--r--   0        0        0      224 2024-05-08 09:24:04.758344 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:04.678346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/__init__.py.tmp
--rw-r--r--   0        0        0    16690 2024-05-08 09:24:04.758344 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py
--rw-r--r--   0        0        0    16465 2024-05-08 09:24:04.698346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp
--rw-r--r--   0        0        0     4725 2024-05-08 09:24:04.738345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py
--rw-r--r--   0        0        0     4501 2024-05-08 09:24:04.668347 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp
--rw-r--r--   0        0        0      224 2024-05-08 09:24:04.738345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:04.678346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/__init__.py.tmp
--rw-r--r--   0        0        0     1900 2024-05-08 09:24:04.758344 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py
--rw-r--r--   0        0        0     1676 2024-05-08 09:24:04.718345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp
--rw-r--r--   0        0        0     1956 2024-05-08 09:24:04.748345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py
--rw-r--r--   0        0        0     1732 2024-05-08 09:24:04.688346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp
--rw-r--r--   0        0        0     1641 2024-05-08 09:24:04.748345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py
--rw-r--r--   0        0        0     1417 2024-05-08 09:24:04.688346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp
--rw-r--r--   0        0        0     1984 2024-05-08 09:24:04.738345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py
--rw-r--r--   0        0        0     1760 2024-05-08 09:24:04.688346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp
--rw-r--r--   0        0        0     2002 2024-05-08 09:24:04.738345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py
--rw-r--r--   0        0        0     1778 2024-05-08 09:24:04.688346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp
--rw-r--r--   0        0        0     4836 2024-05-08 09:24:04.748345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py
--rw-r--r--   0        0        0     4612 2024-05-08 09:24:04.708346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp
--rw-r--r--   0        0        0     4294 2024-05-08 09:24:04.748345 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py
--rw-r--r--   0        0        0     4070 2024-05-08 09:24:04.708346 aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 aissemble_machine_learning_training-1.7.0.dev1715160270/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 09:24:24.220643 aissemble_machine_learning_training-1.7.0.dev1715160290/LICENSE
+-rw-r--r--   0        0        0     1725 2024-05-08 09:24:50.589658 aissemble_machine_learning_training-1.7.0.dev1715160290/pyproject.toml
+-rw-r--r--   0        0        0      224 2024-05-08 09:24:24.199643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:24:24.110643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/__init__.py.tmp
+-rw-r--r--   0        0        0    16690 2024-05-08 09:24:24.203643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py
+-rw-r--r--   0        0        0    16465 2024-05-08 09:24:24.130643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp
+-rw-r--r--   0        0        0     4725 2024-05-08 09:24:24.177643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0     4501 2024-05-08 09:24:24.099644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp
+-rw-r--r--   0        0        0      224 2024-05-08 09:24:24.178644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:24:24.109644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/__init__.py.tmp
+-rw-r--r--   0        0        0     1900 2024-05-08 09:24:24.199643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py
+-rw-r--r--   0        0        0     1676 2024-05-08 09:24:24.150643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0     1956 2024-05-08 09:24:24.187643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py
+-rw-r--r--   0        0        0     1732 2024-05-08 09:24:24.119644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp
+-rw-r--r--   0        0        0     1641 2024-05-08 09:24:24.189643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py
+-rw-r--r--   0        0        0     1417 2024-05-08 09:24:24.121643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp
+-rw-r--r--   0        0        0     1984 2024-05-08 09:24:24.184643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py
+-rw-r--r--   0        0        0     1760 2024-05-08 09:24:24.116644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp
+-rw-r--r--   0        0        0     2002 2024-05-08 09:24:24.182644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py
+-rw-r--r--   0        0        0     1778 2024-05-08 09:24:24.113644 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp
+-rw-r--r--   0        0        0     4836 2024-05-08 09:24:24.197643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py
+-rw-r--r--   0        0        0     4612 2024-05-08 09:24:24.146643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0     4294 2024-05-08 09:24:24.193643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py
+-rw-r--r--   0        0        0     4070 2024-05-08 09:24:24.141643 aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 aissemble_machine_learning_training-1.7.0.dev1715160290/PKG-INFO
```

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/LICENSE` & `aissemble_machine_learning_training-1.7.0.dev1715160290/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/pyproject.toml` & `aissemble_machine_learning_training-1.7.0.dev1715160290/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 # Originally generated from templates/general-mlflow/pyproject.toml.vm.
 
 [tool.poetry]
 name = "aissemble-machine-learning-training"
-version = "1.7.0.dev1715160270"
+version = "1.7.0.dev1715160290"
 description = "Description of package"
 authors = ["Your Name <you@example.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_machine_learning_training/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/example_machine_learning_pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/pipeline/pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/custom_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_custom_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_freeform_post_action_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_keras_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/example_onnx_sklearn_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_keras_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp` & `aissemble_machine_learning_training-1.7.0.dev1715160290/src/aissemble_machine_learning_training/generated/post_action/onnx_sklearn_model_conversion_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_training-1.7.0.dev1715160270/PKG-INFO` & `aissemble_machine_learning_training-1.7.0.dev1715160290/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-machine-learning-training
-Version: 1.7.0.dev1715160270
+Version: 1.7.0.dev1715160290
 Summary: Description of package
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-core-python (==1.7.0.*)
```

