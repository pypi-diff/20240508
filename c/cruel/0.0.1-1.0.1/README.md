# Comparing `tmp/cruel-0.0.1.tar.gz` & `tmp/cruel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruel-0.0.1.tar", last modified: Wed May  8 13:01:06 2024, max compression
+gzip compressed data, was "cruel-1.0.1.tar", last modified: Wed May  8 12:59:19 2024, max compression
```

## Comparing `cruel-0.0.1.tar` & `cruel-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:01:06.690862 cruel-0.0.1/
--rw-r--r--   0 codie     (1000) codie     (1000)    35148 2024-04-09 16:46:37.000000 cruel-0.0.1/LICENCE
--rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 13:01:06.690862 cruel-0.0.1/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)     1468 2024-05-08 12:59:00.000000 cruel-0.0.1/README.md
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:01:06.689862 cruel-0.0.1/cruel/
--rw-r--r--   0 codie     (1000) codie     (1000)       31 2024-05-08 12:42:21.000000 cruel-0.0.1/cruel/__init__.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:01:06.689862 cruel-0.0.1/cruel/utils/
--rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-04-09 16:46:37.000000 cruel-0.0.1/cruel/utils/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1801 2024-05-08 12:45:33.000000 cruel-0.0.1/cruel/utils/req.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:01:06.690862 cruel-0.0.1/cruel.egg-info/
--rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 13:01:06.000000 cruel-0.0.1/cruel.egg-info/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)      231 2024-05-08 13:01:06.000000 cruel-0.0.1/cruel.egg-info/SOURCES.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-05-08 13:01:06.000000 cruel-0.0.1/cruel.egg-info/dependency_links.txt
--rw-r--r--   0 codie     (1000) codie     (1000)      173 2024-05-08 13:01:06.000000 cruel-0.0.1/cruel.egg-info/requires.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-05-08 13:01:06.000000 cruel-0.0.1/cruel.egg-info/top_level.txt
--rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-05-08 13:01:06.690862 cruel-0.0.1/setup.cfg
--rw-r--r--   0 codie     (1000) codie     (1000)     1163 2024-05-08 13:00:01.000000 cruel-0.0.1/setup.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.094668 cruel-1.0.1/
+-rw-r--r--   0 codie     (1000) codie     (1000)    35148 2024-04-09 16:46:37.000000 cruel-1.0.1/LICENCE
+-rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 12:59:19.094668 cruel-1.0.1/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)     1468 2024-05-08 12:59:00.000000 cruel-1.0.1/README.md
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel/
+-rw-r--r--   0 codie     (1000) codie     (1000)       31 2024-05-08 12:42:21.000000 cruel-1.0.1/cruel/__init__.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel/utils/
+-rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-04-09 16:46:37.000000 cruel-1.0.1/cruel/utils/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1801 2024-05-08 12:45:33.000000 cruel-1.0.1/cruel/utils/req.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel.egg-info/
+-rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)      231 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/SOURCES.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/dependency_links.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)      173 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/requires.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/top_level.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-05-08 12:59:19.094668 cruel-1.0.1/setup.cfg
+-rw-r--r--   0 codie     (1000) codie     (1000)     1164 2024-05-08 12:59:00.000000 cruel-1.0.1/setup.py
```

### Comparing `cruel-0.0.1/LICENCE` & `cruel-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cruel-0.0.1/PKG-INFO` & `cruel-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruel
-Version: 0.0.1
+Version: 1.0.1
 Summary: Cruel - Scrape everything or anything from the web.
 Home-page: https://github.com/Bishwas-py/cruel
 Author: Bishwas Bhandari
 Author-email: yo@bishwas.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cruel-0.0.1/README.md` & `cruel-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cruel-0.0.1/cruel/utils/req.py` & `cruel-1.0.1/cruel/utils/req.py`

 * *Files identical despite different names*

### Comparing `cruel-0.0.1/cruel.egg-info/PKG-INFO` & `cruel-1.0.1/cruel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruel
-Version: 0.0.1
+Version: 1.0.1
 Summary: Cruel - Scrape everything or anything from the web.
 Home-page: https://github.com/Bishwas-py/cruel
 Author: Bishwas Bhandari
 Author-email: yo@bishwas.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cruel-0.0.1/setup.py` & `cruel-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cruel",
-    version="0.0.1",
+    version="1.0.01",
     description="Cruel - Scrape everything or anything from the web.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bishwas-py/cruel",
     author="Bishwas Bhandari",
     author_email="yo@bishwas.net",
     py_modules=["cruel"],
```

