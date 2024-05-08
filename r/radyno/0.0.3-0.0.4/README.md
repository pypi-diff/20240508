# Comparing `tmp/radyno-0.0.3.tar.gz` & `tmp/radyno-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radyno-0.0.3.tar", last modified: Tue May  7 15:01:26 2024, max compression
+gzip compressed data, was "radyno-0.0.4.tar", last modified: Tue May  7 15:05:52 2024, max compression
```

## Comparing `radyno-0.0.3.tar` & `radyno-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 15:01:26.566681 radyno-0.0.3/
--rw-rw-rw-   0        0        0      537 2024-05-07 15:01:26.566681 radyno-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-03-24 21:47:43.000000 radyno-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 15:01:26.566681 radyno-0.0.3/radyno.egg-info/
--rw-rw-rw-   0        0        0      537 2024-05-07 15:01:26.000000 radyno-0.0.3/radyno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-05-07 15:01:26.000000 radyno-0.0.3/radyno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 15:01:26.000000 radyno-0.0.3/radyno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 15:01:26.000000 radyno-0.0.3/radyno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 15:01:26.566681 radyno-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1097 2024-05-07 15:00:40.000000 radyno-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:05:52.369499 radyno-0.0.4/
+-rw-rw-rw-   0        0        0      537 2024-05-07 15:05:52.368994 radyno-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-03-24 21:47:43.000000 radyno-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 15:05:52.367989 radyno-0.0.4/radyno.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-07 15:05:52.000000 radyno-0.0.4/radyno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-05-07 15:05:52.000000 radyno-0.0.4/radyno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:05:52.000000 radyno-0.0.4/radyno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:05:52.000000 radyno-0.0.4/radyno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:05:52.369499 radyno-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1097 2024-05-07 15:05:28.000000 radyno-0.0.4/setup.py
```

### Comparing `radyno-0.0.3/PKG-INFO` & `radyno-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radyno
-Version: 0.0.3
+Version: 0.0.4
 Summary: Particles tracking and radiation spectrum evaluation
 Author: exborgg (Andrea Frazzitta)
 Author-email: <andrea.frazzitta@uniroma1.it>
 Keywords: python,beam,radiation,spectrum,mpi,parallel
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `radyno-0.0.3/radyno.egg-info/PKG-INFO` & `radyno-0.0.4/radyno.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radyno
-Version: 0.0.3
+Version: 0.0.4
 Summary: Particles tracking and radiation spectrum evaluation
 Author: exborgg (Andrea Frazzitta)
 Author-email: <andrea.frazzitta@uniroma1.it>
 Keywords: python,beam,radiation,spectrum,mpi,parallel
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `radyno-0.0.3/setup.py` & `radyno-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Particles tracking and radiation spectrum evaluation'
 
 # Setting up
 setup(
     name="radyno",
     version=VERSION,
     author="exborgg (Andrea Frazzitta)",
```

