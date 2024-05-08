# Comparing `tmp/ls_packers-0.5.0.tar.gz` & `tmp/ls_packers-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_packers-0.5.0.tar", last modified: Tue Apr 30 12:54:44 2024, max compression
+gzip compressed data, was "ls_packers-0.5.1.tar", last modified: Tue May  7 23:59:24 2024, max compression
```

## Comparing `ls_packers-0.5.0.tar` & `ls_packers-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:54:44.560713 ls_packers-0.5.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-04-30 12:54:20.000000 ls_packers-0.5.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-04-30 12:54:44.556713 ls_packers-0.5.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2024-04-30 12:54:20.000000 ls_packers-0.5.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:54:44.556713 ls_packers-0.5.0/ls_packers/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      493 2024-04-30 12:54:20.000000 ls_packers-0.5.0/ls_packers/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2024-04-30 12:54:20.000000 ls_packers-0.5.0/ls_packers/converters.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2024-04-30 12:54:20.000000 ls_packers-0.5.0/ls_packers/packers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:54:44.556713 ls_packers-0.5.0/ls_packers.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-04-30 12:54:44.000000 ls_packers-0.5.0/ls_packers.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      335 2024-04-30 12:54:44.000000 ls_packers-0.5.0/ls_packers.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-30 12:54:44.000000 ls_packers-0.5.0/ls_packers.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-30 12:54:44.000000 ls_packers-0.5.0/ls_packers.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-04-30 12:54:44.000000 ls_packers-0.5.0/ls_packers.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-30 12:54:41.000000 ls_packers-0.5.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-30 12:54:44.560713 ls_packers-0.5.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-30 12:54:44.556713 ls_packers-0.5.0/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-04-30 12:54:20.000000 ls_packers-0.5.0/tests/test_float_array_packers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      747 2024-04-30 12:54:20.000000 ls_packers-0.5.0/tests/test_triu_conversion.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:59:24.327097 ls_packers-0.5.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-05-07 23:56:49.000000 ls_packers-0.5.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-07 23:59:24.327097 ls_packers-0.5.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2024-05-07 23:56:49.000000 ls_packers-0.5.1/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:59:24.327097 ls_packers-0.5.1/ls_packers/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      493 2024-05-07 23:56:49.000000 ls_packers-0.5.1/ls_packers/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1152 2024-05-07 23:56:49.000000 ls_packers-0.5.1/ls_packers/converters.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2024-05-07 23:56:49.000000 ls_packers-0.5.1/ls_packers/packers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:59:24.327097 ls_packers-0.5.1/ls_packers.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-07 23:59:24.000000 ls_packers-0.5.1/ls_packers.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      335 2024-05-07 23:59:24.000000 ls_packers-0.5.1/ls_packers.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 23:59:24.000000 ls_packers-0.5.1/ls_packers.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-07 23:59:24.000000 ls_packers-0.5.1/ls_packers.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-07 23:59:24.000000 ls_packers-0.5.1/ls_packers.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      649 2024-05-07 23:59:21.000000 ls_packers-0.5.1/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 23:59:24.327097 ls_packers-0.5.1/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 23:59:24.327097 ls_packers-0.5.1/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-07 23:56:49.000000 ls_packers-0.5.1/tests/test_float_array_packers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      747 2024-05-07 23:56:49.000000 ls_packers-0.5.1/tests/test_triu_conversion.py
```

### Comparing `ls_packers-0.5.0/LICENSE` & `ls_packers-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.0/PKG-INFO` & `ls_packers-0.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ls-packers
-Version: 0.5.0
+Version: 0.5.1
 Summary: An internal client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: msgpack
```

### Comparing `ls_packers-0.5.0/ls_packers/converters.py` & `ls_packers-0.5.1/ls_packers/converters.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.0/ls_packers/packers.py` & `ls_packers-0.5.1/ls_packers/packers.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.0/ls_packers.egg-info/PKG-INFO` & `ls_packers-0.5.1/ls_packers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ls-packers
-Version: 0.5.0
+Version: 0.5.1
 Summary: An internal client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: msgpack
```

### Comparing `ls_packers-0.5.0/pyproject.toml` & `ls_packers-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-packers"
-version = "0.5.0"
+version = "0.5.1"
 description = "An internal client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "msgpack",]
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

### Comparing `ls_packers-0.5.0/tests/test_float_array_packers.py` & `ls_packers-0.5.1/tests/test_float_array_packers.py`

 * *Files identical despite different names*

### Comparing `ls_packers-0.5.0/tests/test_triu_conversion.py` & `ls_packers-0.5.1/tests/test_triu_conversion.py`

 * *Files identical despite different names*

