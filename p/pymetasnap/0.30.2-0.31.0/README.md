# Comparing `tmp/pymetasnap-0.30.2.tar.gz` & `tmp/pymetasnap-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.30.2.tar", max compression
+gzip compressed data, was "pymetasnap-0.31.0.tar", max compression
```

## Comparing `pymetasnap-0.30.2.tar` & `pymetasnap-0.31.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/LICENSE
--rw-r--r--   0        0        0     3043 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/README.md
--rw-r--r--   0        0        0        0 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/__init__.py
--rw-r--r--   0        0        0     3678 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/checks.py
--rw-r--r--   0        0        0     7141 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/core.py
--rw-r--r--   0        0        0      227 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/logger.py
--rw-r--r--   0        0        0     1345 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/main.py
--rw-r--r--   0        0        0     3262 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/extractor/render.py
--rw-r--r--   0        0        0      925 2024-04-02 00:41:05.568461 pymetasnap-0.30.2/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 pymetasnap-0.30.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/LICENSE
+-rw-r--r--   0        0        0     3035 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/__init__.py
+-rw-r--r--   0        0        0     3678 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/checks.py
+-rw-r--r--   0        0        0     7141 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/core.py
+-rw-r--r--   0        0        0      227 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/logger.py
+-rw-r--r--   0        0        0     1345 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/main.py
+-rw-r--r--   0        0        0     3262 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/extractor/render.py
+-rw-r--r--   0        0        0      925 2024-05-08 02:12:46.354459 pymetasnap-0.31.0/pyproject.toml
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 pymetasnap-0.31.0/PKG-INFO
```

### Comparing `pymetasnap-0.30.2/LICENSE` & `pymetasnap-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.2/README.md` & `pymetasnap-0.31.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 ## Acknowledgments
 
 The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
-For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com
+For any inquiries or feedback, please contact the project maintainer at using the issues tab.
```

### Comparing `pymetasnap-0.30.2/extractor/checks.py` & `pymetasnap-0.31.0/extractor/checks.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.2/extractor/core.py` & `pymetasnap-0.31.0/extractor/core.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.2/extractor/main.py` & `pymetasnap-0.31.0/extractor/main.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.2/extractor/render.py` & `pymetasnap-0.31.0/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.2/pyproject.toml` & `pymetasnap-0.31.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.30.2"
+version = "0.31.0"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.30.2/PKG-INFO` & `pymetasnap-0.31.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.30.2
+Version: 0.31.0
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -83,9 +83,9 @@
 
 ## Acknowledgments
 
 The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
-For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com
+For any inquiries or feedback, please contact the project maintainer at using the issues tab.
```

