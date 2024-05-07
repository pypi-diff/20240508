# Comparing `tmp/ternviz-0.6.2.tar.gz` & `tmp/ternviz-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ternviz-0.6.2.tar", last modified: Tue Mar 19 09:30:01 2024, max compression
+gzip compressed data, was "ternviz-0.6.3.tar", last modified: Tue May  7 23:36:51 2024, max compression
```

## Comparing `ternviz-0.6.2.tar` & `ternviz-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:30:01.908575 ternviz-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-19 09:29:32.000000 ternviz-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-19 09:30:01.908575 ternviz-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-19 09:29:32.000000 ternviz-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 09:30:01.908575 ternviz-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-19 09:29:32.000000 ternviz-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:30:01.908575 ternviz-0.6.2/ternviz/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:30:01.908575 ternviz-0.6.2/ternviz/vmd/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/vmd/render-lq.vmd
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/vmd/render-pdb.vmd
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/vmd/render-points.vmd
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-19 09:29:32.000000 ternviz-0.6.2/ternviz/vmd/render.vmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:30:01.908575 ternviz-0.6.2/ternviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 09:30:01.000000 ternviz-0.6.2/ternviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:29:37.000000 ternviz-0.6.2/ternviz.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:30:01.908575 ternviz-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-19 09:29:32.000000 ternviz-0.6.2/tests/test_ternviz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:36:51.831826 ternviz-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 23:36:26.000000 ternviz-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 23:36:51.831826 ternviz-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-07 23:36:26.000000 ternviz-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:36:51.831826 ternviz-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-07 23:36:26.000000 ternviz-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:36:51.827826 ternviz-0.6.3/ternviz/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:36:51.831826 ternviz-0.6.3/ternviz/vmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/vmd/render-lq.vmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/vmd/render-pdb.vmd
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/vmd/render-points.vmd
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-07 23:36:26.000000 ternviz-0.6.3/ternviz/vmd/render.vmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:36:51.831826 ternviz-0.6.3/ternviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 23:36:51.000000 ternviz-0.6.3/ternviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:36:32.000000 ternviz-0.6.3/ternviz.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:36:51.831826 ternviz-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 23:36:26.000000 ternviz-0.6.3/tests/test_ternviz.py
```

### Comparing `ternviz-0.6.2/LICENSE` & `ternviz-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/PKG-INFO` & `ternviz-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ternviz
-Version: 0.6.2
+Version: 0.6.3
 Summary: Render SMILES into 3D video
 Home-page: https://github.com/whitead/ternviz
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ternviz-0.6.2/README.md` & `ternviz-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/setup.py` & `ternviz-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz/bot.py` & `ternviz-0.6.3/ternviz/bot.py`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz/lib.py` & `ternviz-0.6.3/ternviz/lib.py`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz/main.py` & `ternviz-0.6.3/ternviz/main.py`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz/vmd/render-lq.vmd` & `ternviz-0.6.3/ternviz/vmd/render-lq.vmd`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz/vmd/render-points.vmd` & `ternviz-0.6.3/ternviz/vmd/render-points.vmd`

 * *Files identical despite different names*

### Comparing `ternviz-0.6.2/ternviz.egg-info/PKG-INFO` & `ternviz-0.6.3/ternviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ternviz
-Version: 0.6.2
+Version: 0.6.3
 Summary: Render SMILES into 3D video
 Home-page: https://github.com/whitead/ternviz
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

