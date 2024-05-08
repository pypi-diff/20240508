# Comparing `tmp/pytest_batch_regression-0.1.3.tar.gz` & `tmp/pytest_batch_regression-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_batch_regression-0.1.3.tar", last modified: Wed May  8 10:23:29 2024, max compression
+gzip compressed data, was "pytest_batch_regression-0.1.4.tar", last modified: Wed May  8 10:37:21 2024, max compression
```

## Comparing `pytest_batch_regression-0.1.3.tar` & `pytest_batch_regression-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:23:29.609117 pytest_batch_regression-0.1.3/
--rw-rw-r--   0 vipul     (1000) vipul     (1000)      520 2024-05-08 05:59:46.000000 pytest_batch_regression-0.1.3/LICENSE
--rw-r--r--   0 vipul     (1000) vipul     (1000)      920 2024-05-08 10:23:29.609117 pytest_batch_regression-0.1.3/PKG-INFO
--rw-rw-r--   0 vipul     (1000) vipul     (1000)      218 2024-05-08 07:16:48.000000 pytest_batch_regression-0.1.3/README.md
-drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:23:29.609117 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/
--rw-r--r--   0 vipul     (1000) vipul     (1000)      920 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/PKG-INFO
--rw-rw-r--   0 vipul     (1000) vipul     (1000)      368 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/SOURCES.txt
--rw-rw-r--   0 vipul     (1000) vipul     (1000)        1 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/dependency_links.txt
--rw-rw-r--   0 vipul     (1000) vipul     (1000)       56 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/entry_points.txt
--rw-rw-r--   0 vipul     (1000) vipul     (1000)       14 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/requires.txt
--rw-rw-r--   0 vipul     (1000) vipul     (1000)       18 2024-05-08 10:23:29.000000 pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/top_level.txt
-drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:23:29.609117 pytest_batch_regression-0.1.3/pytest_regression/
--rw-rw-r--   0 vipul     (1000) vipul     (1000)        0 2024-05-08 05:51:51.000000 pytest_batch_regression-0.1.3/pytest_regression/__init__.py
--rw-rw-r--   0 vipul     (1000) vipul     (1000)     1076 2024-05-08 10:23:07.000000 pytest_batch_regression-0.1.3/pytest_regression/plugin.py
--rw-rw-r--   0 vipul     (1000) vipul     (1000)       38 2024-05-08 10:23:29.609117 pytest_batch_regression-0.1.3/setup.cfg
--rw-rw-r--   0 vipul     (1000) vipul     (1000)      990 2024-05-08 10:23:19.000000 pytest_batch_regression-0.1.3/setup.py
+drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:37:21.962910 pytest_batch_regression-0.1.4/
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)      520 2024-05-08 05:59:46.000000 pytest_batch_regression-0.1.4/LICENSE
+-rw-r--r--   0 vipul     (1000) vipul     (1000)      920 2024-05-08 10:37:21.962910 pytest_batch_regression-0.1.4/PKG-INFO
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)      218 2024-05-08 07:16:48.000000 pytest_batch_regression-0.1.4/README.md
+drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:37:21.962910 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/
+-rw-r--r--   0 vipul     (1000) vipul     (1000)      920 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/PKG-INFO
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)      368 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/SOURCES.txt
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)        1 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/dependency_links.txt
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)       56 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/entry_points.txt
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)       14 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/requires.txt
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)       18 2024-05-08 10:37:21.000000 pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/top_level.txt
+drwxrwxr-x   0 vipul     (1000) vipul     (1000)        0 2024-05-08 10:37:21.962910 pytest_batch_regression-0.1.4/pytest_regression/
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)        0 2024-05-08 05:51:51.000000 pytest_batch_regression-0.1.4/pytest_regression/__init__.py
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)     1076 2024-05-08 10:23:07.000000 pytest_batch_regression-0.1.4/pytest_regression/plugin.py
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)       38 2024-05-08 10:37:21.962910 pytest_batch_regression-0.1.4/setup.cfg
+-rw-rw-r--   0 vipul     (1000) vipul     (1000)      990 2024-05-08 10:37:01.000000 pytest_batch_regression-0.1.4/setup.py
```

### Comparing `pytest_batch_regression-0.1.3/LICENSE` & `pytest_batch_regression-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_batch_regression-0.1.3/PKG-INFO` & `pytest_batch_regression-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-batch-regression
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytest plugin to repeat the entire test suite in batches.
 Home-page: https://github.com/Renzai777/pytest-regression/blob/master/calculator.py
 Author: Vipul Singh
 Author-email: vipulsingh161@gmail.com
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytest_batch_regression-0.1.3/pytest_batch_regression.egg-info/PKG-INFO` & `pytest_batch_regression-0.1.4/pytest_batch_regression.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-batch-regression
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytest plugin to repeat the entire test suite in batches.
 Home-page: https://github.com/Renzai777/pytest-regression/blob/master/calculator.py
 Author: Vipul Singh
 Author-email: vipulsingh161@gmail.com
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytest_batch_regression-0.1.3/pytest_regression/plugin.py` & `pytest_batch_regression-0.1.4/pytest_regression/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_batch_regression-0.1.3/setup.py` & `pytest_batch_regression-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="pytest-batch-regression",
-    version="0.1.3",
+    version="0.1.4",
     description="A pytest plugin to repeat the entire test suite in batches.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Vipul Singh",
     author_email="vipulsingh161@gmail.com",
     url="https://github.com/Renzai777/pytest-regression/blob/master/calculator.py",
     packages=find_packages(),
```

