# Comparing `tmp/realtime_operator-0.2.6.tar.gz` & `tmp/realtime_operator-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.2.6.tar", last modified: Sun Apr 28 19:18:38 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.7.tar", last modified: Wed May  8 13:09:23 2024, max compression
```

## Comparing `realtime_operator-0.2.6.tar` & `realtime_operator-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.919562 realtime_operator-0.2.6/
--rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     4367 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/README.md
--rw-rw-rw-   0        0        0      695 2024-04-28 19:17:22.000000 realtime_operator-0.2.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.874516 realtime_operator-0.2.6/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0    13298 2024-04-28 19:16:31.000000 realtime_operator-0.2.6/realtime_operator/compression.py
--rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.6/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4367 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-28 19:18:38.000000 realtime_operator-0.2.6/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 19:18:38.919562 realtime_operator-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 19:18:38.912043 realtime_operator-0.2.6/tests/
--rw-rw-rw-   0        0        0     2805 2024-04-28 19:15:16.000000 realtime_operator-0.2.6/tests/test_compression.py
--rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.6/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.814570 realtime_operator-0.2.7/
+-rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-05-08 13:09:23.812181 realtime_operator-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/README.md
+-rw-rw-rw-   0        0        0      695 2024-05-08 13:05:19.000000 realtime_operator-0.2.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.744767 realtime_operator-0.2.7/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0    13467 2024-05-08 13:04:57.000000 realtime_operator-0.2.7/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.7/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.810939 realtime_operator-0.2.7/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:09:23.814570 realtime_operator-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.808457 realtime_operator-0.2.7/tests/
+-rw-rw-rw-   0        0        0     2805 2024-04-28 19:15:16.000000 realtime_operator-0.2.7/tests/test_compression.py
+-rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.7/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.2.6/LICENSE` & `realtime_operator-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.6/PKG-INFO` & `realtime_operator-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.6/README.md` & `realtime_operator-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.6/pyproject.toml` & `realtime_operator-0.2.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "realtime_operator"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `realtime_operator-0.2.6/realtime_operator/compression.py` & `realtime_operator-0.2.7/realtime_operator/compression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 import math
 import numba as nb
 import numpy as np
 from numba.typed import List
 import sys
 from enum import Enum
 
-COMPRESSION_TYPE={"DEDUPLICATE" : 0,
-    "MINIMUM_TIMEDELTA" : 1,
-    "EXCEPTION_DEVIATION" : 2,
-    "EXCEPTION_DEVIATION_PREVIOUS" : 3,
-    "SWINGING_DOOR": 4
+COMPRESSION_TYPE = {
+    "DEDUPLICATE": 0,
+    "MINIMUM_TIMEDELTA": 1,
+    "EXCEPTION_DEVIATION": 2,
+    "EXCEPTION_DEVIATION_PREVIOUS": 3,
+    "SWINGING_DOOR": 4,
 }
 EPSILON = 1e-15
 
-def interpolate(t,tn,zn):
+
+def interpolate(t, tn, zn):
     return np.interp(t, tn, zn, left=np.nan, right=np.nan)
 
+
 @nb.jit(nopython=True)
-def interpolate_fast(t,tn,zn):
-    npointer=0
+def interpolate_fast(t, tn, zn):
+    npointer = 0
     len_t = len(t)
     len_tn = len(tn)
     z = np.full(len_t, np.nan, dtype=float)
     # start condition: t[i]>=tn[0]
     left_t = 0
     left_tn = 0
 
     # no interpolation left of the first point
     while left_t < len_t and t[left_t] < tn[0]:
         left_t += 1
 
     # llop through all t values
     for i in range(left_t, len_t):
-        while left_tn < len_tn-1 and t[i] > tn[left_tn+1]:
+        while left_tn < len_tn - 1 and t[i] > tn[left_tn + 1]:
             left_tn += 1
         if left_tn == len_tn - 1:
             break
-        if t[i] >= tn[left_tn] and t[i] <= tn[left_tn+1]:
-            m=(zn[left_tn+1]-zn[left_tn])/(tn[left_tn+1]-tn[left_tn])
+        if t[i] >= tn[left_tn] and t[i] <= tn[left_tn + 1]:
+            m = (zn[left_tn + 1] - zn[left_tn]) / (tn[left_tn + 1] - tn[left_tn])
             z[i] = zn[left_tn] + m * (t[i] - tn[left_tn])
     return z
 
 
-
 @nb.jit(nopython=True)
-def any_compression(t,z,delta, ftype):
-    tn=[]
-    zn=[]
-    cn=[]
+def any_compression(t, z, delta, ftype):
+    tn = []
+    zn = []
+    cn = []
     n = len(z)
     if ftype == 0:
         state = np.zeros(3, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = deduplicate(state, t[i], z[i],0.0, 1.0e6)
+            tn_, zn_, cn_ = deduplicate(state, t[i], z[i], 0.0, 1.0e6)
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 1:
         state = np.zeros(3, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = minimum_timedelta(delta,state, t[i], z[i])
+            tn_, zn_, cn_ = minimum_timedelta(delta, state, t[i], z[i])
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 2:
         state = np.zeros(3, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = exception_deviation(delta,state, t[i], z[i],0.0, 1.0e6)
+            tn_, zn_, cn_ = exception_deviation(delta, state, t[i], z[i], 0.0, 1.0e6)
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 3:
         state = np.zeros(5, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = exception_deviation_previous(delta,state, t[i], z[i],0.0, 1.0e6)
+            tn_, zn_, cn_ = exception_deviation_previous(
+                delta, state, t[i], z[i], 0.0, 1.0e6
+            )
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     elif ftype == 4:
         state = np.zeros(7, dtype=float)
         for i in range(n):
-            tn_ , zn_, cn_ = swinging_door(delta,state, t[i], z[i],0.0, 1.0e6)
+            tn_, zn_, cn_ = swinging_door(delta, state, t[i], z[i], 0.0, 1.0e6)
             for i in range(len(tn_)):
                 tn.append(tn_[i])
                 zn.append(zn_[i])
                 cn.append(cn_[i])
     # always capture the last point to allow for interpolation:
     if abs(tn[-1] - t[-1]) >= EPSILON:
         tn.append(t[-1])
         zn.append(z[-1])
         cn.append(0)
-    return np.array(tn,np.float64),np.array(zn,np.float64),np.array(cn,np.float64)
+    return np.array(tn, np.float64), np.array(zn, np.float64), np.array(cn, np.float64)
+
 
 @nb.jit("Tuple((f8[:], f8[:], f8[:]))(f8[:], f8, f8, f8, f8)", nopython=True)
 def deduplicate(state, t, z, min_duration_seconds=0, max_duration_seconds=1e9):
     """
     Deduplicates data points based on time and value.
 
     Args:
@@ -107,15 +112,15 @@
         z (float): Current value.
         min_duration_seconds (float, optional): Minimum duration between data points in seconds. Defaults to 0.
         max_duration_seconds (float, optional): Maximum duration between data points in seconds. Defaults to 1e9.
 
     Returns:
         Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]: Tuple containing arrays of deduplicated time, value, and count.
     """
-    
+
     if state[0] == 0:
         state[0] = t
         state[1] = z
         state[2] = 0
         return (
             np.array([t], dtype=np.float64),
             np.array([z], dtype=np.float64),
@@ -323,16 +328,16 @@
 
     Returns:
         Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]: Tuple containing arrays of filtered time, value, and count.
     """
     if state[0] == 0:
         state[0] = t
         state[1] = z
-        state[2] = -np.inf  # min slope
-        state[3] = np.inf  # max slope
+        state[2] = np.finfo(dtype=np.float64).min  # min slope
+        state[3] = np.finfo(dtype=np.float64).max  # max slope
         state[4] = t
         state[5] = z
         state[6] = 0
         return (
             np.array([t], dtype=np.float64),
             np.array([z], dtype=np.float64),
             np.array([0], dtype=np.float64),
@@ -350,16 +355,16 @@
     max_duration_condition = (t - state[0]) >= max_duration_seconds
 
     if (slope_condition and min_duration_condition) or max_duration_condition:
         tp = state[4]
         zp = state[5]
         state[0] = tp
         state[1] = zp
-        state[2] = -np.inf  # min slope
-        state[3] = np.inf  # max slope
+        state[2] = np.finfo(dtype=np.float64).min  # min slope
+        state[3] = np.finfo(dtype=np.float64).max  # max slope
         state[4] = t
         state[5] = z
         count = state[6]
         state[6] = 0
         return (
             np.array([tp], dtype=np.float64),
             np.array([zp], dtype=np.float64),
@@ -374,8 +379,7 @@
         state[4] = t
         state[5] = z
         return (
             np.zeros(0, np.float64),
             np.zeros(0, np.float64),
             np.zeros(0, np.float64),
         )
-
```

### Comparing `realtime_operator-0.2.6/realtime_operator/single_operator.py` & `realtime_operator-0.2.7/realtime_operator/single_operator.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.6/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.7/realtime_operator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.6/tests/test_compression.py` & `realtime_operator-0.2.7/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.6/tests/test_single_operator.py` & `realtime_operator-0.2.7/tests/test_single_operator.py`

 * *Files identical despite different names*

