# Comparing `tmp/pyneople-0.3.4.tar.gz` & `tmp/pyneople-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.3.4.tar", last modified: Wed May  8 08:25:35 2024, max compression
+gzip compressed data, was "pyneople-0.3.5.tar", last modified: Wed May  8 08:54:44 2024, max compression
```

## Comparing `pyneople-0.3.4.tar` & `pyneople-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:25:35.142019 pyneople-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 08:25:20.000000 pyneople-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:25:35.142019 pyneople-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 08:25:20.000000 pyneople-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 08:25:20.000000 pyneople-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:25:35.142019 pyneople-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 08:25:20.000000 pyneople-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:25:35.138019 pyneople-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:25:35.138019 pyneople-0.3.4/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 08:25:20.000000 pyneople-0.3.4/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 08:25:20.000000 pyneople-0.3.4/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37543 2024-05-08 08:25:20.000000 pyneople-0.3.4/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-08 08:25:20.000000 pyneople-0.3.4/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-08 08:25:20.000000 pyneople-0.3.4/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:25:35.138019 pyneople-0.3.4/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:25:35.000000 pyneople-0.3.4/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:25:35.000000 pyneople-0.3.4/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:25:35.000000 pyneople-0.3.4/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 08:25:35.000000 pyneople-0.3.4/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:54:44.907388 pyneople-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 08:54:28.000000 pyneople-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:54:44.907388 pyneople-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 08:54:28.000000 pyneople-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 08:54:28.000000 pyneople-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:54:44.907388 pyneople-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 08:54:28.000000 pyneople-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:54:44.907388 pyneople-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:54:44.907388 pyneople-0.3.5/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 08:54:28.000000 pyneople-0.3.5/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 08:54:28.000000 pyneople-0.3.5/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37543 2024-05-08 08:54:28.000000 pyneople-0.3.5/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-08 08:54:28.000000 pyneople-0.3.5/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-08 08:54:28.000000 pyneople-0.3.5/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:54:44.907388 pyneople-0.3.5/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:54:44.000000 pyneople-0.3.5/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:54:44.000000 pyneople-0.3.5/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:54:44.000000 pyneople-0.3.5/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 08:54:44.000000 pyneople-0.3.5/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.3.4/LICENSE` & `pyneople-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.4/PKG-INFO` & `pyneople-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.4
+Version: 0.3.5
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.3.4/setup.py` & `pyneople-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.3.4",
+    version="0.3.5",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.3.4/src/pyneople/METADATA.py` & `pyneople-0.3.5/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.4/src/pyneople/character.py` & `pyneople-0.3.5/src/pyneople/character.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.4/src/pyneople/database_connecter.py` & `pyneople-0.3.5/src/pyneople/database_connecter.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.4/src/pyneople/functions.py` & `pyneople-0.3.5/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.4/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.3.5/src/pyneople.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.4
+Version: 0.3.5
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

