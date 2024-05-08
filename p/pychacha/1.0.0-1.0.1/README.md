# Comparing `tmp/pychacha-1.0.0.tar.gz` & `tmp/pychacha-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychacha-1.0.0.tar", last modified: Wed May  8 14:20:11 2024, max compression
+gzip compressed data, was "pychacha-1.0.1.tar", last modified: Wed May  8 16:03:31 2024, max compression
```

## Comparing `pychacha-1.0.0.tar` & `pychacha-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:20:11.330845 pychacha-1.0.0/
--rw-rw-rw-   0        0        0    17098 2024-05-08 13:14:07.000000 pychacha-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      482 2024-05-08 14:20:11.327843 pychacha-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-08 13:57:08.000000 pychacha-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 14:20:11.252432 pychacha-1.0.0/pychacha/
--rw-rw-rw-   0        0        0      117 2024-05-08 13:14:07.000000 pychacha-1.0.0/pychacha/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:20:11.303853 pychacha-1.0.0/pychacha/classes/
--rw-rw-rw-   0        0        0       85 2024-05-08 13:14:07.000000 pychacha-1.0.0/pychacha/classes/__init__.py
--rw-rw-rw-   0        0        0    12232 2024-05-08 13:54:10.000000 pychacha-1.0.0/pychacha/classes/chacha.py
--rw-rw-rw-   0        0        0     4458 2024-05-08 13:14:07.000000 pychacha-1.0.0/pychacha/classes/rsachacha.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:20:11.306851 pychacha-1.0.0/pychacha.egg-info/
--rw-rw-rw-   0        0        0      482 2024-05-08 14:20:11.000000 pychacha-1.0.0/pychacha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-05-08 14:20:11.000000 pychacha-1.0.0/pychacha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:20:11.000000 pychacha-1.0.0/pychacha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 14:20:11.000000 pychacha-1.0.0/pychacha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 14:20:11.330845 pychacha-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      535 2024-05-08 13:57:18.000000 pychacha-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.881389 pychacha-1.0.1/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 13:14:07.000000 pychacha-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      482 2024-05-08 16:03:31.877390 pychacha-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-08 13:57:08.000000 pychacha-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.741436 pychacha-1.0.1/pychacha/
+-rw-rw-rw-   0        0        0      118 2024-05-08 16:01:09.000000 pychacha-1.0.1/pychacha/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.861395 pychacha-1.0.1/pychacha/classes/
+-rw-rw-rw-   0        0        0       85 2024-05-08 13:14:07.000000 pychacha-1.0.1/pychacha/classes/__init__.py
+-rw-rw-rw-   0        0        0    12232 2024-05-08 13:54:10.000000 pychacha-1.0.1/pychacha/classes/chacha.py
+-rw-rw-rw-   0        0        0     4458 2024-05-08 13:14:07.000000 pychacha-1.0.1/pychacha/classes/rsachacha.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.875391 pychacha-1.0.1/pychacha.egg-info/
+-rw-rw-rw-   0        0        0      482 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 16:03:31.881389 pychacha-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      535 2024-05-08 16:02:54.000000 pychacha-1.0.1/setup.py
```

### Comparing `pychacha-1.0.0/LICENSE` & `pychacha-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychacha-1.0.0/pychacha/classes/chacha.py` & `pychacha-1.0.1/pychacha/classes/chacha.py`

 * *Files identical despite different names*

### Comparing `pychacha-1.0.0/pychacha/classes/rsachacha.py` & `pychacha-1.0.1/pychacha/classes/rsachacha.py`

 * *Files identical despite different names*

### Comparing `pychacha-1.0.0/setup.py` & `pychacha-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pychacha",
-    version="1.0.0",
+    version="1.0.1",
     description="ChaCha20 encryption tools for Python.",
     url="https://github.com/thecodeforge/pychacha",
     py_modules=["pychacha"],
     install_requires=[],
     packages=setuptools.find_packages(),
     package_dir={
         "pychacha":"pychacha"
```

