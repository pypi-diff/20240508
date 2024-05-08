# Comparing `tmp/disko-0.9.5b4.tar.gz` & `tmp/disko-0.9.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disko-0.9.5b4.tar", last modified: Tue Dec  5 19:52:34 2023, max compression
+gzip compressed data, was "disko-0.9.6b2.tar", last modified: Wed May  8 01:55:15 2024, max compression
```

## Comparing `disko-0.9.5b4.tar` & `disko-0.9.6b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 19:52:34.028138 disko-0.9.5b4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-05 19:52:22.000000 disko-0.9.5b4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 19:52:22.000000 disko-0.9.5b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-12-05 19:52:34.028138 disko-0.9.5b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2023-12-05 19:52:22.000000 disko-0.9.5b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 19:52:34.028138 disko-0.9.5b4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2023-12-05 19:52:22.000000 disko-0.9.5b4/bin/disko
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2023-12-05 19:52:22.000000 disko-0.9.5b4/bin/disko_bayes
--rwxr-xr-x   0 runner    (1001) docker     (127)     4141 2023-12-05 19:52:22.000000 disko-0.9.5b4/bin/disko_draw
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2023-12-05 19:52:22.000000 disko-0.9.5b4/bin/disko_svd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 19:52:34.028138 disko-0.9.5b4/disko/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31263 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/disko.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/draw_sky.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 19:52:34.028138 disko-0.9.5b4/disko/fov/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/fov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/fov/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19263 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/healpix_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/multivariate_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/parser_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/projection_lsqr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/sphere_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    16019 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/telescope_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-12-05 19:52:22.000000 disko-0.9.5b4/disko/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 19:52:34.028138 disko-0.9.5b4/disko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-12-05 19:52:34.000000 disko-0.9.5b4/disko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-12-05 19:52:34.000000 disko-0.9.5b4/disko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 19:52:34.000000 disko-0.9.5b4/disko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-05 19:52:34.000000 disko-0.9.5b4/disko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-05 19:52:34.000000 disko-0.9.5b4/disko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-05 19:52:22.000000 disko-0.9.5b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-05 19:52:34.032138 disko-0.9.5b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-05 19:52:22.000000 disko-0.9.5b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:15.623224 disko-0.9.6b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 01:55:11.000000 disko-0.9.6b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:55:11.000000 disko-0.9.6b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 01:55:15.623224 disko-0.9.6b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-08 01:55:11.000000 disko-0.9.6b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:15.619224 disko-0.9.6b2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-08 01:55:11.000000 disko-0.9.6b2/bin/disko
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-08 01:55:11.000000 disko-0.9.6b2/bin/disko_bayes
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5070 2024-05-08 01:55:11.000000 disko-0.9.6b2/bin/disko_draw
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-08 01:55:11.000000 disko-0.9.6b2/bin/disko_svd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:15.619224 disko-0.9.6b2/disko/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31182 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/disko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/draw_sky.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:15.623224 disko-0.9.6b2/disko/fov/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/fov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/fov/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/healpix_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/multivariate_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/parser_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/projection_lsqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/sphere_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/telescope_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-08 01:55:11.000000 disko-0.9.6b2/disko/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:15.623224 disko-0.9.6b2/disko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 01:55:15.000000 disko-0.9.6b2/disko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-08 01:55:15.000000 disko-0.9.6b2/disko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:55:15.000000 disko-0.9.6b2/disko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 01:55:15.000000 disko-0.9.6b2/disko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 01:55:15.000000 disko-0.9.6b2/disko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 01:55:11.000000 disko-0.9.6b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 01:55:15.623224 disko-0.9.6b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-08 01:55:11.000000 disko-0.9.6b2/setup.py
```

### Comparing `disko-0.9.5b4/LICENSE.txt` & `disko-0.9.6b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/PKG-INFO` & `disko-0.9.6b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disko
-Version: 0.9.5b4
+Version: 0.9.6b2
 Summary: Discrete Sky Operator (DiSkO) Aperture Synthesis Radio Imaging
 Home-page: http://github.com/tmolteno/disko
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
@@ -83,16 +83,22 @@
 
 * Add a --full-sphere option which fixes the sphere in celestial coordinates, and then points the phase center of an observation correctly. Requires a beam pattern to be specified (or at least a hemispherical beam). A beam is a sky vector mask. I.e., should fall to zero 'outside' the beam.
 * Deal with flagging, output residuals in a way that can be used to flag in the measurement set. This means some casa expression that changes the MS.
 
 ## Changelog
 
 ```
+0.9.6b2 Fix the --elevation limit to actually implement this for disko draw
+0.9.6b1 Add a minimum elevation to the sphere.el_min_r. This is for setting bounds in imagers.
+        Explicitly manage the tart2ms logging
 0.9.5b4 Add a timestamp to images (or a title if specified) in SVG mode
+        clean up logging so that only happens when --debug is present.
 0.9.5b3 Use gmsh rather than optimesh... (WIP)
+        Use much faster measurement set reading via casa_read_ms() about 200x faster!
+        disko_draw timestamps the image
 0.9.5b2 Fix RA direction in generated FITS files (thanks Ben Hugo)
 0.9.5b1 Add --min and --max to disko_draw so allow manual setting the range of images
 0.9.4b6 Fix bug in drawing PDF.
 0.9.4b5 Import Resolution in disko to get array beam width.
         Fix sphere power.
 0.9.4b4 Expose parent parsers.
         Refer to min_res() rather than nside for spheres
```

