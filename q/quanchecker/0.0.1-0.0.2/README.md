# Comparing `tmp/quanchecker-0.0.1.tar.gz` & `tmp/quanchecker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanchecker-0.0.1.tar", last modified: Tue May  7 20:14:30 2024, max compression
+gzip compressed data, was "quanchecker-0.0.2.tar", last modified: Wed May  8 09:56:25 2024, max compression
```

## Comparing `quanchecker-0.0.1.tar` & `quanchecker-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 20:14:30.540436 quanchecker-0.0.1/
--rw-rw-rw-   0        0        0      506 2024-05-07 20:14:30.538416 quanchecker-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 20:14:30.476346 quanchecker-0.0.1/quanchecker/
--rw-rw-rw-   0        0        0       66 2024-05-07 19:59:06.000000 quanchecker-0.0.1/quanchecker/__init__.py
--rw-rw-rw-   0        0        0     5291 2024-05-07 19:56:36.000000 quanchecker-0.0.1/quanchecker/checker_lib.py
-drwxrwxrwx   0        0        0        0 2024-05-07 20:14:30.538210 quanchecker-0.0.1/quanchecker.egg-info/
--rw-rw-rw-   0        0        0      506 2024-05-07 20:14:30.000000 quanchecker-0.0.1/quanchecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-07 20:14:30.000000 quanchecker-0.0.1/quanchecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 20:14:30.000000 quanchecker-0.0.1/quanchecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-07 20:14:30.000000 quanchecker-0.0.1/quanchecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 20:14:30.000000 quanchecker-0.0.1/quanchecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 20:14:30.540436 quanchecker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-05-07 20:05:10.000000 quanchecker-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:56:25.120364 quanchecker-0.0.2/
+-rw-rw-rw-   0        0        0      506 2024-05-08 09:56:25.115734 quanchecker-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 09:56:25.031511 quanchecker-0.0.2/quanchecker/
+-rw-rw-rw-   0        0        0      145 2024-05-08 09:55:31.000000 quanchecker-0.0.2/quanchecker/__init__.py
+-rw-rw-rw-   0        0        0     5291 2024-05-07 19:56:36.000000 quanchecker-0.0.2/quanchecker/checker_lib.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:56:25.112169 quanchecker-0.0.2/quanchecker.egg-info/
+-rw-rw-rw-   0        0        0      506 2024-05-08 09:56:24.000000 quanchecker-0.0.2/quanchecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-08 09:56:24.000000 quanchecker-0.0.2/quanchecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:56:24.000000 quanchecker-0.0.2/quanchecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 09:56:24.000000 quanchecker-0.0.2/quanchecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 09:56:24.000000 quanchecker-0.0.2/quanchecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:56:25.120364 quanchecker-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-05-08 09:55:59.000000 quanchecker-0.0.2/setup.py
```

### Comparing `quanchecker-0.0.1/quanchecker/checker_lib.py` & `quanchecker-0.0.2/quanchecker/checker_lib.py`

 * *Files identical despite different names*

### Comparing `quanchecker-0.0.1/setup.py` & `quanchecker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Checker Library for QuanC'
 
 # Setting up
 setup(
     name="quanchecker",
     version=VERSION,
     author="QuanC",
```

