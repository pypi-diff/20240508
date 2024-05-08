# Comparing `tmp/funcnodes_sklearn-0.1.2.tar.gz` & `tmp/funcnodes_sklearn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_sklearn-0.1.2.tar", max compression
+gzip compressed data, was "funcnodes_sklearn-0.1.3.tar", max compression
```

## Comparing `funcnodes_sklearn-0.1.2.tar` & `funcnodes_sklearn-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      756 2024-05-08 07:16:34.090473 funcnodes_sklearn-0.1.2/funcnodes_sklearn/__init__.py
--rw-r--r--   0        0        0   229607 2024-04-24 08:58:59.562515 funcnodes_sklearn-0.1.2/funcnodes_sklearn/_utils.py
--rw-r--r--   0        0        0    12766 2024-05-08 07:10:08.759985 funcnodes_sklearn-0.1.2/funcnodes_sklearn/calibration.py
--rw-r--r--   0        0        0   102351 2024-04-24 11:28:16.308084 funcnodes_sklearn-0.1.2/funcnodes_sklearn/cluster.py
--rw-r--r--   0        0        0    40551 2024-04-23 11:49:14.387966 funcnodes_sklearn-0.1.2/funcnodes_sklearn/covariance.py
--rw-r--r--   0        0        0    15614 2024-04-24 08:09:56.771355 funcnodes_sklearn-0.1.2/funcnodes_sklearn/cross_decomposition.py
--rw-r--r--   0        0        0   146000 2024-05-08 07:16:24.318939 funcnodes_sklearn-0.1.2/funcnodes_sklearn/datasets.py
--rw-r--r--   0        0        0     8556 2024-05-08 07:13:03.834488 funcnodes_sklearn-0.1.2/funcnodes_sklearn/decomposition.py
--rw-r--r--   0        0        0      594 2024-05-08 07:16:38.756229 funcnodes_sklearn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 13:48:43.396597 funcnodes_sklearn-0.1.2/README.md
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 funcnodes_sklearn-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      756 2024-05-08 07:36:44.245253 funcnodes_sklearn-0.1.3/funcnodes_sklearn/__init__.py
+-rw-r--r--   0        0        0   229607 2024-04-24 08:58:59.562515 funcnodes_sklearn-0.1.3/funcnodes_sklearn/_utils.py
+-rw-r--r--   0        0        0    12766 2024-05-08 07:10:08.759985 funcnodes_sklearn-0.1.3/funcnodes_sklearn/calibration.py
+-rw-r--r--   0        0        0   102351 2024-04-24 11:28:16.308084 funcnodes_sklearn-0.1.3/funcnodes_sklearn/cluster.py
+-rw-r--r--   0        0        0    40551 2024-04-23 11:49:14.387966 funcnodes_sklearn-0.1.3/funcnodes_sklearn/covariance.py
+-rw-r--r--   0        0        0    15614 2024-04-24 08:09:56.771355 funcnodes_sklearn-0.1.3/funcnodes_sklearn/cross_decomposition.py
+-rw-r--r--   0        0        0   146000 2024-05-08 07:16:24.318939 funcnodes_sklearn-0.1.3/funcnodes_sklearn/datasets.py
+-rw-r--r--   0        0        0     8556 2024-05-08 07:13:03.834488 funcnodes_sklearn-0.1.3/funcnodes_sklearn/decomposition.py
+-rw-r--r--   0        0        0      700 2024-05-08 07:36:36.605991 funcnodes_sklearn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 13:48:43.396597 funcnodes_sklearn-0.1.3/README.md
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 funcnodes_sklearn-0.1.3/PKG-INFO
```

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/__init__.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .covariance import COVARIANCE_NODE_SHELFE
 from .calibration import CALIBRATION_NODE_SHELFE
 from .cluster import CLUSTER_NODE_SHELFE
 from .cross_decomposition import CROSS_DECOMPOSITION_NODE_SHELFE
 from .datasets import DATASET_LOADER_NODE_SHELF
 from .decomposition import DECOMPOSITION_NODE_SHELFE
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 NODE_SHELF = fn.Shelf(
     name="sklearn",
     description="scikit-learn for funcnodes",
     nodes=[],
     subshelves=[
         CALIBRATION_NODE_SHELFE,
```

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/_utils.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/_utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/calibration.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/calibration.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/cluster.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/covariance.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/covariance.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/cross_decomposition.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/datasets.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/datasets.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/funcnodes_sklearn/decomposition.py` & `funcnodes_sklearn-0.1.3/funcnodes_sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `funcnodes_sklearn-0.1.2/pyproject.toml` & `funcnodes_sklearn-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "funcnodes-sklearn"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Kourosh Rezaei <kouroshrezaei90@gmail.com>"]
 readme = "README.md"
 
+homepage = "https://linkdlab.de/"
+
+repository = "https://github.com/kouroshrezaei/funcnodes_sklearn"
+
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 scikit-learn = "^1.4.2"
 funcnodes = "^0.2"
 funcnodes-pandas = "^0.1.3"
 funcnodes-numpy = "^0.1.52"
```