### Comparing `disko-0.9.5b4/README.md` & `disko-0.9.6b2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,22 @@
 
 * Add a --full-sphere option which fixes the sphere in celestial coordinates, and then points the phase center of an observation correctly. Requires a beam pattern to be specified (or at least a hemispherical beam). A beam is a sky vector mask. I.e., should fall to zero 'outside' the beam.
 * Deal with flagging, output residuals in a way that can be used to flag in the measurement set. This means some casa expression that changes the MS.
 
 ## Changelog
 
 ```
+0.9.6b2 Fix the --elevation limit to actually implement this for disko draw
+0.9.6b1 Add a minimum elevation to the sphere.el_min_r. This is for setting bounds in imagers.
+        Explicitly manage the tart2ms logging
 0.9.5b4 Add a timestamp to images (or a title if specified) in SVG mode
+        clean up logging so that only happens when --debug is present.
 0.9.5b3 Use gmsh rather than optimesh... (WIP)
+        Use much faster measurement set reading via casa_read_ms() about 200x faster!
+        disko_draw timestamps the image
 0.9.5b2 Fix RA direction in generated FITS files (thanks Ben Hugo)
 0.9.5b1 Add --min and --max to disko_draw so allow manual setting the range of images
 0.9.4b6 Fix bug in drawing PDF.
 0.9.4b5 Import Resolution in disko to get array beam width.
         Fix sphere power.
 0.9.4b4 Expose parent parsers.
         Refer to min_res() rather than nside for spheres
```

### Comparing `disko-0.9.5b4/bin/disko` & `disko-0.9.6b2/bin/disko`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from tart_tools import api_imaging
 from tart.imaging import elaz
 
 from dask.distributed import Client
 
 from disko import DiSkO, get_source_list, AdaptiveMeshSphere, Resolution, sphere_from_args, sphere_args_parser
 
+import tart2ms
 from tart2ms import get_array_location
 
 if __name__ == '__main__':
     sphere_parsers = sphere_args_parser()
         
 
 
@@ -71,46 +72,55 @@
     parser.add_argument('--HDF', required=False, help="Generate a HDF format field of view.")
     parser.add_argument('--VTK', action="store_true", help="Generate a VTK mesh format image.")
     parser.add_argument('--FITS', action="store_true", help="Generate a FITS format image.")
 
     parser.add_argument('--cv', action="store_true", help="Use Cross Validation")
     parser.add_argument('--dask', action="store_true", help="Use dask")
     
+    parser.add_argument('--debug', action="store_true", help="Display debugging information")
     parser.add_argument('--version', action="store_true", help="Display the current version")
 
 
     source_json = None
 
     ARGS = parser.parse_args()
-        
-    logger = logging.getLogger()
-    logger.setLevel(logging.INFO)
 
