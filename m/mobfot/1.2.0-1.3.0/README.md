# Comparing `tmp/mobfot-1.2.0.tar.gz` & `tmp/mobfot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobfot-1.2.0.tar", last modified: Tue Aug 22 02:57:17 2023, max compression
+gzip compressed data, was "mobfot-1.3.0.tar", last modified: Wed May  8 01:22:12 2024, max compression
```

## Comparing `mobfot-1.2.0.tar` & `mobfot-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 02:57:17.542192 mobfot-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-22 02:57:03.000000 mobfot-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-22 02:57:17.542192 mobfot-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-22 02:57:03.000000 mobfot-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 02:57:17.538192 mobfot-1.2.0/mobfot/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-22 02:57:03.000000 mobfot-1.2.0/mobfot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-22 02:57:03.000000 mobfot-1.2.0/mobfot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 02:57:17.542192 mobfot-1.2.0/mobfot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-22 02:57:17.000000 mobfot-1.2.0/mobfot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-22 02:57:17.000000 mobfot-1.2.0/mobfot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-22 02:57:17.000000 mobfot-1.2.0/mobfot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-22 02:57:17.000000 mobfot-1.2.0/mobfot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-22 02:57:17.000000 mobfot-1.2.0/mobfot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-22 02:57:03.000000 mobfot-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-22 02:57:17.542192 mobfot-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 01:22:02.000000 mobfot-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-08 01:22:12.562515 mobfot-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-08 01:22:02.000000 mobfot-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/mobfot/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 01:22:02.000000 mobfot-1.3.0/mobfot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-08 01:22:02.000000 mobfot-1.3.0/mobfot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:12.562515 mobfot-1.3.0/mobfot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 01:22:12.000000 mobfot-1.3.0/mobfot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 01:22:02.000000 mobfot-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:22:12.566515 mobfot-1.3.0/setup.cfg
```

### Comparing `mobfot-1.2.0/LICENSE` & `mobfot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobfot-1.2.0/PKG-INFO` & `mobfot-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.2.0
-Summary: A Python wrapper around the unofficial FotMob API
+Version: 1.3.0
+Summary: An unofficial Python client for the FotMob API
 Author: Brian Greenwood
 License: MIT
-Project-URL: homepage, https://github.com/bgrnwd/mobfot
+Project-URL: homepage, https://bgrnwd.com/mobfot/
 Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: CacheControl>=0.13.1
+Provides-Extra: test
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: behave; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: reformat-gherkin; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: mkdocs; extra == "test"
+Requires-Dist: mkdocstrings[python]; extra == "test"
+Requires-Dist: mkdocs-material; extra == "test"
 
 # mobfot
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
 [![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
-A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
+An unofficial Python client for the [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [Usage](#usage)
+    - [Quick Start](#quick-start)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Install
 
 ```sh
 pip install mobfot
 ```
 
 ## Usage
 
+### Quick Start
+
 ```python
 from mobfot import MobFot
 client = MobFot()
 client.get_matches_by_date("20221205")
 ```
 
 ## Contributing
 
-Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
+- Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
 
 ## License
 
 [MIT](./LICENSE) © Brian Greenwood
```

### Comparing `mobfot-1.2.0/README.md` & `mobfot-1.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
 [![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
-A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
+An unofficial Python client for the [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [Usage](#usage)
+    - [Quick Start](#quick-start)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Install
 
 ```sh
 pip install mobfot
 ```
 
 ## Usage
 
+### Quick Start
+
 ```python
 from mobfot import MobFot
 client = MobFot()
 client.get_matches_by_date("20221205")
 ```
 
 ## Contributing
 
-Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
+- Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
 
 ## License
 
 [MIT](./LICENSE) © Brian Greenwood
```

### Comparing `mobfot-1.2.0/mobfot.egg-info/PKG-INFO` & `mobfot-1.3.0/mobfot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.2.0
-Summary: A Python wrapper around the unofficial FotMob API
+Version: 1.3.0
+Summary: An unofficial Python client for the FotMob API
 Author: Brian Greenwood
 License: MIT
-Project-URL: homepage, https://github.com/bgrnwd/mobfot
+Project-URL: homepage, https://bgrnwd.com/mobfot/
 Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: CacheControl>=0.13.1
+Provides-Extra: test
+Requires-Dist: ruff; extra == "test"
+Requires-Dist: behave; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: reformat-gherkin; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: mkdocs; extra == "test"
+Requires-Dist: mkdocstrings[python]; extra == "test"
+Requires-Dist: mkdocs-material; extra == "test"
 
 # mobfot
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
 [![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
-A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
+An unofficial Python client for the [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [Usage](#usage)
+    - [Quick Start](#quick-start)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Install
 
 ```sh
 pip install mobfot
 ```
 
 ## Usage
 
+### Quick Start
+
 ```python
 from mobfot import MobFot
 client = MobFot()
 client.get_matches_by_date("20221205")
 ```
 
 ## Contributing
 
-Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
+- Feel free to [open an issue](https://github.com/bgrnwd/mobfot/issues/new) or submit a pull request.
 
 ## License
 
 [MIT](./LICENSE) © Brian Greenwood
```

### Comparing `mobfot-1.2.0/pyproject.toml` & `mobfot-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,55 @@
-[tool.black]
-line-length = 88
-
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mobfot"
-description = "A Python wrapper around the unofficial FotMob API"
+description = "An unofficial Python client for the FotMob API"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.7"
-authors = [
-  { name = "Brian Greenwood" },
-]
-keywords = [
-    "fotmob",
-    "soccer",
-    "api",
-    "football"
-]
+authors = [{ name = "Brian Greenwood" }]
+keywords = ["fotmob", "soccer", "api", "football"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dependencies = [
-  "requests==2.31.0",
-  "CacheControl==0.13.1"
-]
+dependencies = ["requests>=2.31.0", "CacheControl>=0.13.1"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
-    "black",
-    "mypy",
-    "isort",
-    "behave",
-    "reformat-gherkin",
-    "types-requests"
+  "ruff",
+  "behave",
+  "mypy",
+  "reformat-gherkin",
+  "types-requests",
+  "mkdocs",
+  "mkdocstrings[python]",
+  "mkdocs-material",
 ]
 
 [project.urls]
-homepage = "https://github.com/bgrnwd/mobfot"
+homepage = "https://bgrnwd.com/mobfot/"
 repository = "https://github.com/bgrnwd/mobfot"
 
-[tool.isort]
-atomic = true
-line_length = 88
-skip_gitignore = true
+[tool.ruff]
+lint.ignore = ["F401"]
 
 [tool.setuptools.dynamic]
-version = {attr = "mobfot.client.VERSION"}
+version = { attr = "mobfot.client.VERSION" }
 
 [[tool.mypy.overrides]]
 module = "cachecontrol.*"
 ignore_missing_imports = true
```

