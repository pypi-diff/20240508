# Comparing `tmp/compressedcrack-1.0.0.zip` & `tmp/compressedcrack-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,8 @@
-Zip file size: 8944 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 22:16 compressedcrack-1.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/
--rw-r--r--  2.0 unx     4371 b- defN 24-May-08 22:16 compressedcrack-1.0.0/PKG-INFO
--rw-r--r--  2.0 unx     1084 b- defN 24-Apr-07 22:58 compressedcrack-1.0.0/LICENSE
--rw-r--r--  2.0 unx     1037 b- defN 24-May-08 22:09 compressedcrack-1.0.0/pyproject.toml
--rw-r--r--  2.0 unx     2160 b- defN 24-Apr-07 23:15 compressedcrack-1.0.0/README.md
--rw-r--r--  2.0 unx      521 b- defN 24-May-08 21:51 compressedcrack-1.0.0/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-May-08 22:16 compressedcrack-1.0.0/setup.cfg
--rw-r--r--  2.0 unx     4371 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      277 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       46 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-08 22:16 compressedcrack-1.0.0/compressedcrack.egg-info/dependency_links.txt
-14 files, 13916 bytes uncompressed, 6622 bytes compressed:  52.4%
+Zip file size: 4043 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1084 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4395 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      528 b- defN 24-May-08 15:17 compressedcrack-1.0.1.dist-info/RECORD
+6 files, 6146 bytes uncompressed, 3071 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,43 +1,19 @@
-Filename: compressedcrack-1.0.0/
+Filename: compressedcrack-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/
+Filename: compressedcrack-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: compressedcrack-1.0.0/PKG-INFO
+Filename: compressedcrack-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: compressedcrack-1.0.0/LICENSE
+Filename: compressedcrack-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: compressedcrack-1.0.0/pyproject.toml
+Filename: compressedcrack-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: compressedcrack-1.0.0/README.md
-Comment: 
-
-Filename: compressedcrack-1.0.0/setup.py
-Comment: 
-
-Filename: compressedcrack-1.0.0/setup.cfg
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/PKG-INFO
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/SOURCES.txt
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/entry_points.txt
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/requires.txt
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/top_level.txt
-Comment: 
-
-Filename: compressedcrack-1.0.0/compressedcrack.egg-info/dependency_links.txt
+Filename: compressedcrack-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `compressedcrack-1.0.0/PKG-INFO` & `compressedcrack-1.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressedcrack
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line tool to crack password-protected compressed files using brute force.
 Home-page: https://github.com/mnismt/CompressedCrack
 Author: Thanh Minh
 Author-email: Minh Thanh <thanhdoantranminh@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 - 2024 Doan Tran Minh Thanh
@@ -37,14 +37,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: patoolib
 
 # CompressedCrack
 
 ![Banner](./assets/banner.png)
 
 CompressedCrack is a command-line tool that utilizes the brute-force method to crack any password-protected compressed file. It generates password combinations based on user-defined character sets and length range, and attempts to extract the archive using each generated password until the correct password is found.
```

## Comparing `compressedcrack-1.0.0/LICENSE` & `compressedcrack-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

