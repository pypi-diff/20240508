# Comparing `tmp/abstract_shapes-0.0.0.1.tar.gz` & `tmp/abstract_shapes-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_shapes-0.0.0.1.tar", last modified: Tue May  7 03:09:55 2024, max compression
+gzip compressed data, was "abstract_shapes-0.0.0.2.tar", last modified: Wed May  8 21:39:32 2024, max compression
```

## Comparing `abstract_shapes-0.0.0.1.tar` & `abstract_shapes-0.0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      517 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.1/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      923 2024-05-07 03:07:41.000000 abstract_shapes-0.0.0.1/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/src/abstract_shapes/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       30 2024-05-07 03:09:46.000000 abstract_shapes-0.0.0.1/src/abstract_shapes/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3280 2024-05-07 03:07:52.000000 abstract_shapes-0.0.0.1/src/abstract_shapes/transform.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-07 03:09:55.830937 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      517 2024-05-07 03:09:55.000000 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      297 2024-05-07 03:09:55.000000 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-07 03:09:55.000000 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       14 2024-05-07 03:09:55.000000 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-07 03:09:55.000000 abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      569 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_shapes-0.0.0.2/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      949 2024-05-08 21:39:17.000000 abstract_shapes-0.0.0.2/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/src/abstract_shapes/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       30 2024-05-07 03:09:46.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2565 2024-05-08 21:37:06.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/abstractShapeManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3664 2024-05-08 21:34:26.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/cardinalDirections.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5311 2024-05-08 21:39:03.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/direction.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2297 2024-05-08 20:51:19.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/fileAssociations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3409 2024-05-08 21:33:02.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/file_associations.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3377 2024-05-08 21:36:00.000000 abstract_shapes-0.0.0.2/src/abstract_shapes/transform.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-08 21:39:32.453030 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      569 2024-05-08 21:39:32.000000 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      497 2024-05-08 21:39:32.000000 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-08 21:39:32.000000 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       36 2024-05-08 21:39:32.000000 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-08 21:39:32.000000 abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/top_level.txt
```

### Comparing `abstract_shapes-0.0.0.1/PKG-INFO` & `abstract_shapes-0.0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: osgeo
 Requires-Dist: shapely
+Requires-Dist: abstract_pandas
+Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

### Comparing `abstract_shapes-0.0.0.1/setup.py` & `abstract_shapes-0.0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_shapes',
-    version='0.0.0.1',
+    version='0.0.0.2',
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
-    install_requires=['osgeo','shapely'],
+    install_requires=['osgeo','shapely','abstract_pandas','osgeo'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

### Comparing `abstract_shapes-0.0.0.1/src/abstract_shapes/transform.py` & `abstract_shapes-0.0.0.2/src/abstract_shapes/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,7 +69,10 @@
         # Check if the new geometry is different from the existing geometry
         if not existing_geom.equals(new_geom):
             gdf.at[index, 'geometry'] = new_geom
             print(f"Updated row {index} with new geometry.")
         else:
             print(f"No update needed for row {index}.")
         return gdf
+def update_geop_json(desig,epsg=4326):
+    gdj = get_shp(desig).to_crs(epsg=epsg)
+    return gdj
```

### Comparing `abstract_shapes-0.0.0.1/src/abstract_shapes.egg-info/PKG-INFO` & `abstract_shapes-0.0.0.2/src/abstract_shapes.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: abstract_shapes
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: osgeo
 Requires-Dist: shapely
+Requires-Dist: abstract_pandas
+Requires-Dist: osgeo
 
 #magnets... how do they work? who invented them?
```

