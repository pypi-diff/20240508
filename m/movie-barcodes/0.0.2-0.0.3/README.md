# Comparing `tmp/movie-barcodes-0.0.2.tar.gz` & `tmp/movie-barcodes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-barcodes-0.0.2.tar", last modified: Wed May  8 14:22:34 2024, max compression
+gzip compressed data, was "movie-barcodes-0.0.3.tar", last modified: Wed May  8 14:29:47 2024, max compression
```

## Comparing `movie-barcodes-0.0.2.tar` & `movie-barcodes-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/movie_barcodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:22:34.000000 movie-barcodes-0.0.2/movie_barcodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/src/video_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:34.202070 movie-barcodes-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/test_barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/test_color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-08 14:22:16.000000 movie-barcodes-0.0.2/tests/test_video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.533081 movie-barcodes-0.0.3/movie_barcodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_video_processing.py
```

### Comparing `movie-barcodes-0.0.2/LICENSE` & `movie-barcodes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/PKG-INFO` & `movie-barcodes-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
```

### Comparing `movie-barcodes-0.0.2/README.md` & `movie-barcodes-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/movie_barcodes.egg-info/PKG-INFO` & `movie-barcodes-0.0.3/movie_barcodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
```

### Comparing `movie-barcodes-0.0.2/movie_barcodes.egg-info/SOURCES.txt` & `movie-barcodes-0.0.3/movie_barcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/setup.py` & `movie-barcodes-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/src/barcode_generation.py` & `movie-barcodes-0.0.3/src/barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/src/color_extraction.py` & `movie-barcodes-0.0.3/src/color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/src/main.py` & `movie-barcodes-0.0.3/src/main.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/src/utility.py` & `movie-barcodes-0.0.3/src/utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/src/video_processing.py` & `movie-barcodes-0.0.3/src/video_processing.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/tests/test_barcode_generation.py` & `movie-barcodes-0.0.3/tests/test_barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/tests/test_color_extraction.py` & `movie-barcodes-0.0.3/tests/test_color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/tests/test_integration.py` & `movie-barcodes-0.0.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/tests/test_utility.py` & `movie-barcodes-0.0.3/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.2/tests/test_video_processing.py` & `movie-barcodes-0.0.3/tests/test_video_processing.py`

 * *Files identical despite different names*

