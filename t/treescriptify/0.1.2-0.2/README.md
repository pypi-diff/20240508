# Comparing `tmp/treescriptify-0.1.2.tar.gz` & `tmp/treescriptify-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treescriptify-0.1.2.tar", last modified: Sun Apr 21 14:12:01 2024, max compression
+gzip compressed data, was "treescriptify-0.2.tar", last modified: Wed May  8 14:04:17 2024, max compression
```

## Comparing `treescriptify-0.1.2.tar` & `treescriptify-0.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:12:01.376984 treescriptify-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-21 14:11:51.000000 treescriptify-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 14:12:01.376984 treescriptify-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-21 14:11:51.000000 treescriptify-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:11:51.000000 treescriptify-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:12:01.376984 treescriptify-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-21 14:11:51.000000 treescriptify-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:12:01.376984 treescriptify-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-21 14:11:52.000000 treescriptify-0.1.2/test/test_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-21 14:11:52.000000 treescriptify-0.1.2/test/test_script_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-21 14:11:52.000000 treescriptify-0.1.2/test/test_tree_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-21 14:11:52.000000 treescriptify-0.1.2/test/test_tree_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:12:01.376984 treescriptify-0.1.2/treescriptify/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/script_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/tree_node_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/tree_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-21 14:11:52.000000 treescriptify-0.1.2/treescriptify/tree_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:12:01.376984 treescriptify-0.1.2/treescriptify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 14:12:01.000000 treescriptify-0.1.2/treescriptify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 14:12:01.000000 treescriptify-0.1.2/treescriptify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:12:01.000000 treescriptify-0.1.2/treescriptify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 14:12:01.000000 treescriptify-0.1.2/treescriptify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 14:12:01.000000 treescriptify-0.1.2/treescriptify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:04:17.266701 treescriptify-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-08 14:04:02.000000 treescriptify-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 14:04:17.266701 treescriptify-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 14:04:02.000000 treescriptify-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 14:04:02.000000 treescriptify-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:04:17.266701 treescriptify-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-08 14:04:02.000000 treescriptify-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:04:17.262701 treescriptify-0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 14:04:02.000000 treescriptify-0.2/test/test_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 14:04:02.000000 treescriptify-0.2/test/test_script_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-08 14:04:02.000000 treescriptify-0.2/test/test_tree_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-08 14:04:02.000000 treescriptify-0.2/test/test_tree_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 14:04:02.000000 treescriptify-0.2/test/test_windows_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:04:17.266701 treescriptify-0.2/treescriptify/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/script_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/tree_node_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/tree_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/tree_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 14:04:02.000000 treescriptify-0.2/treescriptify/windows_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:04:17.266701 treescriptify-0.2/treescriptify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 14:04:17.000000 treescriptify-0.2/treescriptify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 14:04:17.000000 treescriptify-0.2/treescriptify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:04:17.000000 treescriptify-0.2/treescriptify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 14:04:17.000000 treescriptify-0.2/treescriptify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 14:04:17.000000 treescriptify-0.2/treescriptify.egg-info/top_level.txt
```

### Comparing `treescriptify-0.1.2/LICENSE` & `treescriptify-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/PKG-INFO` & `treescriptify-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treescriptify
-Version: 0.1.2
+Version: 0.2
 Summary: Create TreeScript from an existing filesystem tree.
 Home-page: https://github.com/DK96-OS/treescriptify
 Author: DK96-OS
 License: GPLv2
 Project-URL: Issues, https://github.com/DK96-OS/treescriptify/issues
 Project-URL: Source Code, https://github.com/DK96-OS/treescriptify
 Classifier: Natural Language :: English
```

### Comparing `treescriptify-0.1.2/README.md` & `treescriptify-0.2/README.md`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/setup.py` & `treescriptify-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup Package Configuration
 """
 from setuptools import setup, find_packages
 
 
 setup(
     name="treescriptify",
-    version="0.1.2",
+    version="0.2",
     description="Create TreeScript from an existing filesystem tree.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="DK96-OS",
     url="https://github.com/DK96-OS/treescriptify",
     project_urls={
         "Issues": "https://github.com/DK96-OS/treescriptify/issues",
```

### Comparing `treescriptify-0.1.2/test/test_argument_parser.py` & `treescriptify-0.2/test/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/test/test_script_writer.py` & `treescriptify-0.2/test/test_script_writer.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/test/test_tree_reader.py` & `treescriptify-0.2/test/test_tree_reader.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/test/test_tree_runner.py` & `treescriptify-0.2/test/test_tree_runner.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/treescriptify/argument_parser.py` & `treescriptify-0.2/treescriptify/argument_parser.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/treescriptify/script_writer.py` & `treescriptify-0.2/treescriptify/script_writer.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/treescriptify/tree_reader.py` & `treescriptify-0.2/treescriptify/tree_reader.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/treescriptify/tree_runner.py` & `treescriptify-0.2/treescriptify/tree_runner.py`

 * *Files identical despite different names*

### Comparing `treescriptify-0.1.2/treescriptify.egg-info/PKG-INFO` & `treescriptify-0.2/treescriptify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treescriptify
-Version: 0.1.2
+Version: 0.2
 Summary: Create TreeScript from an existing filesystem tree.
 Home-page: https://github.com/DK96-OS/treescriptify
 Author: DK96-OS
 License: GPLv2
 Project-URL: Issues, https://github.com/DK96-OS/treescriptify/issues
 Project-URL: Source Code, https://github.com/DK96-OS/treescriptify
 Classifier: Natural Language :: English
```

### Comparing `treescriptify-0.1.2/treescriptify.egg-info/SOURCES.txt` & `treescriptify-0.2/treescriptify.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 README.md
 pyproject.toml
 setup.py
 test/test_argument_parser.py
 test/test_script_writer.py
 test/test_tree_reader.py
 test/test_tree_runner.py
+test/test_windows_tree.py
 treescriptify/__init__.py
 treescriptify/__main__.py
 treescriptify/argument_parser.py
 treescriptify/input_data.py
 treescriptify/script_writer.py
 treescriptify/tree_node_data.py
 treescriptify/tree_reader.py
 treescriptify/tree_runner.py
+treescriptify/windows_tree.py
 treescriptify.egg-info/PKG-INFO
 treescriptify.egg-info/SOURCES.txt
 treescriptify.egg-info/dependency_links.txt
 treescriptify.egg-info/entry_points.txt
 treescriptify.egg-info/top_level.txt
```

