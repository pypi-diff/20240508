# Comparing `tmp/eintorch-0.1.1.tar.gz` & `tmp/eintorch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eintorch-0.1.1.tar", max compression
+gzip compressed data, was "eintorch-0.2.1.tar", max compression
```

## Comparing `eintorch-0.1.1.tar` & `eintorch-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1515 2024-01-29 14:31:55.780653 eintorch-0.1.1/LICENSE
--rw-r--r--   0        0        0       63 2024-01-29 13:50:58.821026 eintorch-0.1.1/README.md
--rw-r--r--   0        0        0      621 2024-01-29 14:32:02.709779 eintorch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       46 2024-01-29 13:51:13.829017 eintorch-0.1.1/src/eintorch/__init__.py
--rw-r--r--   0        0        0      430 2024-01-29 13:51:26.875367 eintorch-0.1.1/src/eintorch/_callbacks.py
--rw-r--r--   0        0        0      579 2024-01-29 14:31:47.313778 eintorch-0.1.1/src/eintorch/_core.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 eintorch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2024-02-04 11:41:26.968966 eintorch-0.2.1/LICENSE
+-rw-r--r--   0        0        0       63 2024-05-06 21:43:46.710723 eintorch-0.2.1/README.md
+-rw-r--r--   0        0        0      678 2024-05-08 16:00:57.377873 eintorch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-06 21:46:30.204115 eintorch-0.2.1/src/eintorch/.DS_Store
+-rw-r--r--   0        0        0       99 2024-05-02 15:12:31.395026 eintorch-0.2.1/src/eintorch/__init__.py
+-rw-r--r--   0        0        0     4347 2024-05-07 12:38:20.849516 eintorch-0.2.1/src/eintorch/_core.py
+-rw-r--r--   0        0        0     1369 2024-05-06 23:31:40.470828 eintorch-0.2.1/src/eintorch/_functions.py
+-rw-r--r--   0        0        0     2412 2024-05-06 21:10:54.810858 eintorch-0.2.1/src/eintorch/_preprocessing.py
+-rw-r--r--   0        0        0     1017 2024-05-06 21:29:42.595030 eintorch-0.2.1/src/eintorch/_utils.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 eintorch-0.2.1/PKG-INFO
```

### Comparing `eintorch-0.1.1/LICENSE` & `eintorch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eintorch-0.1.1/PKG-INFO` & `eintorch-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: eintorch
-Version: 0.1.1
+Version: 0.2.1
 Summary: An alternative interface for torchdim
 Author: Jakub Bachurski
 Author-email: kbachurski@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: functorch (>=2.0.0,<3.0.0)
-Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # eintorch
 
 An alternative interface for `functorch.torchdim`.
```

