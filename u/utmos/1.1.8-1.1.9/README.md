# Comparing `tmp/utmos-1.1.8.tar.gz` & `tmp/utmos-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utmos-1.1.8.tar", last modified: Thu Feb 15 22:58:37 2024, max compression
+gzip compressed data, was "utmos-1.1.9.tar", last modified: Wed May  8 00:35:37 2024, max compression
```

## Comparing `utmos-1.1.8.tar` & `utmos-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:58:37.111362 utmos-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-15 22:58:29.000000 utmos-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-15 22:58:37.111362 utmos-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-15 22:58:29.000000 utmos-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 22:58:37.111362 utmos-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-15 22:58:29.000000 utmos-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:58:37.107362 utmos-1.1.8/utmos/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/score.old.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-15 22:58:29.000000 utmos-1.1.8/utmos/score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:58:37.111362 utmos-1.1.8/utmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-15 22:58:37.000000 utmos-1.1.8/utmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:35:37.492025 utmos-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 00:35:33.000000 utmos-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-08 00:35:37.492025 utmos-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-08 00:35:33.000000 utmos-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:35:37.492025 utmos-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-08 00:35:33.000000 utmos-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:35:37.492025 utmos-1.1.9/utmos/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/score.old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 00:35:33.000000 utmos-1.1.9/utmos/score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:35:37.492025 utmos-1.1.9/utmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 00:35:37.000000 utmos-1.1.9/utmos.egg-info/top_level.txt
```

### Comparing `utmos-1.1.8/LICENSE` & `utmos-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/PKG-INFO` & `utmos-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utmos
-Version: 1.1.8
+Version: 1.1.9
 Summary: UT-Sarulab MOS prediction system using SSL models
 Home-page: https://github.com/ttseval/utmos
 Author: mrfakename
 Author-email: me@mrfake.name
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `utmos-1.1.8/README.md` & `utmos-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/setup.py` & `utmos-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='utmos',
-    version='1.1.8',
+    version='1.1.9',
     install_requires=[
         'numpy',
         'fairseq',
         'cached-path',
         'click',
         'torchaudio',
         'pytorch-lightning',
```

### Comparing `utmos-1.1.8/utmos/cli.py` & `utmos-1.1.9/utmos/cli.py`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/utmos/gui.py` & `utmos-1.1.9/utmos/gui.py`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/utmos/model.py` & `utmos-1.1.9/utmos/model.py`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/utmos/score.old.py` & `utmos-1.1.9/utmos/score.old.py`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/utmos/score.py` & `utmos-1.1.9/utmos/score.py`

 * *Files identical despite different names*

### Comparing `utmos-1.1.8/utmos.egg-info/PKG-INFO` & `utmos-1.1.9/utmos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utmos
-Version: 1.1.8
+Version: 1.1.9
 Summary: UT-Sarulab MOS prediction system using SSL models
 Home-page: https://github.com/ttseval/utmos
 Author: mrfakename
 Author-email: me@mrfake.name
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

