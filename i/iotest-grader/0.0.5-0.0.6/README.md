# Comparing `tmp/iotest_grader-0.0.5.tar.gz` & `tmp/iotest_grader-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotest_grader-0.0.5.tar", last modified: Wed May  8 03:00:20 2024, max compression
+gzip compressed data, was "iotest_grader-0.0.6.tar", last modified: Wed May  8 03:11:59 2024, max compression
```

## Comparing `iotest_grader-0.0.5.tar` & `iotest_grader-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.973026 iotest_grader-0.0.5/iotest/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.5/iotest/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1535 2024-05-08 02:54:13.000000 iotest_grader-0.0.5/iotest/harness.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/iotest_grader.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 03:00:20.000000 iotest_grader-0.0.5/iotest_grader.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 03:00:16.000000 iotest_grader-0.0.5/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 03:00:20.977026 iotest_grader-0.0.5/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:11:59.469002 iotest_grader-0.0.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2024-05-08 02:30:38.000000 iotest_grader-0.0.6/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:11:59.469002 iotest_grader-0.0.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2024-05-08 02:30:38.000000 iotest_grader-0.0.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:11:59.465002 iotest_grader-0.0.6/iotest/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       62 2024-05-08 02:30:38.000000 iotest_grader-0.0.6/iotest/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1519 2024-05-08 03:11:43.000000 iotest_grader-0.0.6/iotest/harness.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-08 03:11:59.469002 iotest_grader-0.0.6/iotest_grader.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      725 2024-05-08 03:11:59.000000 iotest_grader-0.0.6/iotest_grader.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      253 2024-05-08 03:11:59.000000 iotest_grader-0.0.6/iotest_grader.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-08 03:11:59.000000 iotest_grader-0.0.6/iotest_grader.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       49 2024-05-08 03:11:59.000000 iotest_grader-0.0.6/iotest_grader.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-05-08 03:11:59.000000 iotest_grader-0.0.6/iotest_grader.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2024-05-08 03:11:54.000000 iotest_grader-0.0.6/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-08 03:11:59.469002 iotest_grader-0.0.6/setup.cfg
```

### Comparing `iotest_grader-0.0.5/LICENSE` & `iotest_grader-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iotest_grader-0.0.5/PKG-INFO` & `iotest_grader-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iotest_grader-0.0.5/iotest/harness.py` & `iotest_grader-0.0.6/iotest/harness.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     for i in inp:
         child.sendline(i)
 
     actual = [x.strip() for x in child.read().decode('ascii').split('\r\n') if x]
     with open(actual_file, 'w') as outfile:
         outfile.writelines([x + '\n' for x in actual])
     
-    in_vscode = 'TERM_PROGRAM' in os.environ.keys() and os.environ['TERM_PROGRAM'] == 'vscode'
+    in_vscode = 'USER' in os.environ.keys() and os.environ['USER'] == 'vscode'
     if in_vscode and (actual != expected):
         subprocess.run(['code', '-d', actual_file, expected_file])
 
     assert actual == expected, f"Comparison failed, run this command to see the differences:\ncode -d {expected_file} {actual_file}"
```

### Comparing `iotest_grader-0.0.5/iotest_grader.egg-info/PKG-INFO` & `iotest_grader-0.0.6/iotest_grader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotest-grader
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pytest harness for input/output tests, intended for use in VSCode
 Author-email: Joe Delfino <jdelfino@brandeis.edu>
 Project-URL: Homepage, https://github.com/brandeis-cosi-10a/input-output-test
 Project-URL: Issues, https://github.com/brandeis-cosi-10a/input-output-test/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

