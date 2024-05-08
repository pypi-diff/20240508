# Comparing `tmp/lightcurver-1.0.5.tar.gz` & `tmp/lightcurver-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurver-1.0.5.tar", last modified: Mon Apr 29 15:28:04 2024, max compression
+gzip compressed data, was "lightcurver-1.0.6.tar", last modified: Wed May  8 15:43:02 2024, max compression
```

## Comparing `lightcurver-1.0.5.tar` & `lightcurver-1.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 15:27:55.000000 lightcurver-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-29 15:28:04.972880 lightcurver-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-29 15:27:55.000000 lightcurver-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/pipeline_dependency_graph.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/state_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/task_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/pipeline/workflow_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.964880 lightcurver-1.0.5/lightcurver/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/footprint_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/image_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/normalization_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/psf_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/sources_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/plotting/star_photometry_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.968880 lightcurver-1.0.5/lightcurver/processes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/alternate_plate_solving_with_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/background_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/cutout_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_importation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/frame_star_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/normalization_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/plate_solving.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/psf_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/roi_deconv_file_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/roi_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/processes/star_querying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.968880 lightcurver-1.0.5/lightcurver/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/structure/user_header_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/lightcurver/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/chi2_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/lightcurves_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/star_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/starred_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-29 15:27:55.000000 lightcurver-1.0.5/lightcurver/utilities/zeropoint_from_gaia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:28:04.972880 lightcurver-1.0.5/lightcurver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 15:28:04.000000 lightcurver-1.0.5/lightcurver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-29 15:27:55.000000 lightcurver-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:28:04.972880 lightcurver-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:42:52.000000 lightcurver-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-08 15:43:02.340828 lightcurver-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-08 15:42:52.000000 lightcurver-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.332827 lightcurver-1.0.6/lightcurver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.332827 lightcurver-1.0.6/lightcurver/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/pipeline_dependency_graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/state_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/task_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/workflow_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/footprint_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/image_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/normalization_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/psf_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/sources_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/star_photometry_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/alternate_plate_solving_with_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/background_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/cutout_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_importation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_star_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/normalization_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/plate_solving.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/psf_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/roi_deconv_file_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/roi_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_querying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/user_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/lightcurver/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/chi2_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/lightcurves_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/star_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/starred_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/zeropoint_from_gaia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/lightcurver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 15:42:52.000000 lightcurver-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:43:02.340828 lightcurver-1.0.6/setup.cfg
```

### Comparing `lightcurver-1.0.5/LICENSE` & `lightcurver-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/PKG-INFO` & `lightcurver-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.5
+Version: 1.0.6
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lightcurver-1.0.5/README.md` & `lightcurver-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/pipeline/pipeline_dependency_graph.yaml` & `lightcurver-1.0.6/lightcurver/pipeline/pipeline_dependency_graph.yaml`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/pipeline/state_checkers.py` & `lightcurver-1.0.6/lightcurver/pipeline/state_checkers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/pipeline/task_wrappers.py` & `lightcurver-1.0.6/lightcurver/pipeline/task_wrappers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/pipeline/workflow_manager.py` & `lightcurver-1.0.6/lightcurver/pipeline/workflow_manager.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/footprint_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/footprint_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/image_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/image_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/normalization_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/normalization_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/psf_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/psf_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/sources_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/sources_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/plotting/star_photometry_plotting.py` & `lightcurver-1.0.6/lightcurver/plotting/star_photometry_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/alternate_plate_solving_with_gaia.py` & `lightcurver-1.0.6/lightcurver/processes/alternate_plate_solving_with_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/background_estimation.py` & `lightcurver-1.0.6/lightcurver/processes/background_estimation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/cutout_making.py` & `lightcurver-1.0.6/lightcurver/processes/cutout_making.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/frame_characterization.py` & `lightcurver-1.0.6/lightcurver/processes/frame_characterization.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/frame_importation.py` & `lightcurver-1.0.6/lightcurver/processes/frame_importation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/frame_star_assignment.py` & `lightcurver-1.0.6/lightcurver/processes/frame_star_assignment.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/normalization_calculation.py` & `lightcurver-1.0.6/lightcurver/processes/normalization_calculation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/plate_solving.py` & `lightcurver-1.0.6/lightcurver/processes/plate_solving.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/psf_modelling.py` & `lightcurver-1.0.6/lightcurver/processes/psf_modelling.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/roi_deconv_file_preparation.py` & `lightcurver-1.0.6/lightcurver/processes/roi_deconv_file_preparation.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,25 @@
     :param constraints_on_frame_columns_dict: a dictionary, with keys identical to that of the frames table and values
                                               intervals of allowed values. E.g., {'seeing_arcseconds': (0, 1.1), ...}
     :param constraints_on_normalization_coeff_dict: a dictionary, with keys identical to the columns of the
                                                     normalization_coefficients table columns, and values same as
                                                     argument constraints_on_frame_columns_dict.
     :return: A pandas dataframe of frames and associated PSFs that meet the criteria.
     """
+    # so, select all frames with a normalization coefficient and psf.
+    # if multiple psfs, select the one with the smallest chi2.
+    # (done with the subquery)
     query = """
     SELECT f.*, ps.*, nc.*
     FROM frames f
-    JOIN PSFs ps ON f.id = ps.frame_id 
+    JOIN (
+        SELECT *,
+        ROW_NUMBER() OVER (PARTITION BY frame_id ORDER BY chi2 ASC) as rn
+        FROM PSFs
+    ) ps ON f.id = ps.frame_id AND ps.rn = 1
     JOIN normalization_coefficients nc ON f.id = nc.frame_id AND nc.combined_footprint_hash = ps.combined_footprint_hash
     WHERE nc.combined_footprint_hash = ?
     AND ps.chi2 BETWEEN ? AND ?
     """
 
     # params of the query:
     params = [combined_footprint_hash, psf_fit_chi2_min, psf_fit_chi2_max]
@@ -65,27 +72,27 @@
 
     Params:
         combined_footprint_hash: as usual the hash of the footprint we're working with at the moment.
 
     """
 
     zeropoint_query = """
-    SELECT 
-        az.frame_id, 
-        az.zeropoint, 
-        az.zeropoint_uncertainty, 
+    SELECT
+        az.frame_id,
+        az.zeropoint,
+        az.zeropoint_uncertainty,
         nc.coefficient
-    FROM 
+    FROM
         approximate_zeropoints az
-    JOIN 
+    JOIN
         normalization_coefficients nc ON az.frame_id = nc.frame_id
     AND
         az.combined_footprint_hash = nc.combined_footprint_hash
-    WHERE 
-        az.combined_footprint_hash = ? 
+    WHERE
+        az.combined_footprint_hash = ?
     """
     zeropoints_data = execute_sqlite_query(zeropoint_query, (combined_footprint_hash,), is_select=True, use_pandas=True)
 
     if zeropoints_data.empty:
         return None, None
 
     # convert normalization coefficient to magnitude adjustment,
@@ -174,15 +181,15 @@
         # and we can open the deconvolution ready file.
 
     # get the zeropoint:
     global_zp, global_zp_scatter = fetch_and_adjust_zeropoints(combined_footprint_hash=combined_footprint_hash)
 
     # where we save the ready to deconvolve cutouts:
     save_path = user_config['prepared_roi_cutouts_path']
-    
+
     if save_path is None:
         roi = user_config['roi_name']
         save_path = user_config['workdir'] / 'prepared_roi_cutouts' / f"cutouts_{combined_footprint_hash}_{roi}.h5"
     save_path.parent.mkdir(exist_ok=True, parents=True)
     with h5py.File(save_path, 'w') as f:
         f['frame_id'] = np.array(frame_id)
         f['data'] = np.array(data)
```

