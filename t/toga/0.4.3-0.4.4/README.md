# Comparing `tmp/toga-0.4.3.tar.gz` & `tmp/toga-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-0.4.3.tar", last modified: Mon May  6 06:43:33 2024, max compression
+gzip compressed data, was "toga-0.4.4.tar", last modified: Wed May  8 00:59:02 2024, max compression
```

## Comparing `toga-0.4.3.tar` & `toga-0.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.304445 toga-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:03.000000 toga-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:03.000000 toga-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 06:43:33.304445 toga-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 06:43:03.000000 toga-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-06 06:43:03.000000 toga-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:33.304445 toga-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.304445 toga-0.4.3/toga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:02.101843 toga-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:29.000000 toga-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:58:29.000000 toga-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-08 00:59:02.101843 toga-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-08 00:58:29.000000 toga-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-08 00:58:29.000000 toga-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:59:02.101843 toga-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:59:02.101843 toga-0.4.4/toga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-08 00:59:01.000000 toga-0.4.4/toga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 00:59:02.000000 toga-0.4.4/toga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:59:01.000000 toga-0.4.4/toga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 00:59:01.000000 toga-0.4.4/toga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:59:01.000000 toga-0.4.4/toga.egg-info/top_level.txt
```

### Comparing `toga-0.4.3/LICENSE` & `toga-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-0.4.3/PKG-INFO` & `toga-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,21 +26,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-winforms==0.4.3; sys_platform == "win32"
-Requires-Dist: toga-gtk==0.4.3; sys_platform == "linux"
-Requires-Dist: toga-gtk==0.4.3; "freebsd" in sys_platform
-Requires-Dist: toga-cocoa==0.4.3; sys_platform == "darwin"
-Requires-Dist: toga-iOS==0.4.3; sys_platform == "ios"
-Requires-Dist: toga-android==0.4.3; sys_platform == "android"
-Requires-Dist: toga-web==0.4.3; sys_platform == "emscripten"
+Requires-Dist: toga-winforms==0.4.4; sys_platform == "win32"
+Requires-Dist: toga-gtk==0.4.4; sys_platform == "linux"
+Requires-Dist: toga-gtk==0.4.4; "freebsd" in sys_platform
+Requires-Dist: toga-cocoa==0.4.4; sys_platform == "darwin"
+Requires-Dist: toga-iOS==0.4.4; sys_platform == "ios"
+Requires-Dist: toga-android==0.4.4; sys_platform == "android"
+Requires-Dist: toga-web==0.4.4; sys_platform == "emscripten"
 
 toga
 ====
 
 A meta-package for installing the `Toga widget toolkit`_.
 
 This package installs the `toga-core <https://pypi.org/project/toga-core>`__ library,
```

### Comparing `toga-0.4.3/README.rst` & `toga-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga-0.4.3/pyproject.toml` & `toga-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga-0.4.3/toga.egg-info/PKG-INFO` & `toga-0.4.4/toga.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,21 +26,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-winforms==0.4.3; sys_platform == "win32"
-Requires-Dist: toga-gtk==0.4.3; sys_platform == "linux"
-Requires-Dist: toga-gtk==0.4.3; "freebsd" in sys_platform
-Requires-Dist: toga-cocoa==0.4.3; sys_platform == "darwin"
-Requires-Dist: toga-iOS==0.4.3; sys_platform == "ios"
-Requires-Dist: toga-android==0.4.3; sys_platform == "android"
-Requires-Dist: toga-web==0.4.3; sys_platform == "emscripten"
+Requires-Dist: toga-winforms==0.4.4; sys_platform == "win32"
+Requires-Dist: toga-gtk==0.4.4; sys_platform == "linux"
+Requires-Dist: toga-gtk==0.4.4; "freebsd" in sys_platform
+Requires-Dist: toga-cocoa==0.4.4; sys_platform == "darwin"
+Requires-Dist: toga-iOS==0.4.4; sys_platform == "ios"
+Requires-Dist: toga-android==0.4.4; sys_platform == "android"
+Requires-Dist: toga-web==0.4.4; sys_platform == "emscripten"
 
 toga
 ====
 
 A meta-package for installing the `Toga widget toolkit`_.
 
 This package installs the `toga-core <https://pypi.org/project/toga-core>`__ library,
```

