# Comparing `tmp/pylutron-0.2.8.tar.gz` & `tmp/pylutron-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylutron-0.2.8.tar", last modified: Thu Jul  8 03:41:18 2021, max compression
+gzip compressed data, was "pylutron-0.2.9.tar", last modified: Sat Jul 17 01:22:22 2021, max compression
```

## Comparing `pylutron-0.2.8.tar` & `pylutron-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jongilmore   (502) staff       (20)        0 2021-07-08 03:41:18.648240 pylutron-0.2.8/
--rw-r--r--   0 jongilmore   (502) staff       (20)     1077 2021-07-08 03:39:37.000000 pylutron-0.2.8/LICENSE
--rw-r--r--   0 jongilmore   (502) staff       (20)      593 2021-07-08 03:41:18.647664 pylutron-0.2.8/PKG-INFO
--rw-r--r--   0 jongilmore   (502) staff       (20)      405 2021-07-08 03:39:37.000000 pylutron-0.2.8/README.md
-drwxr-xr-x   0 jongilmore   (502) staff       (20)        0 2021-07-08 03:41:18.643034 pylutron-0.2.8/pylutron/
--rw-r--r--   0 jongilmore   (502) staff       (20)    43238 2021-07-08 03:39:37.000000 pylutron-0.2.8/pylutron/__init__.py
-drwxr-xr-x   0 jongilmore   (502) staff       (20)        0 2021-07-08 03:41:18.646945 pylutron-0.2.8/pylutron.egg-info/
--rw-r--r--   0 jongilmore   (502) staff       (20)      593 2021-07-08 03:41:18.000000 pylutron-0.2.8/pylutron.egg-info/PKG-INFO
--rw-r--r--   0 jongilmore   (502) staff       (20)      202 2021-07-08 03:41:18.000000 pylutron-0.2.8/pylutron.egg-info/SOURCES.txt
--rw-r--r--   0 jongilmore   (502) staff       (20)        1 2021-07-08 03:41:18.000000 pylutron-0.2.8/pylutron.egg-info/dependency_links.txt
--rw-r--r--   0 jongilmore   (502) staff       (20)        9 2021-07-08 03:41:18.000000 pylutron-0.2.8/pylutron.egg-info/top_level.txt
--rw-r--r--   0 jongilmore   (502) staff       (20)        1 2021-07-08 03:41:18.000000 pylutron-0.2.8/pylutron.egg-info/zip-safe
--rw-r--r--   0 jongilmore   (502) staff       (20)       38 2021-07-08 03:41:18.648460 pylutron-0.2.8/setup.cfg
--rw-r--r--   0 jongilmore   (502) staff       (20)      757 2021-07-08 03:40:18.000000 pylutron-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-17 01:22:22.067795 pylutron-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-07-17 01:22:13.000000 pylutron-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-07-17 01:22:22.067795 pylutron-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-07-17 01:22:13.000000 pylutron-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-17 01:22:22.063795 pylutron-0.2.9/pylutron/
+-rw-r--r--   0 runner    (1001) docker     (121)    43238 2021-07-17 01:22:13.000000 pylutron-0.2.9/pylutron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-17 01:22:22.067795 pylutron-0.2.9/pylutron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-07-17 01:22:21.000000 pylutron-0.2.9/pylutron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-07-17 01:22:21.000000 pylutron-0.2.9/pylutron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-17 01:22:21.000000 pylutron-0.2.9/pylutron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-17 01:22:21.000000 pylutron-0.2.9/pylutron.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-17 01:22:21.000000 pylutron-0.2.9/pylutron.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-17 01:22:22.067795 pylutron-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-07-17 01:22:13.000000 pylutron-0.2.9/setup.py
```

### Comparing `pylutron-0.2.8/LICENSE` & `pylutron-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylutron-0.2.8/PKG-INFO` & `pylutron-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pylutron
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library for Lutron RadioRA 2
 Home-page: http://github.com/thecynic/pylutron
 Author: Dima Zavin
 Author-email: thecynic@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pylutron-0.2.8/pylutron/__init__.py` & `pylutron-0.2.9/pylutron/__init__.py`

 * *Files identical despite different names*

### Comparing `pylutron-0.2.8/pylutron.egg-info/PKG-INFO` & `pylutron-0.2.9/pylutron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pylutron
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library for Lutron RadioRA 2
 Home-page: http://github.com/thecynic/pylutron
 Author: Dima Zavin
 Author-email: thecynic@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pylutron-0.2.8/setup.py` & `pylutron-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'pylutron',
-    version = '0.2.8',
+    version = '0.2.9',
     license = 'MIT',
     description = 'Python library for Lutron RadioRA 2',
     author = 'Dima Zavin',
     author_email = 'thecynic@gmail.com',
     url = 'http://github.com/thecynic/pylutron',
     packages=find_packages(),
     classifiers = [
```

