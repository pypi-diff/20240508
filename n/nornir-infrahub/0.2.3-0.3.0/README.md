# Comparing `tmp/nornir_infrahub-0.2.3.tar.gz` & `tmp/nornir_infrahub-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_infrahub-0.2.3.tar", max compression
+gzip compressed data, was "nornir_infrahub-0.3.0.tar", max compression
```

## Comparing `nornir_infrahub-0.2.3.tar` & `nornir_infrahub-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      738 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/nornir_infrahub/__init__.py
--rw-r--r--   0        0        0     8816 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/nornir_infrahub/plugins/inventory/infrahub.py
--rw-r--r--   0        0        0      174 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/nornir_infrahub/plugins/tasks/__init__.py
--rw-r--r--   0        0        0     2046 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/nornir_infrahub/plugins/tasks/artifact.py
--rw-r--r--   0        0        0     2169 2023-12-28 13:20:32.142902 nornir_infrahub-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 nornir_infrahub-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      738 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/__init__.py
+-rw-r--r--   0        0        0     8816 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/inventory/infrahub.py
+-rw-r--r--   0        0        0      174 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/artifact.py
+-rw-r--r--   0        0        0     2231 2024-05-08 08:41:15.898480 nornir_infrahub-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 nornir_infrahub-0.3.0/PKG-INFO
```

### Comparing `nornir_infrahub-0.2.3/README.md` & `nornir_infrahub-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nornir_infrahub-0.2.3/nornir_infrahub/plugins/inventory/infrahub.py` & `nornir_infrahub-0.3.0/nornir_infrahub/plugins/inventory/infrahub.py`

 * *Files identical despite different names*

### Comparing `nornir_infrahub-0.2.3/nornir_infrahub/plugins/tasks/artifact.py` & `nornir_infrahub-0.3.0/nornir_infrahub/plugins/tasks/artifact.py`

 * *Files identical despite different names*

### Comparing `nornir_infrahub-0.2.3/pyproject.toml` & `nornir_infrahub-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 [tool.poetry]
 name = "nornir-infrahub"
-version = "0.2.3"
+version = "0.3.0"
 description = "Nornir plugin for Infrahub"
 authors = ["OpsMill <info@opsmill.com>"]
 readme = "README.md"
 packages = [{include = "nornir_infrahub"}]
 license = "Apache-2.0"
 homepage = "https://opsmill.io"
 repository = "https://opsmill.io"
 documentation = "https://opsmill.io"
 
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.plugins."nornir.plugins.inventory"]
 "InfrahubInventory" = "nornir_infrahub.plugins.inventory.infrahub:InfrahubInventory"
 
 [tool.poetry.dependencies]
-python = "^3.8, <3.12"
-infrahub-sdk = "^0,>=0.2"
+python = "^3.9, <3.13"
+infrahub-sdk = {version = "^0,>=0.9.1", extras=["tests"]}
 ruamel-yaml = "^0.18.5"
 nornir = "^3.4.1"
 nornir-utils = "^0.2.0"
 python-slugify = "^8.0.1"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
-ruff = "^0.1"
-mypy = "^1.6"
-pytest-asyncio = "*"
+ruff = "0.3.3"
+mypy = "*"
+pytest-asyncio = "^0.21.1"
 types-python-slugify = "*"
-invoke = "^2.2.0"
-yamllint = "^1.32.0"
+invoke = "2.2.0"
+yamllint = "*"
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
     "if TYPE_CHECKING:",
@@ -62,15 +62,17 @@
 
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 
 [tool.ruff]
+line-length = 120
 
+[tool.ruff.lint]
 select = [
     "C90",      # mccabe
     "ASYNC",    # flake8-async
     "DTZ",      # flake8-datetimez
     "E",        # style errors
     "F",        # flakes
     "I",        # isort
@@ -79,21 +81,20 @@
     "T10",      # flake8-debugger
     "PL",       # pylint
     "Q",        # flake8-quotes
     "W",        # pycodestyle
     "YTT",      # flake8-2020
 ]
 
-line-length = 120
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-third-party = ["nornir_infrahub"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nornir_infrahub-0.2.3/PKG-INFO` & `nornir_infrahub-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nornir-infrahub
-Version: 0.2.3
+Version: 0.3.0
 Summary: Nornir plugin for Infrahub
 Home-page: https://opsmill.io
 License: Apache-2.0
 Author: OpsMill
 Author-email: info@opsmill.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: infrahub-sdk (>=0.2,<1)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: infrahub-sdk[tests] (>=0.9.1,<1)
 Requires-Dist: nornir (>=3.4.1,<4.0.0)
 Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
 Requires-Dist: pydantic (>=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.5,<0.19.0)
 Project-URL: Documentation, https://opsmill.io
 Project-URL: Repository, https://opsmill.io
```

