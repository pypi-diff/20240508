# Comparing `tmp/faim_ipa-0.3.2.tar.gz` & `tmp/faim_ipa-0.3.3.tar.gz`

## Comparing `faim_ipa-0.3.2.tar` & `faim_ipa-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/MetaSeriesUtils_dask.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/UIntHistogram.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/Zarr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/dask_utils.py
--rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/mobie.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/alignment/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/alignment/alignment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/__init__.py
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/acquisition.py
--rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/converter.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/plate.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/StackedTile.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/io/ChannelMetadata.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/io/MetaSeriesTiff.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/io/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/stitching/BoundingBox5D.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/stitching/DaskTileStitcher.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/stitching/Tile.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/stitching/__init__.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/stitching/stitching_utils.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/visiview/RegionAcquisition.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/visiview/StackedTile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/visiview/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/src/faim_ipa/visiview/ome_companion_utils.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/LICENSE
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/README.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 faim_ipa-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/MetaSeriesUtils_dask.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/UIntHistogram.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/Zarr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/dask_utils.py
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/mobie.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/alignment/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/alignment/alignment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/__init__.py
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/acquisition.py
+-rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/converter.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/plate.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackedTile.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/ChannelMetadata.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/MetaSeriesTiff.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/BoundingBox5D.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/DaskTileStitcher.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/Tile.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/stitching_utils.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/RegionAcquisition.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/StackedTile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/ome_companion_utils.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/LICENSE
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/README.md
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/PKG-INFO
```

### Comparing `faim_ipa-0.3.2/src/faim_ipa/MetaSeriesUtils_dask.py` & `faim_ipa-0.3.3/src/faim_ipa/MetaSeriesUtils_dask.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/UIntHistogram.py` & `faim_ipa-0.3.3/src/faim_ipa/UIntHistogram.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/Zarr.py` & `faim_ipa-0.3.3/src/faim_ipa/Zarr.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/dask_utils.py` & `faim_ipa-0.3.3/src/faim_ipa/dask_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/mobie.py` & `faim_ipa-0.3.3/src/faim_ipa/mobie.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/utils.py` & `faim_ipa-0.3.3/src/faim_ipa/utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/alignment/alignment.py` & `faim_ipa-0.3.3/src/faim_ipa/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/acquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/acquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/converter.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/converter.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/plate.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/plate.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/StackedTile.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/hcs/imagexpress/StackAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/StackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/io/MetaSeriesTiff.py` & `faim_ipa-0.3.3/src/faim_ipa/io/MetaSeriesTiff.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/stitching/BoundingBox5D.py` & `faim_ipa-0.3.3/src/faim_ipa/stitching/BoundingBox5D.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/stitching/DaskTileStitcher.py` & `faim_ipa-0.3.3/src/faim_ipa/stitching/DaskTileStitcher.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/stitching/Tile.py` & `faim_ipa-0.3.3/src/faim_ipa/stitching/Tile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/stitching/stitching_utils.py` & `faim_ipa-0.3.3/src/faim_ipa/stitching/stitching_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/visiview/RegionAcquisition.py` & `faim_ipa-0.3.3/src/faim_ipa/visiview/RegionAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/visiview/StackedTile.py` & `faim_ipa-0.3.3/src/faim_ipa/visiview/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/src/faim_ipa/visiview/ome_companion_utils.py` & `faim_ipa-0.3.3/src/faim_ipa/visiview/ome_companion_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/.gitignore` & `faim_ipa-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/LICENSE` & `faim_ipa-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.2/pyproject.toml` & `faim_ipa-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic==1.10.13",
+  "pydantic",
   "distributed",
   "numpy",
   "matplotlib",
-  "scikit-image>=0.20.0",
+  "scikit-image",
   "pandas",
   "ome-zarr",
   "tqdm",
   "pint"
 ]
 
 [project.urls]
```

### Comparing `faim_ipa-0.3.2/PKG-INFO` & `faim_ipa-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faim-ipa
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools used at FMI-FAIM for Image Processing and Analysis.
 Project-URL: Bug Tracker, https://github.com/fmi-faim/faim-ipa/issues
 Project-URL: Documentation, https://github.com/fmi-faim/faim-ipa#README.md
 Project-URL: Homepage, https://github.com/fmi-faim/faim-ipa.git
 Project-URL: Source Code, https://github.com/fmi-faim/faim-ipa
 Project-URL: User Support, https://github.com/fmi-faim/faim-ipa/issues
 Author-email: Tim-Oliver Buchholz <tim-oliver.buchholz@fmi.ch>, Jan Eglinger <jan.eglinger@fmi.ch>
@@ -21,14 +21,14 @@
 Requires-Python: >=3.9
 Requires-Dist: distributed
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: ome-zarr
 Requires-Dist: pandas
 Requires-Dist: pint
-Requires-Dist: pydantic==1.10.13
-Requires-Dist: scikit-image>=0.20.0
+Requires-Dist: pydantic
+Requires-Dist: scikit-image
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # FAIM-IPA
 A collection of __I__mage __P__rocessing and __A__nalysis (IPA) functions we use at the Facility for Advanced Imaging and Microscopy (FAIM) at the Friedrich Miescher Institute for Biomedical Research (FMI).
```

