# Comparing `tmp/radioplayer_dataclasses-0.5.9.tar.gz` & `tmp/radioplayer_dataclasses-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.5.9.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.6.0.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.5.9.tar` & `radioplayer_dataclasses-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34520 2024-03-10 12:07:15.519234 radioplayer_dataclasses-0.5.9/LICENSE
--rw-r--r--   0        0        0     3627 2024-03-10 12:07:15.519234 radioplayer_dataclasses-0.5.9/README.md
--rw-r--r--   0        0        0     2160 2024-03-10 12:07:32.638979 radioplayer_dataclasses-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     2443 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    58103 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-05-08 05:27:35.863344 radioplayer_dataclasses-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3627 2024-05-08 05:27:35.863344 radioplayer_dataclasses-0.6.0/README.md
+-rw-r--r--   0        0        0     1727 2024-05-08 05:28:02.479594 radioplayer_dataclasses-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2443 2024-05-08 05:27:35.863344 radioplayer_dataclasses-0.6.0/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    58103 2024-05-08 05:27:35.863344 radioplayer_dataclasses-0.6.0/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2024-05-08 05:27:35.863344 radioplayer_dataclasses-0.6.0/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.6.0/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.5.9/LICENSE` & `radioplayer_dataclasses-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.9/README.md` & `radioplayer_dataclasses-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.9/pyproject.toml` & `radioplayer_dataclasses-0.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.5.9" # 0.0.0 placeholder is replaced on release
+version = "v0.6.0" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -18,57 +18,41 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 xsdata = ">=22.12,<25.0"
 
 [tool.poetry.group.dev.dependencies]
-black = ">=22.12,<25.0"
-flake8 = ">=6,<8"
-flake8-docstrings = "^1.6.0"
-flake8-isort = ">=5.0.3,<7.0.0"
-flake8-string-format = "^0.3.0"
-flake8-tuple = "^0.4.1"
 lxml = ">=4.9.2,<6.0.0"
-pytest = ">=7.2,<9.0"
-pytest-cov = "^4.0.0"
-pytest-pylint = ">=0.19,<0.22"
-wheel = ">=0.38.4,<0.43.0"
-xmldiff = "^2.4"
-xsdata = {extras = ["cli"], version = ">=22.12,<25.0"}
-pytest-random-order = "^1.1.0"
-pytest-mypy = "^0.10.3"
-mkdocstrings = {extras = ["python"], version = ">=0.20,<0.25"}
-mkdocs-material = ">=8,<10"
+lxml-stubs = "^0.5.1"
 mkdocs = "^1.4.2"
+mkdocs-material = ">=8,<10"
 mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.26"}
+pytest = ">=7.2,<9.0"
+pytest-cov = ">=4,<6"
+pytest-mypy = "^0.10.3"
+pytest-random-order = "^1.1.0"
+wheel = ">=0.38.4,<0.44.0"
+xmldiff = "^2.4"
+xsdata = {extras = ["cli"], version = ">=22.12,<25.0"}
+pytest-ruff = "^0.3.1"
 
-[tool.isort]
-line_length = 120
-profile = "black"
-
-[tool.pylint.format]
-max-line-lenth = 120
-
-[tool.pylint.main]
-extension-pkg-allow-list = ["lxml"]
-ignore-paths = ["radioplayer/dataclasses/dataclasses.py"]
-
-[tool.pylint.messages_control]
-# C0114 = missing-module-docstring
-# C0116 = missing-function-docstring
-disable = ["C0114","C0116"]
+[tool.ruff]
+extend-exclude = [
+	"radioplayer/dataclasses",
+]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
-addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=radioplayer.dataclasses --cov-fail-under=100 --pylint --mypy --ignore=docs/"
+addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=radioplayer.dataclasses --cov-fail-under=100 --ruff --mypy --ignore=docs/"
 filterwarnings = [
-    "ignore::DeprecationWarning:pytest_pylint",
-    "ignore::DeprecationWarning:pylint",
+    "ignore::DeprecationWarning:mypy",
     "ignore::DeprecationWarning:pkg_resources",
+    "ignore::DeprecationWarning:xsdata",
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.6.0/radioplayer/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.6.0/radioplayer/dataclasses/dataclasses.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.9/PKG-INFO` & `radioplayer_dataclasses-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioplayer-dataclasses
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python dataclasses for radioplayer generated from XSD
 Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

