# Comparing `tmp/infoindia-1.0.1.tar.gz` & `tmp/infoindia-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoindia-1.0.1.tar", last modified: Wed May  8 13:39:45 2024, max compression
+gzip compressed data, was "infoindia-1.1.0.tar", last modified: Wed May  8 13:48:59 2024, max compression
```

## Comparing `infoindia-1.0.1.tar` & `infoindia-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:39:45.638164 infoindia-1.0.1/
--rw-rw-rw-   0        0        0     1359 2024-05-08 13:39:45.638164 infoindia-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      951 2024-05-08 13:33:19.000000 infoindia-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:39:45.638164 infoindia-1.0.1/infoindia.egg-info/
--rw-rw-rw-   0        0        0     1359 2024-05-08 13:39:45.000000 infoindia-1.0.1/infoindia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-05-08 13:39:45.000000 infoindia-1.0.1/infoindia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:39:45.000000 infoindia-1.0.1/infoindia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 13:39:45.000000 infoindia-1.0.1/infoindia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:39:45.000000 infoindia-1.0.1/infoindia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 13:39:45.638164 infoindia-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-05-08 13:39:25.000000 infoindia-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:48:59.328587 infoindia-1.1.0/
+-rw-rw-rw-   0        0        0     1359 2024-05-08 13:48:59.328587 infoindia-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2024-05-08 13:33:19.000000 infoindia-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:48:59.328587 infoindia-1.1.0/infoindia.egg-info/
+-rw-rw-rw-   0        0        0     1359 2024-05-08 13:48:59.000000 infoindia-1.1.0/infoindia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-05-08 13:48:59.000000 infoindia-1.1.0/infoindia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:48:59.000000 infoindia-1.1.0/infoindia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 13:48:59.000000 infoindia-1.1.0/infoindia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:48:59.000000 infoindia-1.1.0/infoindia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:48:59.328587 infoindia-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-08 13:48:42.000000 infoindia-1.1.0/setup.py
```

### Comparing `infoindia-1.0.1/PKG-INFO` & `infoindia-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoindia
-Version: 1.0.1
+Version: 1.1.0
 Summary: Wrapper for State Data APIs
 Home-page: https://github.com/NarutoUzumvki/state_data_api
 Author: Vijay Chouhan
 Author-email: vijay977364@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `infoindia-1.0.1/README.md` & `infoindia-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `infoindia-1.0.1/infoindia.egg-info/PKG-INFO` & `infoindia-1.1.0/infoindia.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoindia
-Version: 1.0.1
+Version: 1.1.0
 Summary: Wrapper for State Data APIs
 Home-page: https://github.com/NarutoUzumvki/state_data_api
 Author: Vijay Chouhan
 Author-email: vijay977364@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `infoindia-1.0.1/setup.py` & `infoindia-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='infoindia',
-    version='1.0.1',
+    version='1.1.0',
     packages=find_packages(),
     install_requires=['requests'],
     author='Vijay Chouhan',
     author_email='vijay977364@gmail.com',
     description='Wrapper for State Data APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