-    fh = logging.FileHandler('disko.log')
-    fh.setLevel(logging.INFO)
-    
-    # create console handler and set level to debug
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
-
-    # create formatter
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-
-    # add formatter to ch
-    ch.setFormatter(formatter)
-    fh.setFormatter(formatter)
-
-    # add ch to logger
-    #logger.addHandler(ch)
-    logger.addHandler(fh)
-    
+    if ARGS.debug:
+        level = logging.DEBUG
+    else:
+        level = logging.ERROR
+
+    logging.basicConfig()
+    logger = logging.getLogger('disko')
+    logger.setLevel(level)
+    tart2ms_log = logging.getLogger("tart2ms")
+    tart2ms_log.setLevel(level)
+
+    if ARGS.debug:
+        fh = logging.FileHandler('disko.log')
+        fh.setLevel(level)
+
+        # create console handler and set level to debug
+        ch = logging.StreamHandler()
+        ch.setLevel(level)
+
+        # create formatter
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+        # add formatter to ch
+        ch.setFormatter(formatter)
+        fh.setFormatter(formatter)
+
+        # add ch to logger
+        logger.addHandler(ch)
+
     if ARGS.version:
         version = version("disko")
-        print(f"DiSkO: Version {version}")
-        print("       (c) 2022 Tim Molteno")
+        print(f"disko: Version {version}")
+        print("       (c) 2022-2023 Tim Molteno")
         sys.exit(0)
     
     sphere = sphere_from_args(ARGS)
     
     if ARGS.file:
         logger.info("Getting Data from file: {}".format(ARGS.file))
         # Load data from a JSON file
```

### Comparing `disko-0.9.5b4/bin/disko_bayes` & `disko-0.9.6b2/bin/disko_bayes`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/bin/disko_draw` & `disko-0.9.6b2/bin/disko_draw`

 * *Files 15% similar despite different names*

```diff
@@ -53,18 +53,50 @@
     parser.add_argument('--FITS', default=None,
                         help="Generate a FITS format image.")
 
     parser.add_argument('--display', action="store_true",
                         help="Display the field of view")
     parser.add_argument('--version', action="store_true",
                         help="Display the current version")
+    parser.add_argument('--debug', action="store_true",
+                        help="Display debugging information")
 
     ARGS = parser.parse_args()
 
-    logger.setLevel(logging.INFO)
+    if ARGS.debug:
+        level = logging.DEBUG
+    else:
+        level = logging.ERROR
+
+    logger = logging.getLogger('disko')
+    logger.setLevel(level)
+
+    if ARGS.debug:
+        fh = logging.FileHandler('disko_draw.log')
+        fh.setLevel(level)
+
+        # create console handler and set level to debug
+        ch = logging.StreamHandler()
+        ch.setLevel(level)
+
+        # create formatter
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+        # add formatter to ch
+        ch.setFormatter(formatter)
+        fh.setFormatter(formatter)
+
+        # add ch to logger
+        logger.addHandler(ch)
+
+    if ARGS.version:
+        version = version("disko")
+        print(f"disko_draw: Version {version}")
+        print("       (c) 2022-2023 Tim Molteno")
+        sys.exit(0)
 
     field_of_view = fov.from_hdf(ARGS.filename)
     ts = field_of_view.timestamp
     geo = field_of_view.geolocation
     logger.info(f"geo {geo}")
     
     if ARGS.version:
@@ -77,15 +109,15 @@
     if ARGS.show_sources:
         api = api_handler.APIhandler("")
         cat_url = api.catalog_url(lon=geo.lon.to_value('deg'),
                                   lat=geo.lat.to_value('deg'),
                                   datestr=ts.isoformat())
         logger.info(f"catalog url: {cat_url}")
         source_json = api.get_url(cat_url)
-        src_list = get_source_list(source_json, el_limit=5, jy_limit=1e4)
+        src_list = get_source_list(source_json, el_limit=ARGS.elevation, jy_limit=1e4)
         # print("Source list")
         # for s in src_list:
         #     print(f"   src: el:{np.degrees(s.el_r) :5.2f}")
 
 
     if ARGS.max == -1:
         max_img = np.max(field_of_view.pixels)
```

