# Comparing `tmp/allelefinder-0.4.3.tar.gz` & `tmp/allelefinder-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.4.3.tar", last modified: Mon May  6 20:00:35 2024, max compression
+gzip compressed data, was "allelefinder-0.4.4.tar", last modified: Tue May  7 13:50:59 2024, max compression
```

## Comparing `allelefinder-0.4.3.tar` & `allelefinder-0.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:35.179852 allelefinder-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:35.179852 allelefinder-0.4.3/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 20:00:35.000000 allelefinder-0.4.3/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 20:00:26.000000 allelefinder-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 20:00:26.000000 allelefinder-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 20:00:35.179852 allelefinder-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 20:00:26.000000 allelefinder-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:35.175852 allelefinder-0.4.3/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:00:26.000000 allelefinder-0.4.3/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 20:00:26.000000 allelefinder-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:00:35.179852 allelefinder-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-06 20:00:26.000000 allelefinder-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:35.179852 allelefinder-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 20:00:26.000000 allelefinder-0.4.3/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:59.084498 allelefinder-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:59.084498 allelefinder-0.4.4/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:50:59.000000 allelefinder-0.4.4/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-07 13:50:50.000000 allelefinder-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 13:50:50.000000 allelefinder-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-07 13:50:59.084498 allelefinder-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-07 13:50:50.000000 allelefinder-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:59.080498 allelefinder-0.4.4/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 13:50:50.000000 allelefinder-0.4.4/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 13:50:50.000000 allelefinder-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:50:59.084498 allelefinder-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-07 13:50:50.000000 allelefinder-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:59.080498 allelefinder-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-07 13:50:50.000000 allelefinder-0.4.4/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.4.3/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.4.4/AlleleFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.4.3
+Version: 0.4.4
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.4.3/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.4.4/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/LICENSE` & `allelefinder-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/PKG-INFO` & `allelefinder-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.4.3
+Version: 0.4.4
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.4.3/README.md` & `allelefinder-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/allele_profiler.py` & `allelefinder-0.4.4/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/allele_translate_reduce.py` & `allelefinder-0.4.4/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/allele_updater.py` & `allelefinder-0.4.4/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/methods.py` & `allelefinder-0.4.4/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/profile_reduce.py` & `allelefinder-0.4.4/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/allele_tools/stec.py` & `allelefinder-0.4.4/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/setup.py` & `allelefinder-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_0_profile_reduce.py` & `allelefinder-0.4.4/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.4.4/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_2_allele_updater.py` & `allelefinder-0.4.4/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.4.4/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.4.4/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_5_stec_allele_find.py` & `allelefinder-0.4.4/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.4.4/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_7_stec_allele_split.py` & `allelefinder-0.4.4/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.4.4/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.4.3/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.4.4/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*

