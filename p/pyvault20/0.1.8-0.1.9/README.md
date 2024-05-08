# Comparing `tmp/pyvault20-0.1.8.tar.gz` & `tmp/pyvault20-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvault20-0.1.8.tar", last modified: Wed May  8 16:27:39 2024, max compression
+gzip compressed data, was "pyvault20-0.1.9.tar", last modified: Wed May  8 17:01:30 2024, max compression
```

## Comparing `pyvault20-0.1.8.tar` & `pyvault20-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 16:27:39.244181 pyvault20-0.1.8/
--rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      328 2024-05-08 16:27:39.242186 pyvault20-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 16:27:39.180486 pyvault20-0.1.8/pyvault/
--rw-rw-rw-   0        0        0       30 2024-05-08 15:25:58.000000 pyvault20-0.1.8/pyvault/__init__.py
--rw-rw-rw-   0        0        0      688 2024-05-08 16:27:14.000000 pyvault20-0.1.8/pyvault/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:27:39.240165 pyvault20-0.1.8/pyvault20.egg-info/
--rw-rw-rw-   0        0        0      328 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 16:27:39.000000 pyvault20-0.1.8/pyvault20.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 16:27:39.244181 pyvault20-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-05-08 16:27:26.000000 pyvault20-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:01:30.693287 pyvault20-0.1.9/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      328 2024-05-08 17:01:30.690273 pyvault20-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 17:01:30.669833 pyvault20-0.1.9/pyvault/
+-rw-rw-rw-   0        0        0       30 2024-05-08 15:25:58.000000 pyvault20-0.1.9/pyvault/__init__.py
+-rw-rw-rw-   0        0        0     2387 2024-05-08 17:00:50.000000 pyvault20-0.1.9/pyvault/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:01:30.688288 pyvault20-0.1.9/pyvault20.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 17:01:30.000000 pyvault20-0.1.9/pyvault20.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 17:01:30.693287 pyvault20-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      666 2024-05-08 17:01:18.000000 pyvault20-0.1.9/setup.py
```

### Comparing `pyvault20-0.1.8/LICENSE` & `pyvault20-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvault20-0.1.8/setup.py` & `pyvault20-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pyvault20",
-    version="0.1.8",
+    version="0.1.9",
     description="Vault encryption tool.",
     url="https://github.com/thecodeforge/pyvault",
     py_modules=["pyvault"],
     install_requires=[
         "requests",
         "pychacha"
         ],
```

