# Comparing `tmp/bastet-0.1.0.dev1.tar.gz` & `tmp/bastet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastet-0.1.0.dev1.tar", last modified: Mon Apr 22 13:52:10 2024, max compression
+gzip compressed data, was "bastet-0.1.1.tar", last modified: Wed May  8 13:19:02 2024, max compression
```

## Comparing `bastet-0.1.0.dev1.tar` & `bastet-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.455565 bastet-0.1.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.455565 bastet-0.1.0.dev1/src/bastet/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/src/bastet/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/codeclimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/reporting/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/src/bastet/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/reuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-04-22 13:52:04.000000 bastet-0.1.0.dev1/src/bastet/tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:52:10.459565 bastet-0.1.0.dev1/src/bastet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 13:52:10.000000 bastet-0.1.0.dev1/src/bastet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 13:52:08.000000 bastet-0.1.0.dev1/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.995634 bastet-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-08 13:18:58.000000 bastet-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 13:19:02.995634 bastet-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-08 13:18:58.000000 bastet-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-08 13:18:58.000000 bastet-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:19:02.995634 bastet-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.987634 bastet-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.991634 bastet-0.1.1/src/bastet/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.991634 bastet-0.1.1/src/bastet/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/codeclimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/reporting/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.991634 bastet-0.1.1/src/bastet/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/reuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-08 13:18:58.000000 bastet-0.1.1/src/bastet/tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:19:02.995634 bastet-0.1.1/src/bastet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 13:19:02.000000 bastet-0.1.1/src/bastet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 13:19:01.000000 bastet-0.1.1/version
```

### Comparing `bastet-0.1.0.dev1/LICENSE.md` & `bastet-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/PKG-INFO` & `bastet-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.1.0.dev1
+Version: 0.1.1
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.1.0.dev1/README.md` & `bastet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/pyproject.toml` & `bastet-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/__main__.py` & `bastet-0.1.1/src/bastet/__main__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/config.py` & `bastet-0.1.1/src/bastet/config.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/__init__.py` & `bastet-0.1.1/src/bastet/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/abc.py` & `bastet-0.1.1/src/bastet/reporting/abc.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/codeclimate.py` & `bastet-0.1.1/src/bastet/reporting/codeclimate.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/console.py` & `bastet-0.1.1/src/bastet/reporting/console.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/file.py` & `bastet-0.1.1/src/bastet/reporting/file.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/reporting/github.py` & `bastet-0.1.1/src/bastet/reporting/github.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/runner.py` & `bastet-0.1.1/src/bastet/runner.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/__init__.py` & `bastet-0.1.1/src/bastet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/audit.py` & `bastet-0.1.1/src/bastet/tools/audit.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/exceptions.py` & `bastet-0.1.1/src/bastet/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/format.py` & `bastet-0.1.1/src/bastet/tools/format.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/lint.py` & `bastet-0.1.1/src/bastet/tools/lint.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/reuse.py` & `bastet-0.1.1/src/bastet/tools/reuse.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/test.py` & `bastet-0.1.1/src/bastet/tools/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
         Pytest command -- runs with coverage by default.
         """
         return [
             "pytest",
             f"--junit-xml={(self._paths.report_path / 'junit-test.xml')!s}",
             f"--cov-report=html:{self._paths.report_path!s}",
             f"--cov-report=xml:{(self._paths.report_path / 'coverage.xml')!s}",
-            *(f"--cov={module!s}" for module in self._paths.python_module_path),
+            *(
+                f"--cov={module.relative_to(self._paths.root_path)!s}"
+                for module in self._paths.python_module_path
+            ),
         ]
 
     def get_environment(self) -> dict[str, str]:
         """
         Environment variables to set when calling this tool.
         """
         return {}
```

### Comparing `bastet-0.1.0.dev1/src/bastet/tools/tool.py` & `bastet-0.1.1/src/bastet/tools/tool.py`

 * *Files identical despite different names*

### Comparing `bastet-0.1.0.dev1/src/bastet.egg-info/PKG-INFO` & `bastet-0.1.1/src/bastet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastet
-Version: 0.1.0.dev1
+Version: 0.1.1
 Summary: Bastet Python Developers Tools (https://github.com/mewbotorg/bastet)
 Author-email: MewBot Org <mewbot@quicksilver.london>
 Maintainer-email: MewBot Org <mewbot@quicksilver.london>
 Project-URL: Source, https://github.com/mewbotorg/bastet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bastet-0.1.0.dev1/src/bastet.egg-info/SOURCES.txt` & `bastet-0.1.1/src/bastet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

