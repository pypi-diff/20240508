# Comparing `tmp/pyvault20-0.1.0.tar.gz` & `tmp/pyvault20-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvault20-0.1.0.tar", last modified: Wed May  8 14:58:53 2024, max compression
+gzip compressed data, was "pyvault20-0.1.1.tar", last modified: Wed May  8 15:07:07 2024, max compression
```

## Comparing `pyvault20-0.1.0.tar` & `pyvault20-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:58:53.506886 pyvault20-0.1.0/
--rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      328 2024-05-08 14:58:53.504905 pyvault20-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 14:58:53.480365 pyvault20-0.1.0/pyvault/
--rw-rw-rw-   0        0        0       60 2024-05-08 14:43:18.000000 pyvault20-0.1.0/pyvault/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 14:44:37.000000 pyvault20-0.1.0/pyvault/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:58:53.502887 pyvault20-0.1.0/pyvault20.egg-info/
--rw-rw-rw-   0        0        0      328 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 14:58:53.000000 pyvault20-0.1.0/pyvault20.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 14:58:53.506886 pyvault20-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      664 2024-05-08 14:58:21.000000 pyvault20-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:07:07.415466 pyvault20-0.1.1/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 14:00:56.000000 pyvault20-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:07:07.413467 pyvault20-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2024-05-08 14:00:56.000000 pyvault20-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:07:07.391474 pyvault20-0.1.1/pyvault/
+-rw-rw-rw-   0        0        0       60 2024-05-08 14:43:18.000000 pyvault20-0.1.1/pyvault/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 14:44:37.000000 pyvault20-0.1.1/pyvault/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:07:07.411468 pyvault20-0.1.1/pyvault20.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 15:07:07.000000 pyvault20-0.1.1/pyvault20.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:07:07.415466 pyvault20-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-05-08 15:06:42.000000 pyvault20-0.1.1/setup.py
```

### Comparing `pyvault20-0.1.0/LICENSE` & `pyvault20-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvault20-0.1.0/setup.py` & `pyvault20-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pyvault20",
-    version="0.1.0",
+    version="0.1.1",
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
-        "console_scripts": ["pyvault=pyvault.command_line.main"]
+        "console_scripts": ["pyvault=pyvault.pyvault.command_line.main"]
     }
 )
```

