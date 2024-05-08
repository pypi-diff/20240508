# Comparing `tmp/toga_textual-0.4.3.tar.gz` & `tmp/toga_textual-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_textual-0.4.3.tar", last modified: Mon May  6 06:43:37 2024, max compression
+gzip compressed data, was "toga_textual-0.4.4.tar", last modified: Wed May  8 00:58:55 2024, max compression
```

## Comparing `toga_textual-0.4.3.tar` & `toga_textual-0.4.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:05.000000 toga_textual-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-06 06:43:37.640369 toga_textual-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-06 06:43:05.000000 toga_textual-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-06 06:43:05.000000 toga_textual-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:37.640369 toga_textual-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.636369 toga_textual-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.636369 toga_textual-0.4.3/src/toga_textual/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/src/toga_textual/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/src/toga_textual/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-06 06:43:05.000000 toga_textual-0.4.3/src/toga_textual/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/src/toga_textual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 06:43:37.000000 toga_textual-0.4.3/src/toga_textual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/tests_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/images.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:37.640369 toga_textual-0.4.3/tests_backend/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:05.000000 toga_textual-0.4.3/tests_backend/widgets/button.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.570342 toga_textual-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:25.000000 toga_textual-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-08 00:58:55.570342 toga_textual-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-08 00:58:25.000000 toga_textual-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-08 00:58:25.000000 toga_textual-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:55.570342 toga_textual-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.562342 toga_textual-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.566342 toga_textual-0.4.4/src/toga_textual/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.566342 toga_textual-0.4.4/src/toga_textual/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.566342 toga_textual-0.4.4/src/toga_textual/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-08 00:58:25.000000 toga_textual-0.4.4/src/toga_textual/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.570342 toga_textual-0.4.4/src/toga_textual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 00:58:55.000000 toga_textual-0.4.4/src/toga_textual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.566342 toga_textual-0.4.4/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.570342 toga_textual-0.4.4/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:25.000000 toga_textual-0.4.4/tests_backend/widgets/button.py
```

### Comparing `toga_textual-0.4.3/PKG-INFO` & `toga_textual-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-textual
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Textual backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: textual>=0.44.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-textual
 ============
 
 A Textual backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_textual-0.4.3/README.rst` & `toga_textual-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/pyproject.toml` & `toga_textual-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/app.py` & `toga_textual-0.4.4/src/toga_textual/app.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/container.py` & `toga_textual-0.4.4/src/toga_textual/container.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/dialogs.py` & `toga_textual-0.4.4/src/toga_textual/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/factory.py` & `toga_textual-0.4.4/src/toga_textual/factory.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/paths.py` & `toga_textual-0.4.4/src/toga_textual/paths.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/resources/toga.png` & `toga_textual-0.4.4/src/toga_textual/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/screens.py` & `toga_textual-0.4.4/src/toga_textual/screens.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/widgets/base.py` & `toga_textual-0.4.4/src/toga_textual/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/widgets/box.py` & `toga_textual-0.4.4/src/toga_textual/widgets/box.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/widgets/button.py` & `toga_textual-0.4.4/src/toga_textual/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/widgets/textinput.py` & `toga_textual-0.4.4/src/toga_textual/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual/window.py` & `toga_textual-0.4.4/src/toga_textual/window.py`

 * *Files identical despite different names*

### Comparing `toga_textual-0.4.3/src/toga_textual.egg-info/PKG-INFO` & `toga_textual-0.4.4/src/toga_textual.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-textual
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Textual backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: textual>=0.44.0
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-textual
 ============
 
 A Textual backend for the `Toga widget toolkit`_.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_textual-0.4.3/src/toga_textual.egg-info/SOURCES.txt` & `toga_textual-0.4.4/src/toga_textual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

