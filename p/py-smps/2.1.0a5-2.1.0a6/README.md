# Comparing `tmp/py_smps-2.1.0a5.tar.gz` & `tmp/py_smps-2.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_smps-2.1.0a5.tar", max compression
+gzip compressed data, was "py_smps-2.1.0a6.tar", max compression
```

## Comparing `py_smps-2.1.0a5.tar` & `py_smps-2.1.0a6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-05-07 02:59:20.275804 py_smps-2.1.0a5/LICENSE
--rw-r--r--   0        0        0     2614 2024-05-07 02:59:20.275804 py_smps-2.1.0a5/README.md
--rw-r--r--   0        0        0     1183 2024-05-07 02:59:20.287804 py_smps-2.1.0a5/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/__init__.py
--rw-r--r--   0        0        0    19832 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/fit.py
--rw-r--r--   0        0        0     7881 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/io.py
--rw-r--r--   0        0        0    30952 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/models.py
--rw-r--r--   0        0        0     5414 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/plots.py
--rw-r--r--   0        0        0      801 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/rcmod.py
--rw-r--r--   0        0        0     9321 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/utils.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 py_smps-2.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-08 21:43:22.232657 py_smps-2.1.0a6/LICENSE
+-rw-r--r--   0        0        0     2614 2024-05-08 21:43:22.232657 py_smps-2.1.0a6/README.md
+-rw-r--r--   0        0        0     1169 2024-05-08 21:43:22.244657 py_smps-2.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/__init__.py
+-rw-r--r--   0        0        0    19832 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/fit.py
+-rw-r--r--   0        0        0     7881 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/io.py
+-rw-r--r--   0        0        0    30952 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/models.py
+-rw-r--r--   0        0        0     5414 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/plots.py
+-rw-r--r--   0        0        0      801 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/rcmod.py
+-rw-r--r--   0        0        0     9321 2024-05-08 21:43:22.272657 py_smps-2.1.0a6/smps/utils.py
+-rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 py_smps-2.1.0a6/PKG-INFO
```

### Comparing `py_smps-2.1.0a5/LICENSE` & `py_smps-2.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/README.md` & `py_smps-2.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/pyproject.toml` & `py_smps-2.1.0a6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-smps"
-version = "2.1.0a5"
+version = "2.1.0a6"
 description = "A simple python library to import and visualize data from particle sizing instruments"
 authors = ["David H Hagan <david.hagan@quant-aq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/quant-aq/py-smps"
 homepage = "https://github.com/quant-aq/py-smps"
 documentation = "https://github.com/quant-aq/py-smps"
@@ -15,18 +15,18 @@
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 pandas = ">=1.2"
 scipy = ">1.7"
 setuptools = ">48.0"
 joblib = "^1.3"
 seaborn = ">=0.12"
-matplotlib = ">=3.4,<3.6.1 || >3.6.1"
-numpy = ">1.20,<1.24.0 || >1.24.0"
-statsmodels = ">=0.12.0"
-lock = "^2018.3.25.2110"
+matplotlib = ">=3.4,!=3.6.1"
+numpy = ">1.20,!=1.24.0"
+statsmodels = ">=0.13.0"
+requests = ">=2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0"
 coverage = "^5.2"
 pytest-coverage = "^0.0"
 sphinx = "^4.5"
 toml = "^0.10.1"
@@ -36,12 +36,12 @@
 numpydoc = "^1.2"
 sphinx-issues = "^3.0.1"
 nbsphinx = "^0.9.2"
 sphinx-gallery = "^0.13.0"
 ipykernel = "^6.24.0"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/quant-aq/py-smps/issues"
```

### Comparing `py_smps-2.1.0a5/smps/fit.py` & `py_smps-2.1.0a6/smps/fit.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/smps/io.py` & `py_smps-2.1.0a6/smps/io.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/smps/models.py` & `py_smps-2.1.0a6/smps/models.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/smps/plots.py` & `py_smps-2.1.0a6/smps/plots.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/smps/rcmod.py` & `py_smps-2.1.0a6/smps/rcmod.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/smps/utils.py` & `py_smps-2.1.0a6/smps/utils.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a5/PKG-INFO` & `py_smps-2.1.0a6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: py-smps
-Version: 2.1.0a5
+Version: 2.1.0a6
 Summary: A simple python library to import and visualize data from particle sizing instruments
 Home-page: https://github.com/quant-aq/py-smps
 License: MIT
 Author: David H Hagan
 Author-email: david.hagan@quant-aq.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.3,<2.0)
-Requires-Dist: lock (>=2018.3.25.2110,<2019.0.0.0)
 Requires-Dist: matplotlib (>=3.4,!=3.6.1)
 Requires-Dist: numpy (>1.20,!=1.24.0)
 Requires-Dist: pandas (>=1.2)
+Requires-Dist: requests (>=2.0)
 Requires-Dist: scipy (>1.7)
 Requires-Dist: seaborn (>=0.12)
 Requires-Dist: setuptools (>48.0)
-Requires-Dist: statsmodels (>=0.12.0)
+Requires-Dist: statsmodels (>=0.13.0)
 Project-URL: Bug Tracker, https://github.com/quant-aq/py-smps/issues
 Project-URL: Documentation, https://github.com/quant-aq/py-smps
 Project-URL: Repository, https://github.com/quant-aq/py-smps
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/py-smps.svg)](https://badge.fury.io/py/py-smps)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