### Comparing `disko-0.9.5b4/bin/disko_svd` & `disko-0.9.6b2/bin/disko_svd`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/disko/__init__.py` & `disko-0.9.6b2/disko/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright Tim Molteno 2019 tim@elec.ac.nz
+# Copyright Tim Molteno 2019-2023 tim@elec.ac.nz
 #
 # Init for the DiSkO imaging algorithm
 from .disko import (
     DiSkO,
     get_source_list,
     DiSkOOperator,
     DirectImagingOperator,
@@ -21,7 +21,10 @@
     plot_uv,
 )
 from .draw_sky import mask_to_sky
 from .projection_lsqr import plsqr
 from .multivariate_gaussian import MultivariateGaussian
 from .resolution import Resolution
 from .parser_support import sphere_from_args, sphere_args_parser
+
+import logging
+logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `disko-0.9.5b4/disko/disko.py` & `disko-0.9.6b2/disko/disko.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 # Tim Molteno 2017-2019 tim@elec.ac.nz
 #
 import logging
 import time
 import pylops
 import scipy
 
+import tart2ms
+
 import numpy as np
 import healpy as hp
 import dask.array as da
 import scipy.sparse.linalg as spalg
 
 
 from sklearn import linear_model
 
 from tart.imaging import elaz
-from tart2ms import read_ms
+# from tart2ms import casa_read_ms as read_ms
 
 from astropy import constants as const
 
 from .healpix_sphere import HealpixSphere
 from .multivariate_gaussian import MultivariateGaussian
 from .resolution import Resolution
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
 
 
 def get_all_uvw(ant_pos):
     """
         Little helper function to get the UVW positions from the antennas positions.
         The test (i != j) can be changed to (i > j) to avoid the duplicated conjugate
         measurements.
@@ -335,20 +333,21 @@
         # Get u, v, w from the antenna positions
         baselines, u_arr, v_arr, w_arr = get_all_uvw(ant_pos)
         ret = cls(u_arr, v_arr, w_arr, frequency)
         ret.info = {}
         return ret
 
     @classmethod
-    def from_ms(cls, ms, num_vis, res, chunks=50000, channel=0, field_id=0, ddid=0):
-        u_arr, v_arr, w_arr, frequency, cv_vis, hdr, tstamp, rms, indices = read_ms(
-            ms, num_vis, angular_resolution=res.degrees(),
-            chunks=chunks, channel=channel,
-            field_id=field_id, ddid=ddid
-        )
+    def from_ms(cls, ms, num_vis, res, channel=0, field_id=0, ddid=0):
+        u_arr, v_arr, w_arr, frequency, cv_vis, \
+            hdr, tstamp, rms, indices = tart2ms.casa_read_ms(
+                ms, num_vis, angular_resolution=res.degrees(), 
+                channel=channel,
+                field_id=field_id, ddid=ddid, pol=0
+            )
 
         # Measurement sets do not return the conjugate pairs of visibilities
 
         full_u_arr = np.concatenate((u_arr, -u_arr), 0)
         full_v_arr = np.concatenate((v_arr, -v_arr), 0)
         full_w_arr = np.concatenate((w_arr, -w_arr), 0)
         full_rms = np.concatenate((rms, rms), 0)
@@ -359,27 +358,27 @@
         ret.vis_arr = full_cv_vis / full_rms
         ret.timestamp = tstamp
         ret.rms = full_rms
         ret.info = hdr
         ret.indices = indices
 
         logger.info(f"Visibilities: {ret.vis_arr.shape}")
-        logger.info(f"u,v,w: {ret.u_arr.shape}")
+        logger.debug(f"u,v,w: {ret.u_arr.shape}")
         return ret
 
     def vis_stats(self):
         vabs = np.abs(self.vis_arr)
 
         p05, p50, p95, p100 = np.percentile(vabs, [5, 50, 95, 100])
-        logger.info(
+        logger.debug(
             "Vis Range: [{:5.4g} {:5.4g} {:5.4g} {:5.4g}]".format(
                 p05, p50, p95, p100)
         )
 
-        logger.info("Vis Energy: {:5.4g}".format(np.sum(vabs)))
+        logger.debug("Vis Energy: {:5.4g}".format(np.sum(vabs)))
 
         return p05, p50, p95, p100
 
     @classmethod
     def from_cal_vis(cls, cal_vis):
 
         c = cal_vis.get_config()
@@ -436,15 +435,15 @@
         """
         Create a DiSkO image from visibilities using the direct ajoint of the
         measurement operator (corresponds to the inverse DFT)
 
         Args:
 
             vis_arr (np.array): An array of complex visibilities
-            sphere (Sphere):    a sphere to place 
+            sphere (Sphere):    a sphere to place
         """
 
         assert len(vis_arr) == len(self.u_arr)
         logger.info(
             "Imaging Visabilities resolution={}".format(sphere.min_res()))
         t0 = time.time()
 
@@ -545,18 +544,18 @@
                 if alpha <= 0:
                     alpha = 10**(-np.log10(self.n_v) + 2)  # Empirical fit
                 eps = 1.0/alpha
                 if eps > 0.1:
                     eps = 0.01
             else:
                 eps = 1e-3
-                
-            eps = 1e-5
+
+            eps = 1e-9
             sky, niter, cost_history = pylops.optimization.sparsity.fista(
-                Op=A, y=d, SOp=Apre, # x0=np.abs(Apre @ d)**2,  # 
+                Op=A, y=d, SOp=Apre,  x0=np.zeros_like(Apre @ d)**2,
                 eps=eps,
                 tol=1e-10, niter=niter, alpha=alpha, show=True,
                 # A, d, niter=niter, alpha=None, show=True, x0=np.abs(Apre @ d),
                 threshkind="soft", callback=A
             )
             # sky, niter = pylops.optimization.sparsity.FISTA(
             # Op=A, data=d, niter=niter,  x0=np.zeros_like(Apre @ d), show=True, alpha=alpha, eps=eps
@@ -626,28 +625,28 @@
 
         n_s = len(harmonic_list[0])
         n_v = len(harmonic_list)
 
         gamma = np.asarray(harmonic_list)  # , dtype=COMPLEX_DATATYPE)
         logger.info("Gamma Shape: {}".format(gamma.shape))
         gamma = gamma.reshape((n_v, n_s))
-        logger.info("Complex Gamma Shape: {}".format(gamma.shape))
+        logger.debug("Complex Gamma Shape: {}".format(gamma.shape))
         # gamma = gamma.conj()  # .rechunk('auto')
 
         if makecomplex:
             return gamma
 
         # Build an augmented matrix for separating the real and imaginary
         # parts, so that the operator matrix can be real-valued
         g_real = np.real(gamma)
         g_imag = np.imag(gamma)
         ret = np.block([[g_real],
                         [g_imag]])  # .rechunk('auto')
 
-        logger.info("Real Gamma Shape: {}".format(ret.shape))
+        logger.debug("Real Gamma Shape: {}".format(ret.shape))
 
         return ret
 
     def image_lasso(self, vis_arr, sphere, alpha, l1_ratio, scale=False, use_cv=False):
         gamma = self.make_gamma(sphere)
 
         vis_aux = vis_to_real(vis_arr)
@@ -744,15 +743,15 @@
         logger.info("Elapsed {}s".format(time.time() - t0))
         return posterior
 
     def image_tikhonov(self, vis_arr, sphere, alpha, scale=True, usedask=False):
         n_s = sphere.pixels.shape[0]
         n_v = self.u_arr.shape[0]
 
-        print(
+        logger.info(
             f"image_tikhonov({vis_arr.shape}, {sphere}, {alpha}, scale={scale}, usedask={usedask})"
         )
 
         if alpha is None:
             raise RuntimeError(
                 "The --alpha option must be specified when using --tikhonov")
```

