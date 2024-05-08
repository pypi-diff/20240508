# Comparing `tmp/panorma-0.1.0.tar.gz` & `tmp/panorma-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panorma-0.1.0.tar", max compression
+gzip compressed data, was "panorma-0.1.1.tar", max compression
```

## Comparing `panorma-0.1.0.tar` & `panorma-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-28 20:33:03.134192 panorma-0.1.0/panorma/__init__.py
--rw-r--r--   0        0        0      518 2023-06-03 21:15:18.239720 panorma-0.1.0/panorma/exceptions.py
--rw-r--r--   0        0        0      357 2023-06-03 21:48:03.557331 panorma-0.1.0/panorma/fields.py
--rw-r--r--   0        0        0     1681 2023-06-03 21:48:03.575958 panorma-0.1.0/panorma/frames.py
--rw-r--r--   0        0        0      302 2023-05-28 20:48:40.868989 panorma-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1799 2023-06-11 11:35:56.903592 panorma-0.1.0/README.md
--rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 panorma-0.1.0/setup.py
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 panorma-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 10:15:09.038543 panorma-0.1.1/panorma/__init__.py
+-rw-r--r--   0        0        0      518 2024-05-08 10:15:09.038543 panorma-0.1.1/panorma/exceptions.py
+-rw-r--r--   0        0        0     1316 2024-05-08 10:15:09.039541 panorma-0.1.1/panorma/fields.py
+-rw-r--r--   0        0        0     2014 2024-05-08 10:15:09.039541 panorma-0.1.1/panorma/frames.py
+-rw-r--r--   0        0        0      275 2024-05-08 10:21:54.798264 panorma-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1743 2024-05-08 10:15:09.037546 panorma-0.1.1/README.md
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 panorma-0.1.1/PKG-INFO
```

### Comparing `panorma-0.1.0/panorma/exceptions.py` & `panorma-0.1.1/panorma/exceptions.py`

 * *Files identical despite different names*

### Comparing `panorma-0.1.0/README.md` & `panorma-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,39 +8,43 @@
 Simplify your data modeling and enhance the reliability of your DataFrame workflows.
 
 Installation:
 - 
 ```shell script
   pip install panorma
 ```
+or
+```shell script
+  poetry add panorma
+```
 
 Example:
 -
 - Create some models:
 ```python
-from panorma.fields import StringDtype, Int16Dtype, Float32Dtype, Timestamp, CategoricalDtype
+from panorma.fields import String, Int, Float, DateTime, Categorical
 from panorma.frames import DataFrame
 
 class Users(DataFrame):
-    name: StringDtype
-    age: Int16Dtype
-    percentage: Float32Dtype
-    birth_date: Timestamp
+    name: String
+    age: Int
+    percentage: Float
+    birth_date: DateTime
 
 
 class Cars(DataFrame):
-    car: StringDtype
-    mpg: Float32Dtype
-    cylinders: Int16Dtype
-    displacement: Float32Dtype
-    horsepower: Float32Dtype
-    weight: Float32Dtype
-    acceleration: Float32Dtype
-    model: Int16Dtype
-    origin: CategoricalDtype
+    car: String
+    mpg: Float
+    cylinders: Int
+    displacement: Float
+    horsepower: Float
+    weight: Float
+    acceleration: Float
+    model: Int
+    origin: Categorical
 ```
 
 - Instantiate your models as you instantiate a simple pandas dataframe
 
 ```python
 import pandas as pd
```

