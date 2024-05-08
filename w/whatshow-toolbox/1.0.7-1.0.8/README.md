# Comparing `tmp/whatshow_toolbox-1.0.7.tar.gz` & `tmp/whatshow_toolbox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_toolbox-1.0.7.tar", last modified: Sun Apr 28 08:10:20 2024, max compression
+gzip compressed data, was "whatshow_toolbox-1.0.8.tar", last modified: Tue May  7 12:44:33 2024, max compression
```

## Comparing `whatshow_toolbox-1.0.7.tar` & `whatshow_toolbox-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:10:20.322384 whatshow_toolbox-1.0.7/
--rw-rw-rw-   0        0        0     2154 2024-04-28 08:10:20.319417 whatshow_toolbox-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-04-28 08:10:19.000000 whatshow_toolbox-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 08:10:20.322384 whatshow_toolbox-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-04-28 08:10:19.000000 whatshow_toolbox-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:10:20.304275 whatshow_toolbox-1.0.7/whatshow_toolbox/
--rw-rw-rw-   0        0        0    13775 2024-04-28 08:10:19.000000 whatshow_toolbox-1.0.7/whatshow_toolbox/MatlabFuncHelper.py
--rw-rw-rw-   0        0        0       46 2024-04-28 08:10:19.000000 whatshow_toolbox-1.0.7/whatshow_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:10:20.318624 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/
--rw-rw-rw-   0        0        0     2154 2024-04-28 08:10:20.000000 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-28 08:10:20.000000 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:10:20.000000 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-28 08:10:20.000000 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 08:10:20.000000 whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 12:44:33.823973 whatshow_toolbox-1.0.8/
+-rw-rw-rw-   0        0        0     2154 2024-05-07 12:44:33.820594 whatshow_toolbox-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-07 12:44:32.000000 whatshow_toolbox-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:44:33.823973 whatshow_toolbox-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-05-07 12:44:32.000000 whatshow_toolbox-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:44:33.771099 whatshow_toolbox-1.0.8/whatshow_toolbox/
+-rw-rw-rw-   0        0        0    14513 2024-05-07 12:44:32.000000 whatshow_toolbox-1.0.8/whatshow_toolbox/MatlabFuncHelper.py
+-rw-rw-rw-   0        0        0       46 2024-05-07 12:44:32.000000 whatshow_toolbox-1.0.8/whatshow_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:44:33.818592 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     2154 2024-05-07 12:44:33.000000 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-07 12:44:33.000000 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:44:33.000000 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 12:44:33.000000 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 12:44:33.000000 whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/top_level.txt
```

### Comparing `whatshow_toolbox-1.0.7/PKG-INFO` & `whatshow_toolbox-1.0.8/whatshow_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: whatshow_toolbox
-Version: 1.0.7
+Name: whatshow-toolbox
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.7-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.8-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.7/README.md` & `whatshow_toolbox-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.7-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.8-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

### Comparing `whatshow_toolbox-1.0.7/whatshow_toolbox/MatlabFuncHelper.py` & `whatshow_toolbox-1.0.8/whatshow_toolbox/MatlabFuncHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,19 @@
     
     ###########################################################################
     # transformers
     '''
     remove redundant dimension except for the batch_size
     '''
     def squeeze(self, mat):
+        mat = np.asarray(mat);
         out = np.squeeze(mat);
         if self.batch_size == 1 and mat.ndim > 0:
-            out = np.expand_dims(out, 0);
+            if mat.shape[0] == self.batch_size:
+                out = np.expand_dims(out, 0);
         return out;
     
     '''
     reshape
     @in1:   1st dimension
     @in...: other dimensions
     @order: 'C': only consider given dimensions, 'F': if only given 1 dimension, this is for the row and column
@@ -289,15 +291,20 @@
 
     ###########################################################################
     # Maths
     '''
     sum
     '''
     def sum(self, mat, *, axis=-1):
-        return np.sum(mat, axis=-1);
+        return np.sum(mat, axis=axis);
+    '''
+    sum (the return value has the same dimension number as the given)
+    '''
+    def sum1(self, mat, *, axis=-1):
+        return np.expand_dims(np.sum(mat, axis=axis), axis=axis);
     
     '''
     return the maximum of a matrix or the maximum of two matrices (for complex value, we compare the magnitude)
     @in1:   the matrix to find the maximal value
     @in2:   a scalar or a matrix to be compared with in1. If not given, it means return the maximal value of in1
     @axis:  the axis to compare or find the maximal value
     '''
@@ -322,14 +329,25 @@
         else:
             if len(args) == 0:
                 out = np.take_along_axis(in1, abs(in1).argmax(axis=axis, keepdims=True), axis).squeeze(axis);
             else:
                 out = np.where(abs(in1)>abs(in2), in1, in2);
         return out;
     
+    def max1(self, in1, *args, axis=-1):
+        in1 = np.asarray(in1);
+        if len(args) > 0:
+            return self.max(in1, *args, axis=axis);
+        else:
+            # non-complex value
+            if in1.dtype != np.csingle and in1.dtype != np.complex_:
+                return np.max(in1, axis=axis);
+            else:
+                return np.take_along_axis(in1, np.argmax(abs(in1), axis=axis, keepdims=True), axis);
+    
     '''
     Kronecker product
     @a: a matrix like [(batch_size), ..., i, j]
     @b: a matrix like [(batch_size), ..., k, l]
     '''
     def kron(self, a, b):
         a = np.asarray(a);
@@ -344,14 +362,15 @@
             if len(a.shape) != len(b.shape):
                 raise Exception("The two inputs dimensions are not same.");
             shape = list(a.shape);
             shape[-1] = a.shape[-1]*b.shape[-1];
             shape[-2] = a.shape[-1]*b.shape[-1];
             out = np.einsum('...ij,...kl->...ikjl', a, b).reshape(shape);
         return out;
+        
 
     ###########################################################################
     # private methods
     '''
     calculate the shape based on the given dimensions
     '''
     def _shape_calc_(self, in1, *args, order='C'):
```

### Comparing `whatshow_toolbox-1.0.7/whatshow_toolbox.egg-info/PKG-INFO` & `whatshow_toolbox-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: whatshow-toolbox
-Version: 1.0.7
+Name: whatshow_toolbox
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # Toolbox
-[![PyPi](https://img.shields.io/badge/PyPi-1.0.7-blue)](https://pypi.org/project/whatshow-toolbox/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.0.8-blue)](https://pypi.org/project/whatshow-toolbox/)
 
 
 This repositories offers a toolbox across platforms.
 ## How to use
 * MatlabFuncHelper: this class simulate all Matlab functions in python (batch is supported).
     * batch
         * setBatchSize(batch_size)
```

