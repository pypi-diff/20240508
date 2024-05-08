# Comparing `tmp/osmx-0.0.4.tar.gz` & `tmp/osmx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osmx-0.0.4.tar", last modified: Mon Jul 13 14:16:11 2020, max compression
+gzip compressed data, was "osmx-0.0.5.tar", last modified: Wed May  8 06:31:31 2024, max compression
```

## Comparing `osmx-0.0.4.tar` & `osmx-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2020-07-13 14:16:11.000000 osmx-0.0.4/
--rw-r--r--   0 bdon       (501) staff       (20)     1174 2020-07-13 14:16:11.000000 osmx-0.0.4/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)      497 2019-09-17 20:26:47.000000 osmx-0.0.4/README.md
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2020-07-13 14:16:11.000000 osmx-0.0.4/osmx/
--rw-r--r--   0 bdon       (501) staff       (20)       19 2019-09-17 20:26:47.000000 osmx-0.0.4/osmx/__init__.py
--rw-r--r--   0 bdon       (501) staff       (20)      547 2020-06-09 06:26:22.000000 osmx-0.0.4/osmx/messages.capnp
--rw-r--r--   0 bdon       (501) staff       (20)     3307 2020-06-19 15:26:58.000000 osmx-0.0.4/osmx/osmx.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2020-07-13 14:16:11.000000 osmx-0.0.4/osmx.egg-info/
--rw-r--r--   0 bdon       (501) staff       (20)     1174 2020-07-13 14:16:10.000000 osmx-0.0.4/osmx.egg-info/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)      207 2020-07-13 14:16:10.000000 osmx-0.0.4/osmx.egg-info/SOURCES.txt
--rw-r--r--   0 bdon       (501) staff       (20)        1 2020-07-13 14:16:10.000000 osmx-0.0.4/osmx.egg-info/dependency_links.txt
--rw-r--r--   0 bdon       (501) staff       (20)       26 2020-07-13 14:16:10.000000 osmx-0.0.4/osmx.egg-info/requires.txt
--rw-r--r--   0 bdon       (501) staff       (20)        5 2020-07-13 14:16:10.000000 osmx-0.0.4/osmx.egg-info/top_level.txt
--rw-r--r--   0 bdon       (501) staff       (20)       38 2020-07-13 14:16:11.000000 osmx-0.0.4/setup.cfg
--rw-r--r--   0 bdon       (501) staff       (20)      822 2020-06-19 08:51:52.000000 osmx-0.0.4/setup.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2024-05-08 06:31:31.122947 osmx-0.0.5/
+-rw-r--r--   0 bdon       (501) staff       (20)     1366 2024-05-08 06:31:31.122836 osmx-0.0.5/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)      932 2022-01-20 15:46:21.000000 osmx-0.0.5/README.md
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2024-05-08 06:31:31.122105 osmx-0.0.5/osmx/
+-rw-r--r--   0 bdon       (501) staff       (20)       19 2022-01-20 15:46:21.000000 osmx-0.0.5/osmx/__init__.py
+-rw-r--r--   0 bdon       (501) staff       (20)      547 2022-01-20 15:46:21.000000 osmx-0.0.5/osmx/messages.capnp
+-rw-r--r--   0 bdon       (501) staff       (20)     3307 2022-01-20 15:46:21.000000 osmx-0.0.5/osmx/osmx.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2024-05-08 06:31:31.122668 osmx-0.0.5/osmx.egg-info/
+-rw-r--r--   0 bdon       (501) staff       (20)     1366 2024-05-08 06:31:31.000000 osmx-0.0.5/osmx.egg-info/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)      207 2024-05-08 06:31:31.000000 osmx-0.0.5/osmx.egg-info/SOURCES.txt
+-rw-r--r--   0 bdon       (501) staff       (20)        1 2024-05-08 06:31:31.000000 osmx-0.0.5/osmx.egg-info/dependency_links.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       27 2024-05-08 06:31:31.000000 osmx-0.0.5/osmx.egg-info/requires.txt
+-rw-r--r--   0 bdon       (501) staff       (20)        5 2024-05-08 06:31:31.000000 osmx-0.0.5/osmx.egg-info/top_level.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       38 2024-05-08 06:31:31.122988 osmx-0.0.5/setup.cfg
+-rw-r--r--   0 bdon       (501) staff       (20)      824 2024-05-08 06:30:37.000000 osmx-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `osmx-0.0.4/osmx/messages.capnp` & `osmx-0.0.5/osmx/messages.capnp`

 * *Files identical despite different names*

### Comparing `osmx-0.0.4/osmx/osmx.py` & `osmx-0.0.5/osmx/osmx.py`

 * *Files identical despite different names*

### Comparing `osmx-0.0.4/setup.py` & `osmx-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [
-    'lmdb~=0.98',
-    'pycapnp~=0.6.4',
+    'lmdb~=1.4.1',
+    'pycapnp~=2.0.0',
 ]
 
 setuptools.setup(
     name='osmx',
-    version='0.0.4',
+    version='0.0.5',
     author="Brandon Liu",
     author_email='brandon@protomaps.com',
     description='Read OSM Express (.osmx) database files.',
     license="BSD-2-Clause",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/protomaps/OSMExpress",
@@ -23,8 +23,8 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     install_requires = requirements,
     requires_python='>=3.0',
     package_data={'osmx':['messages.capnp']}
-)
+)
```

