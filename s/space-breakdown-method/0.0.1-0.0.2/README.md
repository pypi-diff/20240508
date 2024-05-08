# Comparing `tmp/space-breakdown-method-0.0.1.tar.gz` & `tmp/space-breakdown-method-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\space-breakdown-method-0.0.1.tar", last modified: Wed May  8 07:06:02 2024, max compression
+gzip compressed data, was "dist\space-breakdown-method-0.0.2.tar", last modified: Wed May  8 07:07:15 2024, max compression
```

## Comparing `space-breakdown-method-0.0.1.tar` & `space-breakdown-method-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/
--rw-rw-rw-   0        0        0     1079 2024-05-07 09:07:35.000000 space-breakdown-method-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7390 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2024-05-08 07:04:51.000000 space-breakdown-method-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/sbm/
--rw-rw-rw-   0        0        0    14369 2024-05-08 06:51:32.000000 space-breakdown-method-0.0.1/sbm/ISBM.py
--rw-rw-rw-   0        0        0    13403 2024-05-08 06:51:33.000000 space-breakdown-method-0.0.1/sbm/SBM.py
--rw-rw-rw-   0        0        0    20129 2024-05-08 07:04:51.000000 space-breakdown-method-0.0.1/sbm/TFBM.py
--rw-rw-rw-   0        0        0      211 2024-05-08 07:01:00.000000 space-breakdown-method-0.0.1/sbm/__init__.py
--rw-rw-rw-   0        0        0      258 2024-05-08 06:24:43.000000 space-breakdown-method-0.0.1/sbm/constants.py
--rw-rw-rw-   0        0        0    12020 2024-05-08 06:53:32.000000 space-breakdown-method-0.0.1/sbm/main.py
--rw-rw-rw-   0        0        0       42 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-08 07:05:56.000000 space-breakdown-method-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/
--rw-rw-rw-   0        0        0     7390 2024-05-08 07:06:01.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:06:01.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-08 07:06:02.000000 space-breakdown-method-0.0.1/space_breakdown_method.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/
+-rw-rw-rw-   0        0        0     1079 2024-05-07 09:07:35.000000 space-breakdown-method-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7409 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7774 2024-05-08 07:07:12.000000 space-breakdown-method-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/sbm/
+-rw-rw-rw-   0        0        0    14369 2024-05-08 06:51:32.000000 space-breakdown-method-0.0.2/sbm/ISBM.py
+-rw-rw-rw-   0        0        0    13403 2024-05-08 06:51:33.000000 space-breakdown-method-0.0.2/sbm/SBM.py
+-rw-rw-rw-   0        0        0    20129 2024-05-08 07:04:51.000000 space-breakdown-method-0.0.2/sbm/TFBM.py
+-rw-rw-rw-   0        0        0      211 2024-05-08 07:01:00.000000 space-breakdown-method-0.0.2/sbm/__init__.py
+-rw-rw-rw-   0        0        0      258 2024-05-08 06:24:43.000000 space-breakdown-method-0.0.2/sbm/constants.py
+-rw-rw-rw-   0        0        0    12020 2024-05-08 06:53:32.000000 space-breakdown-method-0.0.2/sbm/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-08 07:07:12.000000 space-breakdown-method-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/
+-rw-rw-rw-   0        0        0     7409 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-08 07:07:15.000000 space-breakdown-method-0.0.2/space_breakdown_method.egg-info/top_level.txt
```

### Comparing `space-breakdown-method-0.0.1/LICENSE.txt` & `space-breakdown-method-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `space-breakdown-method-0.0.1/PKG-INFO` & `space-breakdown-method-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-breakdown-method
-Version: 0.0.1
+Version: 0.0.2
 Summary: Space Breakdown Method (SBM) is a clustering algorithm developed for Spike Sorting handling overlapping and imbalanced data. Improved Space Breakdown Method (ISBM) is the updated and improved version of SBM. A new algorithm for the detection of brain oscillations packets has been developed based on SBM, called Time-Frequency Breakdown Method (TFBM)
 Home-page: https://https://github.com/ArdeleanRichard/Space-Breakdown-Method
 Author: Eugen-Richard Ardelean
 Author-email: ardeleaneugenrichard@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 License-File: LICENSE.txt
 
 # Space Breakdown Method
 Space Breakdown Method (SBM) is a clustering algorithm that can be used to cluster low-dimensional neural data with efficiency, due to its linear complexity scaling with the data size. SBM has been published by IEEE in September 2019.
 
 # Install:
 ```
