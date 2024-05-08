# Comparing `tmp/strangeworks-0.5.8.tar.gz` & `tmp/strangeworks-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks-0.5.8.tar", max compression
+gzip compressed data, was "strangeworks-0.5.9.tar", max compression
```

## Comparing `strangeworks-0.5.8.tar` & `strangeworks-0.5.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      222 2024-04-22 20:45:06.511352 strangeworks-0.5.8/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2024-04-22 20:45:06.511352 strangeworks-0.5.8/LICENSE
--rw-r--r--   0        0        0      818 2024-04-22 20:45:19.271413 strangeworks-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      981 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/__init__.py
--rw-r--r--   0        0        0       19 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/__init__.py
--rw-r--r--   0        0        0      558 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/auth.py
--rw-r--r--   0        0        0     2883 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/backends.py
--rw-r--r--   0        0        0    16008 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/experiments.py
--rw-r--r--   0        0        0     5494 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/file.py
--rw-r--r--   0        0        0     6411 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/jobs.py
--rw-r--r--   0        0        0     1571 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/resource.py
--rw-r--r--   0        0        0    11287 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/rest_client.py
--rw-r--r--   0        0        0     3275 2024-04-22 20:45:06.511352 strangeworks-0.5.8/strangeworks/core/client/transport.py
--rw-r--r--   0        0        0     1056 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/client/workspace.py
--rw-r--r--   0        0        0        0 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/__init__.py
--rw-r--r--   0        0        0     1640 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/base.py
--rw-r--r--   0        0        0     5604 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/config.py
--rw-r--r--   0        0        0      876 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/defaults.py
--rw-r--r--   0        0        0     1611 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/env.py
--rw-r--r--   0        0        0     6719 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/config/file.py
--rw-r--r--   0        0        0       17 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/errors/__init__.py
--rw-r--r--   0        0        0     2614 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/errors/error.py
--rw-r--r--   0        0        0      714 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/core/utils.py
--rw-r--r--   0        0        0      475 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/platform/gql.py
--rw-r--r--   0        0        0    31966 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/sw_client.py
--rw-r--r--   0        0        0      323 2024-04-22 20:45:06.515352 strangeworks-0.5.8/strangeworks/utils.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 strangeworks-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      222 2024-05-08 20:27:09.234878 strangeworks-0.5.9/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2024-05-08 20:27:09.234878 strangeworks-0.5.9/LICENSE
+-rw-r--r--   0        0        0      819 2024-05-08 20:27:20.674953 strangeworks-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      981 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/__init__.py
+-rw-r--r--   0        0        0      558 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/auth.py
+-rw-r--r--   0        0        0     2883 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/backends.py
+-rw-r--r--   0        0        0    16008 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/experiments.py
+-rw-r--r--   0        0        0     5494 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/file.py
+-rw-r--r--   0        0        0     6411 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/jobs.py
+-rw-r--r--   0        0        0     1571 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/resource.py
+-rw-r--r--   0        0        0    11287 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/rest_client.py
+-rw-r--r--   0        0        0     3275 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/transport.py
+-rw-r--r--   0        0        0     1056 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/client/workspace.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:27:09.234878 strangeworks-0.5.9/strangeworks/core/config/__init__.py
+-rw-r--r--   0        0        0     1640 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/config/base.py
+-rw-r--r--   0        0        0     5604 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/config/config.py
+-rw-r--r--   0        0        0      876 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/config/defaults.py
+-rw-r--r--   0        0        0     1168 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/config/env.py
+-rw-r--r--   0        0        0     6719 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/config/file.py
+-rw-r--r--   0        0        0       17 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/errors/__init__.py
+-rw-r--r--   0        0        0     2614 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/errors/error.py
+-rw-r--r--   0        0        0      714 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/core/utils.py
+-rw-r--r--   0        0        0      475 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/platform/gql.py
+-rw-r--r--   0        0        0    31966 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/sw_client.py
+-rw-r--r--   0        0        0      323 2024-05-08 20:27:09.238879 strangeworks-0.5.9/strangeworks/utils.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 strangeworks-0.5.9/PKG-INFO
```

### Comparing `strangeworks-0.5.8/LICENSE` & `strangeworks-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/pyproject.toml` & `strangeworks-0.5.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "strangeworks"
-version = "0.5.8"
+version = "0.5.9"
 description = "Strangeworks Python SDK"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.30.0"
 pyyaml = "^6.0.0"
 tomlkit = "^0.11.1"
 gql = "^3.4.1"
 requests-toolbelt = "^1.0.0"
-strangeworks-core = "^0.3.5"
+strangeworks-core = "^0.3.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
 flake8-docstrings = "^1.6.0"
```

### Comparing `strangeworks-0.5.8/strangeworks/__init__.py` & `strangeworks-0.5.9/strangeworks/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/auth.py` & `strangeworks-0.5.9/strangeworks/core/client/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/backends.py` & `strangeworks-0.5.9/strangeworks/core/client/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/experiments.py` & `strangeworks-0.5.9/strangeworks/core/client/experiments.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/file.py` & `strangeworks-0.5.9/strangeworks/core/client/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/jobs.py` & `strangeworks-0.5.9/strangeworks/core/client/jobs.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/resource.py` & `strangeworks-0.5.9/strangeworks/core/client/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/rest_client.py` & `strangeworks-0.5.9/strangeworks/core/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/transport.py` & `strangeworks-0.5.9/strangeworks/core/client/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/client/workspace.py` & `strangeworks-0.5.9/strangeworks/core/client/workspace.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/config/base.py` & `strangeworks-0.5.9/strangeworks/core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/config/config.py` & `strangeworks-0.5.9/strangeworks/core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/config/defaults.py` & `strangeworks-0.5.9/strangeworks/core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/config/file.py` & `strangeworks-0.5.9/strangeworks/core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/errors/error.py` & `strangeworks-0.5.9/strangeworks/core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/core/utils.py` & `strangeworks-0.5.9/strangeworks/core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/strangeworks/sw_client.py` & `strangeworks-0.5.9/strangeworks/sw_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.8/PKG-INFO` & `strangeworks-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: strangeworks
-Version: 0.5.8
+Version: 0.5.9
 Summary: Strangeworks Python SDK
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
-Requires-Dist: strangeworks-core (>=0.3.5,<0.4.0)
+Requires-Dist: strangeworks-core (>=0.3.12,<0.4.0)
 Requires-Dist: tomlkit (>=0.11.1,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Strangeworks SDK
 
 The Strangeworks Python SDK grants easy access to the Strangeworks API. For more information on using the SDK check out the [Strangeworks docs](https://docs.strangeworks.com/tools/strangeworks-python).
```

