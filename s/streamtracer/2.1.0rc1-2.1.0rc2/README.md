# Comparing `tmp/streamtracer-2.1.0rc1.tar.gz` & `tmp/streamtracer-2.1.0rc2.tar.gz`

## Comparing `streamtracer-2.1.0rc1.tar` & `streamtracer-2.1.0rc2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc1/Cargo.toml
--rw-r--r--   0     1001      127      291 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.cargo/config.toml
--rw-r--r--   0     1001      127      155 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.codecov.yaml
--rw-r--r--   0     1001      127      276 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.codespellrc
--rw-r--r--   0     1001      127      836 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.coveragerc
--rw-r--r--   0     1001      127     1055 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.cruft.json
--rw-r--r--   0     1001      127      532 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.flake8
--rw-r--r--   0     1001      127      513 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/dependabot.yml
--rw-r--r--   0     1001      127     4437 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      390 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/pre-commit.yml
--rw-r--r--   0     1001      127     2907 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/sub_package_update.yml
--rw-r--r--   0     1001      127     4408 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.gitignore
--rw-r--r--   0     1001      127      422 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.isort.cfg
--rw-r--r--   0     1001      127     1700 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      476 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.readthedocs.yaml
--rw-r--r--   0     1001      127      122 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.rtd-environment.yml
--rw-r--r--   0     1001      127      993 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.ruff.toml
--rwxr-xr-x   0     1001      127    35147 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/LICENSE
--rw-r--r--   0     1001      127      111 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/MANIFEST.in
--rw-r--r--   0     1001      127      854 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/README.md
--rw-r--r--   0     1001      127     6930 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/asv.conf.json
--rw-r--r--   0     1001      127        0 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/__init__.py
--rw-r--r--   0     1001      127     1108 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmark.py
--rw-r--r--   0     1001      127      651 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmark_plot.py
--rw-r--r--   0     1001      127      809 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmarks.py
--rw-r--r--   0     1001      127      448 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/pyinst.py
--rw-r--r--   0     1001      127      634 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/Makefile
--rw-r--r--   0     1001      127     2876 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/conf.py
--rw-r--r--   0     1001      127     4359 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/index.rst
--rw-r--r--   0     1001      127      795 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/make.bat
--rw-r--r--   0     1001      127       99 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/requirements.txt
--rw-r--r--   0     1001      127       57 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/streamtracer.rst
--rw-r--r--   0     1001      127     1304 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/pyproject.toml
--rw-r--r--   0     1001      127      814 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/pytest.ini
--rw-r--r--   0     1001      127       70 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/__init__.py
--rwxr-xr-x   0     1001      127     9891 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/streamline.py
--rw-r--r--   0     1001      127     9551 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/tests/test_streamline.py
--rw-r--r--   0     1001      127      237 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/version.py
--rw-r--r--   0     1001      127     5507 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/field.rs
--rw-r--r--   0     1001      127     1090 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/interp.rs
--rw-r--r--   0     1001      127     1962 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/lib.rs
--rw-r--r--   0     1001      127     2150 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_field.rs
--rw-r--r--   0     1001      127      339 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_interp.rs
--rw-r--r--   0     1001      127     1428 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_tracer.rs
--rw-r--r--   0     1001      127     5393 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/trace.rs
--rw-r--r--   0     1001      127     2332 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/tox.ini
--rw-r--r--   0     1001      127    11905 2024-05-08 12:33:11.000000 streamtracer-2.1.0rc1/Cargo.lock
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc2/Cargo.toml
+-rw-r--r--   0     1001      127      291 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.cargo/config.toml
+-rw-r--r--   0     1001      127      155 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.codecov.yaml
+-rw-r--r--   0     1001      127      276 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.codespellrc
+-rw-r--r--   0     1001      127      836 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.coveragerc
+-rw-r--r--   0     1001      127     1055 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.cruft.json
+-rw-r--r--   0     1001      127      532 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.flake8
+-rw-r--r--   0     1001      127      513 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4437 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      390 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.github/workflows/pre-commit.yml
+-rw-r--r--   0     1001      127     2907 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.github/workflows/sub_package_update.yml
+-rw-r--r--   0     1001      127     4408 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.gitignore
+-rw-r--r--   0     1001      127      422 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.isort.cfg
+-rw-r--r--   0     1001      127     1700 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      476 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.readthedocs.yaml
+-rw-r--r--   0     1001      127      122 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.rtd-environment.yml
+-rw-r--r--   0     1001      127      993 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/.ruff.toml
+-rwxr-xr-x   0     1001      127    35147 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/LICENSE
+-rw-r--r--   0     1001      127      111 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/MANIFEST.in
+-rw-r--r--   0     1001      127      628 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/README.md
+-rw-r--r--   0     1001      127      100 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/RELEASING.md
+-rw-r--r--   0     1001      127     6930 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/asv.conf.json
+-rw-r--r--   0     1001      127        0 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/benchmarks/__init__.py
+-rw-r--r--   0     1001      127     1108 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/benchmarks/benchmark.py
+-rw-r--r--   0     1001      127      651 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/benchmarks/benchmark_plot.py
+-rw-r--r--   0     1001      127      809 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/benchmarks/benchmarks.py
+-rw-r--r--   0     1001      127      448 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/benchmarks/pyinst.py
+-rw-r--r--   0     1001      127      634 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/Makefile
+-rw-r--r--   0     1001      127     2876 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/conf.py
+-rw-r--r--   0     1001      127     4359 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/index.rst
+-rw-r--r--   0     1001      127      795 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/make.bat
+-rw-r--r--   0     1001      127       99 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/requirements.txt
+-rw-r--r--   0     1001      127       57 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/docs/streamtracer.rst
+-rw-r--r--   0     1001      127      814 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/pytest.ini
+-rw-r--r--   0     1001      127       70 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/python/streamtracer/__init__.py
+-rwxr-xr-x   0     1001      127     9891 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/python/streamtracer/streamline.py
+-rw-r--r--   0     1001      127     9551 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/python/streamtracer/tests/test_streamline.py
+-rw-r--r--   0     1001      127      237 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/python/streamtracer/version.py
+-rw-r--r--   0     1001      127     5507 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/field.rs
+-rw-r--r--   0     1001      127     1090 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/interp.rs
+-rw-r--r--   0     1001      127     1962 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/lib.rs
+-rw-r--r--   0     1001      127     2150 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/test_field.rs
+-rw-r--r--   0     1001      127      339 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/test_interp.rs
+-rw-r--r--   0     1001      127     1428 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/test_tracer.rs
+-rw-r--r--   0     1001      127     5393 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/src/trace.rs
+-rw-r--r--   0     1001      127     2332 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/tox.ini
+-rw-r--r--   0     1001      127    11910 2024-05-08 15:33:31.000000 streamtracer-2.1.0rc2/Cargo.lock
+-rw-r--r--   0     1001      127     1796 2024-05-08 15:33:22.000000 streamtracer-2.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc2/PKG-INFO
```

### Comparing `streamtracer-2.1.0rc1/Cargo.toml` & `streamtracer-2.1.0rc2/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 [package]
 name = "streamtracer"
