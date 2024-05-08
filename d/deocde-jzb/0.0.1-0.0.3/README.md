# Comparing `tmp/deocde_jzb-0.0.1.tar.gz` & `tmp/deocde_jzb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deocde_jzb-0.0.1.tar", last modified: Wed May  8 04:52:13 2024, max compression
+gzip compressed data, was "deocde_jzb-0.0.3.tar", last modified: Wed May  8 05:38:18 2024, max compression
```

## Comparing `deocde_jzb-0.0.1.tar` & `deocde_jzb-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mk        (1000) mk        (1000)        0 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/
--rw-rw-r--   0 mk        (1000) mk        (1000)     1074 2024-05-08 04:39:38.000000 deocde_jzb-0.0.1/LICENSE
--rw-r--r--   0 mk        (1000) mk        (1000)      662 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/PKG-INFO
--rw-rw-r--   0 mk        (1000) mk        (1000)      132 2024-05-08 04:38:45.000000 deocde_jzb-0.0.1/README.md
--rw-rw-r--   0 mk        (1000) mk        (1000)      512 2024-05-08 04:47:17.000000 deocde_jzb-0.0.1/pyproject.toml
--rw-rw-r--   0 mk        (1000) mk        (1000)       38 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/setup.cfg
-drwxrwxr-x   0 mk        (1000) mk        (1000)        0 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/src/
-drwxrwxr-x   0 mk        (1000) mk        (1000)        0 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/src/deocde_jzb/
--rw-rw-r--   0 mk        (1000) mk        (1000)        2 2024-05-08 04:36:34.000000 deocde_jzb-0.0.1/src/deocde_jzb/__init__.py
--rw-rw-r--   0 mk        (1000) mk        (1000)      470 2024-05-07 07:29:36.000000 deocde_jzb-0.0.1/src/deocde_jzb/decode_jzb.py
-drwxrwxr-x   0 mk        (1000) mk        (1000)        0 2024-05-08 04:52:13.323976 deocde_jzb-0.0.1/src/deocde_jzb.egg-info/
--rw-r--r--   0 mk        (1000) mk        (1000)      662 2024-05-08 04:52:13.000000 deocde_jzb-0.0.1/src/deocde_jzb.egg-info/PKG-INFO
--rw-rw-r--   0 mk        (1000) mk        (1000)      240 2024-05-08 04:52:13.000000 deocde_jzb-0.0.1/src/deocde_jzb.egg-info/SOURCES.txt
--rw-rw-r--   0 mk        (1000) mk        (1000)        1 2024-05-08 04:52:13.000000 deocde_jzb-0.0.1/src/deocde_jzb.egg-info/dependency_links.txt
--rw-rw-r--   0 mk        (1000) mk        (1000)       11 2024-05-08 04:52:13.000000 deocde_jzb-0.0.1/src/deocde_jzb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 05:38:13.000000 deocde_jzb-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 05:38:13.000000 deocde_jzb-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 05:38:13.000000 deocde_jzb-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/src/deocde_jzb/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-08 05:38:13.000000 deocde_jzb-0.0.3/src/deocde_jzb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 05:38:13.000000 deocde_jzb-0.0.3/src/deocde_jzb/decode_jzb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:38:18.929906 deocde_jzb-0.0.3/src/deocde_jzb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 05:38:18.000000 deocde_jzb-0.0.3/src/deocde_jzb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 05:38:18.000000 deocde_jzb-0.0.3/src/deocde_jzb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 05:38:18.000000 deocde_jzb-0.0.3/src/deocde_jzb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 05:38:18.000000 deocde_jzb-0.0.3/src/deocde_jzb.egg-info/top_level.txt
```

### Comparing `deocde_jzb-0.0.1/LICENSE` & `deocde_jzb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deocde_jzb-0.0.1/PKG-INFO` & `deocde_jzb-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: deocde_jzb
-Version: 0.0.1
-Summary: A small example package
-Author-email: A tiny Python program for decoding a jzb string <menachemkornreich@gmail.com>
+Version: 0.0.3
+Summary: A tiny Python program for decoding a jzb string
+Author-email: Menachem Kornreich <menachemkornreich@gmail.com>
 Project-URL: Homepage, https://github.com/mkornreich/jzb
 Project-URL: Issues, https://github.com/mkornreich/jzb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  Decoding JZB with Python
 
 A tiny Python program for decoding a jzb string
```

### Comparing `deocde_jzb-0.0.1/src/deocde_jzb.egg-info/PKG-INFO` & `deocde_jzb-0.0.3/src/deocde_jzb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: deocde_jzb
-Version: 0.0.1
-Summary: A small example package
-Author-email: A tiny Python program for decoding a jzb string <menachemkornreich@gmail.com>
+Version: 0.0.3
+Summary: A tiny Python program for decoding a jzb string
+Author-email: Menachem Kornreich <menachemkornreich@gmail.com>
 Project-URL: Homepage, https://github.com/mkornreich/jzb
 Project-URL: Issues, https://github.com/mkornreich/jzb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  Decoding JZB with Python
 
 A tiny Python program for decoding a jzb string
```

