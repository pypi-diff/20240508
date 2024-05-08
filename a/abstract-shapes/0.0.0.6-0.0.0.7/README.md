# Comparing `tmp/abstract_shapes-0.0.0.6.tar.gz` & `tmp/abstract_shapes-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_shapes-0.0.0.6.tar", last modified: Wed May  8 21:47:48 2024, max compression
+gzip compressed data, was "abstract_shapes-0.0.0.7.tar", last modified: Wed May  8 21:48:18 2024, max compression
```

## Comparing `abstract_shapes-0.0.0.6.tar` & `abstract_shapes-0.0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:47:48.084188 abstract_shapes-0.0.0.6/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      548 2024-05-08 21:47:48.084188 abstract_shapes-0.0.0.6/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.6/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:47:48.084188 abstract_shapes-0.0.0.6/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      941 2024-05-08 21:47:39.000000 abstract_shapes-0.0.0.6/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:47:48.080188 abstract_shapes-0.0.0.6/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:47:48.080188 abstract_shapes-0.0.0.6/src/abstract_shapes/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      120 2024-05-08 21:40:35.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/abstractShapeManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/cardinalDirections.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/direction.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/fileAssociations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3397 2024-05-08 21:47:32.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/file_associations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.6/src/abstract_shapes/transform.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:47:48.080188 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      548 2024-05-08 21:47:48.000000 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:47:48.000000 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:47:48.000000 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       30 2024-05-08 21:47:48.000000 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:47:48.000000 abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.7/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      933 2024-05-08 21:48:12.000000 abstract_shapes-0.0.0.7/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/src/abstract_shapes/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      120 2024-05-08 21:40:35.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/abstractShapeManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/cardinalDirections.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/direction.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/fileAssociations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3397 2024-05-08 21:47:32.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/file_associations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.7/src/abstract_shapes/transform.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:48:18.863883 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      527 2024-05-08 21:48:18.000000 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:48:18.000000 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:48:18.000000 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       24 2024-05-08 21:48:18.000000 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:48:18.000000 abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/top_level.txt
```

### Comparing `abstract_shapes-0.0.0.6/PKG-INFO` & `abstract_shapes-0.0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.6
+Version: 0.0.0.7
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: shapely
 Requires-Dist: abstract_pandas
-Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

### Comparing `abstract_shapes-0.0.0.6/setup.py` & `abstract_shapes-0.0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_shapes',
-    version='0.0.0.6',
+    version='0.0.0.7',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
-    install_requires=['shapely','abstract_pandas','osgeo'],
+    install_requires=['shapely','abstract_pandas'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/abstractShapeManager.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/abstractShapeManager.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/cardinalDirections.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/cardinalDirections.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/direction.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/direction.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/fileAssociations.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/fileAssociations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/file_associations.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/file_associations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes/transform.py` & `abstract_shapes-0.0.0.7/src/abstract_shapes/transform.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.6/src/abstract_shapes.egg-info/PKG-INFO` & `abstract_shapes-0.0.0.7/src/abstract_shapes.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.6
+Version: 0.0.0.7
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: shapely
 Requires-Dist: abstract_pandas
-Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

