# Comparing `tmp/pyvault20-0.1.2.tar.gz` & `tmp/pyvault20-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvault20-0.1.2.tar", last modified: Wed May  8 15:10:17 2024, max compression
+gzip compressed data, was "pyvault20-0.1.3.tar", last modified: Wed May  8 15:15:50 2024, max compression
```

## Comparing `pyvault20-0.1.2.tar` & `pyvault20-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 15:10:17.572345 pyvault20-0.1.2/
--rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      328 2024-05-08 15:10:17.570345 pyvault20-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 15:10:17.551187 pyvault20-0.1.2/pyvault/
--rw-rw-rw-   0        0        0       60 2024-05-08 14:43:18.000000 pyvault20-0.1.2/pyvault/__init__.py
--rw-rw-rw-   0        0        0      128 2024-05-08 15:08:43.000000 pyvault20-0.1.2/pyvault/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:10:17.569346 pyvault20-0.1.2/pyvault20.egg-info/
--rw-rw-rw-   0        0        0      328 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 15:10:17.000000 pyvault20-0.1.2/pyvault20.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 15:10:17.573344 pyvault20-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-05-08 15:09:48.000000 pyvault20-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:15:50.240548 pyvault20-0.1.3/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:15:50.237549 pyvault20-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:15:50.216475 pyvault20-0.1.3/pyvault/
+-rw-rw-rw-   0        0        0       60 2024-05-08 14:43:18.000000 pyvault20-0.1.3/pyvault/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-05-08 15:14:04.000000 pyvault20-0.1.3/pyvault/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:15:50.236550 pyvault20-0.1.3/pyvault20.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 15:15:50.000000 pyvault20-0.1.3/pyvault20.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:15:50.240548 pyvault20-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      666 2024-05-08 15:15:35.000000 pyvault20-0.1.3/setup.py
```

### Comparing `pyvault20-0.1.2/LICENSE` & `pyvault20-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvault20-0.1.2/setup.py` & `pyvault20-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pyvault20",
-    version="0.1.2",
+    version="0.1.3",
     description="Vault encryption tool.",
     url="https://github.com/thecodeforge/pyvault",
     py_modules=["pyvault"],
     install_requires=[
         "requests",
         "pychacha"
         ],
```

