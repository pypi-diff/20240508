# Comparing `tmp/odlabel-0.7.26.tar.gz` & `tmp/odlabel-0.7.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.tar", last modified: Mon May  6 11:52:47 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.1.tar", last modified: Wed May  8 19:14:51 2024, max compression
```

## Comparing `odlabel-0.7.26.tar` & `odlabel-0.7.26.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-06 11:52:47.949344 odlabel-0.7.26/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26/LICENSE
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7657 2024-05-06 11:52:47.949344 odlabel-0.7.26/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6898 2024-05-06 11:50:34.000000 odlabel-0.7.26/README.md
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-06 11:52:47.949344 odlabel-0.7.26/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-05 13:42:42.000000 odlabel-0.7.26/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-06 11:07:09.000000 odlabel-0.7.26/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-06 11:52:47.949344 odlabel-0.7.26/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-02 17:12:53.000000 odlabel-0.7.26/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14360 2024-05-05 23:39:38.000000 odlabel-0.7.26/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-06 11:52:47.949344 odlabel-0.7.26/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10458 2024-05-02 20:55:30.000000 odlabel-0.7.26/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-05 19:35:10.000000 odlabel-0.7.26/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1044 2024-05-02 17:12:49.000000 odlabel-0.7.26/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-06 11:52:47.949344 odlabel-0.7.26/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7657 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-06 11:52:47.000000 odlabel-0.7.26/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-06 11:52:47.949344 odlabel-0.7.26/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1263 2024-05-06 11:51:28.000000 odlabel-0.7.26/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.1/LICENSE
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7054 2024-05-08 19:12:44.000000 odlabel-0.7.26.1/README.md
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-05 13:42:42.000000 odlabel-0.7.26.1/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.1/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-06 11:07:09.000000 odlabel-0.7.26.1/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.1/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-02 17:12:53.000000 odlabel-0.7.26.1/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14360 2024-05-05 23:39:38.000000 odlabel-0.7.26.1/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.1/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10458 2024-05-02 20:55:30.000000 odlabel-0.7.26.1/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-05 19:35:10.000000 odlabel-0.7.26.1/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1044 2024-05-02 17:12:49.000000 odlabel-0.7.26.1/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.1/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-08 19:14:51.875652 odlabel-0.7.26.1/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-08 19:14:51.000000 odlabel-0.7.26.1/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-08 19:14:51.879652 odlabel-0.7.26.1/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-08 19:12:05.000000 odlabel-0.7.26.1/setup.py
```

### Comparing `odlabel-0.7.26/LICENSE` & `odlabel-0.7.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/PKG-INFO` & `odlabel-0.7.26.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26
+Version: 0.7.26.1
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/9fb27b28-eab1-4edb-9c1d-0535c4e0e99a)
 
 # ODLabel
 
@@ -130,12 +130,14 @@
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
 
+ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-0.7.26/README.md` & `odlabel-0.7.26.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,10 +109,12 @@
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
 
+ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-0.7.26/app/main_window.py` & `odlabel-0.7.26.1/app/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/chart_worker.py` & `odlabel-0.7.26.1/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/detection_worker.py` & `odlabel-0.7.26.1/app/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.1/app/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.1/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/utils/draw_utils.py` & `odlabel-0.7.26.1/app/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/app/workers/utils/write_utils.py` & `odlabel-0.7.26.1/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/odlabel.egg-info/PKG-INFO` & `odlabel-0.7.26.1/odlabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26
+Version: 0.7.26.1
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/9fb27b28-eab1-4edb-9c1d-0535c4e0e99a)
 
 # ODLabel
 
@@ -130,12 +130,14 @@
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
 
+ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-0.7.26/odlabel.egg-info/SOURCES.txt` & `odlabel-0.7.26.1/odlabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26/setup.py` & `odlabel-0.7.26.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26",
+    version="0.7.26.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
@@ -26,15 +26,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/Ziad-Algrafi/odlabel",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     setup_requires=["setuptools>=38.6.0", "wheel"],
 )
```

