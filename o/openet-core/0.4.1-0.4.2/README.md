# Comparing `tmp/openet-core-0.4.1.tar.gz` & `tmp/openet_core-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet-core-0.4.1.tar", last modified: Tue Mar 19 03:25:24 2024, max compression
+gzip compressed data, was "openet_core-0.4.2.tar", last modified: Tue May  7 22:41:30 2024, max compression
```

## Comparing `openet-core-0.4.1.tar` & `openet_core-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-19 03:25:24.713694 openet-core-0.4.1/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2967 2024-03-19 03:25:24.713381 openet-core-0.4.1/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2337 2024-03-05 20:31:20.000000 openet-core-0.4.1/README.rst
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-19 03:25:24.702394 openet-core-0.4.1/openet/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-09-20 21:11:17.000000 openet-core-0.4.1/openet/__init__.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-19 03:25:24.706658 openet-core-0.4.1/openet/core/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      324 2024-03-05 04:16:16.000000 openet-core-0.4.1/openet/core/__init__.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3346 2024-03-05 04:16:16.000000 openet-core-0.4.1/openet/core/api.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    18001 2024-03-18 22:52:27.000000 openet-core-0.4.1/openet/core/common.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4976 2024-03-05 04:16:16.000000 openet-core-0.4.1/openet/core/ensemble.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    49790 2024-03-12 20:16:00.000000 openet-core-0.4.1/openet/core/interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    12654 2024-03-05 04:16:51.000000 openet-core-0.4.1/openet/core/landsat.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-19 03:25:24.710800 openet-core-0.4.1/openet/core/tests/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet-core-0.4.1/openet/core/tests/conftest.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8196 2024-03-09 19:52:55.000000 openet-core-0.4.1/openet/core/tests/test_common.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8271 2024-03-05 04:16:16.000000 openet-core-0.4.1/openet/core/tests/test_ensemble.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    51588 2024-03-11 21:03:23.000000 openet-core-0.4.1/openet/core/tests/test_interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9351 2024-03-05 04:16:51.000000 openet-core-0.4.1/openet/core/tests/test_landsat.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     7620 2024-03-05 04:16:16.000000 openet-core-0.4.1/openet/core/tests/test_utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    18912 2024-03-07 13:53:45.000000 openet-core-0.4.1/openet/core/utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)   378148 2023-06-06 21:29:21.000000 openet-core-0.4.1/openet/core/wrs2.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-19 03:25:24.712976 openet-core-0.4.1/openet_core.egg-info/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2967 2024-03-19 03:25:24.000000 openet-core-0.4.1/openet_core.egg-info/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      600 2024-03-19 03:25:24.000000 openet-core-0.4.1/openet_core.egg-info/SOURCES.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-03-19 03:25:24.000000 openet-core-0.4.1/openet_core.egg-info/dependency_links.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       56 2024-03-19 03:25:24.000000 openet-core-0.4.1/openet_core.egg-info/requires.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-03-19 03:25:24.000000 openet-core-0.4.1/openet_core.egg-info/top_level.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      995 2024-03-11 21:10:41.000000 openet-core-0.4.1/pyproject.toml
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-03-19 03:25:24.713738 openet-core-0.4.1/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.663577 openet_core-0.4.2/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-07 22:41:30.663185 openet_core-0.4.2/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2338 2024-03-23 18:48:00.000000 openet_core-0.4.2/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.654460 openet_core-0.4.2/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-09-20 21:11:17.000000 openet_core-0.4.2/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.657144 openet_core-0.4.2/openet/core/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      324 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3346 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/api.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17694 2024-05-07 20:34:56.000000 openet_core-0.4.2/openet/core/common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4976 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    49790 2024-03-12 20:16:00.000000 openet_core-0.4.2/openet/core/interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    12654 2024-05-07 20:43:24.000000 openet_core-0.4.2/openet/core/landsat.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.660153 openet_core-0.4.2/openet/core/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-11 21:05:06.000000 openet_core-0.4.2/openet/core/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8123 2024-03-23 18:43:57.000000 openet_core-0.4.2/openet/core/tests/test_a_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9351 2024-03-05 04:16:51.000000 openet_core-0.4.2/openet/core/tests/test_b_landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8849 2024-05-07 21:05:23.000000 openet_core-0.4.2/openet/core/tests/test_common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8271 2024-03-05 04:16:16.000000 openet_core-0.4.2/openet/core/tests/test_ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    51588 2024-03-11 21:03:23.000000 openet_core-0.4.2/openet/core/tests/test_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    18851 2024-03-24 05:24:24.000000 openet_core-0.4.2/openet/core/utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)   378148 2023-06-06 21:29:21.000000 openet_core-0.4.2/openet/core/wrs2.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-07 22:41:30.662726 openet_core-0.4.2/openet_core.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2968 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      604 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       56 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-05-07 22:41:30.000000 openet_core-0.4.2/openet_core.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      995 2024-05-07 20:18:43.000000 openet_core-0.4.2/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-05-07 22:41:30.663622 openet_core-0.4.2/setup.cfg
```

### Comparing `openet-core-0.4.1/PKG-INFO` & `openet_core-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: OpenET Core Components
 Author-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-core
 Keywords: OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -77,13 +77,13 @@
     import openet.ssebop
 
 Development and Testing
 =======================
 
 Please see the `CONTRIBUTING.rst <CONTRIBUTING.rst>`__.
 
