# Comparing `tmp/jaxutils-nightly-0.0.8.dev20240506.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240506.tar", last modified: Mon May  6 00:06:43 2024, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240507.tar", last modified: Tue May  7 00:06:29 2024, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20240506.tar` & `jaxutils-nightly-0.0.8.dev20240507.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-06 00:06:43.226571 jaxutils-nightly-0.0.8.dev20240506/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-06 00:06:43.226571 jaxutils-nightly-0.0.8.dev20240506/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-06 00:06:43.234571 jaxutils-nightly-0.0.8.dev20240506/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-05-06 00:06:43.234571 jaxutils-nightly-0.0.8.dev20240506/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-06 00:06:43.226571 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-06 00:06:43.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-05-06 00:06:43.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-06 00:06:43.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-05-06 00:06:43.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-05-06 00:06:43.000000 jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-05-06 00:06:43.234571 jaxutils-nightly-0.0.8.dev20240506/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-05-06 00:06:35.000000 jaxutils-nightly-0.0.8.dev20240506/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 00:06:29.933305 jaxutils-nightly-0.0.8.dev20240507/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-07 00:06:29.933305 jaxutils-nightly-0.0.8.dev20240507/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 00:06:29.937305 jaxutils-nightly-0.0.8.dev20240507/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-05-07 00:06:29.937305 jaxutils-nightly-0.0.8.dev20240507/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-07 00:06:29.933305 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-05-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-05-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-05-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-05-07 00:06:29.937305 jaxutils-nightly-0.0.8.dev20240507/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-05-07 00:06:22.000000 jaxutils-nightly-0.0.8.dev20240507/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20240506/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240506
+Version: 0.0.8.dev20240507
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240506/README.md` & `jaxutils-nightly-0.0.8.dev20240507/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240507/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240506
+Version: 0.0.8.dev20240507
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240506/setup.py` & `jaxutils-nightly-0.0.8.dev20240507/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240506/versioneer.py` & `jaxutils-nightly-0.0.8.dev20240507/versioneer.py`

 * *Files identical despite different names*