### Comparing `disko-0.9.5b4/disko/draw_sky.py` & `disko-0.9.6b2/disko/draw_sky.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,15 @@
 from scipy import misc
 
 from .healpix_sphere import HealpixSphere
 from .disko import DiSkO
 from .telescope_operator import TelescopeOperator
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
-
+# logger.setLevel(logging.INFO)
 
 def mask_to_sky(mask, nside):
     height, width, col = mask.shape
     mask = mask / np.max(mask)
 
     rmax = min(width, height) / 2
```

### Comparing `disko-0.9.5b4/disko/fov/factory.py` & `disko-0.9.6b2/disko/fov/factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 
 
 from ..healpix_sphere import HealpixSphere, HealpixSubSphere
 from ..sphere_mesh import AdaptiveMeshSphere
 from ..sphere import GeoLocation
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
-
 
 def from_hdf(filename):
     ret = None
     with h5py.File(filename, "r") as h5f:
         info_string = np.string_(h5f['information'][0]).decode('UTF-8')
         info_json = json.loads(info_string)
```

### Comparing `disko-0.9.5b4/disko/healpix_sphere.py` & `disko-0.9.6b2/disko/healpix_sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 from .sphere import image_stats
 
 from .sphere import hp2elaz, elaz2lmn, PlotCoords, HpAngle, elaz2hp, ElAz
 
 from .resolution import Resolution
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
-
+# logger.setLevel(logging.INFO)
 
 def create_fov(nside, fov, res, theta=0.0, phi=0.0):
     """
     Create an appropriate Sphere object based on:
 
     - fov : The field of view as a Resolution object
     """
