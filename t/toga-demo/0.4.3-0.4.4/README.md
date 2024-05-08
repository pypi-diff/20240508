# Comparing `tmp/toga_demo-0.4.3.tar.gz` & `tmp/toga_demo-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_demo-0.4.3.tar", last modified: Mon May  6 06:43:32 2024, max compression
+gzip compressed data, was "toga_demo-0.4.4.tar", last modified: Wed May  8 00:58:11 2024, max compression
```

## Comparing `toga_demo-0.4.3.tar` & `toga_demo-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.411673 toga_demo-0.4.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-06 06:43:01.000000 toga_demo-0.4.3/AUTHORS
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-06 06:43:01.000000 toga_demo-0.4.3/CONTRIBUTING.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1525 2024-05-06 06:43:01.000000 toga_demo-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-06 06:43:32.411673 toga_demo-0.4.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-06 06:43:01.000000 toga_demo-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-06 06:43:01.000000 toga_demo-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:32.411673 toga_demo-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.407673 toga_demo-0.4.3/toga_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2959 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.411673 toga_demo-0.4.3/toga_demo/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2011 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/resources/brutus-32.png
--rw-r--r--   0 runner    (1001) docker     (127)   316755 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/resources/brutus.icns
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/resources/brutus.ico
--rw-r--r--   0 runner    (1001) docker     (127)   316755 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/resources/toga-demo.icns
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-06 06:43:01.000000 toga_demo-0.4.3/toga_demo/resources/toga-demo.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:32.411673 toga_demo-0.4.3/toga_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 06:43:32.000000 toga_demo-0.4.3/toga_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.421625 toga_demo-0.4.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-08 00:57:41.000000 toga_demo-0.4.4/AUTHORS
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-08 00:57:41.000000 toga_demo-0.4.4/CONTRIBUTING.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1525 2024-05-08 00:57:41.000000 toga_demo-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-08 00:58:11.421625 toga_demo-0.4.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-08 00:57:41.000000 toga_demo-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-08 00:57:41.000000 toga_demo-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:11.421625 toga_demo-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.417625 toga_demo-0.4.4/toga_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2959 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.421625 toga_demo-0.4.4/toga_demo/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2011 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/resources/brutus-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)   316755 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/resources/brutus.icns
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/resources/brutus.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   316755 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/resources/toga-demo.icns
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 00:57:41.000000 toga_demo-0.4.4/toga_demo/resources/toga-demo.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:11.421625 toga_demo-0.4.4/toga_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 00:58:11.000000 toga_demo-0.4.4/toga_demo.egg-info/top_level.txt
```

### Comparing `toga_demo-0.4.3/LICENSE` & `toga_demo-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/PKG-INFO` & `toga_demo-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-demo
-Version: 0.4.3
+Version: 0.4.4
 Summary: A demonstration of the capabilities of the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -27,15 +27,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: toga==0.4.3
+Requires-Dist: toga==0.4.4
 
 Toga Demo
 =========
 
 A demonstration of the capabilities of the `Toga widget toolkit`_.
 
 **Toga requires Python 3**
```

### Comparing `toga_demo-0.4.3/README.rst` & `toga_demo-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/pyproject.toml` & `toga_demo-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/app.py` & `toga_demo-0.4.4/toga_demo/app.py`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/resources/brutus-32.png` & `toga_demo-0.4.4/toga_demo/resources/brutus-32.png`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/resources/brutus.icns` & `toga_demo-0.4.4/toga_demo/resources/brutus.icns`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/resources/brutus.ico` & `toga_demo-0.4.4/toga_demo/resources/brutus.ico`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/resources/toga-demo.icns` & `toga_demo-0.4.4/toga_demo/resources/toga-demo.icns`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo/resources/toga-demo.ico` & `toga_demo-0.4.4/toga_demo/resources/toga-demo.ico`

 * *Files identical despite different names*

### Comparing `toga_demo-0.4.3/toga_demo.egg-info/PKG-INFO` & `toga_demo-0.4.4/toga_demo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-demo
-Version: 0.4.3
+Version: 0.4.4
 Summary: A demonstration of the capabilities of the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -27,15 +27,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: toga==0.4.3
+Requires-Dist: toga==0.4.4
 
 Toga Demo
 =========
 
 A demonstration of the capabilities of the `Toga widget toolkit`_.
 
 **Toga requires Python 3**
```

