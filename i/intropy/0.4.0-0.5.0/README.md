# Comparing `tmp/intropy-0.4.0.tar.gz` & `tmp/intropy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intropy-0.4.0.tar", last modified: Mon Apr 15 20:53:16 2024, max compression
+gzip compressed data, was "intropy-0.5.0.tar", last modified: Tue May  7 22:25:13 2024, max compression
```

## Comparing `intropy-0.4.0.tar` & `intropy-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.078311 intropy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 20:53:10.000000 intropy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-15 20:53:16.078311 intropy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-15 20:53:10.000000 intropy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.062310 intropy-0.4.0/intropy/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 20:53:10.000000 intropy-0.4.0/intropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-15 20:53:10.000000 intropy-0.4.0/intropy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/intropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 20:53:16.000000 intropy-0.4.0/intropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 20:53:10.000000 intropy-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements-style.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 20:53:10.000000 intropy-0.4.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:53:16.078311 intropy-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:53:16.066311 intropy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-15 20:53:10.000000 intropy-0.4.0/tests/test_generated_project_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 22:25:10.000000 intropy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-07 22:25:13.738426 intropy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-07 22:25:10.000000 intropy-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/intropy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 22:25:10.000000 intropy-0.5.0/intropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-07 22:25:10.000000 intropy-0.5.0/intropy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/intropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-07 22:25:10.000000 intropy-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:25:13.738426 intropy-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_generated_project_test_suite.py
```

### Comparing `intropy-0.4.0/LICENSE` & `intropy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intropy-0.4.0/README.md` & `intropy-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 # Intropy
 
 [![Version](https://img.shields.io/pypi/v/intropy?color=blue)](https://pypi.org/project/intropy/)
 [![Build Status](https://github.com/RicNord/intropy/actions/workflows/ci.yaml/badge.svg)](https://github.com/RicNord/intropy/actions)
 
 Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter),
-intropy is a framework for jump-starting production-ready python projects. The
+intropy is a framework for jump-starting production-grade python projects. The
 python project will be generated and configured automatically with:
 
 - Build system
 - Test and code quality tooling
 - Documentation
 - Automation pipelines
 - etc...
 
 ## Features
 
-- [Ruff](https://docs.astral.sh/ruff/) | Linter and formatter
+- [Ruff](https://docs.astral.sh/ruff/) | Linter and formatter (Optionally
+  strict [Black](https://black.readthedocs.io/en/stable/) as code formatter)
 - [Pytest](https://docs.pytest.org/en/latest/) | Test framework
 - [Tox](https://tox.wiki/en/latest/) | Standardized testing and automation
 - [Coverage](https://coverage.readthedocs.io/en/latest/) | Code coverage
 - [Mypy](https://www.mypy-lang.org/) | Static type checker
-- [Pipenv](https://pipenv.pypa.io/en/latest/) | Package management
+- Package and environment management
+  - Deployable applications: [Pipenv](https://pipenv.pypa.io/en/latest/) |
+    Version pinning and virtual environment setup
+  - Libraries: Pyproject explicit defined dependencies
 - [Pre-commit](https://pre-commit.com/) | pre-commit hooks
 - [Bump my version](https://callowayproject.github.io/bump-my-version/) | Bump
   semantic version
 - [Sphinx](https://www.sphinx-doc.org/) | Documentation tool
-- Github workflows | CI and publishing to PyPi
-- Github templates | Pull Requests and Issues
+- [Logging](https://docs.python.org/3/library/logging.html) boilerplate
+- DevOps platform options
+  - Github
+    - Github workflows | CI and publishing to PyPi
+    - Github templates | Pull Requests and Issues
+  - Azure Devops
+    - Azure pipelines | CI
 - Makefile for convenience
 
-## Optional feature alternatives
-
-- [Black](https://black.readthedocs.io/en/stable/) | Code formatter
-
 ## Usage
 
 Install cookiecutter:
 
 ```shell
 pip install cookiecutter
 ```
@@ -45,15 +50,15 @@
 
 ```shell
 cookiecutter https://github.com/RicNord/intropy
 ```
 
 You will be prompted for some values. After that the project will be generated!
 
-### (Optional) CLI
+### (Optional) Standalone CLI
 
 A wrapper around the `cookiecutter` CLI is also provided and can be installed
 with:
 
 ```shell
 pip install intropy
 ```
```

### Comparing `intropy-0.4.0/intropy/cli.py` & `intropy-0.5.0/intropy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import argparse
 import logging
 from typing import Optional, Sequence
 
 from cookiecutter.main import cookiecutter
 
+from intropy import setup_logging
+
 logger = logging.getLogger(__name__)
 
 
 def main(argv: Optional[Sequence[str]] = None) -> int:
     """Entry point"""
 
-    logger.info("Parse arguments")
+    setup_logging()
+    logger.debug(f"Got {argv=}")
 
     parser = argparse.ArgumentParser(
         description="Generate a new python project",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("template", help="Path to template to generate")
+    parser.add_argument(
+        "template",
+        help="Path to template to generate",
+        nargs="?",
+        default="https://github.com/RicNord/intropy",
+    )
     parser.add_argument(
         "extra_context",
         nargs="*",
         default=[],
         help="Description of extra_context argument",
     )
     parser.add_argument(
```

### Comparing `intropy-0.4.0/pyproject.toml` & `intropy-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 [project]
 name = "intropy"
 description = "Jump-start your python project"
 readme = "README.md"
-dynamic = ["version", "dependencies", "optional-dependencies"]
+dynamic = ["version"]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
+dependencies = ["cookiecutter"]
+
+[project.optional-dependencies]
+dev = [
+    "build",
+    "bump-my-version",
+    "mypy",
+    "pre-commit",
+    "pytest",
+    "pytest-cookies",
+    "pytest-cov",
+    "ruff",
+]
+style = ["ruff"]
+docs = ["myst-parser", "sphinx", "sphinx-autobuild", "sphinx-rtd-theme"]
 
 [project.scripts]
 intropy = "intropy.cli:main"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements/requirements.txt"] }
-optional-dependencies = { dev = { file = [
-    "requirements/requirements-dev.txt",
-] }, docs = { file = [
-    "requirements/requirements-docs.txt",
-] }, style = { file = [
-    "requirements/requirements-style.txt",
-] } }
 version = { attr = "intropy.__version__" }
 
 [tool.setuptools.packages.find]
 include = ["intropy"]
 exclude = ["{{cookiecutter.project_slug}}*", "tests*", "hooks*"]
 
 [tool.pytest.ini_options]
@@ -107,15 +114,15 @@
 
     # Dont complain typing
     "@(typing(_extensions)?\\.)?overload",
     "if (typing(_extensions)?\\.)?TYPE_CHECKING:",
 ]
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.5.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
```

### Comparing `intropy-0.4.0/tests/test_cli.py` & `intropy-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `intropy-0.4.0/tests/test_cookiecutter.py` & `intropy-0.5.0/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `intropy-0.4.0/tests/test_generated_project_test_suite.py` & `intropy-0.5.0/tests/test_generated_project_test_suite.py`

 * *Files identical despite different names*

