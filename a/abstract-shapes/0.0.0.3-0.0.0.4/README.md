# Comparing `tmp/abstract_shapes-0.0.0.3.tar.gz` & `tmp/abstract_shapes-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_shapes-0.0.0.3.tar", last modified: Wed May  8 21:41:00 2024, max compression
+gzip compressed data, was "abstract_shapes-0.0.0.4.tar", last modified: Wed May  8 21:45:03 2024, max compression
```

## Comparing `abstract_shapes-0.0.0.3.tar` & `abstract_shapes-0.0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      569 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.3/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      949 2024-05-08 21:40:45.000000 abstract_shapes-0.0.0.3/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/src/abstract_shapes/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      120 2024-05-08 21:40:35.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/abstractShapeManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/cardinalDirections.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/direction.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/fileAssociations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3409 2024-05-08 21:33:02.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/file_associations.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes/transform.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:41:00.488184 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      569 2024-05-08 21:41:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:41:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:41:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       36 2024-05-08 21:41:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:41:00.000000 abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      548 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.4/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      941 2024-05-08 21:44:59.000000 abstract_shapes-0.0.0.4/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/src/abstract_shapes/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      120 2024-05-08 21:40:35.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/abstractShapeManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/cardinalDirections.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/direction.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/fileAssociations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3409 2024-05-08 21:33:02.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/file_associations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.4/src/abstract_shapes/transform.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:45:03.825811 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      548 2024-05-08 21:45:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:45:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:45:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       30 2024-05-08 21:45:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:45:03.000000 abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/top_level.txt
```

### Comparing `abstract_shapes-0.0.0.3/PKG-INFO` & `abstract_shapes-0.0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: osgeo
 Requires-Dist: shapely
 Requires-Dist: abstract_pandas
 Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

### Comparing `abstract_shapes-0.0.0.3/setup.py` & `abstract_shapes-0.0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_shapes',
-    version='0.0.0.3',
+    version='0.0.0.4',
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
-    install_requires=['osgeo','shapely','abstract_pandas','osgeo'],
+    install_requires=['shapely','abstract_pandas','osgeo'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/abstractShapeManager.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/abstractShapeManager.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/cardinalDirections.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/cardinalDirections.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/direction.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/direction.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/fileAssociations.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/fileAssociations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/file_associations.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/file_associations.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes/transform.py` & `abstract_shapes-0.0.0.4/src/abstract_shapes/transform.py`

 * *Files identical despite different names*

### Comparing `abstract_shapes-0.0.0.3/src/abstract_shapes.egg-info/PKG-INFO` & `abstract_shapes-0.0.0.4/src/abstract_shapes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: osgeo
 Requires-Dist: shapely
 Requires-Dist: abstract_pandas
 Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

