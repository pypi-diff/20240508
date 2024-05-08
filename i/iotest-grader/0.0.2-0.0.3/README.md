# Comparing `tmp/iotest_grader-0.0.2.tar.gz` & `tmp/iotest_grader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotest_grader-0.0.2.tar", last modified: Mon Apr 22 18:10:53 2024, max compression
+gzip compressed data, was "iotest_grader-0.0.3.tar", last modified: Wed May  8 02:41:10 2024, max compression
```

## Comparing `iotest_grader-0.0.2.tar` & `iotest_grader-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 18:10:53.022285 iotest_grader-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-04-21 21:01:51.000000 iotest_grader-0.0.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      697 2024-04-22 18:10:53.022285 iotest_grader-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-04-21 21:01:51.000000 iotest_grader-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 18:10:53.018285 iotest_grader-0.0.2/iotest/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-04-21 22:01:11.000000 iotest_grader-0.0.2/iotest/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1315 2024-04-22 18:09:42.000000 iotest_grader-0.0.2/iotest/harness.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-22 18:10:53.018285 iotest_grader-0.0.2/iotest_grader.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      697 2024-04-22 18:10:53.000000 iotest_grader-0.0.2/iotest_grader.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-04-22 18:10:53.000000 iotest_grader-0.0.2/iotest_grader.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-22 18:10:53.000000 iotest_grader-0.0.2/iotest_grader.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-04-22 18:10:53.000000 iotest_grader-0.0.2/iotest_grader.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-04-22 18:10:53.000000 iotest_grader-0.0.2/iotest_grader.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      706 2024-04-22 18:10:19.000000 iotest_grader-0.0.2/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-22 18:10:53.022285 iotest_grader-0.0.2/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/iotest/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/iotest/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1414 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/iotest/harness.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/iotest_grader.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/setup.cfg
```

### Comparing `iotest_grader-0.0.2/LICENSE` & `iotest_grader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iotest_grader-0.0.2/PKG-INFO` & `iotest_grader-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.2
-Summary: A pytest harness for input/output tests
+Version: 0.0.3
+Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `iotest_grader-0.0.2/iotest/harness.py` & `iotest_grader-0.0.3/iotest/harness.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 import pexpect
-import pytest
 import inspect
+import subprocess
 
 def find_cases():
     caller_dir = pathlib.Path(inspect.stack()[1][1]).parent
     cases_dir = caller_dir / 'testcases'
     return [x.name for x in cases_dir.iterdir() if x.is_dir()]
 
 
@@ -27,8 +27,11 @@
     for i in inp:
         child.sendline(i)
 
     actual = [x.strip() for x in child.read().decode('ascii').split('\r\n') if x]
     with open(actual_file, 'w') as outfile:
         outfile.writelines([x + '\n' for x in actual])
     
+    if actual != expected:
+        subprocess.run(['code', '-d', actual_file, expected_file])
+
     assert actual == expected, f"Comparison failed, run this command to see the differences:\ncode -d {expected_file} {actual_file}"
```

### Comparing `iotest_grader-0.0.2/iotest_grader.egg-info/PKG-INFO` & `iotest_grader-0.0.3/iotest_grader.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.2
-Summary: A pytest harness for input/output tests
+Version: 0.0.3
+Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `iotest_grader-0.0.2/pyproject.toml` & `iotest_grader-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iotest-grader"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Joe Delfino", email="jdelfino@brandeis.edu" },
 ]
-description = "A pytest harness for input/output tests"
+description = "A pytest harness for input/output tests, intended for use in VSCode"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

