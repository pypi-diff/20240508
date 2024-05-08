# Comparing `tmp/hospitalpy-0.1.23.tar.gz` & `tmp/hospitalpy-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hospitalpy-0.1.23.tar", last modified: Wed May  8 00:55:48 2024, max compression
+gzip compressed data, was "hospitalpy-0.1.24.tar", last modified: Wed May  8 01:00:39 2024, max compression
```

## Comparing `hospitalpy-0.1.23.tar` & `hospitalpy-0.1.24.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:48.285307 hospitalpy-0.1.23/
--rw-r--r--   0 michaelchary   (501) staff       (20)     1074 2024-05-08 00:29:19.000000 hospitalpy-0.1.23/LICENSE
--rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 00:55:48.285084 hospitalpy-0.1.23/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.23/README.md
--rw-r--r--   0 michaelchary   (501) staff       (20)      527 2024-05-08 00:55:26.000000 hospitalpy-0.1.23/pyproject.toml
--rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-08 00:55:48.285353 hospitalpy-0.1.23/setup.cfg
--rw-r--r--   0 michaelchary   (501) staff       (20)      535 2024-05-08 00:55:37.000000 hospitalpy-0.1.23/setup.py
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:48.282842 hospitalpy-0.1.23/src/
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:48.284026 hospitalpy-0.1.23/src/hospitalpy/
--rw-r--r--   0 michaelchary   (501) staff       (20)      760 2024-05-08 00:15:32.000000 hospitalpy-0.1.23/src/hospitalpy/Evaluator.py
--rw-r--r--   0 michaelchary   (501) staff       (20)     4359 2024-05-08 00:54:16.000000 hospitalpy-0.1.23/src/hospitalpy/Tokenizer.py
--rw-r--r--   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:10.000000 hospitalpy-0.1.23/src/hospitalpy/__init__.py
--rw-r--r--   0 michaelchary   (501) staff       (20)      159 2024-05-08 00:15:32.000000 hospitalpy-0.1.23/src/hospitalpy/config.py
--rw-r--r--   0 michaelchary   (501) staff       (20)     1205 2024-05-08 00:15:32.000000 hospitalpy-0.1.23/src/hospitalpy/sandbox.py
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:48.284866 hospitalpy-0.1.23/src/hospitalpy.egg-info/
--rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 00:55:48.000000 hospitalpy-0.1.23/src/hospitalpy.egg-info/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)      364 2024-05-08 00:55:48.000000 hospitalpy-0.1.23/src/hospitalpy.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-08 00:55:48.000000 hospitalpy-0.1.23/src/hospitalpy.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)       13 2024-05-08 00:55:48.000000 hospitalpy-0.1.23/src/hospitalpy.egg-info/requires.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)       11 2024-05-08 00:55:48.000000 hospitalpy-0.1.23/src/hospitalpy.egg-info/top_level.txt
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 01:00:39.572256 hospitalpy-0.1.24/
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1074 2024-05-08 00:29:19.000000 hospitalpy-0.1.24/LICENSE
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 01:00:39.572040 hospitalpy-0.1.24/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.24/README.md
+-rw-r--r--   0 michaelchary   (501) staff       (20)      527 2024-05-08 01:00:23.000000 hospitalpy-0.1.24/pyproject.toml
+-rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-08 01:00:39.572301 hospitalpy-0.1.24/setup.cfg
+-rw-r--r--   0 michaelchary   (501) staff       (20)      535 2024-05-08 01:00:30.000000 hospitalpy-0.1.24/setup.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 01:00:39.569964 hospitalpy-0.1.24/src/
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 01:00:39.571079 hospitalpy-0.1.24/src/hospitalpy/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      760 2024-05-08 00:15:32.000000 hospitalpy-0.1.24/src/hospitalpy/Evaluator.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)     4359 2024-05-08 00:54:16.000000 hospitalpy-0.1.24/src/hospitalpy/Tokenizer.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:55:10.000000 hospitalpy-0.1.24/src/hospitalpy/__init__.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)      161 2024-05-08 01:00:02.000000 hospitalpy-0.1.24/src/hospitalpy/config.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1205 2024-05-08 00:15:32.000000 hospitalpy-0.1.24/src/hospitalpy/sandbox.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 01:00:39.571861 hospitalpy-0.1.24/src/hospitalpy.egg-info/
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 01:00:39.000000 hospitalpy-0.1.24/src/hospitalpy.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)      364 2024-05-08 01:00:39.000000 hospitalpy-0.1.24/src/hospitalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-08 01:00:39.000000 hospitalpy-0.1.24/src/hospitalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)       13 2024-05-08 01:00:39.000000 hospitalpy-0.1.24/src/hospitalpy.egg-info/requires.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)       11 2024-05-08 01:00:39.000000 hospitalpy-0.1.24/src/hospitalpy.egg-info/top_level.txt
```

### Comparing `hospitalpy-0.1.23/LICENSE` & `hospitalpy-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `hospitalpy-0.1.23/PKG-INFO` & `hospitalpy-0.1.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hospitalpy
-Version: 0.1.23
+Version: 0.1.24
 Summary: Text Regularization for Unstructured Text from EMS Reports
 Author: Michael Chary
 Author-email: "M. Anand Chary" <mic9189@med.cornell.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hospitalpy-0.1.23/pyproject.toml` & `hospitalpy-0.1.24/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hospitalpy"
-version = "0.1.23"
+version = "0.1.24"
 authors = [{name="M. Anand Chary", email="mic9189@med.cornell.edu"}]
 license = {'file'= 'LICENSE'}
 description = 'Text Regularization for Unstructured Text from EMS Reports'
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["NLP", "Text Regularization", "EMS Reports"]
 dependencies = ['pandas', 'regex']
```

### Comparing `hospitalpy-0.1.23/setup.py` & `hospitalpy-0.1.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.23'
+VERSION = '0.1.24'
 DESCRIPTION = 'Text Regularization for Unstructured Text from EMS Reports'
 LONG_DESCRIPTION = 'Made by Michael Chary'
 
 # Setting up
 setup(
     name="hospitalpy",
     version=VERSION,
```

### Comparing `hospitalpy-0.1.23/src/hospitalpy/Evaluator.py` & `hospitalpy-0.1.24/src/hospitalpy/Evaluator.py`

 * *Files identical despite different names*

### Comparing `hospitalpy-0.1.23/src/hospitalpy/Tokenizer.py` & `hospitalpy-0.1.24/src/hospitalpy/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `hospitalpy-0.1.23/src/hospitalpy/sandbox.py` & `hospitalpy-0.1.24/src/hospitalpy/sandbox.py`

 * *Files identical despite different names*

### Comparing `hospitalpy-0.1.23/src/hospitalpy.egg-info/PKG-INFO` & `hospitalpy-0.1.24/src/hospitalpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hospitalpy
-Version: 0.1.23
+Version: 0.1.24
 Summary: Text Regularization for Unstructured Text from EMS Reports
 Author: Michael Chary
 Author-email: "M. Anand Chary" <mic9189@med.cornell.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

