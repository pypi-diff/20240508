# Comparing `tmp/hfive-0.1.0.tar.gz` & `tmp/hfive-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfive-0.1.0.tar", last modified: Fri Apr 26 14:48:48 2024, max compression
+gzip compressed data, was "hfive-0.1.1.tar", last modified: Tue May  7 22:58:42 2024, max compression
```

## Comparing `hfive-0.1.0.tar` & `hfive-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 14:48:48.107623 hfive-0.1.0/
--rw-r--r--   0 florez    (1000) florez    (1000)     1056 2024-04-26 13:36:33.000000 hfive-0.1.0/LICENSE
--rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-04-26 14:48:48.107623 hfive-0.1.0/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      156 2024-04-26 14:47:26.000000 hfive-0.1.0/README.md
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 14:48:48.107623 hfive-0.1.0/hfive/
--rw-r--r--   0 florez    (1000) florez    (1000)      119 2024-04-26 14:16:16.000000 hfive-0.1.0/hfive/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3428 2024-04-26 14:15:37.000000 hfive-0.1.0/hfive/common.py
--rw-r--r--   0 florez    (1000) florez    (1000)    18315 2024-04-26 14:44:12.000000 hfive-0.1.0/hfive/main.py
--rw-r--r--   0 florez    (1000) florez    (1000)    14665 2024-04-26 14:48:06.000000 hfive-0.1.0/hfive/widgets.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 14:48:48.107623 hfive-0.1.0/hfive.egg-info/
--rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      282 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/SOURCES.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/dependency_links.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       42 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/entry_points.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       17 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/requires.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        6 2024-04-26 14:48:48.000000 hfive-0.1.0/hfive.egg-info/top_level.txt
--rw-r--r--   0 florez    (1000) florez    (1000)      919 2024-04-26 14:47:51.000000 hfive-0.1.0/pyproject.toml
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 14:48:48.107623 hfive-0.1.0/setup.cfg
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 14:08:50.000000 hfive-0.1.0/setup.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.776718 hfive-0.1.1/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1056 2024-04-26 13:36:33.000000 hfive-0.1.1/LICENSE
+-rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-07 22:58:42.773385 hfive-0.1.1/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)      156 2024-04-26 14:47:26.000000 hfive-0.1.1/README.md
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.773385 hfive-0.1.1/hfive/
+-rw-r--r--   0 florez    (1000) florez    (1000)      119 2024-05-07 22:57:19.000000 hfive-0.1.1/hfive/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3656 2024-05-07 22:56:41.000000 hfive-0.1.1/hfive/common.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    18315 2024-04-26 16:16:03.000000 hfive-0.1.1/hfive/main.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    14665 2024-04-26 14:48:06.000000 hfive-0.1.1/hfive/widgets.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.773385 hfive-0.1.1/hfive.egg-info/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)      282 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/SOURCES.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/dependency_links.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       42 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/entry_points.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       17 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/requires.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        6 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/top_level.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)      919 2024-05-07 22:57:09.000000 hfive-0.1.1/pyproject.toml
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-05-07 22:58:42.776718 hfive-0.1.1/setup.cfg
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 14:08:50.000000 hfive-0.1.1/setup.py
```

### Comparing `hfive-0.1.0/LICENSE` & `hfive-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hfive-0.1.0/PKG-INFO` & `hfive-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfive
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple TUI for viewing HDF5 files.
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2024 Flavio Lorez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `hfive-0.1.0/hfive/common.py` & `hfive-0.1.1/hfive/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,22 @@
               raises an ExitMainLoop exception to exit the main loop.
         """
         if len(cls.widget_stack) <= 1:
             raise urwid.ExitMainLoop()
         cls.widget_stack.pop()
         cls.main_loop.widget = cls.widget_stack[-1]
 
+# If a Caller is present from the parent bamboost cli, use it. 
+# It uses the urwid namespace as this is the only way I know currently to share
+# the Caller object
+try:
+    Caller = urwid.Caller
+except AttributeError:
+    pass
+
 
 # ----------------------------------------
 # Type definitions
 # ----------------------------------------
 Keybinds = Dict[str, Tuple[Callable, str, List[str]]]
```

### Comparing `hfive-0.1.0/hfive/main.py` & `hfive-0.1.1/hfive/main.py`

 * *Files identical despite different names*

### Comparing `hfive-0.1.0/hfive/widgets.py` & `hfive-0.1.1/hfive/widgets.py`

 * *Files identical despite different names*

### Comparing `hfive-0.1.0/hfive.egg-info/PKG-INFO` & `hfive-0.1.1/hfive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfive
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple TUI for viewing HDF5 files.
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2024 Flavio Lorez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `hfive-0.1.0/pyproject.toml` & `hfive-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hfive"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple TUI for viewing HDF5 files."
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [{ name = "Flavio Lorez", email = "florez@ethz.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

