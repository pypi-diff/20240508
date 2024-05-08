# Comparing `tmp/rm_tools-1.4.3.tar.gz` & `tmp/rm_tools-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm_tools-1.4.3.tar", last modified: Wed Apr 17 01:45:04 2024, max compression
+gzip compressed data, was "rm_tools-1.4.4.tar", last modified: Wed May  8 07:56:54 2024, max compression
```

## Comparing `rm_tools-1.4.3.tar` & `rm_tools-1.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 01:45:00.000000 rm_tools-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-17 01:45:00.000000 rm_tools-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 01:45:04.734009 rm_tools-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-17 01:45:00.000000 rm_tools-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/RM_Tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 01:45:04.000000 rm_tools-1.4.3/RM_Tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/calculate_RMSF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/cats/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catComplex.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/cat_simple_doQUfit.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catalogue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/catalogue1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/cats/testCat.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/clean_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_QUfit_1D_mnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMclean_1D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D_fromFITS.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/mk_test_ascii_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.726009 rm_tools-1.4.3/RMtools_1D/models_ns/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/models_ns/m7.py
--rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/rmtools_bwdepol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_1D/rmtools_bwpredict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.730009 rm_tools-1.4.3/RMtools_3D/
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/RMpeakfit_3D.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/assemble_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/create_chunks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_RMclean_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_RMsynth_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/do_fitIcube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/extract_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/make_freq_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/mk_test_cube_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMtools_3D/rescale_I_model_3D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:45:04.734009 rm_tools-1.4.3/RMutils/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/mpfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_FITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    84116 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_RM.py
--rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_plotFITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_plotTk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 01:45:00.000000 rm_tools-1.4.3/RMutils/util_rec.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:45:04.734009 rm_tools-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-17 01:45:00.000000 rm_tools-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.629675 rm_tools-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 07:56:50.000000 rm_tools-1.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 07:56:50.000000 rm_tools-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 07:56:54.629675 rm_tools-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-08 07:56:50.000000 rm_tools-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RM_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10722 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/calculate_RMSF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/cats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catComplex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/cat_simple_doQUfit.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catalogue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catalogue1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/testCat.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/clean_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_QUfit_1D_mnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMclean_1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D_fromFITS.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/mk_test_ascii_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/models_ns/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/rmtools_bwdepol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/rmtools_bwpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RMtools_3D/
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/RMpeakfit_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/assemble_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/create_chunks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_RMclean_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_RMsynth_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_fitIcube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/extract_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/make_freq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/mk_test_cube_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/rescale_I_model_3D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RMutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/mpfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_FITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85719 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_RM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_plotFITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_plotTk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:56:54.629675 rm_tools-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-08 07:56:50.000000 rm_tools-1.4.4/setup.py
```

### Comparing `rm_tools-1.4.3/LICENSE.txt` & `rm_tools-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/PKG-INFO` & `rm_tools-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.3
+Version: 1.4.4
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.3.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.4.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy<2
+Requires-Dist: numpy>1.22; python_version == "3.8"
 Requires-Dist: scipy
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: astropy
 Requires-Dist: tdqm
 Requires-Dist: deprecation
 Requires-Dist: finufft
 Provides-Extra: qufitting
```

### Comparing `rm_tools-1.4.3/README.md` & `rm_tools-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RM_Tools.egg-info/PKG-INFO` & `rm_tools-1.4.4/RM_Tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.3
+Version: 1.4.4
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.3.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.4.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy<2
+Requires-Dist: numpy>1.22; python_version == "3.8"
 Requires-Dist: scipy
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: astropy
 Requires-Dist: tdqm
 Requires-Dist: deprecation
 Requires-Dist: finufft
 Provides-Extra: qufitting
