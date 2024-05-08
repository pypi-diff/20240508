# Comparing `tmp/strangeworks_core-0.3.8.tar.gz` & `tmp/strangeworks_core-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.3.8.tar", max compression
+gzip compressed data, was "strangeworks_core-0.3.9.tar", max compression
```

## Comparing `strangeworks_core-0.3.8.tar` & `strangeworks_core-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      655 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/README.md
--rw-r--r--   0        0        0      923 2024-02-13 19:07:56.593371 strangeworks_core-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      109 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/strangeworks_core/batch/__init__.py
--rw-r--r--   0        0        0    22901 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/strangeworks_core/batch/utils.py
--rw-r--r--   0        0        0       53 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2024-02-13 19:07:41.353266 strangeworks_core-0.3.8/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3415 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      979 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     4421 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6289 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     4609 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4991 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3532 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0      817 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/base.py
--rw-r--r--   0        0        0      571 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/batch.py
--rw-r--r--   0        0        0     1687 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/file.py
--rw-r--r--   0        0        0      798 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/func.py
--rw-r--r--   0        0        0     6344 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/job.py
--rw-r--r--   0        0        0      736 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/machine.py
--rw-r--r--   0        0        0      976 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2458 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2024-02-13 19:07:41.357266 strangeworks_core-0.3.8/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 strangeworks_core-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      655 2024-04-22 20:43:40.199322 strangeworks_core-0.3.9/README.md
+-rw-r--r--   0        0        0      923 2024-04-22 20:44:10.123299 strangeworks_core-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    22901 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       53 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3415 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      979 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     4421 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6289 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     4609 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4991 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3532 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0      817 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/base.py
+-rw-r--r--   0        0        0      571 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/batch.py
+-rw-r--r--   0        0        0     1687 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      798 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     6344 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      736 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0      976 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2458 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2024-04-22 20:43:40.203322 strangeworks_core-0.3.9/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 strangeworks_core-0.3.9/PKG-INFO
```

### Comparing `strangeworks_core-0.3.8/README.md` & `strangeworks_core-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/pyproject.toml` & `strangeworks_core-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.3.8"
+version = "0.3.9"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{ include = "strangeworks_core" }]
 license = "Apache-2.0"
```

### Comparing `strangeworks_core-0.3.8/strangeworks_core/batch/utils.py` & `strangeworks_core-0.3.9/strangeworks_core/batch/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/config/base.py` & `strangeworks_core-0.3.9/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/config/config.py` & `strangeworks_core-0.3.9/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/config/defaults.py` & `strangeworks_core-0.3.9/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/config/env.py` & `strangeworks_core-0.3.9/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/config/file.py` & `strangeworks_core-0.3.9/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/errors/error.py` & `strangeworks_core-0.3.9/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/platform/auth.py` & `strangeworks_core-0.3.9/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/platform/gql.py` & `strangeworks_core-0.3.9/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.3.9/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/platform/transport.py` & `strangeworks_core-0.3.9/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/backend.py` & `strangeworks_core-0.3.9/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/base.py` & `strangeworks_core-0.3.9/strangeworks_core/types/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/batch.py` & `strangeworks_core-0.3.9/strangeworks_core/types/batch.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/file.py` & `strangeworks_core-0.3.9/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/func.py` & `strangeworks_core-0.3.9/strangeworks_core/types/func.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/job.py` & `strangeworks_core-0.3.9/strangeworks_core/types/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/machine.py` & `strangeworks_core-0.3.9/strangeworks_core/types/machine.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/product.py` & `strangeworks_core-0.3.9/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/types/resource.py` & `strangeworks_core-0.3.9/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/strangeworks_core/utils.py` & `strangeworks_core-0.3.9/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.3.8/PKG-INFO` & `strangeworks_core-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.3.8
+Version: 0.3.9
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

