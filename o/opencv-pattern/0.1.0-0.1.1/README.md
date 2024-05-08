# Comparing `tmp/opencv_pattern-0.1.0.tar.gz` & `tmp/opencv_pattern-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_pattern-0.1.0.tar", last modified: Tue Apr 30 14:50:27 2024, max compression
+gzip compressed data, was "opencv_pattern-0.1.1.tar", last modified: Wed May  8 09:05:59 2024, max compression
```

## Comparing `opencv_pattern-0.1.0.tar` & `opencv_pattern-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-30 14:50:27.090440 opencv_pattern-0.1.0/
--rw-r--r--   0 alfie      (501) staff       (20)     1068 2024-04-30 13:20:45.000000 opencv_pattern-0.1.0/LICENSE
--rw-r--r--   0 alfie      (501) staff       (20)     5223 2024-04-30 14:50:27.090209 opencv_pattern-0.1.0/PKG-INFO
--rw-r--r--   0 alfie      (501) staff       (20)     4591 2024-04-30 14:47:53.000000 opencv_pattern-0.1.0/README.md
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-30 14:50:27.088828 opencv_pattern-0.1.0/opencv_pattern/
--rw-r--r--   0 alfie      (501) staff       (20)        0 2024-04-30 13:25:23.000000 opencv_pattern-0.1.0/opencv_pattern/__init__.py
--rwxr-xr-x   0 alfie      (501) staff       (20)    18885 2024-04-30 14:43:39.000000 opencv_pattern-0.1.0/opencv_pattern/gen_pattern.py
--rwxr-xr-x   0 alfie      (501) staff       (20)   163481 2024-04-30 13:25:34.000000 opencv_pattern-0.1.0/opencv_pattern/svgfig.py
--rw-r--r--   0 alfie      (501) staff       (20)     8499 2024-04-30 13:36:42.000000 opencv_pattern-0.1.0/opencv_pattern/test_charuco_board.py
--rw-r--r--   0 alfie      (501) staff       (20)     3983 2024-04-30 13:25:34.000000 opencv_pattern-0.1.0/opencv_pattern/tests_common.py
-drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-04-30 14:50:27.089945 opencv_pattern-0.1.0/opencv_pattern.egg-info/
--rw-r--r--   0 alfie      (501) staff       (20)     5223 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/PKG-INFO
--rw-r--r--   0 alfie      (501) staff       (20)      412 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/SOURCES.txt
--rw-r--r--   0 alfie      (501) staff       (20)        1 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/dependency_links.txt
--rw-r--r--   0 alfie      (501) staff       (20)       66 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/entry_points.txt
--rw-r--r--   0 alfie      (501) staff       (20)       38 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/requires.txt
--rw-r--r--   0 alfie      (501) staff       (20)       15 2024-04-30 14:50:27.000000 opencv_pattern-0.1.0/opencv_pattern.egg-info/top_level.txt
--rw-r--r--   0 alfie      (501) staff       (20)      888 2024-04-30 14:47:44.000000 opencv_pattern-0.1.0/pyproject.toml
--rw-r--r--   0 alfie      (501) staff       (20)       38 2024-04-30 14:50:27.090517 opencv_pattern-0.1.0/setup.cfg
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-08 09:05:59.776472 opencv_pattern-0.1.1/
+-rw-r--r--   0 alfie      (501) staff       (20)     1068 2024-04-30 13:20:45.000000 opencv_pattern-0.1.1/LICENSE
+-rw-r--r--   0 alfie      (501) staff       (20)     5223 2024-05-08 09:05:59.776215 opencv_pattern-0.1.1/PKG-INFO
+-rw-r--r--   0 alfie      (501) staff       (20)     4591 2024-05-08 09:01:46.000000 opencv_pattern-0.1.1/README.md
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-08 09:05:59.774972 opencv_pattern-0.1.1/opencv_pattern/
+-rw-r--r--   0 alfie      (501) staff       (20)        0 2024-04-30 13:25:23.000000 opencv_pattern-0.1.1/opencv_pattern/__init__.py
+-rwxr-xr-x   0 alfie      (501) staff       (20)    18885 2024-04-30 14:43:39.000000 opencv_pattern-0.1.1/opencv_pattern/gen_pattern.py
+-rwxr-xr-x   0 alfie      (501) staff       (20)   163481 2024-04-30 13:25:34.000000 opencv_pattern-0.1.1/opencv_pattern/svgfig.py
+-rw-r--r--   0 alfie      (501) staff       (20)     8499 2024-04-30 13:36:42.000000 opencv_pattern-0.1.1/opencv_pattern/test_charuco_board.py
+-rw-r--r--   0 alfie      (501) staff       (20)     3983 2024-04-30 13:25:34.000000 opencv_pattern-0.1.1/opencv_pattern/tests_common.py
+drwxr-xr-x   0 alfie      (501) staff       (20)        0 2024-05-08 09:05:59.775919 opencv_pattern-0.1.1/opencv_pattern.egg-info/
+-rw-r--r--   0 alfie      (501) staff       (20)     5223 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/PKG-INFO
+-rw-r--r--   0 alfie      (501) staff       (20)      412 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/SOURCES.txt
+-rw-r--r--   0 alfie      (501) staff       (20)        1 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/dependency_links.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       60 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/entry_points.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       38 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/requires.txt
+-rw-r--r--   0 alfie      (501) staff       (20)       15 2024-05-08 09:05:59.000000 opencv_pattern-0.1.1/opencv_pattern.egg-info/top_level.txt
+-rw-r--r--   0 alfie      (501) staff       (20)      882 2024-05-08 09:05:23.000000 opencv_pattern-0.1.1/pyproject.toml
+-rw-r--r--   0 alfie      (501) staff       (20)       38 2024-05-08 09:05:59.776515 opencv_pattern-0.1.1/setup.cfg
```

### Comparing `opencv_pattern-0.1.0/LICENSE` & `opencv_pattern-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/PKG-INFO` & `opencv_pattern-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_pattern
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple OpenCV pattern generation python package
 Author: Alfie
 Project-URL: Homepage, https://github.com/alfieroddan/pattern-generation-opencv
 Project-URL: Bug Tracker, https://github.com/alfieroddan/pattern-generation-opencv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencv_pattern-0.1.0/README.md` & `opencv_pattern-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/opencv_pattern/gen_pattern.py` & `opencv_pattern-0.1.1/opencv_pattern/gen_pattern.py`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/opencv_pattern/svgfig.py` & `opencv_pattern-0.1.1/opencv_pattern/svgfig.py`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/opencv_pattern/test_charuco_board.py` & `opencv_pattern-0.1.1/opencv_pattern/test_charuco_board.py`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/opencv_pattern/tests_common.py` & `opencv_pattern-0.1.1/opencv_pattern/tests_common.py`

 * *Files identical despite different names*

### Comparing `opencv_pattern-0.1.0/opencv_pattern.egg-info/PKG-INFO` & `opencv_pattern-0.1.1/opencv_pattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv_pattern
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple OpenCV pattern generation python package
 Author: Alfie
 Project-URL: Homepage, https://github.com/alfieroddan/pattern-generation-opencv
 Project-URL: Bug Tracker, https://github.com/alfieroddan/pattern-generation-opencv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencv_pattern-0.1.0/pyproject.toml` & `opencv_pattern-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opencv_pattern"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Alfie"},
 ]
 description = "A simple OpenCV pattern generation python package"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -26,11 +26,11 @@
 "Bug Tracker" = "https://github.com/alfieroddan/pattern-generation-opencv/issues"
 
 [tool.setuptools]
 packages = ["opencv_pattern"]
 include-package-data = true
 
 [project.scripts]
-pattern = "opencv_pattern_tools.gen_pattern:main"
+pattern = "opencv_pattern.gen_pattern:main"
 
 [tool.setuptools.package-data]
 pattern_tools = ["*.json.gz"]
```

