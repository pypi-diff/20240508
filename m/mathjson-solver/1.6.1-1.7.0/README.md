# Comparing `tmp/mathjson-solver-1.6.1.tar.gz` & `tmp/mathjson_solver-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathjson-solver-1.6.1.tar", last modified: Tue Jul 18 04:58:32 2023, max compression
+gzip compressed data, was "mathjson_solver-1.7.0.tar", last modified: Wed May  8 11:40:55 2024, max compression
```

## Comparing `mathjson-solver-1.6.1.tar` & `mathjson_solver-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/
--rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.6.1/LICENSE
--rw-rw-r--   0 martins   (1000) martins   (1000)     7867 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)     7338 2023-07-18 04:55:26.000000 mathjson-solver-1.6.1/README.md
--rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.6.1/pyproject.toml
--rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/setup.cfg
--rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-07-18 04:37:12.000000 mathjson-solver-1.6.1/setup.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.349267 mathjson-solver-1.6.1/src/
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/src/mathjson_solver/
--rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.6.1/src/mathjson_solver/__init__.py
--rw-rw-r--   0 martins   (1000) martins   (1000)     8671 2023-07-18 04:35:03.000000 mathjson-solver-1.6.1/src/mathjson_solver/__main__.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7867 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/top_level.txt
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/tests/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7852 2023-07-18 04:36:34.000000 mathjson-solver-1.6.1/tests/test_with_pytest.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson_solver-1.7.0/LICENSE
+-rw-r--r--   0 martins   (1000) martins   (1000)     7867 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7338 2023-07-18 04:55:26.000000 mathjson_solver-1.7.0/README.md
+-rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson_solver-1.7.0/pyproject.toml
+-rw-rw-r--   0 martins   (1000) martins   (1000)      654 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/setup.cfg
+-rw-rw-r--   0 martins   (1000) martins   (1000)      829 2024-05-08 11:37:31.000000 mathjson_solver-1.7.0/setup.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2024-05-08 11:40:55.061919 mathjson_solver-1.7.0/src/
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/src/mathjson_solver/
+-rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson_solver-1.7.0/src/mathjson_solver/__init__.py
+-rw-rw-r--   0 martins   (1000) martins   (1000)     9365 2024-05-08 11:36:30.000000 mathjson_solver-1.7.0/src/mathjson_solver/__main__.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/src/mathjson_solver.egg-info/
+-rw-r--r--   0 martins   (1000) martins   (1000)     7867 2024-05-08 11:40:55.000000 mathjson_solver-1.7.0/src/mathjson_solver.egg-info/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)      313 2024-05-08 11:40:55.000000 mathjson_solver-1.7.0/src/mathjson_solver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)        1 2024-05-08 11:40:55.000000 mathjson_solver-1.7.0/src/mathjson_solver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)       16 2024-05-08 11:40:55.000000 mathjson_solver-1.7.0/src/mathjson_solver.egg-info/top_level.txt
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2024-05-08 11:40:55.065919 mathjson_solver-1.7.0/tests/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     8152 2024-05-08 11:38:32.000000 mathjson_solver-1.7.0/tests/test_with_pytest.py
```

### Comparing `mathjson-solver-1.6.1/LICENSE` & `mathjson_solver-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.6.1/PKG-INFO` & `mathjson_solver-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.6.1
+Version: 1.7.0
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathjson-solver-1.6.1/README.md` & `mathjson_solver-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.6.1/setup.cfg` & `mathjson_solver-1.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mathjson-solver
-version = 1.6.1
+version = 1.7.0
 author = Martins Mednis
 author_email = mrt@mednis.info
 description = Utilities for MathJSON evaluation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LongenesisLtd/mathjson-solver
 project_urls =
