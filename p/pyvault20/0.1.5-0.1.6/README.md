# Comparing `tmp/pyvault20-0.1.5.tar.gz` & `tmp/pyvault20-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvault20-0.1.5.tar", last modified: Wed May  8 15:22:06 2024, max compression
+gzip compressed data, was "pyvault20-0.1.6.tar", last modified: Wed May  8 15:26:46 2024, max compression
```

## Comparing `pyvault20-0.1.5.tar` & `pyvault20-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 15:22:06.451640 pyvault20-0.1.5/
--rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      328 2024-05-08 15:22:06.449642 pyvault20-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 15:22:06.429793 pyvault20-0.1.5/pyvault/
--rw-rw-rw-   0        0        0       27 2024-05-08 15:20:57.000000 pyvault20-0.1.5/pyvault/__init__.py
--rw-rw-rw-   0        0        0       53 2024-05-08 15:14:04.000000 pyvault20-0.1.5/pyvault/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-08 15:22:06.447652 pyvault20-0.1.5/pyvault20.egg-info/
--rw-rw-rw-   0        0        0      328 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 15:22:06.000000 pyvault20-0.1.5/pyvault20.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 15:22:06.451640 pyvault20-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-05-08 15:21:30.000000 pyvault20-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:26:46.768393 pyvault20-0.1.6/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:26:46.766393 pyvault20-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:26:46.747417 pyvault20-0.1.6/pyvault/
+-rw-rw-rw-   0        0        0       30 2024-05-08 15:25:58.000000 pyvault20-0.1.6/pyvault/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-05-08 15:14:04.000000 pyvault20-0.1.6/pyvault/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:26:46.764407 pyvault20-0.1.6/pyvault20.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 15:26:46.000000 pyvault20-0.1.6/pyvault20.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:26:46.768393 pyvault20-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-05-08 15:26:30.000000 pyvault20-0.1.6/setup.py
```

### Comparing `pyvault20-0.1.5/LICENSE` & `pyvault20-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvault20-0.1.5/setup.py` & `pyvault20-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pyvault20",
-    version="0.1.5",
+    version="0.1.6",
     description="Vault encryption tool.",
     url="https://github.com/thecodeforge/pyvault",
     py_modules=["pyvault"],
     install_requires=[
         "requests",
         "pychacha"
         ],
@@ -17,10 +17,10 @@
     package_dir={
         "pyvault":"pyvault"
     },
     python_requires= '>=3.11',
     long_description = readme,
     long_description_content_type = "text/markdown",
     entry_points = {
-        "console_scripts": ["pyvault = pyvault.command_line.main"]
+        "console_scripts": ["pyvault = pyvault.main"]
     }
 )
```

