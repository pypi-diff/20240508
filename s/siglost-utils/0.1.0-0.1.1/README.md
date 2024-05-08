# Comparing `tmp/siglost_utils-0.1.0.tar.gz` & `tmp/siglost_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.1.0.tar", last modified: Wed May  8 00:48:25 2024, max compression
+gzip compressed data, was "siglost_utils-0.1.1.tar", last modified: Wed May  8 00:58:13 2024, max compression
```

## Comparing `siglost_utils-0.1.0.tar` & `siglost_utils-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/siglost_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/siglost_utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 00:48:25.000000 siglost_utils-0.1.0/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 00:48:25.000000 siglost_utils-0.1.0/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:48:25.000000 siglost_utils-0.1.0/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 00:48:25.000000 siglost_utils-0.1.0/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:48:25.754786 siglost_utils-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 00:48:17.000000 siglost_utils-0.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/siglost_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/siglost_utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 00:58:13.000000 siglost_utils-0.1.1/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 00:58:13.000000 siglost_utils-0.1.1/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:13.000000 siglost_utils-0.1.1/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 00:58:13.000000 siglost_utils-0.1.1/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:13.043835 siglost_utils-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 00:58:03.000000 siglost_utils-0.1.1/tests/test_util.py
```

### Comparing `siglost_utils-0.1.0/LICENSE` & `siglost_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.0/PKG-INFO` & `siglost_utils-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.0/setup.cfg` & `siglost_utils-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.0/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.1.1/siglost_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

