# Comparing `tmp/TrialPy3-0.0.0.1.tar.gz` & `tmp/TrialPy3-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrialPy3-0.0.0.1.tar", last modified: Wed May  8 13:17:24 2024, max compression
+gzip compressed data, was "TrialPy3-0.0.0.2.tar", last modified: Wed May  8 13:30:02 2024, max compression
```

## Comparing `TrialPy3-0.0.0.1.tar` & `TrialPy3-0.0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:17:24.641020 TrialPy3-0.0.0.1/
--rw-rw-rw-   0        0        0    27028 2023-09-16 09:04:03.000000 TrialPy3-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     7712 2024-05-08 13:17:24.640023 TrialPy3-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7370 2024-05-08 13:17:03.000000 TrialPy3-0.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 13:17:24.641020 TrialPy3-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-05-08 13:11:57.000000 TrialPy3-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:17:24.625064 TrialPy3-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:17:24.633042 TrialPy3-0.0.0.1/src/TrialPy3/
--rw-rw-rw-   0        0        0   209208 2024-05-07 08:55:46.000000 TrialPy3-0.0.0.1/src/TrialPy3/RCFA.py
--rw-rw-rw-   0        0        0   112808 2023-09-08 08:00:59.000000 TrialPy3-0.0.0.1/src/TrialPy3/_RCSingle.py
--rw-rw-rw-   0        0        0        0 2024-04-30 07:11:25.000000 TrialPy3-0.0.0.1/src/TrialPy3/__init__.py
--rw-rw-rw-   0        0        0    12116 2023-09-08 04:56:21.000000 TrialPy3-0.0.0.1/src/TrialPy3/_arrangeCal.py
--rw-rw-rw-   0        0        0     7726 2023-08-08 11:47:29.000000 TrialPy3-0.0.0.1/src/TrialPy3/_forcesCal.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:17:24.638029 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/
--rw-rw-rw-   0        0        0     7712 2024-05-08 13:17:24.000000 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-05-08 13:17:24.000000 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:17:24.000000 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-08 13:17:24.000000 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 13:17:24.000000 TrialPy3-0.0.0.1/src/TrialPy3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 13:17:24.639025 TrialPy3-0.0.0.1/test/
--rw-rw-rw-   0        0        0    23383 2024-05-08 13:11:46.000000 TrialPy3-0.0.0.1/test/test_RCFA.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:30:02.391313 TrialPy3-0.0.0.2/
+-rw-rw-rw-   0        0        0    27028 2023-09-16 09:04:03.000000 TrialPy3-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7708 2024-05-08 13:30:02.390317 TrialPy3-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7366 2024-05-08 13:29:39.000000 TrialPy3-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:30:02.391313 TrialPy3-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-05-08 13:26:39.000000 TrialPy3-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:30:02.374955 TrialPy3-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 13:30:02.382933 TrialPy3-0.0.0.2/src/TrialPy3/
+-rw-rw-rw-   0        0        0   209208 2024-05-07 08:55:46.000000 TrialPy3-0.0.0.2/src/TrialPy3/RCFA.py
+-rw-rw-rw-   0        0        0   112808 2023-09-08 08:00:59.000000 TrialPy3-0.0.0.2/src/TrialPy3/_RCSingle.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 07:11:25.000000 TrialPy3-0.0.0.2/src/TrialPy3/__init__.py
+-rw-rw-rw-   0        0        0    12116 2023-09-08 04:56:21.000000 TrialPy3-0.0.0.2/src/TrialPy3/_arrangeCal.py
+-rw-rw-rw-   0        0        0     7726 2023-08-08 11:47:29.000000 TrialPy3-0.0.0.2/src/TrialPy3/_forcesCal.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:30:02.388319 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/
+-rw-rw-rw-   0        0        0     7708 2024-05-08 13:30:02.000000 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-08 13:30:02.000000 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:30:02.000000 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-08 13:30:02.000000 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 13:30:02.000000 TrialPy3-0.0.0.2/src/TrialPy3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 13:30:02.388319 TrialPy3-0.0.0.2/test/
+-rw-rw-rw-   0        0        0    23383 2024-05-08 13:11:46.000000 TrialPy3-0.0.0.2/test/test_RCFA.py
```

### Comparing `TrialPy3-0.0.0.1/LICENSE` & `TrialPy3-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.1/PKG-INFO` & `TrialPy3-0.0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrialPy3
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Object Oriented Structural Analysis
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -74,15 +74,17 @@
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
 Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
 
-![Alt text](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.JPG)
+![](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.png)
+
+
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
```

### Comparing `TrialPy3-0.0.0.1/README.md` & `TrialPy3-0.0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
 Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
 
-![Alt text](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.JPG)
+![](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.png)
+
+
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
```

### Comparing `TrialPy3-0.0.0.1/setup.py` & `TrialPy3-0.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description= f.read()
 
 setup(
     name="TrialPy3",
-    version="0.0.0.1",
+    version="0.0.0.2",
     description="Object Oriented Structural Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/TabishIzhar/StrucPy.git",
     # author="Tabish Izhar",
     # author_email="tizhar@iul.ac.in",
     license="GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)",
```

### Comparing `TrialPy3-0.0.0.1/src/TrialPy3/RCFA.py` & `TrialPy3-0.0.0.2/src/TrialPy3/RCFA.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.1/src/TrialPy3/_RCSingle.py` & `TrialPy3-0.0.0.2/src/TrialPy3/_RCSingle.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.1/src/TrialPy3/_arrangeCal.py` & `TrialPy3-0.0.0.2/src/TrialPy3/_arrangeCal.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.1/src/TrialPy3/_forcesCal.py` & `TrialPy3-0.0.0.2/src/TrialPy3/_forcesCal.py`

 * *Files identical despite different names*

### Comparing `TrialPy3-0.0.0.1/src/TrialPy3.egg-info/PKG-INFO` & `TrialPy3-0.0.0.2/src/TrialPy3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrialPy3
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Object Oriented Structural Analysis
 License: GNU LESSER GENERAL PUBLIC LICENSE v2.1 or later (GNU LGPLv2.1)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -74,15 +74,17 @@
 * Dynamic Seismic Analysis
 
 -----------------------------------------------------------------------------------------------------------
 ## StrucPy Coordinate System 
 
 Follow left-hand rule for coordinate system, the left thumb points along the y-axis in the positive direction. Gravity loads acting along y-axis.
 
-![Alt text](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.JPG)
+![](https://github.com/TabishIzhar/StrucPy/blob/main/CordSys.png)
+
+
 
 ------------------------------------------------------------------------------------------------------------
 
 ## StrucPy Documentation
 
 https://strucpy.readthedocs.io/
```

### Comparing `TrialPy3-0.0.0.1/test/test_RCFA.py` & `TrialPy3-0.0.0.2/test/test_RCFA.py`

 * *Files identical despite different names*

