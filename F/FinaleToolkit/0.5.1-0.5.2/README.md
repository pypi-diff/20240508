# Comparing `tmp/finaletoolkit-0.5.1.tar.gz` & `tmp/finaletoolkit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finaletoolkit-0.5.1.tar", last modified: Fri May  3 19:00:44 2024, max compression
+gzip compressed data, was "finaletoolkit-0.5.2.tar", last modified: Wed May  8 20:05:46 2024, max compression
```

## Comparing `finaletoolkit-0.5.1.tar` & `finaletoolkit-0.5.2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletoolkit-0.5.1/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5986 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3765 2024-04-30 18:09:21.000000 finaletoolkit-0.5.1/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1131 2024-05-03 18:47:49.000000 finaletoolkit-0.5.1/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5986 2024-05-03 18:52:33.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1143 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       61 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/finaletoolkit/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       40 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    28006 2024-05-03 16:46:05.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      547 2024-04-30 19:02:33.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9703 2024-04-30 18:27:49.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9331 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7555 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14535 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2587 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    29309 2024-05-03 16:40:30.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14869 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8468 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6801 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       39 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    15108 2024-04-30 19:31:47.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      139 2024-04-30 19:02:29.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4889 2024-04-30 19:03:05.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/agg_bw.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3195 2024-04-30 19:59:51.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletoolkit-0.5.2/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6138 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1131 2024-05-08 20:05:10.000000 finaletoolkit-0.5.2/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6138 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1190 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       61 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/finaletoolkit/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       40 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    28006 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      547 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9703 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9331 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7555 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14535 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2587 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    30313 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14869 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8468 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6801 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       39 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    15108 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      139 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4889 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/agg_bw.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3195 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18690 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/tests/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9859 2024-05-08 20:04:29.000000 finaletoolkit-0.5.2/tests/test_end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2128 2024-05-08 20:04:29.000000 finaletoolkit-0.5.2/tests/test_frag_io.py
```

### Comparing `finaletoolkit-0.5.1/LICENSE` & `finaletoolkit-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/PKG-INFO` & `finaletoolkit-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -125,12 +125,17 @@
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
 ```
 
+## Testing
+
+To run unit tests, navigate to the root directory of your local copy of this
+repo and run `pytest`. You may have to download pytest first.
+
 ## FAQ
 Q: When running on an ARM64 Mac, I can install FinaleToolkit without errors.
 However, I get an `ImportError` when I run it.
 
 A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `finaletoolkit-0.5.1/README.md` & `finaletoolkit-0.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -74,12 +74,17 @@
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
 ```
 
+## Testing
+
+To run unit tests, navigate to the root directory of your local copy of this
+repo and run `pytest`. You may have to download pytest first.
+
 ## FAQ
 Q: When running on an ARM64 Mac, I can install FinaleToolkit without errors.
 However, I get an `ImportError` when I run it.
 
 A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `finaletoolkit-0.5.1/pyproject.toml` & `finaletoolkit-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleToolkit"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Ravi Bandaru", email="ravi.bandaru@northwestern.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
```

### Comparing `finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/PKG-INFO` & `finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -125,12 +125,17 @@
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
 ```
 
+## Testing
+
+To run unit tests, navigate to the root directory of your local copy of this
+repo and run `pytest`. You may have to download pytest first.
+
 ## FAQ
 Q: When running on an ARM64 Mac, I can install FinaleToolkit without errors.
 However, I get an `ImportError` when I run it.
 
 A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/SOURCES.txt` & `finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,8 +26,10 @@
 src/finaletoolkit/methylation/__init__.py
 src/finaletoolkit/qc/__init__.py
 src/finaletoolkit/too/__init__.py
 src/finaletoolkit/utils/__init__.py
 src/finaletoolkit/utils/agg_bw.py
 src/finaletoolkit/utils/cli_hist.py
 src/finaletoolkit/utils/filter_bam.py
-src/finaletoolkit/utils/utils.py
+src/finaletoolkit/utils/utils.py
+tests/test_end_motifs.py
+tests/test_frag_io.py
```

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/cli/main_cli.py` & `finaletoolkit-0.5.2/src/finaletoolkit/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/__init__.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/__init__.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/adjust_wps.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/cleavage_profile.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/coverage.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/coverage.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_gc_correct.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_merge_bins.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_merge_bins.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/end_motifs.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/end_motifs.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,46 +44,46 @@
 
     def __init__(
         self,
         kmer_frequencies: Iterable[tuple[str, float]],
         k: int,
         quality_threshold: int = MIN_QUALITY,
     ):
