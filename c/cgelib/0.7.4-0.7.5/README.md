# Comparing `tmp/cgelib-0.7.4.tar.gz` & `tmp/cgelib-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgelib-0.7.4.tar", last modified: Tue Oct 17 09:04:05 2023, max compression
+gzip compressed data, was "cgelib-0.7.5.tar", last modified: Wed May  8 09:56:14 2024, max compression
```

## Comparing `cgelib-0.7.4.tar` & `cgelib-0.7.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.468984 cgelib-0.7.4/
--rw-r--r--   0 rolf       (503) staff       (20)      636 2023-10-17 08:49:02.000000 cgelib-0.7.4/LICENSE.txt
--rw-r--r--   0 rolf       (503) staff       (20)       55 2023-10-17 08:49:02.000000 cgelib-0.7.4/MANIFEST.in
--rw-r--r--   0 rolf       (503) staff       (20)      975 2023-10-17 09:04:05.468914 cgelib-0.7.4/PKG-INFO
--rw-r--r--   0 rolf       (503) staff       (20)      151 2023-10-17 08:49:02.000000 cgelib-0.7.4/README.md
--rw-r--r--   0 rolf       (503) staff       (20)      110 2023-10-17 08:49:02.000000 cgelib-0.7.4/pyproject.toml
--rw-r--r--   0 rolf       (503) staff       (20)     1023 2023-10-17 09:04:05.469305 cgelib-0.7.4/setup.cfg
--rw-r--r--   0 rolf       (503) staff       (20)      445 2023-10-17 08:57:53.000000 cgelib-0.7.4/setup.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.458506 cgelib-0.7.4/src/
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.460549 cgelib-0.7.4/src/cgelib/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/__init__.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.461956 cgelib-0.7.4/src/cgelib/alignment/
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.462686 cgelib-0.7.4/src/cgelib/alignment/KMA/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/KMA/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)    21563 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/KMA/alignment_files.py
--rw-r--r--   0 rolf       (503) staff       (20)     5078 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/KMA/read_files.py
--rw-r--r--   0 rolf       (503) staff       (20)        1 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)    16491 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/aligner.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.463256 cgelib-0.7.4/src/cgelib/alignment/blast/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/blast/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)    10007 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/blast/alignment_files.py
--rw-r--r--   0 rolf       (503) staff       (20)     4420 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/blast/read_files.py
--rw-r--r--   0 rolf       (503) staff       (20)     3624 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/alignment/read_alignment.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.464515 cgelib-0.7.4/src/cgelib/applications/
--rw-r--r--   0 rolf       (503) staff       (20)    22149 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/applications/Blast.py
--rw-r--r--   0 rolf       (503) staff       (20)    25045 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/applications/KMA.py
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/applications/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)    37304 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/applications/command.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.465543 cgelib-0.7.4/src/cgelib/output/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)     1816 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/exceptions.py
--rw-r--r--   0 rolf       (503) staff       (20)     1081 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/parserdict.py
--rw-r--r--   0 rolf       (503) staff       (20)     9083 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/result.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.458990 cgelib-0.7.4/src/cgelib/output/templates_json/
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.466092 cgelib-0.7.4/src/cgelib/output/templates_json/beone/
--rw-r--r--   0 rolf       (503) staff       (20)     6126 2023-10-17 08:49:39.000000 cgelib-0.7.4/src/cgelib/output/templates_json/beone/beone.json
--rw-r--r--   0 rolf       (503) staff       (20)   144690 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/templates_json/beone/example.json
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.466581 cgelib-0.7.4/src/cgelib/output/test_data/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/test_data/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)      465 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/test_data/test_val_parse_fail.py
--rw-r--r--   0 rolf       (503) staff       (20)     3433 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/output/valueparsers.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.467381 cgelib-0.7.4/src/cgelib/sequence/
--rw-r--r--   0 rolf       (503) staff       (20)     5052 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/sequence/Feature.py
--rw-r--r--   0 rolf       (503) staff       (20)    14138 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/sequence/SeqHit.py
--rw-r--r--   0 rolf       (503) staff       (20)        1 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/sequence/__init__.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.468564 cgelib-0.7.4/src/cgelib/utils/
--rw-r--r--   0 rolf       (503) staff       (20)        0 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/__init__.py
--rw-r--r--   0 rolf       (503) staff       (20)     6892 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/file_mixin.py
--rw-r--r--   0 rolf       (503) staff       (20)     2769 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/format_mixin.py
--rw-r--r--   0 rolf       (503) staff       (20)     3941 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/loaders_mixin.py
--rw-r--r--   0 rolf       (503) staff       (20)     3183 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/pliers_mixin.py
--rw-r--r--   0 rolf       (503) staff       (20)     2736 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/savers_mixin.py
--rw-r--r--   0 rolf       (503) staff       (20)      729 2023-10-17 08:49:02.000000 cgelib-0.7.4/src/cgelib/utils/transformer_mixin.py
-drwxr-xr-x   0 rolf       (503) staff       (20)        0 2023-10-17 09:04:05.461298 cgelib-0.7.4/src/cgelib.egg-info/
--rw-r--r--   0 rolf       (503) staff       (20)      975 2023-10-17 09:04:05.000000 cgelib-0.7.4/src/cgelib.egg-info/PKG-INFO
--rw-r--r--   0 rolf       (503) staff       (20)     1417 2023-10-17 09:04:05.000000 cgelib-0.7.4/src/cgelib.egg-info/SOURCES.txt
--rw-r--r--   0 rolf       (503) staff       (20)        1 2023-10-17 09:04:05.000000 cgelib-0.7.4/src/cgelib.egg-info/dependency_links.txt
--rw-r--r--   0 rolf       (503) staff       (20)       26 2023-10-17 09:04:05.000000 cgelib-0.7.4/src/cgelib.egg-info/requires.txt
--rw-r--r--   0 rolf       (503) staff       (20)        7 2023-10-17 09:04:05.000000 cgelib-0.7.4/src/cgelib.egg-info/top_level.txt
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.825452 cgelib-0.7.5/
+-rw-r--r--   0 rolf       (503) staff       (20)      636 2023-11-01 14:19:44.000000 cgelib-0.7.5/LICENSE.txt
+-rw-r--r--   0 rolf       (503) staff       (20)       55 2023-11-01 14:19:44.000000 cgelib-0.7.5/MANIFEST.in
+-rw-r--r--   0 rolf       (503) staff       (20)      970 2024-05-08 09:56:14.825394 cgelib-0.7.5/PKG-INFO
+-rw-r--r--   0 rolf       (503) staff       (20)      151 2023-11-01 14:19:44.000000 cgelib-0.7.5/README.md
+-rw-r--r--   0 rolf       (503) staff       (20)      110 2023-11-01 14:19:44.000000 cgelib-0.7.5/pyproject.toml
+-rw-r--r--   0 rolf       (503) staff       (20)     1013 2024-05-08 09:56:14.825759 cgelib-0.7.5/setup.cfg
+-rw-r--r--   0 rolf       (503) staff       (20)      445 2024-05-08 09:50:52.000000 cgelib-0.7.5/setup.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.814108 cgelib-0.7.5/src/
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.816193 cgelib-0.7.5/src/cgelib/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/__init__.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.817834 cgelib-0.7.5/src/cgelib/alignment/
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.818297 cgelib-0.7.5/src/cgelib/alignment/KMA/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/KMA/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)    21563 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/KMA/alignment_files.py
+-rw-r--r--   0 rolf       (503) staff       (20)     5078 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/KMA/read_files.py
+-rw-r--r--   0 rolf       (503) staff       (20)        1 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)    16491 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/aligner.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.818788 cgelib-0.7.5/src/cgelib/alignment/blast/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/blast/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)    10007 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/blast/alignment_files.py
+-rw-r--r--   0 rolf       (503) staff       (20)     4420 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/blast/read_files.py
+-rw-r--r--   0 rolf       (503) staff       (20)     3624 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/alignment/read_alignment.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.820011 cgelib-0.7.5/src/cgelib/applications/
+-rw-r--r--   0 rolf       (503) staff       (20)    22149 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/applications/Blast.py
+-rw-r--r--   0 rolf       (503) staff       (20)    25045 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/applications/KMA.py
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/applications/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)    37304 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/applications/command.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.820944 cgelib-0.7.5/src/cgelib/output/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)     1816 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/exceptions.py
+-rw-r--r--   0 rolf       (503) staff       (20)     1081 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/parserdict.py
+-rw-r--r--   0 rolf       (503) staff       (20)     9083 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/result.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.814669 cgelib-0.7.5/src/cgelib/output/templates_json/
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.821581 cgelib-0.7.5/src/cgelib/output/templates_json/beone/
+-rw-r--r--   0 rolf       (503) staff       (20)     6126 2023-11-01 14:42:27.000000 cgelib-0.7.5/src/cgelib/output/templates_json/beone/beone.json
+-rw-r--r--   0 rolf       (503) staff       (20)   144690 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/templates_json/beone/example.json
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.823137 cgelib-0.7.5/src/cgelib/output/test_data/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/test_data/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)      465 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/test_data/test_val_parse_fail.py
+-rw-r--r--   0 rolf       (503) staff       (20)     3433 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/output/valueparsers.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.823686 cgelib-0.7.5/src/cgelib/sequence/
+-rw-r--r--   0 rolf       (503) staff       (20)     5052 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/sequence/Feature.py
+-rw-r--r--   0 rolf       (503) staff       (20)    14138 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/sequence/SeqHit.py
+-rw-r--r--   0 rolf       (503) staff       (20)        1 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/sequence/__init__.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.824885 cgelib-0.7.5/src/cgelib/utils/
+-rw-r--r--   0 rolf       (503) staff       (20)        0 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/__init__.py
+-rw-r--r--   0 rolf       (503) staff       (20)     6892 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/file_mixin.py
+-rw-r--r--   0 rolf       (503) staff       (20)     2769 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/format_mixin.py
+-rw-r--r--   0 rolf       (503) staff       (20)     3941 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/loaders_mixin.py
+-rw-r--r--   0 rolf       (503) staff       (20)     3416 2024-05-08 09:35:30.000000 cgelib-0.7.5/src/cgelib/utils/pliers_mixin.py
+-rw-r--r--   0 rolf       (503) staff       (20)     2736 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/savers_mixin.py
+-rw-r--r--   0 rolf       (503) staff       (20)      729 2023-11-01 14:19:44.000000 cgelib-0.7.5/src/cgelib/utils/transformer_mixin.py
+drwxr-xr-x   0 rolf       (503) staff       (20)        0 2024-05-08 09:56:14.825118 cgelib-0.7.5/src/cgelib.egg-info/
+-rw-r--r--   0 rolf       (503) staff       (20)      970 2024-05-08 09:56:14.000000 cgelib-0.7.5/src/cgelib.egg-info/PKG-INFO
+-rw-r--r--   0 rolf       (503) staff       (20)     1417 2024-05-08 09:56:14.000000 cgelib-0.7.5/src/cgelib.egg-info/SOURCES.txt
+-rw-r--r--   0 rolf       (503) staff       (20)        1 2024-05-08 09:56:14.000000 cgelib-0.7.5/src/cgelib.egg-info/dependency_links.txt
+-rw-r--r--   0 rolf       (503) staff       (20)       26 2024-05-08 09:56:14.000000 cgelib-0.7.5/src/cgelib.egg-info/requires.txt
+-rw-r--r--   0 rolf       (503) staff       (20)        7 2024-05-08 09:56:14.000000 cgelib-0.7.5/src/cgelib.egg-info/top_level.txt
```

### Comparing `cgelib-0.7.4/LICENSE.txt` & `cgelib-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/PKG-INFO` & `cgelib-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cgelib
-Version: 0.7.4
+Version: 0.7.5
 Summary: Description of my package
 Home-page: https://bitbucket.org/genomicepidemiology/cgelib.git
 Author: Center for Genomic Epidemiology
 Author-email: food-cgehelp@dtu.dk