### Comparing `lightcurver-1.0.5/lightcurver/processes/roi_modelling.py` & `lightcurver-1.0.6/lightcurver/processes/roi_modelling.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/star_extraction.py` & `lightcurver-1.0.6/lightcurver/processes/star_extraction.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/star_photometry.py` & `lightcurver-1.0.6/lightcurver/processes/star_photometry.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/processes/star_querying.py` & `lightcurver-1.0.6/lightcurver/processes/star_querying.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/structure/database.py` & `lightcurver-1.0.6/lightcurver/structure/database.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/structure/user_config.py` & `lightcurver-1.0.6/lightcurver/structure/user_config.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/structure/user_header_parser.py` & `lightcurver-1.0.6/lightcurver/structure/user_header_parser.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/chi2_selector.py` & `lightcurver-1.0.6/lightcurver/utilities/chi2_selector.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/footprint.py` & `lightcurver-1.0.6/lightcurver/utilities/footprint.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/gaia.py` & `lightcurver-1.0.6/lightcurver/utilities/gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/lightcurves_postprocessing.py` & `lightcurver-1.0.6/lightcurver/utilities/lightcurves_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/star_naming.py` & `lightcurver-1.0.6/lightcurver/utilities/star_naming.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver/utilities/starred_utilities.py` & `lightcurver-1.0.6/lightcurver/utilities/starred_utilities.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/lightcurver.egg-info/PKG-INFO` & `lightcurver-1.0.6/lightcurver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.5
+Version: 1.0.6
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lightcurver-1.0.5/lightcurver.egg-info/SOURCES.txt` & `lightcurver-1.0.6/lightcurver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.5/pyproject.toml` & `lightcurver-1.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.6.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightcurver"
-version = "1.0.5"
+version = "1.0.6"
 authors = [{ name = "Frédéric Dux", email = "duxfrederic@gmail.com" }]
 description = "A thorough structure for precise photometry and deconvolution of time series of wide field images."
 readme = "README.md"
 keywords = ["photometry", "astronomy", "deconvolution", "PSF", "pipeline"]  
 classifiers = [] 
 dependencies = [
     "pyyaml",
```

