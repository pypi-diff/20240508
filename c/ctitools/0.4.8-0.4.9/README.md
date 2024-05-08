# Comparing `tmp/ctitools-0.4.8.tar.gz` & `tmp/ctitools-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctitools-0.4.8.tar", max compression
+gzip compressed data, was "ctitools-0.4.9.tar", max compression
```

## Comparing `ctitools-0.4.8.tar` & `ctitools-0.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.8/LICENSE
--rw-r--r--   0        0        0     1284 2023-12-01 17:25:30.834109 ctitools-0.4.8/README.rst
--rw-r--r--   0        0        0      586 2023-06-10 19:51:29.125002 ctitools-0.4.8/berhoel/__init__.py
--rw-r--r--   0        0        0     8340 2024-01-10 19:54:06.823682 ctitools-0.4.8/berhoel/ctitools/__init__.py
--rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.8/berhoel/ctitools/__main__.py
--rw-r--r--   0        0        0     6377 2024-01-10 20:21:27.902753 ctitools-0.4.8/berhoel/ctitools/ct.py
--rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.8/berhoel/ctitools/cti2bibtex/__init__.py
--rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.8/berhoel/ctitools/cti2bibtex/__main__.py
--rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.8/berhoel/ctitools/cti2bibtex/tests/test_base.py
--rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.8/berhoel/ctitools/cti2bibtex/tests/test_generate.py
--rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.8/berhoel/ctitools/ctientry.py
--rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.8/berhoel/ctitools/ix.py
--rw-r--r--   0        0        0     1998 2024-01-10 19:49:17.980505 ctitools-0.4.8/berhoel/ctitools/tests/test_ct.py
--rw-r--r--   0        0        0     1177 2024-01-10 20:20:47.239443 ctitools-0.4.8/berhoel/ctitools/tests/test_ctitools.py
--rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.8/berhoel/ctitools/tests/test_processing.py
--rw-r--r--   0        0        0     3254 2024-01-10 20:19:10.502833 ctitools-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 ctitools-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1284 2023-12-01 17:25:30.834109 ctitools-0.4.9/README.rst
+-rw-r--r--   0        0        0      586 2023-06-10 19:51:29.125002 ctitools-0.4.9/berhoel/__init__.py
+-rw-r--r--   0        0        0     8340 2024-01-10 19:54:06.823682 ctitools-0.4.9/berhoel/ctitools/__init__.py
+-rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.9/berhoel/ctitools/__main__.py
+-rw-r--r--   0        0        0     6429 2024-02-08 19:53:23.161088 ctitools-0.4.9/berhoel/ctitools/ct.py
+-rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.9/berhoel/ctitools/cti2bibtex/__init__.py
+-rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.9/berhoel/ctitools/cti2bibtex/__main__.py
+-rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.9/berhoel/ctitools/cti2bibtex/tests/test_base.py
+-rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.9/berhoel/ctitools/cti2bibtex/tests/test_generate.py
+-rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.9/berhoel/ctitools/ctientry.py
+-rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.9/berhoel/ctitools/ix.py
+-rw-r--r--   0        0        0     1998 2024-01-10 19:49:17.980505 ctitools-0.4.9/berhoel/ctitools/tests/test_ct.py
+-rw-r--r--   0        0        0     1177 2024-01-10 20:20:47.239443 ctitools-0.4.9/berhoel/ctitools/tests/test_ctitools.py
+-rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.9/berhoel/ctitools/tests/test_processing.py
+-rw-r--r--   0        0        0     3254 2024-02-08 19:59:08.974503 ctitools-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 ctitools-0.4.9/PKG-INFO
```

### Comparing `ctitools-0.4.8/LICENSE` & `ctitools-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/README.rst` & `ctitools-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/__init__.py` & `ctitools-0.4.9/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/__init__.py` & `ctitools-0.4.9/berhoel/ctitools/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/__main__.py` & `ctitools-0.4.9/berhoel/ctitools/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/ct.py` & `ctitools-0.4.9/berhoel/ctitools/ct.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Standard library imports.
 from datetime import datetime, timedelta
 
 # Local library imports.
 from .ctientry import CTIEntry
 
-__date__ = "2024/01/10 21:21:27 hoel"
+__date__ = "2024/02/08 20:53:22 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2022 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
 
@@ -183,14 +183,16 @@
 
         Returns:
           str
         """
         if issue == 27:
             if year == 2022:
                 issue = "c't Jahresrückblick 2022"
+            elif year == 2023:
+                pass
             elif year > 2015:
                 issue = "retro"
         if year < 1997 or year == 1997 and issue < 11:
             return f"{year:04d} / {Ct.month_issue_map[issue]}"
         return f"{year:04d} / {issue}"
```

### Comparing `ctitools-0.4.8/berhoel/ctitools/cti2bibtex/__init__.py` & `ctitools-0.4.9/berhoel/ctitools/cti2bibtex/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/cti2bibtex/__main__.py` & `ctitools-0.4.9/berhoel/ctitools/cti2bibtex/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/cti2bibtex/tests/test_base.py` & `ctitools-0.4.9/berhoel/ctitools/cti2bibtex/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/cti2bibtex/tests/test_generate.py` & `ctitools-0.4.9/berhoel/ctitools/cti2bibtex/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/ctientry.py` & `ctitools-0.4.9/berhoel/ctitools/ctientry.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/ix.py` & `ctitools-0.4.9/berhoel/ctitools/ix.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/tests/test_ct.py` & `ctitools-0.4.9/berhoel/ctitools/tests/test_ct.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/tests/test_ctitools.py` & `ctitools-0.4.9/berhoel/ctitools/tests/test_ctitools.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/berhoel/ctitools/tests/test_processing.py` & `ctitools-0.4.9/berhoel/ctitools/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.8/pyproject.toml` & `ctitools-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctitools"
-version = "0.4.8"
+version = "0.4.9"
 
 description = "Work with cti index files for the Heise papers c't and iX"
 
 packages = [
          { include = "berhoel" }
 ]
 exclude = ["**/.#*.py", "**/#*.py#"]
```

### Comparing `ctitools-0.4.8/PKG-INFO` & `ctitools-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctitools
-Version: 0.4.8
+Version: 0.4.9
 Summary: Work with cti index files for the Heise papers c't and iX
 Home-page: https://python.xn--hllmanns-n4a.de/ctitools/
 License: BSD 3
 Author: Berthold Höllmann
 Author-email: berthold@xn--hllmanns-n4a.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
```