@@ -43,15 +39,15 @@
         res_arcmin = res.arcmin()
         sphere = HealpixSubSphere(res_arcmin=res_arcmin,
                                   theta=theta, phi=phi,
                                   radius_rad=radius_rad)
     else:
         raise RuntimeError("Either nside, or res_arcmin must be specified")
 
-    logger.info(f"create_fov -> {sphere}")
+    logger.debug(f"create_fov -> {sphere}")
     return sphere
 
 
 def cmap(fract):
     '''
         Build a colour map
     '''
@@ -89,15 +85,15 @@
             return
         self.nside = nside
         self.npix = hp.nside2npix(self.nside)
         res = hp.nside2resol(nside, arcmin=True)
         self._min_res = Resolution.from_arcmin(res)
 
         logger.info(
-            f"New Sphere, nside={nside}. npix={self.npix}, res={self.min_res()}")
+            f"New HeadpixSphere, nside={nside}. npix={self.npix}, res={self.min_res()}")
 
         self.pixel_indices = np.arange(self.npix)
         theta, phi = hp.pix2ang(nside, self.pixel_indices)
 
         self.pixels = np.zeros(self.npix)  # + hp.UNSEEN
         self.pixel_areas = 4*np.pi*np.ones(self.npix)/self.npix
 
@@ -451,23 +447,23 @@
             dwg.add(source_circles)
 
         with open(fname, "w", encoding="utf-8") as outfile:
             dwg.write(outfile)
 
     def plot(self, plt, src_list):
         rot = (0, 90, 0)
-        logger.info("self.pixels: {}".format(self.pixels.shape))
+        logger.debug("self.pixels: {}".format(self.pixels.shape))
         if True:
             hp.orthview(
                 self.pixels, rot=rot, xsize=1000, cbar=True, half_sky=False, hold=False
             )
-            hp.graticule(verbose=False)
+            hp.graticule()
         else:
             hp.mollview(self.pixels, rot=rot, xsize=1000, cbar=True)
-            hp.graticule(verbose=True)
+            hp.graticule()
 
         if src_list is not None:
             for s in src_list:
                 self.plot_x(plt, s.el_r, s.az_r)
 
 
 def my_query_disk(nside, x0, radius):
@@ -498,15 +494,15 @@
         logger.info(f"    theta={theta}, phi={phi}, radius_rad={radius_rad})")
         # Theta is co-latitude measured southward from the north pole
         # Phi is [0..2pi]
 
         if nside is None:  # Calculate nside to the appropriate resolution
             nside = 1
             while hp.nside2resol(nside, arcmin=True) > res_arcmin:
