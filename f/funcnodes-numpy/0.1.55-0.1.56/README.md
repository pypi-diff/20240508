# Comparing `tmp/funcnodes_numpy-0.1.55.tar.gz` & `tmp/funcnodes_numpy-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_numpy-0.1.55.tar", max compression
+gzip compressed data, was "funcnodes_numpy-0.1.56.tar", max compression
```

## Comparing `funcnodes_numpy-0.1.55.tar` & `funcnodes_numpy-0.1.56.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    13843 2024-05-08 11:30:26.263542 funcnodes_numpy-0.1.55/funcnodes_numpy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 09:55:21.532750 funcnodes_numpy-0.1.55/funcnodes_numpy/_array_creation.py
--rw-r--r--   0        0        0    85475 2024-05-08 11:28:24.060188 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/__init__.py
--rw-r--r--   0        0        0      481 2024-03-19 16:23:50.188790 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/_datetime.py
--rw-r--r--   0        0        0     1182 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/_defchararray.py
--rw-r--r--   0        0        0        0 2024-03-19 09:12:23.563823 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/_fromnumeric.py
--rw-r--r--   0        0        0        0 2024-03-19 09:13:00.460173 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/_multiarray.py
--rw-r--r--   0        0        0    75951 2024-03-22 06:01:33.436725 funcnodes_numpy-0.1.55/funcnodes_numpy/_core/ufuncs.py
--rw-r--r--   0        0        0     3927 2024-03-22 12:32:44.058278 funcnodes_numpy-0.1.55/funcnodes_numpy/_dtypes.py
--rw-r--r--   0        0        0       91 2024-03-22 12:20:39.204892 funcnodes_numpy-0.1.55/funcnodes_numpy/_lib/__init__.py
--rw-r--r--   0        0        0     3015 2024-03-22 12:20:39.202680 funcnodes_numpy-0.1.55/funcnodes_numpy/_lib/scimath.py
--rw-r--r--   0        0        0       23 2024-03-19 12:34:04.505018 funcnodes_numpy-0.1.55/funcnodes_numpy/_linalg/__init__.py
--rw-r--r--   0        0        0     9828 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.55/funcnodes_numpy/_linalg/_linalg.py
--rw-r--r--   0        0        0    16374 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.55/funcnodes_numpy/_ndarray.py
--rw-r--r--   0        0        0     3582 2024-04-11 20:12:41.922477 funcnodes_numpy-0.1.55/funcnodes_numpy/_types.py
--rw-r--r--   0        0        0      423 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.55/funcnodes_numpy/constants.py
--rw-r--r--   0        0        0      497 2024-05-08 11:30:32.647287 funcnodes_numpy-0.1.55/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 14:46:02.900426 funcnodes_numpy-0.1.55/README.md
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 funcnodes_numpy-0.1.55/PKG-INFO
+-rw-r--r--   0        0        0    13877 2024-05-08 11:35:14.452353 funcnodes_numpy-0.1.56/funcnodes_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 09:55:21.532750 funcnodes_numpy-0.1.56/funcnodes_numpy/_array_creation.py
+-rw-r--r--   0        0        0    86091 2024-05-08 11:35:47.644048 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/__init__.py
+-rw-r--r--   0        0        0      481 2024-03-19 16:23:50.188790 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/_datetime.py
+-rw-r--r--   0        0        0     1182 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/_defchararray.py
+-rw-r--r--   0        0        0        0 2024-03-19 09:12:23.563823 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/_fromnumeric.py
+-rw-r--r--   0        0        0        0 2024-03-19 09:13:00.460173 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/_multiarray.py
+-rw-r--r--   0        0        0    75951 2024-03-22 06:01:33.436725 funcnodes_numpy-0.1.56/funcnodes_numpy/_core/ufuncs.py
+-rw-r--r--   0        0        0     3927 2024-03-22 12:32:44.058278 funcnodes_numpy-0.1.56/funcnodes_numpy/_dtypes.py
+-rw-r--r--   0        0        0       91 2024-03-22 12:20:39.204892 funcnodes_numpy-0.1.56/funcnodes_numpy/_lib/__init__.py
+-rw-r--r--   0        0        0     3015 2024-03-22 12:20:39.202680 funcnodes_numpy-0.1.56/funcnodes_numpy/_lib/scimath.py
+-rw-r--r--   0        0        0       23 2024-03-19 12:34:04.505018 funcnodes_numpy-0.1.56/funcnodes_numpy/_linalg/__init__.py
+-rw-r--r--   0        0        0     9828 2024-03-22 12:20:39.200788 funcnodes_numpy-0.1.56/funcnodes_numpy/_linalg/_linalg.py
+-rw-r--r--   0        0        0    16374 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.56/funcnodes_numpy/_ndarray.py
+-rw-r--r--   0        0        0     3582 2024-04-11 20:12:41.922477 funcnodes_numpy-0.1.56/funcnodes_numpy/_types.py
+-rw-r--r--   0        0        0      423 2024-03-22 12:20:39.199729 funcnodes_numpy-0.1.56/funcnodes_numpy/constants.py
+-rw-r--r--   0        0        0      497 2024-05-08 11:35:03.282202 funcnodes_numpy-0.1.56/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 14:46:02.900426 funcnodes_numpy-0.1.56/README.md
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 funcnodes_numpy-0.1.56/PKG-INFO
```

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/__init__.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from ._dtypes import DTYPE_ENUM
 
 from exposedfunctionality.function_parser.types import type_to_string
 
 import numpy as np
 
-__version__ = "0.1.55"
+__version__ = "0.1.56"
 
 
 # set the print options to display a smaller number of elements for node previews
 np.set_printoptions(
     threshold=100,
     formatter={
         # float_kind is used to format floats in scientific notation
@@ -341,14 +341,15 @@
             subshelves=[],
         ),
         fn.Shelf(
             name="Joining and Splitting",
             description="Joining and Splitting",
             nodes=[
                 core.concatenate,
+                core.concatenat2,
                 core.stack,
                 core.stack2,
                 core.vstack,
                 core.vstack2,
                 core.hstack,
                 core.hstack2,
                 core.dstack,
```

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_core/__init__.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1211,14 +1211,38 @@
         dtype=dtype_from_name(dtype),
         # casting=casting,
     )
     return res
 
 
 @fn.NodeDecorator(
+    node_id="np.concatenate2",
+    name="concatenate2",
+    outputs=[{"name": "res", "type": "ndarray"}],
+)
+@wraps(numpy.concatenate, wrapper_attribute="__fnwrapped__")
+def concatenate2(
+    a: ndarray,
+    b: ndarray,
+    axis: Optional[int] = 0,
+    # out: Optional[ndarray] = None,
+    dtype: Optional[DTYPE_ENUM] = None,
+    # casting: casting_literal = "same_kind",
+):  # params [] ['axis', 'out', 'dtype', 'casting'] []
+    res = numpy.concatenate(
+        (a, b),
+        axis=axis,
+        # out=out,
+        dtype=dtype_from_name(dtype),
+        # casting=casting,
+    )
+    return res
+
+
+@fn.NodeDecorator(
     node_id="np.stack",
     name="stack",
     outputs=[{"name": "stacked", "type": "ndarray"}],
 )
 @wraps(numpy.stack, wrapper_attribute="__fnwrapped__")
 def stack(
     arrays: Sequence[array_like],
```

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_core/_defchararray.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_core/_defchararray.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_core/ufuncs.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_core/ufuncs.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_dtypes.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_dtypes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_lib/scimath.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_lib/scimath.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_linalg/_linalg.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_linalg/_linalg.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_ndarray.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_ndarray.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/funcnodes_numpy/_types.py` & `funcnodes_numpy-0.1.56/funcnodes_numpy/_types.py`

 * *Files identical despite different names*

### Comparing `funcnodes_numpy-0.1.55/PKG-INFO` & `funcnodes_numpy-0.1.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-numpy
-Version: 0.1.55
+Version: 0.1.56
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

