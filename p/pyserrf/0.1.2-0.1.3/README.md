# Comparing `tmp/pyserrf-0.1.2.tar.gz` & `tmp/pyserrf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserrf-0.1.2.tar", max compression
+gzip compressed data, was "pyserrf-0.1.3.tar", max compression
```

## Comparing `pyserrf-0.1.2.tar` & `pyserrf-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      603 2024-05-04 16:40:19.958150 pyserrf-0.1.2/README.md
--rw-r--r--   0        0        0      546 2024-05-06 14:04:08.914546 pyserrf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-26 15:26:59.997208 pyserrf-0.1.2/pyserrf/__init__.py
--rw-r--r--   0        0        0     4293 2024-04-18 18:16:53.290329 pyserrf-0.1.2/pyserrf/read_data.py
--rwxr-xr-x   0        0        0      359 2024-05-06 09:54:41.577379 pyserrf-0.1.2/pyserrf/run.py
--rw-r--r--   0        0        0    27781 2024-05-06 14:01:38.690776 pyserrf-0.1.2/pyserrf/serrf.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 pyserrf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      667 2024-05-08 15:10:30.006285 pyserrf-0.1.3/README.md
+-rw-r--r--   0        0        0      574 2024-05-08 15:13:30.047169 pyserrf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-26 15:26:59.997208 pyserrf-0.1.3/pyserrf/__init__.py
+-rw-r--r--   0        0        0     4293 2024-04-18 18:16:53.290329 pyserrf-0.1.3/pyserrf/read_data.py
+-rwxr-xr-x   0        0        0      359 2024-05-06 09:54:41.577379 pyserrf-0.1.3/pyserrf/run.py
+-rw-r--r--   0        0        0    28004 2024-05-07 19:14:34.221373 pyserrf-0.1.3/pyserrf/serrf.py
+-rw-r--r--   0        0        0     1236 2024-05-07 18:49:51.109853 pyserrf-0.1.3/pyserrf/test2.py
+-rw-r--r--   0        0        0      266 2024-05-07 08:10:56.906400 pyserrf-0.1.3/pyserrf/testrun.py
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 pyserrf-0.1.3/PKG-INFO
```

### Comparing `pyserrf-0.1.2/pyproject.toml` & `pyserrf-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "pyserrf"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python implementation of the Systematic Error Removal Using Random Forest algorithm"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
 pandas = "^2.2.2"
 scikit-learn = "^1.4.2"
 pytest = "^8.2.0"
 tqdm = "^4.66.4"
+sphinx-rtd-theme = "^2.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">7.0"
```

### Comparing `pyserrf-0.1.2/pyserrf/read_data.py` & `pyserrf-0.1.3/pyserrf/read_data.py`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.2/pyserrf/serrf.py` & `pyserrf-0.1.3/pyserrf/serrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,19 +430,22 @@
             list1.
             """
             return [i for i in list1 if i in list2]
 
         selected = []
         for i in range(len(series1)):
             if len(selected) < num:
-                selected.extend(
-                    sorted_intersection(
-                        series1.iloc[0:i].index, series2.iloc[0:i].index
-                    )
-                )
+                templist_1 = list(series1.iloc[0:i].index)
+                templist_2 = list(series2.iloc[0:i].index)
+                temp_intersection = sorted_intersection(templist_1, templist_2)
+                for k in temp_intersection:
+                    if k not in selected:
+                        selected.append(k)
+                        if len(selected) == num:
+                            break
             else:
                 break
         selected = selected[0:num]
         return selected
 
     def _detect_outliers(self, data, threshold=3):
         """
```

### Comparing `pyserrf-0.1.2/PKG-INFO` & `pyserrf-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: pyserrf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of the Systematic Error Removal Using Random Forest algorithm
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pySERRF
 Python implementation of the Systematic Error Removal Using Random Forest (SERRF) algorithm.
 SERRF is a qc-based sample normalization method designed for large-scale untargeted metabolomics data.
 The method was developed by the Fan et al. in 2015 (see https://slfan2013.github.io/SERRF-online/).
 This is simply an attempt to port its functionality from R to python.
 The package structure is based on SKlearn's transformers, with fit and transform methods.
 
+Documentation can be found at https://pyserrf.readthedocs.io
+
+
 TODO: Implement cross-validation
 TODO: Verify if injection time is accounted for with current code
 TODO: Add documentation
 TODO: Add CLI
+
```