-        self._dict = dict(kmer_frequencies)
+        self.freq_dict = dict(kmer_frequencies)
         self.k = k
         self.quality_threshold = quality_threshold
         if not all(len(kmer) == k for kmer, _ in kmer_frequencies):
             raise ValueError(
                 'kmer_frequencies contains a kmer with length not equal'
                 ' to k.'
             )
 
     def __iter__(self) -> Iterator:
         return ((kmer, frequency)
                 for (kmer, frequency)
                 in zip(self.kmers(), self.frequencies()))
 
     def __len__(self) -> int:
-        return self._dict.__len__()
+        return self.freq_dict.__len__()
 
     def __str__(self) -> str:
         return ''.join(f'{kmer}: {freq}\n' for kmer, freq in self)
 
     def kmers(self) -> list:
-        return list(self._dict.keys())
+        return list(self.freq_dict.keys())
 
     def frequencies(self) -> list:
-        return list(self._dict.values())
+        return list(self.freq_dict.values())
 
     def freq(self, kmer: str) -> float:
-        return self._dict[kmer]
+        return self.freq_dict[kmer]
 
-    def to_tsv(self, output_file: str, sep: str='\t'):
+    def to_tsv(self, output_file: Union[str,Path], sep: str='\t'):
         """Prints k-mer frequencies to a tsv"""
-        if type(output_file) == str:
+        if isinstance(output_file, str) or isinstance(output_file, Path):
             try:
                 # open file based on name
                 output_is_file = False
                 if output_file == '-':
                     output = stdout
                 else:
                     output_is_file = True
@@ -93,38 +93,40 @@
                 for kmer, freq in self:
                     output.write(f'{kmer}{sep}{freq}\n')
 
             finally:
                 if output_is_file:
                     output.close()
         else:
-            raise TypeError(f'output_file must be a string.')
+            raise TypeError(f'output_file must be a string or path.')
 
     def motif_diversity_score(self) -> float:
         """
         Calculates a motif diversity score (MDS) using normalized
         Shannon entropy as described by Jiang et al (2020). This
         function is generalized for any k instead of just 4-mers.
         """
         num_kmers = 4**self.k
         freq = np.array(self.frequencies())
         # if freq is 0, ignore
-        mds = np.sum(-freq*np.nan_to_num(np.log(freq), neginf=0)/np.log(num_kmers))
-
+        mds = -np.sum(
+            freq * np.log(
+                freq, out=np.zeros_like(freq, dtype=np.float64), where=(freq!=0)
+                ) / np.log(num_kmers))
         return mds
 
     @classmethod
     def from_file(
             cls,
-            file_path: str,
+            file_path: Union[str, Path],
             quality_threshold: int,
             sep: str='\t',
             header: int=0,) -> EndMotifFreqs:
         """
-        Reads kmer frequency from a two-column tab-delimited file
+        Reads kmer frequency from a two-column tab-delimited file.
 
         Parameters
         ---------
         file_path : str
             Path string containing path to file.
         sep : str, optional
             Delimiter used in file.
@@ -134,18 +136,18 @@
         Return
         ------
         kmer_freqs : EndMotifFreqs
         """
         try:
             # open file
             is_file = False
-            if file_path.endswith('gz'):
+            if str(file_path).endswith('gz'):
                 is_file = True
                 file = gzip.open(file_path)
-            elif file_path == '-':
+            elif str(file_path) == '-':
                 file = stdin
             else:
                 is_file = True
                 file = open(file_path)
 
             # ignore header
             for _ in range(header):