-.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/test.yml/badge.svg
+.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/tests.yml/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-core
 .. |version| image:: https://badge.fury.io/py/openet-core.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-core
```

### Comparing `openet-core-0.4.1/README.rst` & `openet_core-0.4.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -59,13 +59,13 @@
     import openet.ssebop
 
 Development and Testing
 =======================
 
 Please see the `CONTRIBUTING.rst <CONTRIBUTING.rst>`__.
 
-.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/test.yml/badge.svg
+.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/tests.yml/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-core
 .. |version| image:: https://badge.fury.io/py/openet-core.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-core
```

### Comparing `openet-core-0.4.1/openet/core/api.py` & `openet_core-0.4.2/openet/core/api.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/common.py` & `openet_core-0.4.2/openet/core/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 def landsat_c2_sr_lst_correct(sr_image, ndvi):
     """Apply correction to Collection 2 LST using adjusted ASTER emissivity
 
     Parameters
     ----------
     sr_image : ee.Image
         Image from a Landsat Collection 2 SR image collection
-        with the SPACECRAFT_ID and LANDSAT_SCENE_ID metadata properties
+        with the SPACECRAFT_ID and LANDSAT_PRODUCT_ID metadata properties
         (e.g. LANDSAT/LC08/C02/T1_L2).
     ndvi : ee.Image
         Normalized difference vegetation index (NDVI)
 
     Returns
     -------
     lst : ee.Image
@@ -257,76 +257,70 @@
     c = ee.Dictionary({
         'LANDSAT_4': 0.0272, 'LANDSAT_5': 0.0195, 'LANDSAT_7': 0.0058,
         'LANDSAT_8': 0.0584, 'LANDSAT_9': 0.0457,
     })
 
     def get_matched_c2_t1_image(input_img):
         # Find matching Landsat Collection 2 Tier 1 Level 2 image
-        #   based on the LANDSAT_SCENE_ID property
+        #   based on the "LANDSAT_PRODUCT_ID" property
+        # Build the system:index format scene ID from the LANDSAT_PRODUCT_ID
+        scene_id = ee.List(ee.String(input_img.get('LANDSAT_PRODUCT_ID')).split('_'))
+        scene_id = (
+            ee.String(scene_id.get(0)).cat('_').cat(ee.String(scene_id.get(2)))
+            .cat('_').cat(ee.String(scene_id.get(3)))
+        )
+        # scene_id = ee.String(input_img.get('system:index'))
 
         # Testing if it is any faster to filter each collection separately
         # TODO: Test if adding an extra .filterDate() call helps
-        scene_id = input_img.get('LANDSAT_SCENE_ID')
         return ee.Image(
             ee.ImageCollection('LANDSAT/LC09/C02/T1_L2')
-            .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id))
+            .filter(ee.Filter.eq('system:index', scene_id))
             .merge(ee.ImageCollection('LANDSAT/LC08/C02/T1_L2')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LE07/C02/T1_L2')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LT05/C02/T1_L2')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LT04/C02/T1_L2')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .first()
         )
-        # return ee.Image(
-        #     ee.ImageCollection('LANDSAT/LC09/C02/T1_L2')
-        #     .merge(ee.ImageCollection('LANDSAT/LC08/C02/T1_L2'))
-        #     .merge(ee.ImageCollection('LANDSAT/LE07/C02/T1_L2'))
-        #     .merge(ee.ImageCollection('LANDSAT/LT05/C02/T1_L2'))
-        #     .merge(ee.ImageCollection('LANDSAT/LT04/C02/T1_L2'))
-        #     .filter(ee.Filter.eq('LANDSAT_SCENE_ID', input_img.get('LANDSAT_SCENE_ID')))
-        #     .first()
-        # )
 
     def get_matched_c2_t1_radiance_image(input_img):
-        # Find matching Landsat Collection 2 Tier 1 radiance (and RT) image
-        #   based on the LANDSAT_SCENE_ID property
+        # Find matching Landsat Collection 2 Tier 1 Level 2 image
+        #   based on the "LANDSAT_PRODUCT_ID" property
+        # Build the system:index format scene ID from the LANDSAT_PRODUCT_ID
+        satellite = ee.String(input_img.get('SPACECRAFT_ID'))
+        scene_id = ee.List(ee.String(input_img.get('LANDSAT_PRODUCT_ID')).split('_'))
+        scene_id = (
+            ee.String(scene_id.get(0)).cat('_').cat(ee.String(scene_id.get(2)))
+            .cat('_').cat(ee.String(scene_id.get(3)))
+        )
+        # scene_id = ee.String(input_img.get('system:index'))
 
         # TODO: Fix error when images that are in the T1_L2 collections but not in the T1,
         #  will fail with a .get() error because matched_img is 'None',
         #  could cause issues if trying to map over a collection
-        satellite = ee.String(input_img.get('SPACECRAFT_ID'))
-        scene_id = ee.String(input_img.get('LANDSAT_SCENE_ID'))
 
         #  Testing if it is any faster to filter each collection separately
         # TODO: Test if adding an extra .filterDate() call helps
         matched_img = ee.Image(
             ee.ImageCollection('LANDSAT/LC09/C02/T1')
-            .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id))
+            .filter(ee.Filter.eq('system:index', scene_id))
             .merge(ee.ImageCollection('LANDSAT/LC08/C02/T1_RT')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LE07/C02/T1')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LT05/C02/T1')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .merge(ee.ImageCollection('LANDSAT/LT04/C02/T1')
-                   .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id)))
+                   .filter(ee.Filter.eq('system:index', scene_id)))
             .first()
         )
-        # matched_img = ee.Image(
-        #     ee.ImageCollection('LANDSAT/LC09/C02/T1')
-        #     .merge(ee.ImageCollection('LANDSAT/LC08/C02/T1_RT'))
-        #     .merge(ee.ImageCollection('LANDSAT/LE07/C02/T1'))
-        #     .merge(ee.ImageCollection('LANDSAT/LT05/C02/T1'))
-        #     .merge(ee.ImageCollection('LANDSAT/LT04/C02/T1'))
-        #     .filter(ee.Filter.eq('LANDSAT_SCENE_ID', scene_id))
-        #     .first()
-        # )
 
         input_bands = ee.Dictionary({
             'LANDSAT_4': ['B1', 'B2', 'B3', 'B4', 'B5', 'B7', 'B6'],
             'LANDSAT_5': ['B1', 'B2', 'B3', 'B4', 'B5', 'B7', 'B6'],
             'LANDSAT_7': ['B1', 'B2', 'B3', 'B4', 'B5', 'B7', 'B6_VCID_1'],
             'LANDSAT_8': ['B2', 'B3', 'B4', 'B5', 'B6', 'B7', 'B10'],
             'LANDSAT_9': ['B2', 'B3', 'B4', 'B5', 'B6', 'B7', 'B10'],
```

### Comparing `openet-core-0.4.1/openet/core/ensemble.py` & `openet_core-0.4.2/openet/core/ensemble.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/interpolate.py` & `openet_core-0.4.2/openet/core/interpolate.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/landsat.py` & `openet_core-0.4.2/openet/core/landsat.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/tests/conftest.py` & `openet_core-0.4.2/openet/core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/tests/test_common.py` & `openet_core-0.4.2/openet/core/tests/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,20 +153,32 @@
         # This scene (and path/row) is having issues when used in the LST sharpening
         # Test four points in each quadrant of the scene and one point outside
         ['LANDSAT/LC08/C02/T1_L2/LC08_035031_20160714', [-107.4, 42.2], 321.0, 321.2],
         ['LANDSAT/LC08/C02/T1_L2/LC08_035031_20160714', [-106.3, 42.0], 323.0, 323.2],
         ['LANDSAT/LC08/C02/T1_L2/LC08_035031_20160714', [-107.4, 41.5], 318.0, 317.8],
         ['LANDSAT/LC08/C02/T1_L2/LC08_035031_20160714', [-106.5, 41.3], 306.0, 305.9],
         ['LANDSAT/LC08/C02/T1_L2/LC08_035031_20160714', [-107.9, 42.6], None, None],
+        # This scene will not run if matching collections are built using the LANDSAT_SCENE_ID
+        # since the ID has a different version number in the TOA and radiance collections
+        ['LANDSAT/LC09/C02/T1_L2/LC09_035025_20230608', [-103.5, 50.4], 306.55, 306.55],
     ]
 )
 def test_landsat_c2_sr_lst_correct_values(image_id, xy, expected, uncorrected, tol=0.25):
     input_img = ee.Image(image_id)
     ndvi_img = input_img.multiply(0.0000275).add(-0.2).normalizedDifference(['SR_B5', 'SR_B4'])
     # lst_img = input_img.select(['ST_B10']).multiply(0.00341802).add(149.0)
     # original = utils.point_image_value(lst_img, xy, scale=30)['ST_B10']
     output_img = common.landsat_c2_sr_lst_correct(input_img, ndvi_img)
     corrected = utils.point_image_value(output_img, xy, scale=30)
     if expected is None:
         assert corrected['lst'] is None
     else:
         assert abs(corrected['lst'] - expected) <= tol
+
+
+def test_landsat_c2_sr_lst_correct_no_toa():
+    input_img = ee.Image('LANDSAT/LE07/C02/T1_L2/LE07_030026_20200628')
+    output_img = common.landsat_c2_sr_lst_correct(
+        input_img, input_img.multiply(0.0000275).add(-0.2).normalizedDifference(['SR_B4', 'SR_B3'])
+    )
+    with pytest.raises(Exception):
+        utils.point_coll_value(output_img, [-96.7, 48.9], scale=30)
```

### Comparing `openet-core-0.4.1/openet/core/tests/test_ensemble.py` & `openet_core-0.4.2/openet/core/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/tests/test_interpolate.py` & `openet_core-0.4.2/openet/core/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/tests/test_landsat.py` & `openet_core-0.4.2/openet/core/tests/test_b_landsat.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet/core/tests/test_utils.py` & `openet_core-0.4.2/openet/core/tests/test_a_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -216,32 +216,44 @@
     assert abs(output['foo'] - expected) <= tol
     assert abs(output['bar'] - (expected + 1)) <= tol
 
 
 @pytest.mark.parametrize(
     'image_id, xy, scale, expected, tol',
     [
-        ['USGS/NED', [-106.03249, 37.17777], 10, 2364.351, 0.001],
-        ['USGS/NED', [-106.03249, 37.17777], 1, 2364.351, 0.001],
+        ['USGS/3DEP/10m', [-106.03249, 37.17777], 30, 2364.169, 0.001],
+        ['USGS/3DEP/10m', [-106.03249, 37.17777], 10, 2364.138, 0.001],
+        ['USGS/3DEP/10m', [-106.03249, 37.17777], 1, 2364.138, 0.001],
+        ['NASA/NASADEM_HGT/001', [-106.03249, 37.17777], 30, 2361, 0.001],
     ]
 )
 def test_point_image_value(image_id, xy, scale, expected, tol):
-    output = utils.point_image_value(ee.Image(image_id).rename('output'), xy)
+    output = utils.point_image_value(
+        ee.Image(image_id).select(['elevation'], ['output']), xy, scale
+    )
     assert abs(output['output'] - expected) <= tol
 
 
 @pytest.mark.parametrize(
     'image_id, image_date, xy, scale, expected, tol',
     [
-        # CGM - This test stopped working for a scale of 1 and returns a different
-        #   value for a scale of 10 than the point_image_value() function above.
-        # This function uses getRegion() instead of a reduceRegion() call,
-        #   so there might have been some sort of change in getRegion().
-        ['USGS/NED', '2012-04-04', [-106.03249, 37.17777], 10, 2364.286, 0.001],
-        # CGM - The default scale of 1 now returns None/Null for some reason
-        # ['USGS/NED', '2012-04-04', [-106.03249, 37.17777], 1, 2364.351, 0.001],
+        ['USGS/3DEP/10m', '2012-04-04', [-106.03249, 37.17777], 30, 2364.169, 0.001],
+        ['USGS/3DEP/10m', '2012-04-04', [-106.03249, 37.17777], 10, 2364.097, 0.001],
+        ['USGS/3DEP/10m', '2012-04-04', [-106.03249, 37.17777], 1, 2364.138, 0.001],
+        ['NASA/NASADEM_HGT/001', '2012-04-04', [-106.03249, 37.17777], 30, 2361, 0.001],
     ]
 )
 def test_point_coll_value(image_id, image_date, xy, scale, expected, tol):
-    input_img = ee.Image(image_id).rename(['output'])
+    # The image must have a system:time_start for this function to work correctly
+    input_img = (
+        ee.Image(image_id).select(['elevation'], ['output'])
+        .set({'system:time_start': ee.Date(image_date).millis()})
+    )
     output = utils.point_coll_value(ee.ImageCollection([input_img]), xy, scale)
     assert abs(output['output'][image_date] - expected) <= tol
+
+
+def test_point_coll_value_no_system_time_start_exception():
+    # The function should raise an exception for images with no system:time_start
+    input_img = ee.Image('USGS/3DEP/10m').select(['elevation'], ['output'])
+    with pytest.raises(Exception):
+        utils.point_coll_value(ee.ImageCollection([input_img]), [-106, 37], 30)
```

### Comparing `openet-core-0.4.1/openet/core/utils.py` & `openet_core-0.4.2/openet/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,48 +515,47 @@
             output.append('{},{}'.format(b[0][1], b[-1][1]))
         else:
             output.append('{}'.format(b[0][1]))
 
     return ','.join(output)
 
 
-# Should these be test fixtures instead?
-# I'm not sure how to make them fixtures and allow input parameters
 def constant_image_value(image, crs='EPSG:32613', scale=1):
-    """Extract the output value from a calculation done with constant images"""
+    """Extract the output value from a "constant" image"""
     rr_params = {
         'reducer': ee.Reducer.first(),
         'geometry': ee.Geometry.Rectangle([0, 0, 10, 10], crs, False),
         'scale': scale,
     }
     return get_info(ee.Image(image).reduceRegion(**rr_params))
 
 
 def point_image_value(image, xy, scale=1):
-    """Extract the output value from a calculation at a point"""
+    """Extract the output value from an image at a point"""
     rr_params = {
         'reducer': ee.Reducer.first(),
         'geometry': ee.Geometry.Point(xy),
         'scale': scale,
     }
     return get_info(ee.Image(image).reduceRegion(**rr_params))
 
 
 def point_coll_value(coll, xy, scale=1):
-    """Extract the output value from a calculation at a point"""
+    """Extract the output value from a collection at a point"""
     output = get_info(coll.getRegion(ee.Geometry.Point(xy), scale=scale))
-
     # Structure output to easily be converted to a Pandas dataframe
     # First key is band name, second key is the date string
     col_dict = {}
     info_dict = {}
     for i, k in enumerate(output[0][4:]):
         col_dict[k] = i + 4
         info_dict[k] = {}
+
     for row in output[1:]:
+        # TODO: Add support for images that don't have a system:time_start
         date = datetime.utcfromtimestamp(row[3] / 1000.0).strftime('%Y-%m-%d')
         for k, v in col_dict.items():
             info_dict[k][date] = row[col_dict[k]]
 
     return info_dict
     # return pd.DataFrame.from_dict(info_dict)
```

### Comparing `openet-core-0.4.1/openet/core/wrs2.py` & `openet_core-0.4.2/openet/core/wrs2.py`

 * *Files identical despite different names*

### Comparing `openet-core-0.4.1/openet_core.egg-info/PKG-INFO` & `openet_core-0.4.2/openet_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: OpenET Core Components
 Author-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-core
 Keywords: OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -77,13 +77,13 @@
     import openet.ssebop
 
 Development and Testing
 =======================
 
 Please see the `CONTRIBUTING.rst <CONTRIBUTING.rst>`__.
 
-.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/test.yml/badge.svg
+.. |build| image:: https://github.com/Open-ET/openet-core/actions/workflows/tests.yml/badge.svg
    :alt: Build status
    :target: https://github.com/Open-ET/openet-core
 .. |version| image:: https://badge.fury.io/py/openet-core.svg
    :alt: Latest version on PyPI
    :target: https://badge.fury.io/py/openet-core
```

### Comparing `openet-core-0.4.1/openet_core.egg-info/SOURCES.txt` & `openet_core-0.4.2/openet_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 openet/core/common.py
 openet/core/ensemble.py
 openet/core/interpolate.py
 openet/core/landsat.py
 openet/core/utils.py
 openet/core/wrs2.py
 openet/core/tests/conftest.py
+openet/core/tests/test_a_utils.py
+openet/core/tests/test_b_landsat.py
 openet/core/tests/test_common.py
 openet/core/tests/test_ensemble.py
 openet/core/tests/test_interpolate.py
-openet/core/tests/test_landsat.py
-openet/core/tests/test_utils.py
 openet_core.egg-info/PKG-INFO
 openet_core.egg-info/SOURCES.txt
 openet_core.egg-info/dependency_links.txt
 openet_core.egg-info/requires.txt
 openet_core.egg-info/top_level.txt
```

### Comparing `openet-core-0.4.1/pyproject.toml` & `openet_core-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openet-core"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
     { name="Charles Morton", email="charles.morton@dri.edu" },
 ]
 description = "OpenET Core Components"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["OpenET", "Earth Engine", "Evapotranspiration", "Landsat"]
```

