# Comparing `tmp/uhura-2.2.1.tar.gz` & `tmp/uhura-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uhura-2.2.1.tar", last modified: Thu Feb 29 14:25:26 2024, max compression
+gzip compressed data, was "uhura-2.2.2.tar", last modified: Wed May  8 17:14:56 2024, max compression
```

## Comparing `uhura-2.2.1.tar` & `uhura-2.2.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.936595 uhura-2.2.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.932595 uhura-2.2.1/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3027 2024-02-29 14:24:59.000000 uhura-2.2.1/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-02-29 14:24:59.000000 uhura-2.2.1/.coveragerc
--rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2024-02-29 14:24:59.000000 uhura-2.2.1/.flake8
--rw-r--r--   0 circleci  (3434) circleci  (3434)      236 2024-02-29 14:24:59.000000 uhura-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      256 2024-02-29 14:25:26.000000 uhura-2.2.1/AUTHORS
--rw-r--r--   0 circleci  (3434) circleci  (3434)      250 2024-02-29 14:24:59.000000 uhura-2.2.1/CODEOWNERS
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2024-02-29 14:25:26.000000 uhura-2.2.1/ChangeLog
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2024-02-29 14:24:59.000000 uhura-2.2.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17901 2024-02-29 14:25:26.936595 uhura-2.2.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14280 2024-02-29 14:24:59.000000 uhura-2.2.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2024-02-29 14:24:59.000000 uhura-2.2.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2024-02-29 14:24:59.000000 uhura-2.2.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1636 2024-02-29 14:25:26.936595 uhura-2.2.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-02-29 14:24:59.000000 uhura-2.2.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.932595 uhura-2.2.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9285 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_caches.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      784 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_comparison.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4855 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_decorables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1944 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_pandas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.932595 uhura-2.2.1/tests/test_properties/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_properties/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_properties/test_homomorphic_hash.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2591 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_properties/test_property_tester.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9615 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_properties/test_testable_properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1442 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_properties/test_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2024-02-29 14:24:59.000000 uhura-2.2.1/tests/test_serde.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.932595 uhura-2.2.1/uhura/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2572 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/caches.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2615 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/caching.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1559 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/comparison.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2497 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/composition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1312 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/decorables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/functional.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2333 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/modes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      741 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/pandas_tools.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.936595 uhura-2.2.1/uhura/properties/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/properties/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/properties/homomorphic_hash.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6492 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/properties/property_tester.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7511 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/properties/testable_properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3051 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/properties/transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2024-02-29 14:24:59.000000 uhura-2.2.1/uhura/serde.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-29 14:25:26.932595 uhura-2.2.1/uhura.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17901 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1116 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-29 14:25:16.000000 uhura-2.2.1/uhura.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/pbr.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1037 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-02-29 14:25:26.000000 uhura-2.2.1/uhura.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.980669 uhura-2.2.2/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.972669 uhura-2.2.2/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3766 2024-05-08 17:14:31.000000 uhura-2.2.2/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-05-08 17:14:31.000000 uhura-2.2.2/.coveragerc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2024-05-08 17:14:31.000000 uhura-2.2.2/.flake8
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      236 2024-05-08 17:14:31.000000 uhura-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      354 2024-05-08 17:14:56.000000 uhura-2.2.2/AUTHORS
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      250 2024-05-08 17:14:31.000000 uhura-2.2.2/CODEOWNERS
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2024-05-08 17:14:56.000000 uhura-2.2.2/ChangeLog
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2024-05-08 17:14:31.000000 uhura-2.2.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18032 2024-05-08 17:14:56.980669 uhura-2.2.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14403 2024-05-08 17:14:31.000000 uhura-2.2.2/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      444 2024-05-08 17:14:31.000000 uhura-2.2.2/codecov.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      174 2024-05-08 17:14:31.000000 uhura-2.2.2/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2024-05-08 17:14:31.000000 uhura-2.2.2/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1636 2024-05-08 17:14:56.984670 uhura-2.2.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2024-05-08 17:14:31.000000 uhura-2.2.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.976669 uhura-2.2.2/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9285 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_caches.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      784 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_comparison.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4855 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_decorables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_functional.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1944 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_pandas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.976669 uhura-2.2.2/tests/test_properties/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_properties/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_properties/test_homomorphic_hash.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2591 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_properties/test_property_tester.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9615 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_properties/test_testable_properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1442 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_properties/test_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2024-05-08 17:14:31.000000 uhura-2.2.2/tests/test_serde.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.980669 uhura-2.2.2/uhura/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2572 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/caches.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2615 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/caching.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1559 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/comparison.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2497 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/composition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1312 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/decorables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2812 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/functional.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2333 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/modes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      741 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/pandas_tools.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.980669 uhura-2.2.2/uhura/properties/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/properties/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/properties/homomorphic_hash.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6492 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/properties/property_tester.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7511 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/properties/testable_properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3051 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/properties/transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2024-05-08 17:14:31.000000 uhura-2.2.2/uhura/serde.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-08 17:14:56.980669 uhura-2.2.2/uhura.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18032 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1153 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-08 17:14:43.000000 uhura-2.2.2/uhura.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/pbr.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1037 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-05-08 17:14:56.000000 uhura-2.2.2/uhura.egg-info/top_level.txt
```

### Comparing `uhura-2.2.1/LICENSE` & `uhura-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/PKG-INFO` & `uhura-2.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: uhura
-Version: 2.2.1
+Version: 2.2.2
 Summary: Wrapper code for cleaning up IO
 Home-page: UNKNOWN
 Author: Declan Crew
 Author-email: declan.crew@vortexa.com
 License: MIT
 Description: # Uhura  
