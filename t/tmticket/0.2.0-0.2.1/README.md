# Comparing `tmp/tmticket-0.2.0.tar.gz` & `tmp/tmticket-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.0.tar", last modified: Tue May  7 23:52:13 2024, max compression
+gzip compressed data, was "tmticket-0.2.1.tar", last modified: Tue May  7 23:57:31 2024, max compression
```

## Comparing `tmticket-0.2.0.tar` & `tmticket-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.253806 tmticket-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:52:13.252806 tmticket-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 23:52:13.253806 tmticket-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 23:51:23.000000 tmticket-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.250806 tmticket-0.2.0/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.252806 tmticket-0.2.0/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 23:52:13.000000 tmticket-0.2.0/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.558385 tmticket-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:57:31.558385 tmticket-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 23:57:31.558385 tmticket-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 23:57:07.000000 tmticket-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.555385 tmticket-0.2.1/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.557385 tmticket-0.2.1/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 23:57:31.000000 tmticket-0.2.1/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.0/LICENSE` & `tmticket-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.0/PKG-INFO` & `tmticket-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tmticket-0.2.0/setup.py` & `tmticket-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.0',
+    version='0.2.1',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
     #long_description=read('README.rst'), 
     license='MIT',
     keywords='Ticketmaster API',
     url='https://github.com/hokiebrian/pytmtickets',
```

### Comparing `tmticket-0.2.0/tmticket/client.py` & `tmticket-0.2.1/tmticket/client.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.0/tmticket/model.py` & `tmticket-0.2.1/tmticket/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.0/tmticket/query.py` & `tmticket-0.2.1/tmticket/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.0/tmticket.egg-info/PKG-INFO` & `tmticket-0.2.1/tmticket.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```