@@ -219,22 +221,27 @@
         return f'EndMotifsIntervals over {len(self.intervals)} intervals.'
     
     @classmethod
     def from_file(
             cls,
             file_path: str,
             quality_threshold: int,
-            sep: str=',') -> EndMotifFreqs:
+            sep: str = ',',) -> EndMotifFreqs:
         """
-        Reads kmer frequency from a tab-delimited file
+        Reads kmer frequency from a tab-delimited file. Expected columns
+        are contig, start, stop, name, count, *kmers. Because
+        exporting to file includes an option to turn counts to a fraction,
+        this doesn't perfectly correspond to replicating the other file.
 
         Parameters
         ---------
         file_path : str
             Path string containing path to file.
+        quality_threshold : int
+            MAPQ filter used. Only used for some calculations.
         sep : str, optional
             Delimiter used in file.
 
         Return
         ------
         kmer_freqs : EndMotifFreqs
         """
@@ -250,18 +257,18 @@
                 is_file = True
                 file = open(file_path)
 
             intervals = []
             lines = file.readlines()
             _,_,_,_,_,*kmers = lines[0].split(sep)
             k = round(np.log(len(kmers))/np.log(4))
-            assert 4**k == len(kmers), f"We got k={k} but there are {len(kmers)} kmers."
+            assert 4**k == len(kmers), f"k={k} but should be {len(kmers)}."
 
             for line in lines[1:]:
-                contig, start, stop, name, *freqs = line.split(sep)
+                contig, start, stop, name, count, *freqs = line.split(sep)
                 start, stop = int(start), int(stop)
                 float_freqs = [float(freq) for freq in freqs]
                 dict_freqs = dict(zip(kmers, float_freqs))
                 intervals.append(((contig, start, stop, name), dict_freqs))
         finally:
             if is_file:
                 file.close()
@@ -282,56 +289,62 @@
         Calculates a motif diversity score (MDS) for each interval using
         normalized Shannon entropy as described by Jiang et al (2020). This
         function is generalized for any k instead of just 4-mers.
         """
         num_kmers = 4**self.k
         mds = []
         for interval, kmers in self.intervals:
-            freq = np.array(list(kmers.values()))
+            counts = np.array(list(kmers.values()))
+            freq = counts / np.sum(counts)
             try:
-                interval_mds = np.sum(
-                    -freq*np.nan_to_num(np.log(freq), neginf=0)
-                    )/np.log(num_kmers)
+                interval_mds = -np.sum(
+                    freq * np.log(
+                        freq, out=np.zeros_like(freq, dtype=np.float64), where=(freq!=0)
+                        ) / np.log(num_kmers))
             except RuntimeWarning:
                 interval_mds = np.NaN
             mds.append((interval, interval_mds))
         return mds
 
-    def mds_bed(self, output_file: str, sep: str='\t'):
+    def mds_bed(self, output_file: Union[str, Path], sep: str='\t'):
         """Writes MDS for each interval to a bed/bedgraph file."""
         mds = self.motif_diversity_score()
         with open(output_file, 'w') as out:
             for interval, interval_mds in mds:
                 contig, start, stop, name = interval
                 temp_str = sep.join(
                         [contig, str(start), str(stop), name, str(interval_mds)]
                     )
                 out.write(
                     f"{temp_str}\n"
                 )
     
-    def to_tsv(self, output_file: str, calc_freq: bool=True, sep: str='\t'):
+    def to_tsv(
+            self,
+            output_file: Union[str, Path],
+            calc_freq: bool=True, sep: str='\t'):
         """
-        Writes all intervals and associated frquencies to file.
+        Writes all intervals and associated frquencies to file. Columns
+        are contig, start, stop, name, count, *kmers.
         
         Parameters
         ----------
         output_file: str
             File to write frequencies to.
         calc_freq: bool, optional
             Calculates frequency of motifs if true. Otherwise, writes counts
             for each motif. Default is true.
         sep: str, optional
             Separator for table. Tab-separated by default.
         """
-        if type(output_file) == str:
+        if isinstance(output_file, str) or isinstance(output_file, Path):
             try:
                 # open file based on name
                 output_is_file = False
-                if output_file == '-':
+                if str(output_file) == '-':
                     output = stdout
                 else:
                     output_is_file = True
                     output = open(output_file, 'w')
 
                 # write to file
                 kmers = _gen_kmers(self.k, 'ACGT')
@@ -359,20 +372,20 @@
                     )
                     output.write('\n')
 
             finally:
                 if output_is_file:
                     output.close()
         else:
-            raise TypeError(f'output_file must be a string.')
+            raise TypeError(f'output_file must be a string or path.')
     
     def to_bedgraph(
             self,
             kmer: str,
-            output_file: str,
+            output_file: Union[str, Path],
             calc_freq: bool=True,
             sep: str='\t'
         ):
         """
         Take frequency of specified kmer and writes to bedgraph.
         
         Parameters
