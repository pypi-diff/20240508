# Comparing `tmp/iotest_grader-0.0.3.tar.gz` & `tmp/iotest_grader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotest_grader-0.0.3.tar", last modified: Wed May  8 02:41:10 2024, max compression
+gzip compressed data, was "iotest_grader-0.0.4.tar", last modified: Wed May  8 02:53:15 2024, max compression
```

## Comparing `iotest_grader-0.0.3.tar` & `iotest_grader-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/iotest/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/iotest/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1414 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/iotest/harness.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/iotest_grader.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 02:41:10.000000 iotest_grader-0.0.3/iotest_grader.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 02:30:38.000000 iotest_grader-0.0.3/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 02:41:10.361066 iotest_grader-0.0.3/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.401041 iotest_grader-0.0.4/iotest/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.4/iotest/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1525 2024-05-08 02:53:00.000000 iotest_grader-0.0.4/iotest/harness.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/iotest_grader.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 02:53:15.000000 iotest_grader-0.0.4/iotest_grader.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 02:53:11.000000 iotest_grader-0.0.4/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 02:53:15.405041 iotest_grader-0.0.4/setup.cfg
```

### Comparing `iotest_grader-0.0.3/LICENSE` & `iotest_grader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iotest_grader-0.0.3/PKG-INFO` & `iotest_grader-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotest_grader-0.0.3/iotest/harness.py` & `iotest_grader-0.0.4/iotest/harness.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,11 +27,12 @@
     for i in inp:
         child.sendline(i)
 
     actual = [x.strip() for x in child.read().decode('ascii').split('\r\n') if x]
     with open(actual_file, 'w') as outfile:
         outfile.writelines([x + '\n' for x in actual])
     
-    if actual != expected:
+    in_vscode = 'TERM_PROGRAM' in os.environ.keys() and os.environ['TERM_PROGRAM'] == 'vscode'
+    if in_vscode and (actual != expected):
         subprocess.run(['code', '-d', actual_file, expected_file])
 
     assert actual == expected, f"Comparison failed, run this command to see the differences:\ncode -d {expected_file} {actual_file}"
```

### Comparing `iotest_grader-0.0.3/iotest_grader.egg-info/PKG-INFO` & `iotest_grader-0.0.4/iotest_grader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotest_grader-0.0.3/pyproject.toml` & `iotest_grader-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iotest-grader"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Joe Delfino", email="jdelfino@brandeis.edu" },
 ]
 description = "A pytest harness for input/output tests, intended for use in VSCode"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