```

### Comparing `mathjson-solver-1.6.1/setup.py` & `mathjson_solver-1.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mathjson-solver",
-    version="1.6.1",
+    version="1.7.0",
     author="Martins Mednis",
     author_email="mrt@mednis.info",
     description="Utilities for MathJSON evaluation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LongenesisLtd/mathjson-solver",
     project_urls={
```

### Comparing `mathjson-solver-1.6.1/src/mathjson_solver/__main__.py` & `mathjson_solver-1.7.0/src/mathjson_solver/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numbers
 from functools import reduce
 import math
 from copy import deepcopy
 from statistics import median
+import logging
+import traceback
 
 
 class MathJSONException(Exception):
     """Exception for MathJSON processing issues"""
 
     def __init__(self, e, expr, *args, **kwargs):
         super().__init__(args)
@@ -119,16 +121,27 @@
 
             def If(s):
                 if len(s) < 3:
                     raise ValueError(f"Wrong parameters for 'If'")
                 for x in s[1:-1]:
                     if len(x) != 2:
                         raise ValueError(f"Wrong if or elif in 'If'")
-                    if f(x[0], c):
-                        return f(x[1], c)
+                    try:
+                        if f(x[0], c):
+                            try:
+                                return f(x[1], c)
+                            except MathJSONException as e:
+                                logging.error(
+                                    "MathJSONException: %s", traceback.format_exc()
+                                )
+                                continue
+                    except MathJSONException as e:
+                        logging.error("MathJSONException: %s", traceback.format_exc())
+                        return f(s[-1], c)  # return default value (else)
+
                 return f(s[-1], c)
 
             def In(s):
                 if len(s) != 3:
                     raise ValueError(f"Wrong parameters for 'In'")
                 if type(s[2]) == list and s[2][0] == "Array":
                     return f(s[1], c) in [f(x, c) for x in s[2][1:]]
@@ -233,14 +246,15 @@
                 "ContainsAnyOf": Contains_any_of,
                 "ContainsAllOf": Contains_all_of,
                 "ContainsNoneOf": Contains_none_of,
                 "Int": Int,
                 "Float": Float,
                 "Str": Str,
                 "Not": Not,
+                "IsDefined": lambda s: s[1] in c,
             }
             if s[0] in constructs:
                 try:
                     return constructs[s[0]](s)
                 except Exception as e:
                     raise MathJSONException(e, s, mathjson_construct=s[0])
             else:
@@ -249,10 +263,11 @@
                 # )
                 return s
         elif s in solver_parameters:
             return f(solver_parameters[s], c)
         elif s in c:
             return f(c[s], c)
         else:
+            # raise KeyError(f"Parameter '{s}' is not defined")
             return s
 
     return f
```

### Comparing `mathjson-solver-1.6.1/src/mathjson_solver.egg-info/PKG-INFO` & `mathjson_solver-1.7.0/src/mathjson_solver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.6.1
+Version: 1.7.0
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathjson-solver-1.6.1/tests/test_with_pytest.py` & `mathjson_solver-1.7.0/tests/test_with_pytest.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         ({}, ["Constants", ["a", 1], ["b", 2], ["c", 100], ["Sum", "a", "b"]], 3),
         ({}, ["Constants", ["a", 1], ["b", ["Add", 2, "a"]], "b"], 3),
         ({"x": 1}, ["Add", 2, "x"], 3),
         ({"color": "red"}, ["Switch", "color", 0, ["blue", 10], ["red", 30]], 30),
         ({"color": "green"}, ["Switch", "color", 0, ["blue", 10], ["red", 30]], 0),
         ({"color": "green"}, ["Switch", "undefined", 0, ["blue", 10], ["red", 30]], 0),
         ({}, ["If", [["Equal", 1, 0], 10], [["Equal", 2, 2], 20], 9000], 20),
+        ({"a": 10, "b": 10}, ["If", [["Equal", "a", "b"], 10], 9000], 10),
+        ({"a": 10, "b": 20}, ["If", [["Equal", "a", "b"], 10], 9000], 9000),
+        ({"a": 10}, ["If", [["Equal", "a", "b"], 10], 9000], 9000),
+        ({"a": 10}, ["If", [["Equal", "a", ["Sum", 1, "b"]], 10], 9000], 9000),
         ({}, ["Array", 1, 2, 3, 5, 2], ["Array", 1, 2, 3, 5, 2]),
         ({}, ["Max", ["Array", 1, 2, 3, 5, 2]], 5),
         ({}, ["Max", ["Array", 1, 2, ["Sum", 2, 4, 3], 5, 2]], 9),
         ({}, ["Median", ["Array", 1, 2, 3, 5, 2]], 2),
         ({}, ["Average", ["Array", 1, 2, 3, 5, 2]], 2.6),
         (
             {},
```