@@ -381,19 +394,19 @@
             File to write frequencies to.
         calc_freq: bool, optional
             Calculates frequency of motifs if true. Otherwise, writes counts
             for each motif. Default is true.
         sep: str, optional
             Separator for table. Tab-separated by default.
         """
-        if type(output_file) == str:
+        if isinstance(output_file, str) or isinstance(output_file, Path):
             try:
                 # open file based on name
                 output_is_file = False
-                if output_file == '-':
+                if str(output_file) == '-':
                     output = stdout
                 else:
                     output_is_file = True
                     output = open(output_file, 'w')
 
                 # write to file
                 for interval, freqs in self.intervals:
@@ -417,15 +430,15 @@
                     output.close()
         else:
             raise TypeError(f'output_file must be a string.')
         
     def to_bed(
             self,
             kmer: str,
-            output_file: str,
+            output_file: Union[str, Path],
             calc_freq: bool=True,
             sep: str='\t'
         ):
         """
         Take frequency of specified kmer and writes to BED.
         
         Parameters
@@ -434,19 +447,19 @@
             File to write frequencies to.
         calc_freq: bool, optional
             Calculates frequency of motifs if true. Otherwise, writes counts
             for each motif. Default is true.
         sep: str, optional
             Separator for table. Tab-separated by default.
         """
-        if type(output_file) == str:
+        if isinstance(output_file, str) or isinstance(output_file, Path):
             try:
                 # open file based on name
                 output_is_file = False
-                if output_file == '-':
+                if str(output_file) == '-':
                     output = stdout
                 else:
                     output_is_file = True
                     output = open(output_file, 'w')
 
                 # write to file
                 for interval, freqs in self.intervals:
@@ -496,15 +509,15 @@
 
 
 def region_end_motifs(
     input_file: str,
     contig: str,
     start: int,
     stop: int,
-    refseq_file: str,
+    refseq_file: Union[str, Path],
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
     both_strands: bool = True,
     output_file: Union[None, str] = None,
     quality_threshold: int = MIN_QUALITY,
     verbose: Union[bool, int] = False,
@@ -521,15 +534,15 @@
         Path of SAM, BAM, CRAM, or Frag.gz containing pair-end reads.
     contig : str
         Name of contig or chromosome for region.
     start : int
         0-based start coordinate.
     stop : int
         1-based end coordinate.
-    refseq_file : str
+    refseq_file : str or Path
         2bit file with reference sequence `input_file` was aligned to.
     k : int, optional
         Length of end motif kmer. Default is 4.
     fraction_low: int, optional
         Minimum fragment length.
     fraction_high: int, optional
         Maximum fragment length.
@@ -563,15 +576,15 @@
     bases='ACGT'
     kmer_list = _gen_kmers(k, bases)
     end_motif_counts = dict(zip(kmer_list, 4**k*[0]))
 
     # TODO: accept other reference file types e.g. FASTA
     # count end motifs
     try:
-        refseq = py2bit.open(refseq_file, 'r')
+        refseq = py2bit.open(str(refseq_file), 'r')
         if both_strands:   # both strands of fragment
             for frag in frag_ends:
                 # py2bit uses 0-based for start, 1-based for end
                 # forward end-motif
                 forward_kmer = refseq.sequence(
                     contig, int(frag[1]), int(frag[1]+k)
                 )
@@ -648,15 +661,15 @@
 def _region_end_motifs_dict_star(args) -> dict:
     results_dict = region_end_motifs(*args)
     return results_dict
 
 
 def end_motifs(
     input_file: str,
-    refseq_file: str,
+    refseq_file: Union[str, Path],
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
     both_strands: bool = False,
     output_file: Union[None, str] = None,
     quality_threshold: int = 30,
     workers: int = 1,
@@ -668,15 +681,15 @@
     frequencies as a dictionary. Optionally writes data to a tsv. This
     function reproduces the methodology of Zhou et al (2023).
 
     Parameters
     ----------
     input_file : str
         SAM, BAM, CRAM, or Frag.gz file with paired-end reads.
-    refseq_file : str
+    refseq_file : str or Path
         2bit file with sequence of reference genome input_file is
         aligned to.
     k : int, optional
         Length of end motif kmer. Default is 4.
     output_file : None or str, optional
         File path to write results to. Either tsv or csv.
     quality_threshold : int, optional
@@ -693,15 +706,15 @@
         start_time = time()
 
     bases='ACGT'
     kmer_list = _gen_kmers(k, bases)
 
     # read chromosomes from py2bit
     try:
-        refseq = py2bit.open(refseq_file, 'r')
+        refseq = py2bit.open(str(refseq_file), 'r')
         chroms: dict = refseq.chroms()
     finally:
         refseq.close()
 
     # generate list of inputs
     intervals = []
     window_size = 1000000
@@ -776,39 +789,39 @@
         )
 
     return results
 
 
 def interval_end_motifs(
     input_file: str,
-    refseq_file: str,
-    intervals: Union[str, list[Tuple[str,int,int]]],
+    refseq_file: Union[str, Path],
+    intervals: Union[str, Iterable[Tuple[str,int,int,str]]],
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
     both_strands: bool = True,
     output_file: Union[None, str] = None,
     quality_threshold: int = 30,
     workers: int = 1,
     verbose: Union[bool, int] = False,
-) -> EndMotifFreqs:
+) -> EndMotifsIntervals:
     """
     Function that reads fragments from a BAM, SAM, or tabix indexed
     file and user-specified intervals and returns the 5' k-mer
     (default is 4-mer) end motif. Optionally writes data to a tsv.
 
     Parameters
     ----------
     input_file : str
         Path of SAM, BAM, CRAM, or Frag.gz containing pair-end reads.
