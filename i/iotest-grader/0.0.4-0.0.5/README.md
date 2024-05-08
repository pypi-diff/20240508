# Comparing `tmp/iotest_grader-0.0.4.tar.gz` & `tmp/iotest_grader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotest_grader-0.0.4.tar", last modified: Wed May  8 02:53:15 2024, max compression
+gzip compressed data, was "iotest_grader-0.0.5.tar", last modified: Wed May  8 03:00:20 2024, max compression
```

## Comparing `iotest_grader-0.0.4.tar` & `iotest_grader-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.401041 iotest_grader-0.0.4/iotest/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/iotest/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1525 2024-05-08 02:53:00.000000 iotest_grader-0.0.4/iotest/harness.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/iotest_grader.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 02:53:11.000000 iotest_grader-0.0.4/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.973026 iotest_grader-0.0.5/iotest/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/iotest/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1535 2024-05-08 02:54:13.000000 iotest_grader-0.0.5/iotest/harness.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/iotest_grader.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 03:00:16.000000 iotest_grader-0.0.5/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/setup.cfg
```

### Comparing `iotest_grader-0.0.4/LICENSE` & `iotest_grader-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iotest_grader-0.0.4/PKG-INFO` & `iotest_grader-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotest_grader-0.0.4/iotest/harness.py` & `iotest_grader-0.0.5/iotest/harness.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import pexpect
 import inspect
 import subprocess
+import os
 
 def find_cases():
     caller_dir = pathlib.Path(inspect.stack()[1][1]).parent
     cases_dir = caller_dir / 'testcases'
     return [x.name for x in cases_dir.iterdir() if x.is_dir()]
```

### Comparing `iotest_grader-0.0.4/iotest_grader.egg-info/PKG-INFO` & `iotest_grader-0.0.5/iotest_grader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotest_grader-0.0.4/pyproject.toml` & `iotest_grader-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iotest-grader"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Joe Delfino", email="jdelfino@brandeis.edu" },
 ]
 description = "A pytest harness for input/output tests, intended for use in VSCode"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

