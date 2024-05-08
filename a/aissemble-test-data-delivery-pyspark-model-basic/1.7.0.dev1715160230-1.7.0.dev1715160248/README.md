# Comparing `tmp/aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230.tar.gz` & `tmp/aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230.tar", max compression
+gzip compressed data, was "aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248.tar", max compression
```

## Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230.tar` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     9580 2024-05-08 09:23:28.949292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/LICENSE
--rw-r--r--   0        0        0     1827 2024-05-08 09:23:51.048708 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-08 09:23:28.939292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:23:28.899293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py.tmp
--rw-r--r--   0        0        0     1007 2024-05-08 09:23:28.939292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py
--rw-r--r--   0        0        0      799 2024-05-08 09:23:28.889293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp
--rw-r--r--   0        0        0      818 2024-05-08 09:23:28.929292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py
--rw-r--r--   0        0        0      610 2024-05-08 09:23:28.879294 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:23:28.919293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:23:28.879294 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py.tmp
--rw-r--r--   0        0        0     3938 2024-05-08 09:23:28.919293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py
--rw-r--r--   0        0        0     3730 2024-05-08 09:23:28.879294 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp
--rw-r--r--   0        0        0      670 2024-05-08 09:23:28.929292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py
--rw-r--r--   0        0        0      462 2024-05-08 09:23:28.889293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py.tmp
--rw-r--r--   0        0        0     1902 2024-05-08 09:23:28.929292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py
--rw-r--r--   0        0        0     1694 2024-05-08 09:23:28.899293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp
--rw-r--r--   0        0        0     1865 2024-05-08 09:23:28.929292 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py
--rw-r--r--   0        0        0     1657 2024-05-08 09:23:28.909293 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp
--rw-r--r--   0        0        0      602 2024-05-08 08:12:09.063490 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 09:23:46.640631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/LICENSE
+-rw-r--r--   0        0        0     1827 2024-05-08 09:24:09.383639 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-08 09:23:46.620631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:23:46.575631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/__init__.py.tmp
+-rw-r--r--   0        0        0     1007 2024-05-08 09:23:46.620631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py
+-rw-r--r--   0        0        0      799 2024-05-08 09:23:46.574631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp
+-rw-r--r--   0        0        0      818 2024-05-08 09:23:46.618631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py
+-rw-r--r--   0        0        0      610 2024-05-08 09:23:46.561631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:23:46.608631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:23:46.553631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/__init__.py.tmp
+-rw-r--r--   0        0        0     3938 2024-05-08 09:23:46.607631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py
+-rw-r--r--   0        0        0     3730 2024-05-08 09:23:46.552631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp
+-rw-r--r--   0        0        0      670 2024-05-08 09:23:46.610631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py
+-rw-r--r--   0        0        0      462 2024-05-08 09:23:46.574631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py.tmp
+-rw-r--r--   0        0        0     1902 2024-05-08 09:23:46.613631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py
+-rw-r--r--   0        0        0     1694 2024-05-08 09:23:46.579631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp
+-rw-r--r--   0        0        0     1865 2024-05-08 09:23:46.616631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py
+-rw-r--r--   0        0        0     1657 2024-05-08 09:23:46.591631 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp
+-rw-r--r--   0        0        0      602 2024-05-08 08:12:13.148269 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/PKG-INFO
```

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/LICENSE` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/pyproject.toml` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 
 [tool.poetry]
 name = "aissemble-test-data-delivery-pyspark-model-basic"
-version = "1.7.0.dev1715160230"
+version = "1.7.0.dev1715160248"
 description = "Pyspark test module"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_test_data_delivery_pyspark_model_basic/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/environment_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/pipeline/pipeline_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_data_action.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/abstract_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_async_step_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/generated/step/example_sync_step_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/src/aissemble_test_data_delivery_pyspark_model_basic/resources/pipelines/PysparkDataDeliveryBasic.json`

 * *Files identical despite different names*

### Comparing `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160230/PKG-INFO` & `aissemble_test_data_delivery_pyspark_model_basic-1.7.0.dev1715160248/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-test-data-delivery-pyspark-model-basic
-Version: 1.7.0.dev1715160230
+Version: 1.7.0.dev1715160248
 Summary: Pyspark test module
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-extensions-data-delivery-spark-py (==1.7.0.*)
```

