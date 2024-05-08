# Comparing `tmp/NorrisUtils-1.3.3.tar.gz` & `tmp/NorrisUtils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NorrisUtils-1.3.3.tar", last modified: Tue Oct 17 09:28:03 2023, max compression
+gzip compressed data, was "NorrisUtils-1.4.0.tar", last modified: Wed May  8 02:32:53 2024, max compression
```

## Comparing `NorrisUtils-1.3.3.tar` & `NorrisUtils-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2023-10-17 09:28:03.349080 NorrisUtils-1.3.3/
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2023-10-17 09:28:03.346187 NorrisUtils-1.3.3/NorrisUtils/
--rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/BuildConfig.py
--rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.3.3/NorrisUtils/FileUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/GarbageGenius.py
--rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/RawUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/RawUtils.py
--rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/RequestUtils.py
--rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/NorrisUtils/__init__.py
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2023-10-17 09:28:03.348231 NorrisUtils-1.3.3/NorrisUtils.egg-info/
--rw-r--r--   0 htd        (502) staff       (20)      973 2023-10-17 09:28:03.000000 NorrisUtils-1.3.3/NorrisUtils.egg-info/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)      371 2023-10-17 09:28:03.000000 NorrisUtils-1.3.3/NorrisUtils.egg-info/SOURCES.txt
--rw-r--r--   0 htd        (502) staff       (20)        1 2023-10-17 09:28:03.000000 NorrisUtils-1.3.3/NorrisUtils.egg-info/dependency_links.txt
--rw-r--r--   0 htd        (502) staff       (20)       17 2023-10-17 09:28:03.000000 NorrisUtils-1.3.3/NorrisUtils.egg-info/requires.txt
--rw-r--r--   0 htd        (502) staff       (20)       12 2023-10-17 09:28:03.000000 NorrisUtils-1.3.3/NorrisUtils.egg-info/top_level.txt
--rw-r--r--   0 htd        (502) staff       (20)      973 2023-10-17 09:28:03.348622 NorrisUtils-1.3.3/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.3.3/README.md
--rw-r--r--   0 htd        (502) staff       (20)       38 2023-10-17 09:28:03.349233 NorrisUtils-1.3.3/setup.cfg
--rw-r--r--   0 htd        (502) staff       (20)     1203 2023-10-17 09:25:27.000000 NorrisUtils-1.3.3/setup.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.172912 NorrisUtils-1.4.0/
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.170669 NorrisUtils-1.4.0/NorrisUtils/
+-rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/BuildConfig.py
+-rw-r--r--   0 htd        (502) staff       (20)    12573 2024-05-07 09:49:57.000000 NorrisUtils-1.4.0/NorrisUtils/DingTalkGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.0/NorrisUtils/FileUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/GarbageGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     2939 2024-04-30 02:40:51.000000 NorrisUtils-1.4.0/NorrisUtils/ImageUploadUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RawUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RawUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/RequestUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/NorrisUtils/__init__.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 02:32:53.172309 NorrisUtils-1.4.0/NorrisUtils.egg-info/
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/requires.txt
+-rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 02:32:53.000000 NorrisUtils-1.4.0/NorrisUtils.egg-info/top_level.txt
+-rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 02:32:53.172628 NorrisUtils-1.4.0/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.0/README.md
+-rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 02:32:53.172989 NorrisUtils-1.4.0/setup.cfg
+-rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 02:32:47.000000 NorrisUtils-1.4.0/setup.py
```

### Comparing `NorrisUtils-1.3.3/NorrisUtils/FileUtil.py` & `NorrisUtils-1.4.0/NorrisUtils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.3.3/NorrisUtils/GarbageGenius.py` & `NorrisUtils-1.4.0/NorrisUtils/GarbageGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.3.3/NorrisUtils/RawUtil.py` & `NorrisUtils-1.4.0/NorrisUtils/RawUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.3.3/NorrisUtils/RawUtils.py` & `NorrisUtils-1.4.0/NorrisUtils/RawUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.3.3/NorrisUtils/RequestUtils.py` & `NorrisUtils-1.4.0/NorrisUtils/RequestUtils.py`

 * *Files identical despite different names*