-                logger.info(
+                logger.debug(
                     f"nside={nside} res={hp.nside2resol(nside, arcmin=True)}")
                 nside *= 2
 
         self.nside = nside
         self.res_arcmin = res_arcmin
         self.theta = theta
         self.phi = phi
@@ -532,14 +528,16 @@
         self.fov = Resolution.from_rad(radius_rad * 2)
         self.pixels = np.zeros(self.npix)  # + hp.UNSEEN
 
         area = 4*np.pi*(self.npix / hp.nside2npix(nside))
         self.pixel_areas = area*np.ones(self.npix)/self.npix
 
         el_r, az_r = hp2elaz(theta, phi)
+        
+        self.el_min_r = np.min(el_r)
 
         self.el_r = el_r
         self.az_r = az_r
 
         self.l, self.m, self.n = elaz2lmn(self.el_r, self.az_r)
         self.n_minus_1 = self.n - 1
 
@@ -581,20 +579,20 @@
         Modified plot to deal with the reduced number of pixels
         """
         all_npix = hp.nside2npix(self.nside)
         all_pixels = np.zeros(all_npix) + hp.UNSEEN
         all_pixels[self.pixel_indices] = self.pixels
 
         rot = (0, 90, 0)
-        logger.info("self.pixels: {}".format(self.pixels.shape))
+        logger.debug("self.pixels: {}".format(self.pixels.shape))
         if True:
             hp.orthview(
                 all_pixels, rot=rot, xsize=1000, cbar=True, half_sky=True, hold=False
             )
-            hp.graticule(verbose=False)
+            hp.graticule()
         else:
             hp.mollview(all_pixels, rot=rot, xsize=1000, cbar=True)
-            hp.graticule(verbose=True)
+            hp.graticule()
 
         if src_list is not None:
             for s in src_list:
                 self.plot_x(plt, s.el_r, s.az_r)
```

### Comparing `disko-0.9.5b4/disko/multivariate_gaussian.py` & `disko-0.9.6b2/disko/multivariate_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 
 import numpy as np
 import dask.array as da
 
 from .util import log_array
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
+# logger.setLevel(logging.INFO)
 
 
 def factors(n):
     return np.sort(
         list(
             set(
                 factor
```

### Comparing `disko-0.9.5b4/disko/parser_support.py` & `disko-0.9.6b2/disko/parser_support.py`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/disko/projection_lsqr.py` & `disko-0.9.6b2/disko/projection_lsqr.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import numpy as np
 
 import scipy
 from sklearn import linear_model
 
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
 
 
 def plsqr(A, v, alpha, eps=1e-4):
     """
     Solve Ax = v using least squares and subspace projection.
     We'll start using a two-way split of A
```

### Comparing `disko-0.9.5b4/disko/resolution.py` & `disko-0.9.6b2/disko/resolution.py`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/disko/sphere.py` & `disko-0.9.6b2/disko/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 import healpy as hp
 
 from tart.util import utc
 
 from astropy.coordinates import EarthLocation
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
+# logger.setLevel(logging.INFO)
 
 
 PI_OVER_2 = np.pi / 2
 
 
 class GeoLocation(object):
     '''
```

### Comparing `disko-0.9.5b4/disko/sphere_mesh.py` & `disko-0.9.6b2/disko/sphere_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 
 from .sphere import Sphere, hp2elaz, elaz2lmn
 from .resolution import Resolution
 
 import numpy as np
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
+# logger.setLevel(logging.INFO)
 
 
 def centroid(cell, points):
     return np.sum(points[cell].T, axis=1) / 3
 
 
 def area(cell, points):
@@ -195,14 +192,16 @@
             points, simplices, pixel_areas, el_r, az_r, l, m, n = get_lmn(
                 self.radius_rad, self.res_max.radians())
 
             self.l = l
             self.m = m
             self.n_minus_1 = n - 1
 
+            self.el_min_r = np.min(el_r)
+
             self.el_r = el_r
             self.az_r = az_r
 
             self.npix = simplices.shape[0]
             self.pixels = np.zeros(self.npix)
 
             self.points = points
@@ -494,36 +493,36 @@
 
         self.l, self.m, n = elaz2lmn(self.el_r, self.az_r)
         self.n_minus_1 = n - 1
 
 
 if __name__ == "__main__":
 
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
-
-    fh = logging.FileHandler("disko.log")
-    fh.setLevel(logging.INFO)
-
-    # create console handler and set level to debug
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
-
-    # create formatter
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    )
-
-    # add formatter to ch
-    ch.setFormatter(formatter)
-    fh.setFormatter(formatter)
-
-    # add ch to logger
-    logger.addHandler(ch)
-    logger.addHandler(fh)
+    # logger = logging.getLogger()
+    # logger.setLevel(logging.DEBUG)
+    #
+    # fh = logging.FileHandler("disko.log")
+    # fh.setLevel(logging.INFO)
+    #
+    # # create console handler and set level to debug
+    # ch = logging.StreamHandler()
+    # ch.setLevel(logging.INFO)
+    #
+    # # create formatter
+    # formatter = logging.Formatter(
+    #     "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    # )
+    #
+    # # add formatter to ch
+    # ch.setFormatter(formatter)
+    # fh.setFormatter(formatter)
+    #
+    # # add ch to logger
+    # logger.addHandler(ch)
+    # logger.addHandler(fh)
 
     sph = AdaptiveMeshSphere.from_resolution(
         res_arcmin=10,
         res_arcmax=180,
         theta=np.radians(0.0),
         phi=0.0,
         radius=np.radians(20),
```

### Comparing `disko-0.9.5b4/disko/telescope_operator.py` & `disko-0.9.6b2/disko/telescope_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 
 from pathlib import Path
 
 from .disko import vis_to_real
 from .multivariate_gaussian import MultivariateGaussian
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
+# logger.setLevel(logging.INFO)
 
 SVD_TOL = 1e-3
 USE_DASK = True
 
 
 def plot_spectrum(s, n_s, n_v, rank, name):
     plt.figure(num=None, figsize=(6, 4), dpi=300, facecolor="w", edgecolor="k")
```

### Comparing `disko-0.9.5b4/disko/util.py` & `disko-0.9.6b2/disko/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import logging
 
 import numpy as np
 import dask.array as da
 
 logger = logging.getLogger(__name__)
-logger.addHandler(
-    logging.NullHandler()
-)  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
-
+# logger.setLevel(logging.INFO)
 
 def log_array(title, x):
     if isinstance(x, np.ndarray):
         logger.info("   np: {}:{} {:5.2f} GB".format(
             title, x.shape, x.nbytes / 1e9))
     elif isinstance(x, da.core.Array):
         logger.info("   da: {}:{} chunks={}".format(title, x.shape, x.chunks))
```

### Comparing `disko-0.9.5b4/disko.egg-info/PKG-INFO` & `disko-0.9.6b2/disko.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disko
-Version: 0.9.5b4
+Version: 0.9.6b2
 Summary: Discrete Sky Operator (DiSkO) Aperture Synthesis Radio Imaging
 Home-page: http://github.com/tmolteno/disko
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
@@ -83,16 +83,22 @@
 
 * Add a --full-sphere option which fixes the sphere in celestial coordinates, and then points the phase center of an observation correctly. Requires a beam pattern to be specified (or at least a hemispherical beam). A beam is a sky vector mask. I.e., should fall to zero 'outside' the beam.
 * Deal with flagging, output residuals in a way that can be used to flag in the measurement set. This means some casa expression that changes the MS.
 
 ## Changelog
 
 ```
+0.9.6b2 Fix the --elevation limit to actually implement this for disko draw
+0.9.6b1 Add a minimum elevation to the sphere.el_min_r. This is for setting bounds in imagers.
+        Explicitly manage the tart2ms logging
 0.9.5b4 Add a timestamp to images (or a title if specified) in SVG mode
+        clean up logging so that only happens when --debug is present.
 0.9.5b3 Use gmsh rather than optimesh... (WIP)
+        Use much faster measurement set reading via casa_read_ms() about 200x faster!
+        disko_draw timestamps the image
 0.9.5b2 Fix RA direction in generated FITS files (thanks Ben Hugo)
 0.9.5b1 Add --min and --max to disko_draw so allow manual setting the range of images
 0.9.4b6 Fix bug in drawing PDF.
 0.9.4b5 Import Resolution in disko to get array beam width.
         Fix sphere power.
 0.9.4b4 Expose parent parsers.
         Refer to min_res() rather than nside for spheres
```

### Comparing `disko-0.9.5b4/disko.egg-info/SOURCES.txt` & `disko-0.9.6b2/disko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disko-0.9.5b4/setup.py` & `disko-0.9.6b2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(name='disko',
-      version='0.9.5b4',
+      version='0.9.6b2',
       description='Discrete Sky Operator (DiSkO) Aperture Synthesis Radio Imaging',
       long_description=readme,
       long_description_content_type="text/markdown",
       url='http://github.com/tmolteno/disko',
       author='Tim Molteno',
       test_suite='nose.collector',
       tests_require=['nose'],
```

