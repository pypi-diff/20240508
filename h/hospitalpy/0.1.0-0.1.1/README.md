# Comparing `tmp/hospitalpy-0.1.0.tar.gz` & `tmp/hospitalpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hospitalpy-0.1.0.tar", last modified: Wed May  1 20:57:15 2024, max compression
+gzip compressed data, was "hospitalpy-0.1.1.tar", last modified: Tue May  7 22:41:57 2024, max compression
```

## Comparing `hospitalpy-0.1.0.tar` & `hospitalpy-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-01 20:57:15.367535 hospitalpy-0.1.0/
--rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-01 20:57:15.367358 hospitalpy-0.1.0/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.0/README.md
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-01 20:57:15.367185 hospitalpy-0.1.0/hospitalpy.egg-info/
--rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-01 20:57:15.000000 hospitalpy-0.1.0/hospitalpy.egg-info/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)      169 2024-05-01 20:57:15.000000 hospitalpy-0.1.0/hospitalpy.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-01 20:57:15.000000 hospitalpy-0.1.0/hospitalpy.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-01 20:57:15.000000 hospitalpy-0.1.0/hospitalpy.egg-info/top_level.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)      389 2024-05-01 20:57:10.000000 hospitalpy-0.1.0/pyproject.toml
--rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-01 20:57:15.367572 hospitalpy-0.1.0/setup.cfg
--rw-r--r--   0 michaelchary   (501) staff       (20)      534 2024-05-01 12:37:23.000000 hospitalpy-0.1.0/setup.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 22:41:57.639615 hospitalpy-0.1.1/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-07 22:41:57.639442 hospitalpy-0.1.1/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.1/README.md
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 22:41:57.639269 hospitalpy-0.1.1/hospitalpy.egg-info/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)      169 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/top_level.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)      419 2024-05-07 22:41:54.000000 hospitalpy-0.1.1/pyproject.toml
+-rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-07 22:41:57.639655 hospitalpy-0.1.1/setup.cfg
+-rw-r--r--   0 michaelchary   (501) staff       (20)      534 2024-05-07 22:39:19.000000 hospitalpy-0.1.1/setup.py
```

### Comparing `hospitalpy-0.1.0/setup.py` & `hospitalpy-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Text Regularization for Unstructured Text from EMS Reports'
 LONG_DESCRIPTION = 'Made by Michael Chary'
 
 # Setting up
 setup(
     name="hospitalpy",
     version=VERSION,
```