-    refseq_file : str
+    refseq_file : str or Path
         Path of 2bit file for reference genome that reads are aligned to.
     intervals : str or tuple
         Path of BED file containing intervals or list of tuples
-        (chrom, start, stop).
+        (chrom, start, stop, name).
     k : int, optional
         Length of end motif kmer. Default is 4.
     output_file : None or str, optional
         File path to write results to. Either tsv or csv.
     quality_threshold : int, optional
         Minimum MAPQ to filter.
     workers : int, optional
@@ -830,21 +843,21 @@
         with open(intervals, 'r') as interval_file:
             intervals_tuples = [    # parses file lines into a tuple generator
                 (chrom, int(start), int(stop),
                     name[0] if len(name) > 0 else '.')
                 for chrom, start, stop, *name
                 in (line.split() for line in interval_file.readlines())
             ]
-    elif type(intervals) is tuple:
+    elif isinstance(intervals, Iterable):
         intervals_tuples = intervals
     else:
-        raise TypeError("Intervals should be string or tuple.")
+        raise TypeError("Intervals should be string or list.")
     
     mp_intervals = []   # args to be fed into pool processes
-    for chrom, start, stop, _ in intervals_tuples:
+    for chrom, start, stop, *_ in intervals_tuples:
         mp_intervals.append((
             input_file,
             chrom,
             start,
             stop,
             refseq_file,
             k,
@@ -923,8 +936,8 @@
     # 30 is used as a placeholder for the quality threshold. It is not
     # used to calculate MDS and can be ignored.
     motifs = EndMotifsIntervals.from_file(
         file_path,
         30,
         sep,
     )
-    motifs.mds_bed(file_out)
+    motifs.mds_bed(file_out)
```

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/frag_length.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/multi_wps.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/frag/wps.py` & `finaletoolkit-0.5.2/src/finaletoolkit/frag/wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/genome/gaps.py` & `finaletoolkit-0.5.2/src/finaletoolkit/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/utils/agg_bw.py` & `finaletoolkit-0.5.2/src/finaletoolkit/utils/agg_bw.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/utils/cli_hist.py` & `finaletoolkit-0.5.2/src/finaletoolkit/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/utils/filter_bam.py` & `finaletoolkit-0.5.2/src/finaletoolkit/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.1/src/finaletoolkit/utils/utils.py` & `finaletoolkit-0.5.2/src/finaletoolkit/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import time
 import gzip
 import tempfile as tf
 from typing import Union, TextIO, Tuple, List, Generator
 from sys import stderr, stdout
+from pathlib import Path
 
 import numpy as np
 from numpy.typing import NDArray
 from numba import jit
 import pysam
 from tqdm import tqdm
 
@@ -132,15 +133,15 @@
         np.greater_equal(frag_array[:, 1], minimum)
         )
     filtered_frags = frag_array[in_region]
     return filtered_frags
 
 
 def frag_generator(
-    input_file: Union[str, pysam.AlignmentFile, pysam.TabixFile],
+    input_file: Union[str, pysam.AlignmentFile, pysam.TabixFile, Path],
     contig: str,
     quality_threshold: int=30,
     start: int=None,
     stop: int=None,
     fraction_low: int=120,
     fraction_high: int=180,
     intersect_policy: str="midpoint",
@@ -176,40 +177,48 @@
     -------
     frag_ends : Generator
         Generator that yields tuples containing the region covered by
         each fragment in input_file.
     """
     try:
         # check type of input and open if needed
-        input_file_is_str = False   # file was opened in this context
-        is_sam = False  # file is SAM/BAM, not tabix indexed
-        if type(input_file) == str:   # path string
-            input_file_is_str == True
+        input_file_is_path = False
+        if isinstance(input_file, str) or isinstance(input_file, Path):
+            input_file_is_path == True
             # check file type
             if (
-                input_file.endswith('.sam')
-                or input_file.endswith('.bam')
-                or input_file.endswith('.cram')
+                str(input_file).endswith('.sam')
+                or str(input_file).endswith('.bam')
+                or str(input_file).endswith('.cram')
             ):
                 is_sam = True
                 sam_file = pysam.AlignmentFile(input_file, 'r')
             elif (
-                input_file.endswith('frag.gz')
-                or input_file.endswith('bed.gz')
+                str(input_file).endswith('frag.gz')
+                or str(input_file).endswith('bed.gz')
             ):
-                tbx = pysam.TabixFile(input_file, 'r')
+                tbx = pysam.TabixFile(str(input_file), 'r')
+                is_sam = False
+            else:
+                raise ValueError(
+                    "Unaccepted interval file type. Only SAM, CRAM, BAM"
+                    ", and Frag.gz files are accepted.")
         elif type(input_file) == pysam.AlignmentFile:
+            input_file_is_path = False
             is_sam = True
             sam_file = input_file
         elif type(input_file) == pysam.TabixFile:
+            input_file_is_path = False
+            is_sam = False
             tbx = input_file
         else:
             raise TypeError(
                 f'{type(input_file)} is invalid type for input_file.'
             )
+            exit(1)
         
         # setting filter based on intersect policy
         if intersect_policy == 'midpoint':
             check_intersect = lambda r_start, r_stop, f_start, f_stop : (
                 (r_start is None or ((f_start+f_stop)/2) >= r_start)
                 and (r_stop is None or ((f_start+f_stop)/2) < r_stop)
             )
@@ -283,30 +292,31 @@
                         ):
                         yield contig, read_start, read_stop, mapq, read_on_plus
                 # HACK: for some reason read_length is sometimes None
                 except TypeError:
                     continue
 
     finally:
-        if input_file_is_str and is_sam:
+        if input_file_is_path and is_sam:
             sam_file.close()
-        elif input_file_is_str:
+        elif input_file_is_path:
             tbx.close()
 
 
-def frag_array(input_file: Union[str, pysam.AlignmentFile],
-               contig: str,
-               quality_threshold: int=30,
-               start: int=None,
-               stop: int=None,
-               fraction_low: int=120,
-               fraction_high: int=180,
-               intersect_policy: str="midpoint",
-               verbose: bool=False
-               ) -> NDArray:
+def frag_array(
+    input_file: Union[str,pysam.AlignmentFile, pysam.TabixFile, Path],
+    contig: str,
+    quality_threshold: int=30,
+    start: int=None,
+    stop: int=None,
+    fraction_low: int=120,
+    fraction_high: int=180,
+    intersect_policy: str="midpoint",
+    verbose: bool=False
+    ) -> NDArray:
     """
     Reads from BAM, SAM, or BED file and returns a two column matrix
     with fragment start and stop positions.
 
     Parameters
     ----------
     input_file : str or AlignmentFile
```

