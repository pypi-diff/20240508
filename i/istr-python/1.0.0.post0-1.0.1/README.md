# Comparing `tmp/istr_python-1.0.0.post0.tar.gz` & `tmp/istr_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-1.0.0.post0.tar", last modified: Tue May  7 15:27:01 2024, max compression
+gzip compressed data, was "istr_python-1.0.1.tar", last modified: Tue May  7 16:20:03 2024, max compression
```

## Comparing `istr_python-1.0.0.post0.tar` & `istr_python-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.200452 istr_python-1.0.0.post0/
--rw-rw-rw-   0        0        0    16564 2024-05-07 15:27:01.194781 istr_python-1.0.0.post0/PKG-INFO
--rw-rw-rw-   0        0        0     3506 2024-05-07 14:46:38.000000 istr_python-1.0.0.post0/changelog.md
-drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.044344 istr_python-1.0.0.post0/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.0.post0/istr/__init__.py
--rw-rw-rw-   0        0        0    22612 2024-05-07 15:26:00.000000 istr_python-1.0.0.post0/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.189048 istr_python-1.0.0.post0/istr_python.egg-info/
--rw-rw-rw-   0        0        0    16564 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-07 15:27:01.000000 istr_python-1.0.0.post0/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2024-05-07 15:26:52.000000 istr_python-1.0.0.post0/pyproject.toml
--rw-rw-rw-   0        0        0    15395 2024-05-07 15:20:46.000000 istr_python-1.0.0.post0/readme.md
--rw-rw-rw-   0        0        0       42 2024-05-07 15:27:01.202010 istr_python-1.0.0.post0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.179779 istr_python-1.0.0.post0/tests/
--rw-rw-rw-   0        0        0    16873 2024-05-07 14:59:26.000000 istr_python-1.0.0.post0/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:03.264652 istr_python-1.0.1/
+-rw-rw-rw-   0        0        0    16558 2024-05-07 16:20:03.261087 istr_python-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15395 2024-05-07 15:20:46.000000 istr_python-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:03.185354 istr_python-1.0.1/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.1/istr/__init__.py
+-rw-rw-rw-   0        0        0     3506 2024-05-07 14:46:38.000000 istr_python-1.0.1/istr/changelog.md
+-rw-rw-rw-   0        0        0    22675 2024-05-07 16:19:07.000000 istr_python-1.0.1/istr/istr.py
+-rw-rw-rw-   0        0        0    15395 2024-05-07 15:20:46.000000 istr_python-1.0.1/istr/readme.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:03.257741 istr_python-1.0.1/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    16558 2024-05-07 16:20:03.000000 istr_python-1.0.1/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-07 16:20:03.000000 istr_python-1.0.1/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:20:03.000000 istr_python-1.0.1/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-07 16:20:03.000000 istr_python-1.0.1/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2024-05-07 16:19:55.000000 istr_python-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:20:03.264652 istr_python-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 16:20:03.255113 istr_python-1.0.1/tests/
+-rw-rw-rw-   0        0        0    16873 2024-05-07 14:59:26.000000 istr_python-1.0.1/tests/test_istr.py
```

### Comparing `istr_python-1.0.0.post0/PKG-INFO` & `istr_python-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.0.post0
+Version: 1.0.1
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-1.0.0.post0/changelog.md` & `istr_python-1.0.1/istr/changelog.md`

 * *Files identical despite different names*

### Comparing `istr_python-1.0.0.post0/istr/istr.py` & `istr_python-1.0.1/istr/istr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 import functools
 import math
 
 """
 Note: the changelog is now in changelog.md
+
+You can view the changelog on www.salabim/istr_changelog.html
 """
 
 
 class _range:
     """
     based on https://codereview.stackexchange.com/questions/229073/pure-python-range-implementation
     """
```

### Comparing `istr_python-1.0.0.post0/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.1/istr_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.0.post0
+Version: 1.0.1
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-1.0.0.post0/pyproject.toml` & `istr_python-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "1.0.0-0"
+version = "1.0.1"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -22,8 +22,8 @@
 Homepage = "https://github.com/salabim/istr"
 Repository = "https://github.com/salabim/istr"
 
 [tool.setuptools]
 packages = ["istr"]
 
 [tool.setuptools.package-data]
-"*" = ["../*.md"]
+"*" = ["*.md"]
```

### Comparing `istr_python-1.0.0.post0/readme.md` & `istr_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `istr_python-1.0.0.post0/tests/test_istr.py` & `istr_python-1.0.1/tests/test_istr.py`

 * *Files identical despite different names*

