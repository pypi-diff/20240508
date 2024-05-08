# Comparing `tmp/yolosegment2labelme-0.0.2.tar.gz` & `tmp/yolosegment2labelme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolosegment2labelme-0.0.2.tar", last modified: Tue May  7 17:44:55 2024, max compression
+gzip compressed data, was "yolosegment2labelme-0.0.3.tar", last modified: Tue May  7 19:34:58 2024, max compression
```

## Comparing `yolosegment2labelme-0.0.2.tar` & `yolosegment2labelme-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 17:44:55.026029 yolosegment2labelme-0.0.2/
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1073 2024-05-07 11:28:57.000000 yolosegment2labelme-0.0.2/LICENSE
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     4085 2024-05-07 17:44:55.025965 yolosegment2labelme-0.0.2/PKG-INFO
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     3220 2024-05-07 12:12:44.000000 yolosegment2labelme-0.0.2/README.md
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)      510 2024-05-07 17:44:51.000000 yolosegment2labelme-0.0.2/pyproject.toml
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       79 2024-05-07 17:44:55.026245 yolosegment2labelme-0.0.2/setup.cfg
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1551 2024-05-07 17:39:39.000000 yolosegment2labelme-0.0.2/setup.py
-drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 17:44:55.024672 yolosegment2labelme-0.0.2/yolosegment2labelme/
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 11:40:53.000000 yolosegment2labelme-0.0.2/yolosegment2labelme/__init__.py
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     3150 2024-05-07 11:42:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme/polygon_saver.py
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1028 2024-05-07 17:30:51.000000 yolosegment2labelme-0.0.2/yolosegment2labelme/yolosegment2labelme.py
-drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 17:44:55.025652 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     4085 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/PKG-INFO
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)      423 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/SOURCES.txt
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)        1 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/dependency_links.txt
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       85 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/entry_points.txt
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       39 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/requires.txt
--rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       20 2024-05-07 17:44:54.000000 yolosegment2labelme-0.0.2/yolosegment2labelme.egg-info/top_level.txt
+drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 19:34:58.284658 yolosegment2labelme-0.0.3/
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1073 2024-05-07 11:28:57.000000 yolosegment2labelme-0.0.3/LICENSE
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     5366 2024-05-07 19:34:58.284590 yolosegment2labelme-0.0.3/PKG-INFO
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     4501 2024-05-07 19:25:23.000000 yolosegment2labelme-0.0.3/README.md
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)      510 2024-05-07 19:34:05.000000 yolosegment2labelme-0.0.3/pyproject.toml
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       79 2024-05-07 19:34:58.284955 yolosegment2labelme-0.0.3/setup.cfg
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1551 2024-05-07 19:34:46.000000 yolosegment2labelme-0.0.3/setup.py
+drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 19:34:58.282959 yolosegment2labelme-0.0.3/yolosegment2labelme/
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 11:40:53.000000 yolosegment2labelme-0.0.3/yolosegment2labelme/__init__.py
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     3150 2024-05-07 11:42:54.000000 yolosegment2labelme-0.0.3/yolosegment2labelme/polygon_saver.py
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     1028 2024-05-07 17:30:51.000000 yolosegment2labelme-0.0.3/yolosegment2labelme/yolosegment2labelme.py
+drwxr-xr-x   0 aboniasojasingarayar   (501) staff       (20)        0 2024-05-07 19:34:58.284173 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)     5366 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/PKG-INFO
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)      423 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/SOURCES.txt
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)        1 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/dependency_links.txt
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       85 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/entry_points.txt
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       39 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/requires.txt
+-rw-r--r--   0 aboniasojasingarayar   (501) staff       (20)       20 2024-05-07 19:34:58.000000 yolosegment2labelme-0.0.3/yolosegment2labelme.egg-info/top_level.txt
```

### Comparing `yolosegment2labelme-0.0.2/LICENSE` & `yolosegment2labelme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yolosegment2labelme-0.0.2/PKG-INFO` & `yolosegment2labelme-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-Metadata-Version: 2.1
-Name: yolosegment2labelme
-Version: 0.0.2
-Summary: A small example package
-Home-page: https://github.com/Abonia1/yolosegment2labelme
-Download-URL: https://github.com/Abonia1/yolosegment2labelme/archive/refs/tags/v2.0.zip
-Author: Abonia Sojasingarayar
-Author-email: Abonia Sojasingarayar <aboniaa@gmail.com>
-Project-URL: Homepage, https://github.com/Abonia1/yolosegment2labelme
-Project-URL: Issues, https://github.com/Abonia1/yolosegment2labelme/issues
-Keywords: python,yolo,segmentation,json,labelme,anylabeling
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: pillow
-Requires-Dist: ultralytics
+# YOLO Prediction to Labelme and Anylabeling Json
 
