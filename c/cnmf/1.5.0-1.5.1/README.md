# Comparing `tmp/cnmf-1.5.0.tar.gz` & `tmp/cnmf-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmf-1.5.0.tar", last modified: Wed May  8 01:43:24 2024, max compression
+gzip compressed data, was "cnmf-1.5.1.tar", last modified: Wed May  8 02:08:07 2024, max compression
```

## Comparing `cnmf-1.5.0.tar` & `cnmf-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.434764 cnmf-1.5.0/
--rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-07 19:11:38.000000 cnmf-1.5.0/LICENSE
--rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 01:43:24.433735 cnmf-1.5.0/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)     8519 2024-05-08 00:36:16.000000 cnmf-1.5.0/README.md
--rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-07 19:11:38.000000 cnmf-1.5.0/pyproject.toml
--rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 01:43:24.434978 cnmf-1.5.0/setup.cfg
--rw-r--r--   0 dkotliar   (503) staff       (20)     1035 2024-05-07 21:44:08.000000 cnmf-1.5.0/setup.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.424611 cnmf-1.5.0/src/
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.429215 cnmf-1.5.0/src/cnmf/
--rw-r--r--   0 dkotliar   (503) staff       (20)       97 2024-05-07 19:12:10.000000 cnmf-1.5.0/src/cnmf/__init__.py
--rwxr-xr-x   0 dkotliar   (503) staff       (20)    52529 2024-05-07 21:33:04.000000 cnmf-1.5.0/src/cnmf/cnmf.py
--rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 00:41:00.000000 cnmf-1.5.0/src/cnmf/preprocess.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.433030 cnmf-1.5.0/src/cnmf.egg-info/
--rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)      296 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/SOURCES.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/dependency_links.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/entry_points.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/requires.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.585057 cnmf-1.5.1/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-08 01:55:03.000000 cnmf-1.5.1/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 02:08:07.584457 cnmf-1.5.1/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     8519 2024-05-08 01:55:03.000000 cnmf-1.5.1/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-08 01:55:03.000000 cnmf-1.5.1/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 02:08:07.585225 cnmf-1.5.1/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1333 2024-05-08 02:05:15.000000 cnmf-1.5.1/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.572333 cnmf-1.5.1/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.578814 cnmf-1.5.1/src/cnmf/
+-rw-r--r--   0 dkotliar   (503) staff       (20)      131 2024-05-08 02:03:33.000000 cnmf-1.5.1/src/cnmf/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    52529 2024-05-08 01:55:03.000000 cnmf-1.5.1/src/cnmf/cnmf.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 01:55:03.000000 cnmf-1.5.1/src/cnmf/preprocess.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)       22 2024-05-08 02:03:15.000000 cnmf-1.5.1/src/cnmf/version.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.583459 cnmf-1.5.1/src/cnmf.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      316 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/top_level.txt
```

### Comparing `cnmf-1.5.0/LICENSE` & `cnmf-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.0/PKG-INFO` & `cnmf-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmf
-Version: 1.5.0
+Version: 1.5.1
 Summary: Consensus NMF for scRNA-Seq data
 Home-page: https://github.com/dylkot/cNMF
 Author: Dylan Kotliar
 Author-email: dylkot@gmail.com
 Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cnmf-1.5.0/README.md` & `cnmf-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.0/setup.py` & `cnmf-1.5.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import setuptools
+import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
+# Function to read the version from version.py
+def get_version():
+    base_dir = os.path.dirname(os.path.realpath(__file__))
+    with open(os.path.join(base_dir, 'src/cnmf/version.py')) as f:
+        locals = {}
+        exec(f.read(), locals)
+        return locals['__version__']
+
 setuptools.setup(
     name="cnmf",
-    version="1.5.0",
+    version=get_version(),
     author="Dylan Kotliar",
     author_email="dylkot@gmail.com",
     description="Consensus NMF for scRNA-Seq data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dylkot/cNMF",
     project_urls={
```

### Comparing `cnmf-1.5.0/src/cnmf/cnmf.py` & `cnmf-1.5.1/src/cnmf/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.0/src/cnmf/preprocess.py` & `cnmf-1.5.1/src/cnmf/preprocess.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.0/src/cnmf.egg-info/PKG-INFO` & `cnmf-1.5.1/src/cnmf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmf
-Version: 1.5.0
+Version: 1.5.1
 Summary: Consensus NMF for scRNA-Seq data
 Home-page: https://github.com/dylkot/cNMF
 Author: Dylan Kotliar
 Author-email: dylkot@gmail.com
 Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