```

### Comparing `rm_tools-1.4.3/RM_Tools.egg-info/SOURCES.txt` & `rm_tools-1.4.4/RM_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RM_Tools.egg-info/entry_points.txt` & `rm_tools-1.4.4/RM_Tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/calculate_RMSF.py` & `rm_tools-1.4.4/RMtools_1D/calculate_RMSF.py`

 * *Files 20% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     if dphi == None:
         dphi = 0.1 * 2 * np.sqrt(3.0) / (l2_max - l2_min)  # ~10*FWHM
 
     phi_array = np.arange(
         -1 * phi_max / 2, phi_max / 2 + 1e-6, dphi
     )  # division by two accounts for how RMSF is always twice as wide as FDF.
 
-    RMSFcube, phi2Arr, fwhmRMSFArr, statArr = get_rmsf_planes(
+    rmsf_results = get_rmsf_planes(
         lambda2_array,
         phi_array,
         weightArr=weights_array,
         fitRMSF=True,
         fitRMSFreal=super_resolution,
         lam0Sq_m2=0 if super_resolution else None,
     )
@@ -186,15 +186,19 @@
     # Output key results to terminal:
     print("RMSF PROPERTIES:")
     print(
         "Theoretical (unweighted) FWHM:       {:.4g} rad m^-2".format(
             3.8 / (l2_max - l2_min)
         )
     )
-    print("Measured FWHM:                       {:.4g} rad m^-2".format(fwhmRMSFArr))
+    print(
+        "Measured FWHM:                       {:.4g} rad m^-2".format(
+            rmsf_results.fwhmRMSFArr
+        )
+    )
     print("Theoretical largest FD scale probed: {:.4g} rad m^-2".format(np.pi / l2_min))
     print(
         "Theoretical maximum FD*:             {:.4g} rad m^-2".format(
             np.sqrt(3.0) / dl2
         )
     )
     print(
@@ -204,23 +208,29 @@
         "* may not be reliable over very large fractional bandwidths or in data with "
     )
     print("differing channel widths or many frequency gaps.")
     # Explanation for below: This code find the local maxima in the positive half of the RMSF,
     # finds the highest amplitude one, and calls that the first sidelobe.
     try:
         x = np.diff(
-            np.sign(np.diff(np.abs(RMSFcube[RMSFcube.size // 2 :])))
+            np.sign(
+                np.diff(
+                    np.abs(rmsf_results.RMSFcube[rmsf_results.RMSFcube.size // 2 :])
+                )
+            )
         )  # -2=local max, +2=local min
         y = (
             1 + np.where(x == -2)[0]
         )  # indices of peaks, +1 is because of offset from double differencing
-        peaks = np.abs(RMSFcube[RMSFcube.size // 2 :])[y]
+        peaks = np.abs(rmsf_results.RMSFcube[rmsf_results.RMSFcube.size // 2 :])[y]
         print(
             "First sidelobe FD and amplitude:     {:.4g} rad m^-2".format(
-                phi2Arr[phi2Arr.size // 2 :][y[np.argmax(peaks)]]
+                rmsf_results.phi2Arr[rmsf_results.phi2Arr.size // 2 :][
+                    y[np.argmax(peaks)]
+                ]
             )
         )
         print(
             "                                     {:.4g} % of peak".format(
                 np.max(peaks) * 100
             )
         )
@@ -231,17 +241,23 @@
     plt.figure(figsize=(7, 7))
     plt.subplot(211)
     plt.axhline(0, color="k")
     if plotname == None:
         plt.title("Simulated RMSF")
     else:
         plt.title(plotname)
-    plt.plot(phi2Arr, np.real(RMSFcube), "b-", label="Stokes Q")
-    plt.plot(phi2Arr, np.imag(RMSFcube), "r--", label="Stokes U")
-    plt.plot(phi2Arr, np.abs(RMSFcube), "k-", label="Amplitude")
+    plt.plot(
+        rmsf_results.phi2Arr, np.real(rmsf_results.RMSFcube), "b-", label="Stokes Q"
+    )
+    plt.plot(
+        rmsf_results.phi2Arr, np.imag(rmsf_results.RMSFcube), "r--", label="Stokes U"
+    )
+    plt.plot(
+        rmsf_results.phi2Arr, np.abs(rmsf_results.RMSFcube), "k-", label="Amplitude"
+    )
     plt.legend()
     plt.xlabel(r"Faraday depth (rad m$^{-2}$)")
     plt.ylabel("RMSF (unitless)")
     plt.subplot(212)
     ax = plt.gca()
     ax.axis([0, 1, 0, 1])
     ax.axis("off")
@@ -255,15 +271,15 @@
             + "Theoretical maximum FD:              {:.4g} rad m^-2\n"
             + "\n\n\n"
             + "Lowest frequency/wavelength [GHz/cm]:  {:>7.4g}/{:.4g}\n"
             + "Highest frequency/wavelength [GHz/cm]: {:>7.4g}/{:.4g}\n"
             + "# of channels:                                {:.4g}\n"
         ).format(
             3.8 / (l2_max - l2_min),
-            fwhmRMSFArr,
+            rmsf_results.fwhmRMSFArr,
             np.pi / l2_min,
             np.sqrt(3.0) / dl2,
             np.min(freq_array) / 1e9,
             C / np.min(freq_array) * 100.0,
             np.max(freq_array) / 1e9,
             C / np.max(freq_array) * 100.0,
             freq_array.size,
@@ -278,15 +294,18 @@
             0.1,
             0.8,
             (
                 "\n\n\n\n"
                 + "First sidelobe FD and amplitude:     {:.4g} rad m^-2\n"
                 + "                                     {:.4g} % of peak"
             ).format(
-                phi2Arr[phi2Arr.size // 2 :][y[np.argmax(peaks)]], np.max(peaks) * 100
+                rmsf_results.phi2Arr[rmsf_results.phi2Arr.size // 2 :][
+                    y[np.argmax(peaks)]
+                ],
+                np.max(peaks) * 100,
             ),
             family="monospace",
             horizontalalignment="left",
             verticalalignment="top",
         )
     except:
         pass
@@ -294,15 +313,15 @@
     #    ax.text(0.,0.7,('Theoretical (unweighted) FWHM:      {:.4g} rad m^-2'.format(2*np.sqrt(3.0) / (l2_max-l2_min)))
     #    ax.text(0.,0.58,'Measured FWHM:                               {:.4g} rad m^-2'.format(fwhmRMSFArr))
     #    ax.text(0.,0.46,'Theoretical largest FD scale probed: {:.4g} rad m^-2'.format(np.pi/l2_min))
     #    ax.text(0.,0.34,'Theoretical maximum FD:                 {:.4g} rad m^-2'.format(np.sqrt(3.0)/dl2))
     #    ax.text(0.,0.22,'First sidelobe FD and amplitude:       {:.4g} rad m^-2'.format(phi2Arr[phi2Arr.size//2:][y[np.argmax(peaks)]]))
     #    ax.text(0.,0.1,'                                                           {:.4g} % of peak'.format(np.max(peaks)*100))
 
-    if plotfile != None:
+    if plotfile is not None:
         plt.savefig(plotfile, bbox_inches="tight")
     else:
         plt.show()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rm_tools-1.4.3/RMtools_1D/cats/catComplex.csv` & `rm_tools-1.4.4/RMtools_1D/cats/catComplex.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/cats/cat_simple_doQUfit.bat` & `rm_tools-1.4.4/RMtools_1D/cats/cat_simple_doQUfit.bat`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/cats/catalogue.csv` & `rm_tools-1.4.4/RMtools_1D/cats/catalogue.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/cats/catalogue1.csv` & `rm_tools-1.4.4/RMtools_1D/cats/catalogue1.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/cats/testCat.dat` & `rm_tools-1.4.4/RMtools_1D/cats/testCat.dat`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/clean_model.py` & `rm_tools-1.4.4/RMtools_1D/clean_model.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/do_QUfit_1D_mnest.py` & `rm_tools-1.4.4/RMtools_1D/do_QUfit_1D_mnest.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/do_RMclean_1D.py` & `rm_tools-1.4.4/RMtools_1D/do_RMclean_1D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D.py` & `rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/do_RMsynth_1D_fromFITS.py` & `rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D_fromFITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/mk_test_ascii_data.py` & `rm_tools-1.4.4/RMtools_1D/mk_test_ascii_data.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m1.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m1.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m11.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m11.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m111.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m111.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m2.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m2.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m3.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m3.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m4.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m4.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m5.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m5.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m6.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m6.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/models_ns/m7.py` & `rm_tools-1.4.4/RMtools_1D/models_ns/m7.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/rmtools_bwdepol.py` & `rm_tools-1.4.4/RMtools_1D/rmtools_bwdepol.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_1D/rmtools_bwpredict.py` & `rm_tools-1.4.4/RMtools_1D/rmtools_bwpredict.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/RMpeakfit_3D.py` & `rm_tools-1.4.4/RMtools_3D/RMpeakfit_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/assemble_chunks.py` & `rm_tools-1.4.4/RMtools_3D/assemble_chunks.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/create_chunks.py` & `rm_tools-1.4.4/RMtools_3D/create_chunks.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/do_RMclean_3D.py` & `rm_tools-1.4.4/RMtools_3D/do_RMclean_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/do_RMsynth_3D.py` & `rm_tools-1.4.4/RMtools_3D/do_RMsynth_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/do_fitIcube.py` & `rm_tools-1.4.4/RMtools_3D/do_fitIcube.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/extract_region.py` & `rm_tools-1.4.4/RMtools_3D/extract_region.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/make_freq_file.py` & `rm_tools-1.4.4/RMtools_3D/make_freq_file.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/mk_test_cube_data.py` & `rm_tools-1.4.4/RMtools_3D/mk_test_cube_data.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMtools_3D/rescale_I_model_3D.py` & `rm_tools-1.4.4/RMtools_3D/rescale_I_model_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/mpfit.py` & `rm_tools-1.4.4/RMutils/mpfit.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/normalize.py` & `rm_tools-1.4.4/RMutils/normalize.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/util_FITS.py` & `rm_tools-1.4.4/RMutils/util_FITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/util_RM.py` & `rm_tools-1.4.4/RMutils/util_RM.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 # DEALINGS IN THE SOFTWARE.                                                   #
 #                                                                             #
 # =============================================================================#
 
 import gc
 import math as m
 import sys
+from typing import NamedTuple
 
 import finufft
 import numpy as np
 from deprecation import deprecated
 from scipy.stats import anderson, kstest, kurtosis, kurtosistest, norm, skew, skewtest
 from tqdm.auto import tqdm, trange
 
@@ -82,25 +83,34 @@
 from . import __version__
 
 # Constants
 C = 2.99792458e8
 
 
 # -----------------------------------------------------------------------------#
+class RMsynthResults(NamedTuple):
+    """Results of the RM-synthesis calculation"""
+
+    FDFcube: np.ndarray
+    """The Faraday dispersion function cube"""
+    lam0Sq_m2: float
+    """The reference lambda^2 value"""
+
+
 def do_rmsynth_planes(
     dataQ,
     dataU,
     lambdaSqArr_m2,
     phiArr_radm2,
     weightArr=None,
     lam0Sq_m2=None,
     nBits=32,
     eps=1e-6,
     log=print,
-):
+) -> RMsynthResults:
     """Perform RM-synthesis on Stokes Q and U cubes (1,2 or 3D). This version
     of the routine loops through spectral planes and is faster than the pixel-
     by-pixel code. This version also correctly deals with isolated clumps of
     NaN-flagged voxels within the data-cube (unlikely in interferometric cubes,
     but possible in single-dish cubes). Input data must be in standard python
     [z,y,x] order, where z is the frequency axis in ascending order.
 
@@ -210,32 +220,47 @@
         FDFcube = np.reshape(
             FDFcube, (FDFcube.shape[0], old_data_shape[1], old_data_shape[2])
         )
 
     # Remove redundant dimensions in the FDF array
     FDFcube = np.squeeze(FDFcube)
 
-    return FDFcube, lam0Sq_m2
+    return RMsynthResults(FDFcube=FDFcube, lam0Sq_m2=lam0Sq_m2)
 
 
 # -----------------------------------------------------------------------------#
+class RMSFResults(NamedTuple):
+    """Results of the RMSF calculation"""
+
+    RMSFcube: np.ndarray
+    """The RMSF cube"""
+    phi2Arr: np.ndarray
+    """The (double length) Faraday depth array"""
+    fwhmRMSFArr: np.ndarray
+    """The FWHM of the RMSF main lobe"""
+    statArr: np.ndarray
+    """The status of the RMSF fit"""
+    lam0Sq_m2: float
+    """The reference lambda^2 value"""
+
+
 def get_rmsf_planes(
     lambdaSqArr_m2,
     phiArr_radm2,
     weightArr=None,
     mskArr=None,
     lam0Sq_m2=None,
     double=True,
     fitRMSF=False,
     fitRMSFreal=False,
     nBits=32,
     eps=1e-6,
     verbose=False,
     log=print,
-):
+) -> RMSFResults:
     """Calculate the Rotation Measure Spread Function from inputs. This version
     returns a cube (1, 2 or 3D) of RMSF spectra based on the shape of a
     boolean mask array, where flagged data are True and unflagged data False.
     If only whole planes (wavelength channels) are flagged then the RMSF is the
     same for all pixels and the calculation is done once and replicated to the
     dimensions of the mask. If some isolated voxels are flagged then the RMSF
     is calculated by looping through each wavelength plane, which can take some
@@ -419,18 +444,37 @@
     if nDims == 3:
         RMSFcube = np.reshape(
             RMSFcube, (RMSFcube.shape[0], old_data_shape[1], old_data_shape[2])
         )
         fwhmRMSFArr = np.reshape(fwhmRMSFArr, (old_data_shape[1], old_data_shape[2]))
         statArr = np.reshape(statArr, (old_data_shape[1], old_data_shape[2]))
 
-    return RMSFcube, phi2Arr, fwhmRMSFArr, statArr, lam0Sq_m2
+    return RMSFResults(
+        RMSFcube=RMSFcube,
+        phi2Arr=phi2Arr,
+        fwhmRMSFArr=fwhmRMSFArr,
+        statArr=statArr,
+        lam0Sq_m2=lam0Sq_m2,
+    )
 
 
 # -----------------------------------------------------------------------------#
+class RMCleanResults(NamedTuple):
+    """Results of the RM-CLEAN calculation"""
+
+    cleanFDF: np.ndarray
+    """The cleaned Faraday dispersion function cube"""
+    ccArr: np.ndarray
+    """The clean components cube"""
+    iterCountArr: np.ndarray
+    """The number of iterations for each pixel"""
+    residFDF: np.ndarray
+    """The residual Faraday dispersion function cube"""
+
+
 def do_rmclean_hogbom(
     dirtyFDF,
     phiArr_radm2,
     RMSFArr,
     phi2Arr_radm2,
     fwhmRMSFArr,
     cutoff,
@@ -440,15 +484,15 @@
     nBits=32,
     verbose=False,
     doPlots=False,
     pool=None,
     chunksize=None,
     log=print,
     window=0,
-):
+) -> RMCleanResults:
     """Perform Hogbom CLEAN on a cube of complex Faraday dispersion functions
     given a cube of rotation measure spread functions.
 
     dirtyFDF       ... 1, 2 or 3D complex FDF array
     phiArr_radm2   ... 1D Faraday depth array corresponding to the FDF
     RMSFArr        ... 1, 2 or 3D complex RMSF array
     phi2Arr_radm2  ... double size 1D Faraday depth array of the RMSF
@@ -589,18 +633,27 @@
 
     # Remove redundant dimensions
     cleanFDF = np.squeeze(cleanFDF)
     ccArr = np.squeeze(ccArr)
     iterCountArr = np.squeeze(iterCountArr)
     residFDF = np.squeeze(residFDF)
 
-    return cleanFDF, ccArr, iterCountArr, residFDF
+    return RMCleanResults(cleanFDF, ccArr, iterCountArr, residFDF)
 
 
 # -----------------------------------------------------------------------------#
+class CleanLoopResults(NamedTuple):
+    """Results of the RM-CLEAN loop"""
+
+    cleanFDF: np.ndarray
+    """The cleaned Faraday dispersion function cube"""
+    residFDF: np.ndarray
+    """The residual Faraday dispersion function cube"""
+    ccArr: np.ndarray
+    """The clean components cube"""
 
 
 class RMcleaner:
     """Allows do_rmclean_hogbom to be run in parallel
     Designed around use of schwimmbad parallelization tools.
     """
 
@@ -626,18 +679,18 @@
         self.maxIter = maxIter
         self.gain = gain
         self.cutoff = cutoff
         self.verbose = verbose
         self.nbits = nbits
         self.window = window
 
-    def cleanloop(self, args):
+    def cleanloop(self, args) -> CleanLoopResults:
         return self._cleanloop(*args)
 
-    def _cleanloop(self, yi, xi, dirtyFDF):
+    def _cleanloop(self, yi, xi, dirtyFDF) -> CleanLoopResults:
         dirtyFDF = dirtyFDF[:, yi, xi]
         # Initialise arrays to hold the residual FDF, clean components, clean FDF
         residFDF = dirtyFDF.copy()
         ccArr = np.zeros_like(dirtyFDF)
         cleanFDF = np.zeros_like(dirtyFDF)
         RMSFArr = self.RMSFArr[:, yi, xi]
         fwhmRMSFArr = self.fwhmRMSFArr[yi, xi]
@@ -720,15 +773,15 @@
             # Remake masked residual FDF
             residFDF_mask = np.ma.array(residFDF, mask=~mask)
 
         cleanFDF = np.squeeze(cleanFDF)
         residFDF = np.squeeze(residFDF)
         ccArr = np.squeeze(ccArr)
 
-        return cleanFDF, residFDF, ccArr
+        return CleanLoopResults(cleanFDF=cleanFDF, residFDF=residFDF, ccArr=ccArr)
 
 
 # -----------------------------------------------------------------------------#
 def fits_make_lin_axis(head, axis=0, dtype="f4"):
     """Create an array containing the axis values, assuming a simple linear
     projection scheme. Axis selection is zero-indexed."""
```

### Comparing `rm_tools-1.4.3/RMutils/util_misc.py` & `rm_tools-1.4.4/RMutils/util_misc.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/util_plotFITS.py` & `rm_tools-1.4.4/RMutils/util_plotFITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/util_plotTk.py` & `rm_tools-1.4.4/RMutils/util_plotTk.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/RMutils/util_rec.py` & `rm_tools-1.4.4/RMutils/util_rec.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.3/setup.py` & `rm_tools-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 from setuptools import setup
 
 NAME = "RM-Tools"
 DESCRIPTION = "RM-synthesis, RM-clean and QU-fitting on polarised radio spectra"
 URL = "https://github.com/CIRADA-Tools/RM-Tools"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.4.3"
+VERSION = "1.4.4"
 DOWNLOAD_URL = (
     "https://github.com/CIRADA-Tools/RM-Tools/archive/v" + VERSION + ".tar.gz"
 )
 
 REQUIRED = [
     "numpy<2",
+    "numpy>1.22;python_version=='3.8'",
     "scipy",
     "matplotlib>=3.4.0",
     "astropy",
     "tdqm",
     "deprecation",
     "finufft",
 ]
```