-# yolosegment2labelme
+<p align="center">
+  <img alt="yolosegment2labelme" style="width: 128px; max-width: 100%; height: auto;" src="images/labelme_test/logo.png"/>
+  <h1 align="center">🌟 yolosegment2labelme 🌟</h1>
+  <p align="center">Convert your yolo model prediction results to json to view and edit in Labelme and Anylabeling. <b>YOLO Result to Json with single line cmd</b>!</p>
+  <p align="center"><b>yolosegment2labelme = Easy Coversion + Predicted to Json  + Auto-labeling</b></p>
+</p>
+
+![](https://user-images.githubusercontent.com/18329471/234640541-a6a65fbc-d7a5-4ec3-9b65-55305b01a7aa.png)
+
+[![PyPI](https://img.shields.io/pypi/v/yolosegment2labelme)](https://pypi.org/project/yolosegment2labelme/)
+[![license](https://img.shields.io/github/license/abonia1/yolosegment2labelme.svg)](https://github.com/Abonia1/yolosegment2labelme/blob/main/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/abonia1/yolosegment2labelme.svg)](https://github.com/abonia1/yolosegment2labelme/issues)
+[![Article](https://img.shields.io/badge/Read-Documentation-green)](https://abonia1.github.io/)
+[![Follow](https://img.shields.io/badge/+Follow-abonia-blue)](https://www.linkedin.com/in/aboniasojasingarayar/)
+
+> ⭐ Follow [AboniaSojasingarayar](https://www.linkedin.com/in/aboniasojasingarayar) for project updates.
 
 **yolosegment2labelme** is a Python package that allows you to convert YOLO segmentation prediction results to LabelMe JSON format. This tool facilitates the annotation process by generating JSON files that are compatible with LabelMe and other labeling annotation tools.
 
 ## Features
 
 - Convert YOLO segmentation prediction results to LabelMe JSON format.
 - Compatible with various YOLO models.
@@ -51,22 +46,20 @@
 
 or with custom yolo segmentation model
 
 ```bash
 yolosegment2labelme --model yolov8n-seg.pt --images /path/to/images --conf 0.3
 ```
 
-This command will process the images located in the specified directory (`/path/to/images`), using the YOLO model weights file `yolov8n-seg.pt`, and generate LabelMe JSON files with a confidence threshold of 0.3.
+This command will process the images located in the specified directory (`/path/to/images`), using the YOLO model weights file `yolov8n-seg.pt` and here you can add path/to/your/customYOLOModel, and generate LabelMe JSON files with a confidence threshold of your choice and here it is of 0.3.
 
-For more options and advanced usage, refer to the [documentation](https://github.com/Abonia1/yolosegment2labelme).
 
 ## Sample Images
 The table below displays sample images along with their corresponding annotations generated using yolosegment2labelme:
 
-## Sample Images
 
 | Sample Image 1                                      | Sample Image 2                                      |
 |-----------------------------------------------------|-----------------------------------------------------|
 | ![Sample Image 1](images/labelme_test/sample1.png)      | ![Sample Image 2](images/labelme_test/sample2.png)      |
 | Sample Annotation for Image 1                      | Sample Annotation for Image 2                      |
 
 | Sample Image 3                                      | Sample Image 4                                      |
@@ -89,8 +82,8 @@
 
 ## Authors
 
 - Abonia Sojasingarayar - [GitHub](https://github.com/Abonia1)
 
 ## Support
 
-If you encounter any issues or have questions about **yolosegment2labelme**, please feel free to open an issue on GitHub: [yolosegment2labelme Issues](https://github.com/Abonia1/yolosegment2labelme/issues)
+If you encounter any issues or have questions about **yolosegment2labelme**, please feel free to open an issue on GitHub: [yolosegment2labelme Issues](https://github.com/Abonia1/yolosegment2labelme/issues)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yolosegment2labelme-0.0.2/setup.py` & `yolosegment2labelme-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Yolo segmentation prediction to labelme json'
 LONG_DESCRIPTION = 'A package that allows generating JSON from YOLO prediction results, compatible with LabelMe/any labeling annotation tool'
 
 # Setting up
 setup(
     name="yolosegment2labelme",
     version=VERSION,
```

### Comparing `yolosegment2labelme-0.0.2/yolosegment2labelme/polygon_saver.py` & `yolosegment2labelme-0.0.3/yolosegment2labelme/polygon_saver.py`

 * *Files identical despite different names*

### Comparing `yolosegment2labelme-0.0.2/yolosegment2labelme/yolosegment2labelme.py` & `yolosegment2labelme-0.0.3/yolosegment2labelme/yolosegment2labelme.py`

 * *Files identical despite different names*