-version = "2.0.1"
+version = "2.1.0-rc.2"
 edition = "2021"
 
-[package.metadata.maturin]
-python-source = "python"
-name = "streamtracer._streamtracer_rust"
-
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "streamtracer"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = {version = "0.21", features = ["extension-module"]}
```

### Comparing `streamtracer-2.1.0rc1/.coveragerc` & `streamtracer-2.1.0rc2/.coveragerc`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.cruft.json` & `streamtracer-2.1.0rc2/.cruft.json`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.flake8` & `streamtracer-2.1.0rc2/.flake8`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.github/dependabot.yml` & `streamtracer-2.1.0rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.github/workflows/ci.yml` & `streamtracer-2.1.0rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.github/workflows/sub_package_update.yml` & `streamtracer-2.1.0rc2/.github/workflows/sub_package_update.yml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.gitignore` & `streamtracer-2.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.pre-commit-config.yaml` & `streamtracer-2.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/.ruff.toml` & `streamtracer-2.1.0rc2/.ruff.toml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/LICENSE` & `streamtracer-2.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/asv.conf.json` & `streamtracer-2.1.0rc2/asv.conf.json`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/benchmarks/benchmark.py` & `streamtracer-2.1.0rc2/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/benchmarks/benchmark_plot.py` & `streamtracer-2.1.0rc2/benchmarks/benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/benchmarks/benchmarks.py` & `streamtracer-2.1.0rc2/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/docs/Makefile` & `streamtracer-2.1.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/docs/conf.py` & `streamtracer-2.1.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/docs/index.rst` & `streamtracer-2.1.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/docs/make.bat` & `streamtracer-2.1.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/pyproject.toml` & `streamtracer-2.1.0rc2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 [build-system]
 requires = [
-    "maturin>=0.13,<0.14",
+    "maturin>=1.0,<2.0",
 ]
 build-backend = "maturin"
 
 [tool.maturin]
 python-source = "python"
