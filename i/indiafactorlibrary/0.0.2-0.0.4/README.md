# Comparing `tmp/indiafactorlibrary-0.0.2.tar.gz` & `tmp/indiafactorlibrary-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indiafactorlibrary-0.0.2.tar", last modified: Tue May  7 15:12:56 2024, max compression
+gzip compressed data, was "indiafactorlibrary-0.0.4.tar", last modified: Wed May  8 17:53:16 2024, max compression
```

## Comparing `indiafactorlibrary-0.0.2.tar` & `indiafactorlibrary-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:12:56.130839 indiafactorlibrary-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 15:12:52.000000 indiafactorlibrary-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-07 15:12:56.130839 indiafactorlibrary-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-07 15:12:52.000000 indiafactorlibrary-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:12:56.130839 indiafactorlibrary-0.0.2/indiafactorlibrary/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 15:12:52.000000 indiafactorlibrary-0.0.2/indiafactorlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-07 15:12:52.000000 indiafactorlibrary-0.0.2/indiafactorlibrary/indiafactorlibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:12:56.130839 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-07 15:12:56.000000 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-07 15:12:56.000000 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:12:56.000000 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 15:12:56.000000 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 15:12:56.000000 indiafactorlibrary-0.0.2/indiafactorlibrary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:12:56.130839 indiafactorlibrary-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 15:12:52.000000 indiafactorlibrary-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/indiafactorlibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/indiafactorlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/indiafactorlibrary/indiafactorlibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 17:53:16.000000 indiafactorlibrary-0.0.4/indiafactorlibrary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:53:16.578992 indiafactorlibrary-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 17:53:13.000000 indiafactorlibrary-0.0.4/setup.py
```

### Comparing `indiafactorlibrary-0.0.2/LICENSE` & `indiafactorlibrary-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indiafactorlibrary-0.0.2/indiafactorlibrary/indiafactorlibrary.py` & `indiafactorlibrary-0.0.4/indiafactorlibrary/indiafactorlibrary.py`

 * *Files identical despite different names*

### Comparing `indiafactorlibrary-0.0.2/setup.py` & `indiafactorlibrary-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="indiafactorlibrary",
-    version="0.0.2",
+    version="0.0.4",
     description="A Python library to fetch data from Invespar Factor library for Indian equities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "requests",
```