-pip install sbm
+pip install space-breakdown-method
 ```
 
 Usage example:
 ```
 import matplotlib.pyplot as plt
 from sklearn import datasets
```

### Comparing `space-breakdown-method-0.0.1/README.md` & `space-breakdown-method-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 SBM has been published by IEEE in September 2019:
 - https://ieeexplore.ieee.org/document/8959795
 - DOI: 10.1109/ICCP48234.2019.8959795
 - Conference: 2019 IEEE 15th International Conference on Intelligent Computer Communication and Processing (ICCP)
 
 # Install:
 ```
-pip install sbm
+pip install space-breakdown-method
 ```
 
 Usage example:
 ```
 import matplotlib.pyplot as plt
 from sklearn import datasets
```

### Comparing `space-breakdown-method-0.0.1/sbm/ISBM.py` & `space-breakdown-method-0.0.2/sbm/ISBM.py`

 * *Files identical despite different names*

### Comparing `space-breakdown-method-0.0.1/sbm/SBM.py` & `space-breakdown-method-0.0.2/sbm/SBM.py`

 * *Files identical despite different names*

### Comparing `space-breakdown-method-0.0.1/sbm/TFBM.py` & `space-breakdown-method-0.0.2/sbm/TFBM.py`

 * *Files identical despite different names*

### Comparing `space-breakdown-method-0.0.1/sbm/main.py` & `space-breakdown-method-0.0.2/sbm/main.py`

 * *Files identical despite different names*

### Comparing `space-breakdown-method-0.0.1/setup.py` & `space-breakdown-method-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("sbm/README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name="space-breakdown-method",
-    version="0.0.1",
+    version="0.0.2",
     description="Space Breakdown Method (SBM) is a clustering algorithm developed for Spike Sorting handling overlapping and imbalanced data. Improved Space Breakdown Method (ISBM) is the updated and improved version of SBM. A new algorithm for the detection of brain oscillations packets has been developed based on SBM, called Time-Frequency Breakdown Method (TFBM)",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://https://github.com/ArdeleanRichard/Space-Breakdown-Method",
     author="Eugen-Richard Ardelean",
     author_email="ardeleaneugenrichard@gmail.com",
```

### Comparing `space-breakdown-method-0.0.1/space_breakdown_method.egg-info/PKG-INFO` & `space-breakdown-method-0.0.2/space_breakdown_method.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-breakdown-method
-Version: 0.0.1
+Version: 0.0.2
 Summary: Space Breakdown Method (SBM) is a clustering algorithm developed for Spike Sorting handling overlapping and imbalanced data. Improved Space Breakdown Method (ISBM) is the updated and improved version of SBM. A new algorithm for the detection of brain oscillations packets has been developed based on SBM, called Time-Frequency Breakdown Method (TFBM)
 Home-page: https://https://github.com/ArdeleanRichard/Space-Breakdown-Method
 Author: Eugen-Richard Ardelean
 Author-email: ardeleaneugenrichard@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 License-File: LICENSE.txt
 
 # Space Breakdown Method
 Space Breakdown Method (SBM) is a clustering algorithm that can be used to cluster low-dimensional neural data with efficiency, due to its linear complexity scaling with the data size. SBM has been published by IEEE in September 2019.
 
 # Install:
 ```
-pip install sbm
+pip install space-breakdown-method
 ```
 
 Usage example:
 ```
 import matplotlib.pyplot as plt
 from sklearn import datasets
```