+module-name = "streamtracer._streamtracer_rust"
 
 [project]
 name = "streamtracer"
 description = "Python library to calculate streamlines"
-readme = { file = "README.md", content-type = "text/x-markdown" }
+readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.10"
-license = {text = "GPL v3"}
+license = {file = "LICENSE"}
 authors = [
   {name = "The SunPy Developers", email="sunpy@googlegroups.com"},
   {name = "David Stansby"},
   {name = "Lars Mejnertsen"}
 ]
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "Natural Language :: English",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Topic :: Scientific/Engineering :: Physics",
 ]
-version = "2.1.0.rc1"
+version = "2.1.0.rc2"
 dependencies = [
   "numpy>=1.23",
   "packaging>=21.3",
 ]
 
 [project.urls]
-homepage = "https://streamtracer.readthedocs.io/en/stable/"
-documentation = "https://streamtracer.readthedocs.io/en/stable/"
-repository = "https://github.com/sunpy/streamtracer"
+Homepage = "https://docs.sunpy.org/projects/streamtracer"
+Documentation = "https://docs.sunpy.org/projects/streamtracer"
+Repository = "https://github.com/sunpy/streamtracer"
 
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-doctestplus",
   "pytest-cov",
   "pytest-xdist",
```

### Comparing `streamtracer-2.1.0rc1/pytest.ini` & `streamtracer-2.1.0rc2/pytest.ini`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/python/streamtracer/streamline.py` & `streamtracer-2.1.0rc2/python/streamtracer/streamline.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/python/streamtracer/tests/test_streamline.py` & `streamtracer-2.1.0rc2/python/streamtracer/tests/test_streamline.py`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/field.rs` & `streamtracer-2.1.0rc2/src/field.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/interp.rs` & `streamtracer-2.1.0rc2/src/interp.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/lib.rs` & `streamtracer-2.1.0rc2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/test_field.rs` & `streamtracer-2.1.0rc2/src/test_field.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/test_tracer.rs` & `streamtracer-2.1.0rc2/src/test_tracer.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/src/trace.rs` & `streamtracer-2.1.0rc2/src/trace.rs`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/tox.ini` & `streamtracer-2.1.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `streamtracer-2.1.0rc1/Cargo.lock` & `streamtracer-2.1.0rc2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "streamtracer"
-version = "2.0.1"
+version = "2.1.0-rc.2"
 dependencies = [
  "float_eq",
  "ndarray",
  "num-derive",
  "num-traits",
  "numpy",
  "pyo3",
```

