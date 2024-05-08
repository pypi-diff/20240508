# Comparing `tmp/movie-barcodes-0.0.3.tar.gz` & `tmp/movie-barcodes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-barcodes-0.0.3.tar", last modified: Wed May  8 14:29:47 2024, max compression
+gzip compressed data, was "movie-barcodes-0.0.4.tar", last modified: Wed May  8 14:57:42 2024, max compression
```

## Comparing `movie-barcodes-0.0.3.tar` & `movie-barcodes-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.533081 movie-barcodes-0.0.3/movie_barcodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:29:47.000000 movie-barcodes-0.0.3/movie_barcodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/src/video_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:47.537081 movie-barcodes-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-08 14:29:28.000000 movie-barcodes-0.0.3/tests/test_video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/movie_barcodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:57:42.000000 movie-barcodes-0.0.4/movie_barcodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/src/video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:42.442002 movie-barcodes-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-08 14:57:24.000000 movie-barcodes-0.0.4/tests/test_video_processing.py
```

### Comparing `movie-barcodes-0.0.3/LICENSE` & `movie-barcodes-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/PKG-INFO` & `movie-barcodes-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
```

### Comparing `movie-barcodes-0.0.3/README.md` & `movie-barcodes-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/movie_barcodes.egg-info/PKG-INFO` & `movie-barcodes-0.0.4/movie_barcodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
```

### Comparing `movie-barcodes-0.0.3/movie_barcodes.egg-info/SOURCES.txt` & `movie-barcodes-0.0.4/movie_barcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/setup.py` & `movie-barcodes-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/src/barcode_generation.py` & `movie-barcodes-0.0.4/src/barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/src/color_extraction.py` & `movie-barcodes-0.0.4/src/color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/src/main.py` & `movie-barcodes-0.0.4/src/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,53 +86,30 @@
     logging.info("Video Duration: %s", format_time(video_duration))
     logging.info("Video Size: %.2f MB", video_size / (1024 * 1024))
     logging.info("Processing Time: %s", format_time(processing_time))
 
     video.release()
 
 
-def main(args: argparse.Namespace) -> None:
+def main() -> None:
     """
     Main function to generate a barcode from a video file.
-
-    :param args: argparse.Namespace object containing the command-line arguments
-    :return: None
     """
-    # Check if the input video file exists
-    _, frame_count, _, _ = load_video(args.input_video_path)
-
-    # Check if the arguments are valid
-    validate_args(args, frame_count, MAX_PROCESSES, MIN_FRAME_COUNT)
-
-    # Get a list of all available methods
-    methods = ["avg", "hsv", "bgr", "kmeans"]
-
-    # Check if all_methods flag is set
-    if args.all_methods:
-        for method in methods:
-            # Generate barcodes for each method
-            dominant_color_function = get_dominant_color_function(method)
-            generate_and_save_barcode(args, dominant_color_function, method)
-    else:
-        # Use the specified method to generate barcode
-        dominant_color_function = get_dominant_color_function(args.method)
-        generate_and_save_barcode(args, dominant_color_function, args.method)
-
-
-if __name__ == "__main__":
+    # Logging configuration
     logging.basicConfig(
         filename=path.join("..", "logs.txt"),
         level=logging.INFO,
         format="%(asctime)s - %(message)s",
     )
     header_msg = "=" * 40 + " NEW RUN " + "=" * 40
     logging.info("\n%s\n", header_msg)
 
+    # Argument parser setup
     parser = argparse.ArgumentParser(description="Generate a color barcode from a video file.")
-    parser.add_argument("--input_video_path", type=str, help="Path to the video file.")
+    parser.add_argument("--input_video_path", type=str, required=True, help="Path to the video file.")
     parser.add_argument(
         "--destination_path",
         type=str,
         nargs="?",
         help="Path to save the output image. If not provided, the image will be saved in a default location.",
         default=None,
     )
