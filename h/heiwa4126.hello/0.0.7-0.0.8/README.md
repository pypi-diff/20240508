# Comparing `tmp/heiwa4126_hello-0.0.7.tar.gz` & `tmp/heiwa4126_hello-0.0.8.tar.gz`

## Comparing `heiwa4126_hello-0.0.7.tar` & `heiwa4126_hello-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/__about__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/__init__.py
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/cli.py
--rwxr-xr-x   0        0        0      582 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/src/heiwa4126/hello/hello.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/LICENSE
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/README.md
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/src/heiwa4126/hello/__about__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/src/heiwa4126/hello/__init__.py
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/src/heiwa4126/hello/cli.py
+-rwxr-xr-x   0        0        0      582 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/src/heiwa4126/hello/hello.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/LICENSE
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/README.md
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 heiwa4126_hello-0.0.8/PKG-INFO
```

### Comparing `heiwa4126_hello-0.0.7/src/heiwa4126/hello/hello.py` & `heiwa4126_hello-0.0.8/src/heiwa4126/hello/hello.py`

 * *Files identical despite different names*

### Comparing `heiwa4126_hello-0.0.7/.gitignore` & `heiwa4126_hello-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `heiwa4126_hello-0.0.7/LICENSE` & `heiwa4126_hello-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `heiwa4126_hello-0.0.7/README.md` & `heiwa4126_hello-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `heiwa4126_hello-0.0.7/pyproject.toml` & `heiwa4126_hello-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 classifiers = [
   # "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  # "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: Implementation :: CPython",
   # "Programming Language :: Python :: Implementation :: PyPy",
   "Programming Language :: Python",
 ]
 
@@ -42,25 +42,55 @@
 Issues = "https://github.com/heiwa4126/pip-heiwa4126-hello/issues"
 
 [tool.hatch.version]
 path = "src/heiwa4126/hello/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  # "coverage[toml]>=6.5",
-  # "pytest",
+  "coverage[toml]>=6.5",
+  "pytest",
   "ruff",
 ]
 
 [tool.hatch.build.targets.sdist]
 include = [ "/src" ]
 
 [tool.hatch.build.targets.wheel]
 packages = [ "src/heiwa4126" ]
 
+
+[tool.hatch.envs.default.scripts]
+# test = "python -m unittest discover tests -p \"test_*.py\""
+ex0 = "python examples/ex0.py"
+ex1 = "python examples/ex1.py"
+cli = "python src/heiwa4126/fizzbuzz2/cli.py 15"
+check = "ruff check ."
+fix = "ruff check . --fix"
+listwhl = "zipinfo dist/*.whl"
+listtarball = "tar ztvf dist/*.tar.gz"
+test = "pytest {args:tests}"
+test-cov = "coverage run -m pytest {args:tests}"
+cov-report = [
+  "- coverage combine",
+  "coverage report",
+]
+cov = [
+  "cov-report",
+  "test-cov",
+]
+
+[[tool.hatch.envs.all.matrix]]
+python = [
+  "3.10",
+  "3.11",
+  "3.12",
+  "3.8",
+  "3.9",
+]
+
 [tool.ruff]
 target-version = "py39"
 line-length = 119
 
 [tool.ruff.lint]
 select = [
   "E",
@@ -72,42 +102,14 @@
 
 [tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
 
 [tool.ruff.lint.isort]
 force-single-line = false
 
-[tool.hatch.envs.default.scripts]
-test = "python -m unittest discover tests -p \"test_*.py\""
-ex0 = "python examples/ex0.py"
-ex1 = "python examples/ex1.py"
-cli = "python src/heiwa4126/fizzbuzz2/cli.py 15"
-check = "ruff check ."
-fix = "ruff check . --fix"
-listwhl = "zipinfo dist/*.whl"
-listtarball = "tar ztvf dist/*.tar.gz"
-# test = "pytest {args:tests}"
-# test-cov = "coverage run -m pytest {args:tests}"
-# cov-report = [
-#   "- coverage combine",
-#   "coverage report",
-# ]
-# cov = [
-#   "cov-report",
-#   "test-cov",
-# ]
-
-[[tool.hatch.envs.all.matrix]]
-python = [
-  "3.10",
-  "3.11",
-  # "3.12",
-  "3.8",
-  "3.9",
-]
 
 # [tool.hatch.envs.types]
 # dependencies = [
 #   "mypy>=1.0.0",
 # ]
 # [tool.hatch.envs.types.scripts]
 # check = "mypy --install-types --non-interactive {args:src/heiwa4126/fizzbuzz2 tests}"
```

### Comparing `heiwa4126_hello-0.0.7/PKG-INFO` & `heiwa4126_hello-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: heiwa4126.hello
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple hello function.
 Project-URL: Repository, https://github.com/heiwa4126/pip-heiwa4126-hello.git
 Project-URL: Homepage, https://github.com/heiwa4126/pip-heiwa4126-hello#readme
 Project-URL: Issues, https://github.com/heiwa4126/pip-heiwa4126-hello/issues
 Author-email: heiwa4126 <heiwa4126@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # heiwa4126.hello (pip-heiwa4126-hello)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/heiwa4126-hello.svg)](https://pypi.org/project/heiwa4126-hello)
```