-Project-URL: Bug Tracker, https://bitbucket.org/genomicepidemiology/cge_package/issues
+Project-URL: Bug Tracker, https://bitbucket.org/genomicepidemiology/cgelib/issues
 Project-URL: CGE website, http://genomicepidemiology.org
 Project-URL: CGE webtools, http://genomicepidemiology.org/services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cgelib-0.7.4/setup.cfg` & `cgelib-0.7.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = cgelib
-version = 0.7.4
+version = 0.7.5
 author = Center for Genomic Epidemiology
 author_email = food-cgehelp@dtu.dk
 description = Library of modules used throughout the tools developed and maintained by the Center for Genomic Epidemiology (CGE).
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://bitbucket.org/genomicepidemiology/cge_package
+url = https://bitbucket.org/genomicepidemiology/cgelib
 project_urls = 
-	Bug Tracker = https://bitbucket.org/genomicepidemiology/cge_package/issues
+	Bug Tracker = https://bitbucket.org/genomicepidemiology/cgelib/issues
 	CGE website = http://genomicepidemiology.org
 	CGE webtools = http://genomicepidemiology.org/services
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: Unix
 	Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `cgelib-0.7.4/src/cgelib/alignment/KMA/alignment_files.py` & `cgelib-0.7.5/src/cgelib/alignment/KMA/alignment_files.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/alignment/KMA/read_files.py` & `cgelib-0.7.5/src/cgelib/alignment/KMA/read_files.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/alignment/aligner.py` & `cgelib-0.7.5/src/cgelib/alignment/aligner.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/alignment/blast/alignment_files.py` & `cgelib-0.7.5/src/cgelib/alignment/blast/alignment_files.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/alignment/blast/read_files.py` & `cgelib-0.7.5/src/cgelib/alignment/blast/read_files.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/alignment/read_alignment.py` & `cgelib-0.7.5/src/cgelib/alignment/read_alignment.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/applications/Blast.py` & `cgelib-0.7.5/src/cgelib/applications/Blast.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/applications/KMA.py` & `cgelib-0.7.5/src/cgelib/applications/KMA.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/applications/command.py` & `cgelib-0.7.5/src/cgelib/applications/command.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/exceptions.py` & `cgelib-0.7.5/src/cgelib/output/exceptions.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/parserdict.py` & `cgelib-0.7.5/src/cgelib/output/parserdict.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/result.py` & `cgelib-0.7.5/src/cgelib/output/result.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/templates_json/beone/beone.json` & `cgelib-0.7.5/src/cgelib/output/templates_json/beone/beone.json`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/templates_json/beone/example.json` & `cgelib-0.7.5/src/cgelib/output/templates_json/beone/example.json`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/output/valueparsers.py` & `cgelib-0.7.5/src/cgelib/output/valueparsers.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/sequence/Feature.py` & `cgelib-0.7.5/src/cgelib/sequence/Feature.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/sequence/SeqHit.py` & `cgelib-0.7.5/src/cgelib/sequence/SeqHit.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/utils/file_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/file_mixin.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/utils/format_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/format_mixin.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/utils/loaders_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/loaders_mixin.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/utils/pliers_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/pliers_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,30 @@
             commmit_hash: The 40 character hash describing the exact commit of
             the git directory.
             version: The tag of the current commit. If no tag exists the first
             7 characters of the commit hash will be returned instead.
 
             If the given directory is not a git directory the returned values
             will be 'unknown'.
+            Likewise the git module may raise a ValueError if there are
+            problems with permissions in a git directory. In this case the
+            function will also return 'unknown'.
         """
         try:
             repo = Repo(gitdir)
-        except InvalidGitRepositoryError:
-            return ("unknown", "unknown")
 
-        com2tag = {}
-        for tag in repo.tags:
-            com2tag[tag.commit.hexsha] = str(tag)
+            com2tag = {}
+            for tag in repo.tags:
+                com2tag[tag.commit.hexsha] = str(tag)
 
-        version = com2tag.get(repo.commit().hexsha, repo.commit().hexsha[:7])
+            version = com2tag.get(repo.commit().hexsha, repo.commit().hexsha[:7])
 
-        return (version, repo.commit().hexsha)
+            return (version, repo.commit().hexsha)
+        except (InvalidGitRepositoryError, ValueError):
+            return ("unknown", "unknown")
 
     @staticmethod
     def get_version_pymodule(name):
         """
             Input: python module name
             Return: (version)
```

### Comparing `cgelib-0.7.4/src/cgelib/utils/savers_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/savers_mixin.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib/utils/transformer_mixin.py` & `cgelib-0.7.5/src/cgelib/utils/transformer_mixin.py`

 * *Files identical despite different names*

### Comparing `cgelib-0.7.4/src/cgelib.egg-info/PKG-INFO` & `cgelib-0.7.5/src/cgelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cgelib
-Version: 0.7.4
+Version: 0.7.5
 Summary: Description of my package
 Home-page: https://bitbucket.org/genomicepidemiology/cgelib.git
 Author: Center for Genomic Epidemiology
 Author-email: food-cgehelp@dtu.dk
-Project-URL: Bug Tracker, https://bitbucket.org/genomicepidemiology/cge_package/issues
+Project-URL: Bug Tracker, https://bitbucket.org/genomicepidemiology/cgelib/issues
 Project-URL: CGE website, http://genomicepidemiology.org
 Project-URL: CGE webtools, http://genomicepidemiology.org/services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cgelib-0.7.4/src/cgelib.egg-info/SOURCES.txt` & `cgelib-0.7.5/src/cgelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