-          
+        [![codecov](https://codecov.io/gh/VorTECHsa/uhura/graph/badge.svg?token=hRFNDYtArs)](https://codecov.io/gh/VorTECHsa/uhura)
+        d
         A framework for tackling legacy data engineering code.  
           
         Wrap inputs and outputs for your system and take advantage of asyncio + automated testing.  
           
         Uhura makes it easy to run pipelines in a specific "mode". Modes are implemented using context managers and are stored in the `modes` module. Right now Uhura supports two main use cases:  
         1. A testing mode used to run a pipeline and compare its output against pre-generated fixtures. This is executed through the `fixture_builder_mode` and the `task_test_mode` contexts.  
         2. A mode used for testing whether functions respect specific properties. This is executed through the `test_transformers` context.
```

### Comparing `uhura-2.2.1/README.md` & `uhura-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Uhura  
-  
+[![codecov](https://codecov.io/gh/VorTECHsa/uhura/graph/badge.svg?token=hRFNDYtArs)](https://codecov.io/gh/VorTECHsa/uhura)
+d
 A framework for tackling legacy data engineering code.  
   
 Wrap inputs and outputs for your system and take advantage of asyncio + automated testing.  
   
 Uhura makes it easy to run pipelines in a specific "mode". Modes are implemented using context managers and are stored in the `modes` module. Right now Uhura supports two main use cases:  
 1. A testing mode used to run a pipeline and compare its output against pre-generated fixtures. This is executed through the `fixture_builder_mode` and the `task_test_mode` contexts.  
 2. A mode used for testing whether functions respect specific properties. This is executed through the `test_transformers` context.
```

### Comparing `uhura-2.2.1/setup.cfg` & `uhura-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_caches.py` & `uhura-2.2.2/tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_comparison.py` & `uhura-2.2.2/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_decorables.py` & `uhura-2.2.2/tests/test_decorables.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_pandas.py` & `uhura-2.2.2/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_properties/test_homomorphic_hash.py` & `uhura-2.2.2/tests/test_properties/test_homomorphic_hash.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_properties/test_property_tester.py` & `uhura-2.2.2/tests/test_properties/test_property_tester.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_properties/test_testable_properties.py` & `uhura-2.2.2/tests/test_properties/test_testable_properties.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_properties/test_transformer.py` & `uhura-2.2.2/tests/test_properties/test_transformer.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/tests/test_serde.py` & `uhura-2.2.2/tests/test_serde.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/base.py` & `uhura-2.2.2/uhura/base.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/caches.py` & `uhura-2.2.2/uhura/caches.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/caching.py` & `uhura-2.2.2/uhura/caching.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/comparison.py` & `uhura-2.2.2/uhura/comparison.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/composition.py` & `uhura-2.2.2/uhura/composition.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/decorables.py` & `uhura-2.2.2/uhura/decorables.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/functional.py` & `uhura-2.2.2/uhura/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             self.params = signature.bind(*args, **kwargs)
 
         @match_function_type(function)
         def read(self):
             return function(*self.params.args, **self.params.kwargs)
 
         def cache_key(self):
-            return function.__qualname__
+            return function.__qualname__ + ".pkl"
 
     @wraps(function)
     @match_function_type(function)
     def wrapped(*args, **kwargs):
         return _SingleFunctionReadable(*args, **kwargs).read()
 
     return wrapped
@@ -66,15 +66,15 @@
 
         @match_function_type(function)
         def write(self, obj):
             self.params.arguments[output_arg] = obj
             return function(*self.params.args, **self.params.kwargs)
 
         def cache_key(self):
-            return function.__qualname__
+            return function.__qualname__ + ".pkl"
 
     @wraps(function)
     @match_function_type(function)
     def wrapped(*args, **kwargs):
         bound = signature.bind(*args, **kwargs)
         if output_arg:
             written_arg = bound.arguments[output_arg]
```

### Comparing `uhura-2.2.1/uhura/modes.py` & `uhura-2.2.2/uhura/modes.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/pandas_tools.py` & `uhura-2.2.2/uhura/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/properties/homomorphic_hash.py` & `uhura-2.2.2/uhura/properties/homomorphic_hash.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/properties/property_tester.py` & `uhura-2.2.2/uhura/properties/property_tester.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/properties/testable_properties.py` & `uhura-2.2.2/uhura/properties/testable_properties.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/properties/transformer.py` & `uhura-2.2.2/uhura/properties/transformer.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura/serde.py` & `uhura-2.2.2/uhura/serde.py`

 * *Files identical despite different names*

### Comparing `uhura-2.2.1/uhura.egg-info/PKG-INFO` & `uhura-2.2.2/uhura.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: uhura
-Version: 2.2.1
+Version: 2.2.2
 Summary: Wrapper code for cleaning up IO
 Home-page: UNKNOWN
 Author: Declan Crew
 Author-email: declan.crew@vortexa.com
 License: MIT
 Description: # Uhura  
-          
+        [![codecov](https://codecov.io/gh/VorTECHsa/uhura/graph/badge.svg?token=hRFNDYtArs)](https://codecov.io/gh/VorTECHsa/uhura)
+        d
         A framework for tackling legacy data engineering code.  
           
         Wrap inputs and outputs for your system and take advantage of asyncio + automated testing.  
           
         Uhura makes it easy to run pipelines in a specific "mode". Modes are implemented using context managers and are stored in the `modes` module. Right now Uhura supports two main use cases:  
         1. A testing mode used to run a pipeline and compare its output against pre-generated fixtures. This is executed through the `fixture_builder_mode` and the `task_test_mode` contexts.  
         2. A mode used for testing whether functions respect specific properties. This is executed through the `test_transformers` context.
```

### Comparing `uhura-2.2.1/uhura.egg-info/SOURCES.txt` & `uhura-2.2.2/uhura.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 .flake8
 .pre-commit-config.yaml
 AUTHORS
 CODEOWNERS
 ChangeLog
 LICENSE
 README.md
+codecov.yml
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .circleci/config.yml
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
 tests/test_caches.py
 tests/test_comparison.py
 tests/test_decorables.py
+tests/test_functional.py
 tests/test_pandas.py
 tests/test_serde.py
 tests/test_properties/__init__.py
 tests/test_properties/test_homomorphic_hash.py
 tests/test_properties/test_property_tester.py
 tests/test_properties/test_testable_properties.py
 tests/test_properties/test_transformer.py
```

### Comparing `uhura-2.2.1/uhura.egg-info/requires.txt` & `uhura-2.2.2/uhura.egg-info/requires.txt`

 * *Files identical despite different names*