@@ -142,40 +119,57 @@
         default="horizontal",
         help="Type of barcode to generate: horizontal or circular. Default is horizontal.",
     )
     parser.add_argument(
         "--method",
         choices=["avg", "kmeans", "hsv", "bgr"],
         default="avg",
-        help="Method to extract dominant color: avg (average), kmeans (K-Means clustering), hsv (HSV "
-        "histogram), or bgr (BGR histogram). Default is avg.",
+        help="Method to extract dominant color: avg (average), kmeans (K-Means clustering), hsv (HSV histogram), "
+        "or bgr (BGR histogram). Default is avg.",
     )
     parser.add_argument(
         "--workers",
         type=int,
         default=None,
-        help="Number of workers for parallel processing. Default behavior uses all available CPU cores."
-        "Setting this to 1 will use sequential processing. Do not specify a value greater than "
-        "the number of available CPU cores.",
+        help="Number of workers for parallel processing. Default behavior uses all available CPU cores. Setting this "
+        "to 1 will use sequential processing.",
     )
     parser.add_argument(
         "--width",
         type=int,
         default=None,
         help="Width of the output image. If not provided, the width will be the same as the video",
     )
     parser.add_argument(
         "--output_name",
         type=str,
         nargs="?",
-        help="Custom name for the output barcode image. If not provided, a name will be automatically " "generated.",
+        help="Custom name for the output barcode image. If not provided, a name will be automatically generated.",
         default=None,
     )
     parser.add_argument(
         "--all_methods",
-        type=bool,
-        default=False,
-        help="If provided, all methods to extract dominant color will be used to create barcodes. "
-        "Overrides --method argument.",
+        action="store_true",
+        help="If provided, all methods to extract dominant color will be used to create barcodes. Overrides --method "
+        "argument.",
     )
-    arguments = parser.parse_args()
-    main(arguments)
+
+    # Parse arguments
+    args = parser.parse_args()
+
+    # Validate and process video file
+    _, frame_count, _, _ = load_video(args.input_video_path)
+    validate_args(args, frame_count, MAX_PROCESSES, MIN_FRAME_COUNT)
+
+    # Choose the method to generate barcode
+    methods = ["avg", "hsv", "bgr", "kmeans"]
+    if args.all_methods:
+        for method in methods:
+            dominant_color_function = get_dominant_color_function(method)
+            generate_and_save_barcode(args, dominant_color_function, method)
+    else:
+        dominant_color_function = get_dominant_color_function(args.method)
+        generate_and_save_barcode(args, dominant_color_function, args.method)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `movie-barcodes-0.0.3/src/utility.py` & `movie-barcodes-0.0.4/src/utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/src/video_processing.py` & `movie-barcodes-0.0.4/src/video_processing.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/tests/test_barcode_generation.py` & `movie-barcodes-0.0.4/tests/test_barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/tests/test_color_extraction.py` & `movie-barcodes-0.0.4/tests/test_color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/tests/test_integration.py` & `movie-barcodes-0.0.4/tests/test_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,39 @@
-import argparse
 import unittest
 import os
 import glob
+import sys
+from unittest.mock import patch
 
 from src import main
 
 
 class TestIntegration(unittest.TestCase):
     def setUp(self) -> None:
-        """
-        Set up the test case.
-        """
-        # Recreate the parser with minimal necessary setup
-        self.parser = argparse.ArgumentParser(description="Test Parser")
-        self.parser.add_argument("--input_video_path", type=str)
-        self.parser.add_argument("--destination_path", type=str, nargs="?", default=None)
-        self.parser.add_argument("--barcode_type", choices=["horizontal", "circular"], default="horizontal")
-        self.parser.add_argument("--method", choices=["avg", "kmeans", "hsv", "bgr"], default="avg")
-        self.parser.add_argument("--workers", type=int, default=None)
-        self.parser.add_argument("--width", type=int, default=None)
-        self.parser.add_argument("--output_name", type=str, nargs="?", default=None)
-        self.parser.add_argument("--all_methods", type=bool, default=False)
-
         self.input_video_path = "tests/sample.mp4"
 
     def _run_test(self, barcode_type, workers, width=None):
+        # Build the command line arguments list
         args = [
+            "movie-barcodes",
             "--input_video_path",
             self.input_video_path,
             "--barcode_type",
             barcode_type,
             "--method",
             "avg",
             "--workers",
             str(workers),
         ]
         if width is not None:
             args.extend(["--width", str(width)])
 
-        # Parse args using the recreated parser
-        parsed_args = self.parser.parse_args(args)
-
-        # Execute the program with the parsed Namespace object
-        main.main(parsed_args)
+        # Use patch to simulate command line arguments
+        with patch.object(sys, "argv", args):
+            main.main()  # Call the main function which now internally handles args
 
     def test_horizontal_1_worker_default_width(self):
         self._run_test("horizontal", 1)
 
     def test_horizontal_1_worker_defined_width(self):
         self._run_test("horizontal", 1, 90)
```

### Comparing `movie-barcodes-0.0.3/tests/test_utility.py` & `movie-barcodes-0.0.4/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.3/tests/test_video_processing.py` & `movie-barcodes-0.0.4/tests/test_video_processing.py`

 * *Files identical despite different names*

