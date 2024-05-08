# Comparing `tmp/streamtracer-2.0.1.tar.gz` & `tmp/streamtracer-2.1.0rc1.tar.gz`

## Comparing `streamtracer-2.0.1.tar` & `streamtracer-2.1.0rc1.tar`

### file list

```diff
@@ -1,37 +1,48 @@
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 streamtracer-2.0.1/Cargo.toml
--rw-r--r--   0      501       20      291 2022-10-10 20:18:12.000000 streamtracer-2.0.1/.cargo/config.toml
--rw-r--r--   0      501       20      144 2022-10-10 17:18:27.000000 streamtracer-2.0.1/.github/FUNDING.yml
--rw-r--r--   0      501       20      513 2023-03-16 10:05:26.000000 streamtracer-2.0.1/.github/dependabot.yml
--rw-r--r--   0      501       20     1172 2023-03-16 10:05:26.000000 streamtracer-2.0.1/.github/workflows/python-test.yml
--rw-r--r--   0      501       20     1297 2023-03-16 10:05:26.000000 streamtracer-2.0.1/.github/workflows/wheels.yml
--rw-r--r--   0      501       20      165 2022-10-10 20:18:12.000000 streamtracer-2.0.1/.gitignore
--rw-r--r--   0      501       20      718 2023-03-16 10:05:26.000000 streamtracer-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0      501       20      110 2022-03-01 09:33:30.000000 streamtracer-2.0.1/.readthedocs.yml
--rwxr-xr-x   0      501       20    35147 2022-03-01 09:33:30.000000 streamtracer-2.0.1/LICENSE
--rw-r--r--   0      501       20      854 2022-10-10 17:18:27.000000 streamtracer-2.0.1/README.md
--rw-r--r--   0      501       20     6930 2022-10-10 17:18:27.000000 streamtracer-2.0.1/asv.conf.json
--rw-r--r--   0      501       20        1 2022-03-01 09:33:30.000000 streamtracer-2.0.1/benchmarks/__init__.py
--rw-r--r--   0      501       20      868 2023-03-16 10:05:26.000000 streamtracer-2.0.1/benchmarks/benchmark.py
--rw-r--r--   0      501       20      479 2023-03-16 08:59:15.000000 streamtracer-2.0.1/benchmarks/benchmark_plot.py
--rw-r--r--   0      501       20      808 2023-03-16 09:43:12.000000 streamtracer-2.0.1/benchmarks/benchmarks.py
--rw-r--r--   0      501       20      447 2023-03-16 10:05:26.000000 streamtracer-2.0.1/benchmarks/pyinst.py
--rw-r--r--   0      501       20       28 2022-03-01 09:33:30.000000 streamtracer-2.0.1/codecov.yml
--rw-r--r--   0      501       20      634 2022-03-01 09:33:30.000000 streamtracer-2.0.1/doc/Makefile
--rw-r--r--   0      501       20     2203 2022-10-10 17:18:27.000000 streamtracer-2.0.1/doc/conf.py
--rw-r--r--   0      501       20     4347 2023-03-16 10:05:26.000000 streamtracer-2.0.1/doc/index.rst
--rw-r--r--   0      501       20      795 2022-03-01 09:33:30.000000 streamtracer-2.0.1/doc/make.bat
--rw-r--r--   0      501       20       99 2022-03-01 09:33:30.000000 streamtracer-2.0.1/doc/requirements.txt
--rw-r--r--   0      501       20       57 2022-03-01 09:33:30.000000 streamtracer-2.0.1/doc/streamtracer.rst
--rw-r--r--   0      501       20     1093 2023-03-16 10:05:26.000000 streamtracer-2.0.1/pyproject.toml
--rw-r--r--   0      501       20       26 2022-10-26 19:32:21.000000 streamtracer-2.0.1/python/streamtracer/__init__.py
--rwxr-xr-x   0      501       20     9890 2023-03-16 09:43:12.000000 streamtracer-2.0.1/python/streamtracer/streamline.py
--rw-r--r--   0      501       20     9542 2023-03-16 09:43:12.000000 streamtracer-2.0.1/python/streamtracer/tests/test_streamline.py
--rw-r--r--   0      501       20     5548 2022-10-10 20:18:12.000000 streamtracer-2.0.1/src/field.rs
--rw-r--r--   0      501       20     1098 2022-10-10 20:18:12.000000 streamtracer-2.0.1/src/interp.rs
--rw-r--r--   0      501       20     1728 2022-11-02 20:00:25.000000 streamtracer-2.0.1/src/lib.rs
--rw-r--r--   0      501       20     2006 2022-10-10 20:18:12.000000 streamtracer-2.0.1/src/test_field.rs
--rw-r--r--   0      501       20      366 2022-10-10 20:18:12.000000 streamtracer-2.0.1/src/test_interp.rs
--rw-r--r--   0      501       20     1395 2022-10-27 11:05:36.000000 streamtracer-2.0.1/src/test_tracer.rs
--rw-r--r--   0      501       20     4965 2023-03-16 10:05:26.000000 streamtracer-2.0.1/src/trace.rs
--rw-r--r--   0      501       20     9349 2023-03-16 10:05:26.000000 streamtracer-2.0.1/Cargo.lock
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 streamtracer-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc1/Cargo.toml
+-rw-r--r--   0     1001      127      291 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.cargo/config.toml
+-rw-r--r--   0     1001      127      155 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.codecov.yaml
+-rw-r--r--   0     1001      127      276 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.codespellrc
+-rw-r--r--   0     1001      127      836 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.coveragerc
+-rw-r--r--   0     1001      127     1055 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.cruft.json
+-rw-r--r--   0     1001      127      532 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.flake8
+-rw-r--r--   0     1001      127      513 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4437 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      390 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/pre-commit.yml
+-rw-r--r--   0     1001      127     2907 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.github/workflows/sub_package_update.yml
+-rw-r--r--   0     1001      127     4408 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.gitignore
+-rw-r--r--   0     1001      127      422 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.isort.cfg
+-rw-r--r--   0     1001      127     1700 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      476 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.readthedocs.yaml
+-rw-r--r--   0     1001      127      122 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.rtd-environment.yml
+-rw-r--r--   0     1001      127      993 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/.ruff.toml
+-rwxr-xr-x   0     1001      127    35147 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/LICENSE
+-rw-r--r--   0     1001      127      111 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/MANIFEST.in
+-rw-r--r--   0     1001      127      854 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/README.md
+-rw-r--r--   0     1001      127     6930 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/asv.conf.json
+-rw-r--r--   0     1001      127        0 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/__init__.py
+-rw-r--r--   0     1001      127     1108 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmark.py
+-rw-r--r--   0     1001      127      651 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmark_plot.py
+-rw-r--r--   0     1001      127      809 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/benchmarks.py
+-rw-r--r--   0     1001      127      448 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/benchmarks/pyinst.py
+-rw-r--r--   0     1001      127      634 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/Makefile
+-rw-r--r--   0     1001      127     2876 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/conf.py
+-rw-r--r--   0     1001      127     4359 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/index.rst
+-rw-r--r--   0     1001      127      795 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/make.bat
+-rw-r--r--   0     1001      127       99 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/requirements.txt
+-rw-r--r--   0     1001      127       57 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/docs/streamtracer.rst
+-rw-r--r--   0     1001      127     1304 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/pyproject.toml
+-rw-r--r--   0     1001      127      814 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/pytest.ini
+-rw-r--r--   0     1001      127       70 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/__init__.py
+-rwxr-xr-x   0     1001      127     9891 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/streamline.py
+-rw-r--r--   0     1001      127     9551 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/tests/test_streamline.py
+-rw-r--r--   0     1001      127      237 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/python/streamtracer/version.py
+-rw-r--r--   0     1001      127     5507 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/field.rs
+-rw-r--r--   0     1001      127     1090 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/interp.rs
+-rw-r--r--   0     1001      127     1962 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/lib.rs
+-rw-r--r--   0     1001      127     2150 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_field.rs
+-rw-r--r--   0     1001      127      339 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_interp.rs
+-rw-r--r--   0     1001      127     1428 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/test_tracer.rs
+-rw-r--r--   0     1001      127     5393 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/src/trace.rs
+-rw-r--r--   0     1001      127     2332 2024-05-08 12:32:46.000000 streamtracer-2.1.0rc1/tox.ini
+-rw-r--r--   0     1001      127    11905 2024-05-08 12:33:11.000000 streamtracer-2.1.0rc1/Cargo.lock
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 streamtracer-2.1.0rc1/PKG-INFO
```

### Comparing `streamtracer-2.0.1/.github/dependabot.yml` & `streamtracer-2.1.0rc1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/LICENSE` & `streamtracer-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/README.md` & `streamtracer-2.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/asv.conf.json` & `streamtracer-2.1.0rc1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/benchmarks/benchmark.py` & `streamtracer-2.1.0rc1/benchmarks/benchmark.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 import time
+import importlib.metadata
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+
 from streamtracer import StreamTracer, VectorGrid
 
+# Support old 1.x versions
+__version__ = importlib.metadata.version("streamtracer")
+
 nsteps = 1000
 step_size = 0.1
 tracer = StreamTracer(nsteps, step_size)
 
 field = np.random.rand(*(180, 360, 50, 3))
 grid_spacing = [1, 2, 3]
 grid = VectorGrid(field, grid_spacing)
 
 seedlist = 2 ** np.arange(12)
 times = []
 for nseeds in seedlist:
-    t = time.time()
-    # Trace from middle of field
-    seeds = np.repeat([[90, 180, 25]], nseeds, axis=0)
-    tracer.trace(seeds, grid)
-    dt = time.time() - t
-    assert len(tracer.xs) == nseeds
-    times += [dt]
-    print(nseeds, dt / nseeds)
+    dts = []
+    for _ in range(5):
+        # Trace from middle of field
+        seeds = np.repeat([[90, 180, 25]], nseeds, axis=0)
+        t = time.time()
+        tracer.trace(seeds, grid)
+        dts.append(time.time() - t)
+        assert len(tracer.xs) == nseeds
+    times += [np.mean(dts)]
+    print(nseeds, times[-1] / nseeds, times[-1])
 
 
-pd.DataFrame({"nseeds": seedlist, "time": times}).to_csv("v200.csv")
-
-import matplotlib.pyplot as plt
+pd.DataFrame({"nseeds": seedlist, "time": times}).to_csv(
+    f"v{__version__.replace('.', '')}.csv"
+)
 
 fig, ax = plt.subplots()
 
 ax.plot(seedlist, times, marker=".")
 ax.set_xlabel("n seeds")
 ax.set_ylabel("time (s)")
 ax.set_xscale("log")
```

### Comparing `streamtracer-2.0.1/benchmarks/benchmarks.py` & `streamtracer-2.1.0rc1/benchmarks/benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Write the benchmarking functions here.
 # See "Writing benchmarks" in the asv docs for more information.
 import numpy as np
+
 from streamtracer import StreamTracer, VectorGrid
 
 
 class TimeSuite:
     def setup(self):
         self.tracer = StreamTracer(1000, 0.1)
         # A uniform field pointing in the x direction
```

### Comparing `streamtracer-2.0.1/doc/Makefile` & `streamtracer-2.1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/doc/conf.py` & `streamtracer-2.1.0rc1/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
-import sys
-import unittest.mock
-
-modules = ["streamtracer.fortran", "streamtracer.fortran.streamtracer"]
-for module in modules:
-    sys.modules[module] = unittest.mock.MagicMock()
+import datetime
 
 # -- Project information -----------------------------------------------------
 
+# The full version, including alpha/beta/rc tags
+from streamtracer import __version__
+
+release = __version__
+
 project = "streamtracer"
-copyright = "2019-2021, David Stansby"
-author = "David Stansby"
+author = "The SunPy Developers, David Stansby"
+copyright = f"{datetime.datetime.now().year}, {author}"  # noqa: A001
 
 # Home page
 master_doc = "index"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx_automodapi.automodapi",
-    "numpydoc",
+    "sphinx.ext.napoleon",
     "jupyter_sphinx",
 ]
-numpydoc_show_class_members = False
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+# templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+source_suffix = ".rst"
+
+# The master toctree document.
+master_doc = "index"
+
+# Treat everything in single ` as a Python reference.
+default_role = "py:obj"
+
+# -- Options for intersphinx extension ---------------------------------------
+
+# Example configuration for intersphinx: refer to the Python standard library.
+intersphinx_mapping = {"python": ("https://docs.python.org/", None)}
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "pydata_sphinx_theme"
+html_theme = "sunpy"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-# html_static_path = ['_static']
+# html_static_path = ["_static"]
+
+# By default, when rendering docstrings for classes, sphinx.ext.autodoc will
+# make docs with the class-level docstring and the class-method docstrings,
+# but not the __init__ docstring, which often contains the parameters to
+# class constructors across the scientific Python ecosystem. The option below
+# will append the __init__ docstring to the class-level docstring when rendering
+# the docs. For more options, see:
+# https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autoclass_content
+autoclass_content = "both"
+
+# -- Other options ----------------------------------------------------------
```

### Comparing `streamtracer-2.0.1/doc/index.rst` & `streamtracer-2.1.0rc1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+************
 streamtracer
-============
+************
 
 streamtracer is a python package for rapid streamline tracing on regularly spaced grids.
 The actual streamline tracing is done at a low level in Rust, with a nice Python API provided on top.
 
 To use, create a :class:`streamtracer.StreamTracer` object
 
 .. jupyter-execute::
@@ -69,15 +70,15 @@
    streamtracer
 
 Changelog
 =========
 
 2.0.1
 -----
-streamtracer now includes wheels for Python 3.11, and these have now been uploaded to PyPI as a realease (version 2.0.0 was only ever uploaded as an alpha).
+streamtracer now includes wheels for Python 3.11, and these have now been uploaded to PyPI as a release (version 2.0.0 was only ever uploaded as an alpha).
 streamtracer still does not work in parallel, if you require parallel stream tracing then for now either:
 
 - Downgrade to version 1.2.0
 - Manually run several instances of the streamtracer in parallel
 
 2.0.0
 -----
```

### Comparing `streamtracer-2.0.1/doc/make.bat` & `streamtracer-2.1.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `streamtracer-2.0.1/pyproject.toml` & `streamtracer-2.1.0rc1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 [build-system]
 requires = [
-    "setuptools>=45",
-    "setuptools_scm[toml]>=6.2",
-    "oldest-supported-numpy",
-    "maturin>=0.13,<0.14"
+    "maturin>=0.13,<0.14",
 ]
 build-backend = "maturin"
 
 [tool.maturin]
 python-source = "python"
 
-[tool.setuptools_scm]
-
 [project]
 name = "streamtracer"
-version = "2.0.1"
-description = "Python wrapped fortran to calculate streamlines"
+description = "Python library to calculate streamlines"
+readme = { file = "README.md", content-type = "text/x-markdown" }
+requires-python = ">=3.10"
+license = {text = "GPL v3"}
 authors = [
-    {name = "David Stansby", email="dstansby@gmail.com"},
-    {name = "Lars Mejnertsen"}
+  {name = "The SunPy Developers", email="sunpy@googlegroups.com"},
+  {name = "David Stansby"},
+  {name = "Lars Mejnertsen"}
 ]
-readme = "README.md"
-requires-python = ">=3.7"
-license = {text = "GPL v3"}
 classifiers = [
-    "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3",
+]
+version = "2.1.0.rc1"
+dependencies = [
+  "numpy>=1.23",
+  "packaging>=21.3",
 ]
-dependencies = ["numpy>=1.14.5",]
 
 [project.urls]
 homepage = "https://streamtracer.readthedocs.io/en/stable/"
 documentation = "https://streamtracer.readthedocs.io/en/stable/"
-repository = "https://github.com/dstansby/streamtracer"
+repository = "https://github.com/sunpy/streamtracer"
 
 [project.optional-dependencies]
-tests = ["pytest", "pytest-cov"]
+tests = [
+  "pytest",
+  "pytest-doctestplus",
+  "pytest-cov",
+  "pytest-xdist",
+]
 docs = [
-    "jupyter-sphinx",
-    "numpydoc",
-    "pydata-sphinx-theme",
-    "sphinx",
-    "sphinx-automodapi",
-    "sphinx_rtd_theme"
+  "sphinx",
+  "sphinx-automodapi",
+  "jupyter-sphinx",
+  "sunpy-sphinx-theme",
 ]
 
-[tool.pytest.ini_options]
-addopts = "-ra"
-testpaths = ["doc", "python"]
+[tool.cibuildwheel]
+before-build = "rustup show"
+environment = {"PATH" = "$PATH:$HOME/.cargo/bin"}
+
+[tool.cibuildwheel.linux]
+before-all = "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y"
+
+[tool.cibuildwheel.macos]
+before-all = "rustup target add aarch64-apple-darwin"
```

### Comparing `streamtracer-2.0.1/python/streamtracer/streamline.py` & `streamtracer-2.1.0rc1/python/streamtracer/streamline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 from streamtracer._streamtracer_rust import trace_streamlines
 
 __all__ = ["StreamTracer", "VectorGrid"]
 
 
 class VectorGrid:
     """
```

### Comparing `streamtracer-2.0.1/python/streamtracer/tests/test_streamline.py` & `streamtracer-2.1.0rc1/python/streamtracer/tests/test_streamline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pytest
+
 from streamtracer import StreamTracer, VectorGrid
 
 
 @pytest.fixture
 def tracer():
     return StreamTracer(2000, 0.1)
 
@@ -15,15 +16,15 @@
     # Make all vectors point in the x-direction
     v[:, :, :, 0] = 1
     spacing = [1, 1, 1]
     return VectorGrid(v, spacing)
 
 
 @pytest.mark.parametrize(
-    "direction, ROTs",
+    ("direction", "ROTs"),
     [
         [1, np.array([2, 2, 2])],
         [-1, np.array([2, 2, 2])],
         [0, np.array([[2, 2], [2, 2], [2, 2]])],
     ],
 )
 def test_rot(tracer, uniform_x_field, direction, ROTs):
@@ -199,15 +200,15 @@
         VectorGrid(np.zeros((1, 1, 1, 2)), [1, 1, 1])
 
     with pytest.raises(ValueError, match="grid spacing must have shape"):
         VectorGrid(np.zeros((1, 1, 1, 3)), [1, 1])
 
 
 @pytest.mark.parametrize(
-    "val, errstr",
+    ("val", "errstr"),
     [
         (0.1, "max_steps must be an integer"),
         (0, "max_steps must be greater than zero"),
         (-1, "max_steps must be greater than zero"),
     ],
 )
 def test_invalid_max_steps(val, errstr):
```

### Comparing `streamtracer-2.0.1/src/field.rs` & `streamtracer-2.1.0rc1/src/field.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 //! Structure for representing a 3D vector field defined on the corners
 //! of a rectilinear grid.
-use numpy::ndarray::{array, Array1, ArrayView1, ArrayView4, s};
+use numpy::ndarray::{array, s, Array1, ArrayView1, ArrayView4};
 
 use crate::interp::interp_trilinear;
 
 /// Enum denoting whether a point is in or out of the bounds
 /// of a VectorField grid.
 pub enum Bounds {
     /// A position vector is in bounds.
     In,
     /// A position vector is out of bounds.
-    Out
+    Out,
 }
 
 /// A 3D vector field defined at grid corners.
 pub struct VectorField<'a> {
     /// Grid points along x dimension. Must start at 0.
     pub xgrid: ArrayView1<'a, f64>,
     /// Grid points along y dimension. Must start at 0.
@@ -32,25 +32,25 @@
     nx: usize,
     /// Number of y coordinates.
     ny: usize,
     /// Number of z coordinates.
     nz: usize,
 
     /// Upper boundaries
-    upper_bounds: Array1<f64>
+    upper_bounds: Array1<f64>,
 }
 
 impl VectorField<'_> {
     /// Create a new VectorField, checking for appropriate array shapes.
     pub fn new<'a>(
         xgrid: ArrayView1<'a, f64>,
         ygrid: ArrayView1<'a, f64>,
         zgrid: ArrayView1<'a, f64>,
         values: ArrayView4<'a, f64>,
-        cyclic: ArrayView1<'a, bool>
+        cyclic: ArrayView1<'a, bool>,
     ) -> VectorField<'a> {
         // Do some shape checking
         let nx = xgrid.len();
         let ny = ygrid.len();
         let nz = zgrid.len();
         let field_shape = values.shape();
 
@@ -62,125 +62,115 @@
         assert_eq!(cyclic.shape()[0], 3);
 
         // Check first coordinates are zero.
         assert_eq!(xgrid[0], 0.);
         assert_eq!(ygrid[0], 0.);
         assert_eq!(zgrid[0], 0.);
 
-        let upper_bounds = array![
-            xgrid[nx - 1],
-            ygrid[ny - 1],
-            zgrid[nz - 1]
-        ];
+        let upper_bounds = array![xgrid[nx - 1], ygrid[ny - 1], zgrid[nz - 1]];
 
-        VectorField{xgrid, ygrid, zgrid, values, cyclic, nx, ny, nz, upper_bounds}
+        return VectorField {
+            xgrid,
+            ygrid,
+            zgrid,
+            values,
+            cyclic,
+            nx,
+            ny,
+            nz,
+            upper_bounds,
+        };
     }
 
     /// Return grid index of the cell containing `x`.
-    pub fn grid_idx(
-        &self,
-        x: ArrayView1<f64>
-    ) -> Array1<usize>{
-
+    pub fn grid_idx(&self, x: ArrayView1<f64>) -> Array1<usize> {
         // Output array
-        let mut grid_idx = array![self.nx-2, self.ny-2, self.nz-2];
+        let mut grid_idx = array![self.nx - 2, self.ny - 2, self.nz - 2];
 
         // x
-        for i in 0..self.nx-1{
-            if x[0] >= self.xgrid[[i]] && x[0] < self.xgrid[[i+1]]{
+        for i in 0..self.nx - 1 {
+            if x[0] >= self.xgrid[[i]] && x[0] < self.xgrid[[i + 1]] {
                 grid_idx[0] = i;
                 break;
             }
         }
         // y
-        for i in 0..self.ny-1{
-            if x[1] >= self.ygrid[[i]] && x[1] < self.ygrid[[i+1]]{
+        for i in 0..self.ny - 1 {
+            if x[1] >= self.ygrid[[i]] && x[1] < self.ygrid[[i + 1]] {
                 grid_idx[1] = i;
                 break;
             }
         }
         // z
-        for i in 0..self.nz-1{
-            if x[2] >= self.zgrid[[i]] && x[2] < self.zgrid[[i+1]]{
+        for i in 0..self.nz - 1 {
+            if x[2] >= self.zgrid[[i]] && x[2] < self.zgrid[[i + 1]] {
                 grid_idx[2] = i;
                 break;
             }
         }
 
-        return grid_idx
+        return grid_idx;
     }
 
     /// Get vector at position `x` using tri-linear interpolation.
-    pub fn vector_at_position(
-        &self,
-        x0: ArrayView1<f64>
-    ) -> Array1<f64>{
+    pub fn vector_at_position(&self, x0: ArrayView1<f64>) -> Array1<f64> {
         let cell_idx = self.grid_idx(x0);
         let cell_origin = array![
             self.xgrid[cell_idx[0]],
             self.ygrid[cell_idx[1]],
             self.zgrid[cell_idx[2]]
         ];
         let cell_size = array![
-            self.xgrid[cell_idx[0]+1] - cell_origin[0],
-            self.ygrid[cell_idx[1]+1] - cell_origin[1],
-            self.zgrid[cell_idx[2]+1] - cell_origin[2]
+            self.xgrid[cell_idx[0] + 1] - cell_origin[0],
+            self.ygrid[cell_idx[1] + 1] - cell_origin[1],
+            self.zgrid[cell_idx[2] + 1] - cell_origin[2]
         ];
 
         // Distance along each cell edge in normalised units
         let cell_dist: Array1<f64> = (x0.to_owned() - cell_origin) / cell_size;
 
         // Eight corners of the cube that the position vector is
         // currently in
         let vec_cube = self.values.slice(s![
             cell_idx[0]..(cell_idx[0] + 2),
             cell_idx[1]..(cell_idx[1] + 2),
             cell_idx[2]..(cell_idx[2] + 2),
             ..
         ]);
 
-
         let mut vector_at_pos = array![0., 0., 0.];
         // Loop over vector components
-        for i in 0..3{
-            vector_at_pos[[i]] = interp_trilinear(
-                &vec_cube.slice(s![.., .., .., i]),
-                &cell_dist);
+        for i in 0..3 {
+            vector_at_pos[[i]] = interp_trilinear(&vec_cube.slice(s![.., .., .., i]), &cell_dist);
         }
         return vector_at_pos;
     }
 
     /// If any of the dimensions of the grid are cyclic, wrap a coordinate.
-    pub fn wrap_cyclic(
-        &self,
-        mut x: Array1<f64>
-    ) -> Array1<f64> {
+    pub fn wrap_cyclic(&self, mut x: Array1<f64>) -> Array1<f64> {
         if self.cyclic[0] {
             x[0] = (x[0] + self.xgrid[self.nx - 1]) % self.upper_bounds[0];
         }
         if self.cyclic[1] {
             x[1] = (x[1] + self.ygrid[self.ny - 1]) % self.upper_bounds[1];
         }
         if self.cyclic[2] {
             x[2] = (x[2] + self.zgrid[self.nz - 1]) % self.upper_bounds[2];
         }
 
         return x;
     }
 
     /// Check whether a coordinate is in bounds of the grid.
-    pub fn check_bounds(
-        &self,
-        x: ArrayView1<f64>
-    ) -> Bounds {
-        if (x[0] < self.xgrid[0]) || (x[0] > self.xgrid[self.nx - 1]){
-            return Bounds::Out;
-        }
-        else if x[1] < self.ygrid[0] || x[1] > self.ygrid[self.ny - 1] {
-            return Bounds::Out;
-        }
-        else if x[2] < self.zgrid[0] || x[2] > self.zgrid[self.nz - 1] {
+    pub fn check_bounds(&self, x: ArrayView1<f64>) -> Bounds {
+        if (x[0] < self.xgrid[0])
+            || (x[0] > self.xgrid[self.nx - 1])
+            || (x[1] < self.ygrid[0])
+            || (x[1] > self.ygrid[self.ny - 1])
+            || (x[2] < self.zgrid[0])
+            || (x[2] > self.zgrid[self.nz - 1])
+        {
             return Bounds::Out;
         }
         return Bounds::In;
     }
 }
```

### Comparing `streamtracer-2.0.1/src/interp.rs` & `streamtracer-2.1.0rc1/src/interp.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 //! Helper functions for interpolation.
 
-use numpy::ndarray::{Array1, Array, ArrayBase, Ix3, Data};
-
+use numpy::ndarray::{Array, Array1, ArrayBase, Data, Ix3};
 
 /// Trilinear-interpolation of a scalar defined on
 /// the eight corners of a cuboid.
 ///
 /// # Arguments
 ///
 /// * `values` - Values on the eight cube corners. Must be shape `(2, 2, 2)`.
 /// * `x` - Coordinate to interpolate at. Components must be `>= 0` and `<=1`. Must be shape `(3,)`.
-pub fn interp_trilinear<S>(
-    values: &ArrayBase<S, Ix3>,
-    x: &Array1<f64>
-) -> f64
+pub fn interp_trilinear<S>(values: &ArrayBase<S, Ix3>, x: &Array1<f64>) -> f64
 where
-    S: Data<Elem=f64>
+    S: Data<Elem = f64>,
 {
     if values.dim() != (2, 2, 2) {
         panic!("Interp values are not the right shape {:?}", values.shape());
     }
     let m_x = 1. - x;
 
     let mut c = Array::zeros((2, 2));
```

### Comparing `streamtracer-2.0.1/src/test_tracer.rs` & `streamtracer-2.1.0rc1/src/test_tracer.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 #[cfg(test)]
-mod tests{
-    use numpy::ndarray::{array, Array, Array2, s};
+mod tests {
+    use numpy::ndarray::{array, s, Array};
 
     use super::super::field::VectorField;
-    use super::super::trace::{TracerStatus, trace_streamline};
+    use super::super::trace::{trace_streamline, TracerStatus};
 
     #[test]
     fn test_uniform_field() {
         let xgrid = Array::range(0., 10.1, 0.5);
         let ygrid = Array::range(0., 10.1, 0.5);
         let zgrid = Array::range(0., 10.1, 0.5);
         // Create a vector field pointing in the x direction
         let mut field = Array::zeros((xgrid.len(), ygrid.len(), zgrid.len(), 3));
         field.slice_mut(s![.., .., .., 0]).fill(1.);
 
         let cyclic = array![false, false, false];
-        let f = VectorField::new(xgrid.view(), ygrid.view(), zgrid.view(), field.view(), cyclic.view());
+        let f = VectorField::new(
+            xgrid.view(),
+            ygrid.view(),
+            zgrid.view(),
+            field.view(),
+            cyclic.view(),
+        );
 
         let seed = array![5., 5., 5.];
         let direction = 1;
         let step_size = 0.1;
 
         // Should take 50 steps before going out of bounds
-        let mut xs: Array2<f64> = Array::zeros((100, 3));
-        let status = trace_streamline(seed.view(), &f, &direction, &step_size, xs.view_mut());
-        assert_eq![status.n_points, 51];
-        assert_eq![status.rot, TracerStatus::OutOfBounds];
-
-        let mut xs: Array2<f64> = Array::zeros((10, 3));
-        let status = trace_streamline(seed.view(), &f, &direction, &step_size, xs.view_mut());
-        assert_eq![status.n_points, 10];
-        assert_eq![status.rot, TracerStatus::RanOutOfSteps];
+        let max_steps = 100;
+        let result = trace_streamline(seed.view(), &f, &direction, &step_size, max_steps);
+        assert_eq![result.status.n_points, 51];
+        assert_eq![result.status.rot, TracerStatus::OutOfBounds];
+
+        let max_steps = 10;
+        let result = trace_streamline(seed.view(), &f, &direction, &step_size, max_steps);
+        assert_eq![result.status.n_points, max_steps];
+        assert_eq![result.status.rot, TracerStatus::RanOutOfSteps];
     }
 }
```

### Comparing `streamtracer-2.0.1/src/trace.rs` & `streamtracer-2.1.0rc1/src/trace.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,130 @@
 //! Streamline tracing functionality.
+use ndarray::parallel::prelude::*;
 use num_derive::ToPrimitive;
-use numpy::ndarray::{Array, Array1, Array3, ArrayView1, ArrayView2, ArrayView4, ArrayViewMut2, s};
-
-use crate::field::{VectorField, Bounds};
+use numpy::ndarray::{
+    stack, Array, Array1, Array2, Array3, ArrayView1, ArrayView2, ArrayView4, Axis,
+};
 
+use crate::field::{Bounds, VectorField};
 /// Enum denoting status of the streamline tracer
 #[derive(PartialEq, Debug, ToPrimitive, Clone, Copy)]
-pub enum TracerStatus{
+pub enum TracerStatus {
     /// Still running
     Running,
     /// Ran out of steps
     RanOutOfSteps = 1,
     /// Stepped out of bounds
     OutOfBounds = 2,
 }
 
 /// A single stream line status
-pub struct StreamlineStatus{
+#[derive(Clone)]
+pub struct StreamlineStatus {
     /// Reason of termination
     pub rot: TracerStatus,
     /// Number of valid coordinates returned
     /// Can be used to slice away extra bits of the array that were not
     /// used for tracing using `xs.slice(s![:n_points, ..])`.
-    pub n_points: usize
+    pub n_points: usize,
+}
+
+/// A result of tracing a streamline
+pub struct StreamlineResult {
+    /// The status of a trace
+    pub status: StreamlineStatus,
+    /// The array of line coordinates that were traced
+    pub line: Array2<f64>,
 }
 
 /// Trace streamlines
 ///
 /// # Parameters
 ///
 /// * `seeds` - Seed points for streamlines. Must be shape (nseeds, 3).
 /// * `field` - Vector field to track through.
 /// * `direction` - Direction to trace in, `1` for forwards, `-1` for backwards.
 /// * `step_size` - Size of each individual step to take.
 /// * `max_steps` - Maximum number of steps to take per streamline.
 ///   This directly sets the size of the output streamline array.
+#[allow(clippy::too_many_arguments)]
 pub fn trace_streamlines<'a>(
     seeds: ArrayView2<'a, f64>,
     xgrid: ArrayView1<'a, f64>,
     ygrid: ArrayView1<'a, f64>,
     zgrid: ArrayView1<'a, f64>,
     values: ArrayView4<'a, f64>,
     cyclic: ArrayView1<'a, bool>,
     direction: i32,
     step_size: f64,
     max_steps: usize,
-) ->  (Vec<StreamlineStatus>, Array3<f64>) {
+) -> (Vec<StreamlineStatus>, Array3<f64>) {
     let field = VectorField::new(xgrid, ygrid, zgrid, values, cyclic);
-    let n_seeds: usize = seeds.shape()[0];
-
-    let mut xs = Array::zeros((n_seeds, max_steps, 3));
-    let mut statuses: Vec<StreamlineStatus> = vec![];
 
     // Trace from each seed in turn
-    for i in 0..n_seeds{
-        statuses.push(
-            trace_streamline(
-                seeds.slice(s![i, ..]),
-                &field,
-                &direction,
-                &step_size,
-                xs.slice_mut(s![i, .., ..])
-            )
-        )
-    }
-
-    return (statuses, xs)
+    let (statuses, extracted_lines): (Vec<StreamlineStatus>, Vec<Array2<f64>>) = seeds
+        .axis_iter(Axis(0))
+        .into_par_iter()
+        .map(|seed| {
+            let result = trace_streamline(seed, &field, &direction, &step_size, max_steps);
+            return (result.status, result.line);
+        })
+        .unzip();
+
+    let extracted_lines_views: Vec<ArrayView2<f64>> = extracted_lines
+        .iter()
+        .map(|arr| return arr.view())
+        .collect();
+    let xs = stack(Axis(0), &extracted_lines_views).unwrap();
+    return (statuses, xs);
 }
 
 /// Trace a single streamline
 ///
 /// # Parameters
 /// - `x0`: Streamline seed point.
-/// - `field`: Vector field to trace through
+/// - `field`: Vector field to trace through.
 /// - `direction`: Direction to trace in. Can be 1 for forwards or -1 for backwards.
 /// - `step_size`: Step size to take.
-/// - `xs`: Output array. Maximum number of steps to take is set by this.
+/// - `max_steps`: The maximum number of steps to take.
 pub fn trace_streamline(
     x0: ArrayView1<f64>,
     field: &VectorField,
     direction: &i32,
     step_size: &f64,
-    mut xs: ArrayViewMut2<f64>,
-) -> StreamlineStatus{
+    max_steps: usize,
+) -> StreamlineResult {
     // Tracer status
+    let mut xs = Array::zeros((max_steps, 3));
     let mut status = TracerStatus::Running;
     // Number of points traced
     let mut n_points: usize = 1;
     // Fold direction into the definition of step size,
     // using sign(step_size) to determine step direction
     let step = (*step_size) * (*direction as f64);
-    let max_steps: usize = xs.shape()[0];
 
     // Create output array
     // Take a copy of input seed
     let mut x = Array::zeros(3);
     x.assign(&x0);
 
     // Take streamline steps
-    for i in 0..max_steps{
+    for i in 0..max_steps {
         // Copy current coordinate
         for j in 0..3 {
             xs[[i, j]] = x[[j]];
         }
         // +1 to account for the initial point
-        n_points = i+1;
+        n_points = i + 1;
         // Take a single step
         // Updates `x` in place.
         x = rk4_update(x, field, &step);
         x = field.wrap_cyclic(x);
         // Check new point isn't out of bounds
-        match field.check_bounds(x.view()){
+        match field.check_bounds(x.view()) {
             Bounds::Out => {
                 status = TracerStatus::OutOfBounds;
                 break;
             }
             Bounds::In => {
                 continue;
             }
@@ -122,26 +132,25 @@
     }
 
     // Finished tracing maximum steps
     if status == TracerStatus::Running {
         status = TracerStatus::RanOutOfSteps;
     }
 
-    return StreamlineStatus{
-        rot: status,
-        n_points
+    return StreamlineResult {
+        status: StreamlineStatus {
+            rot: status,
+            n_points,
+        },
+        line: xs,
     };
 }
 
-// Update a coordiante (`x`) by taking a single RK4 step
-fn rk4_update(
-    mut x: Array1<f64>,
-    field: &VectorField,
-    step_size: &f64
-) -> Array1<f64> {
+// Update a coordinate (`x`) by taking a single RK4 step
+fn rk4_update(mut x: Array1<f64>, field: &VectorField, step_size: &f64) -> Array1<f64> {
     let mut xu = x.clone();
     let k1 = stream_function(xu.view(), field, step_size);
 
     xu = x.clone() + 0.5 * k1.clone();
     let k2 = stream_function(xu.view(), field, step_size);
 
     xu = x.clone() + 0.5 * k2.clone();
@@ -153,20 +162,12 @@
     let step = (k1 + 2. * k2 + 2. * k3 + k4) / 6.;
     x = x + step;
     return x;
 }
 
 /// Return the step that a linear tracing method would take
 /// at a given position.
-fn stream_function(
-    x: ArrayView1<f64>,
-    field: &VectorField,
-    step_size: &f64
-) -> Array1<f64> {
+fn stream_function(x: ArrayView1<f64>, field: &VectorField, step_size: &f64) -> Array1<f64> {
     let vec = field.vector_at_position(x);
-    let vmag = (
-        vec[[0]].powf(2.) +
-        vec[[1]].powf(2.) +
-        vec[[2]].powf(2.)
-    ).sqrt();
+    let vmag = (vec[[0]].powf(2.) + vec[[1]].powf(2.) + vec[[2]].powf(2.)).sqrt();
     return (*step_size) * vec / vmag;
 }
```

### Comparing `streamtracer-2.0.1/Cargo.lock` & `streamtracer-2.1.0rc1/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,109 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "either"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+
+[[package]]
 name = "float_eq"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b59b6469c35ab601d6487d28879bccfbe8c896c33a3fe699c4d29817e552cc58"
+checksum = "28a80e3145d8ad11ba0995949bbcf48b9df2be62772b3d351ef017dff6ecb853"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "1.0.7"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.135"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68783febc7782c6c5cb401fbda4de5a9898be1762314da0bb2c10ced61f18b0c"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -73,285 +111,337 @@
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
+ "rayon",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-derive"
-version = "0.3.3"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
+checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.18.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.15.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e82dad04139b71a90c080c8463fe0dc7902db5192d939bd0950f074d014339e1"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.3"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.46"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94e2ef8dbfc347b10c094890f778ee2e36ca9bb4262e86dc99cd217e35f3470b"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "streamtracer"
 version = "2.0.1"
 dependencies = [
  "float_eq",
+ "ndarray",
  "num-derive",
  "num-traits",
  "numpy",
  "pyo3",
+ "rayon",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.102"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fcd952facd492f9be3ef0d0b7032a6e442ee9b361d4acc2b1d0c4aaa5f613a1"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "windows-sys"
-version = "0.36.1"
+name = "windows-targets"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
+ "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `streamtracer-2.0.1/PKG-INFO` & `streamtracer-2.1.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: streamtracer
-Version: 2.0.1
+Version: 2.1.0rc1
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: numpy>=1.14.5
+Requires-Dist: numpy>=1.23
+Requires-Dist: packaging>=21.3
 Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-doctestplus; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
-Requires-Dist: jupyter-sphinx; extra == 'docs'
-Requires-Dist: numpydoc; extra == 'docs'
-Requires-Dist: pydata-sphinx-theme; extra == 'docs'
+Requires-Dist: pytest-xdist; extra == 'tests'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-automodapi; extra == 'docs'
-Requires-Dist: sphinx_rtd_theme; extra == 'docs'
+Requires-Dist: jupyter-sphinx; extra == 'docs'
+Requires-Dist: sunpy-sphinx-theme; extra == 'docs'
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
-Summary: Python wrapped fortran to calculate streamlines
-Author: Lars Mejnertsen
-Author-email: David Stansby <dstansby@gmail.com>
+Summary: Python library to calculate streamlines
+Author: David Stansby, Lars Mejnertsen
+Author-email: The SunPy Developers <sunpy@googlegroups.com>
 License: GPL v3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://streamtracer.readthedocs.io/en/stable/
+Requires-Python: >=3.10
 Project-URL: homepage, https://streamtracer.readthedocs.io/en/stable/
-Project-URL: repository, https://github.com/dstansby/streamtracer
+Project-URL: documentation, https://streamtracer.readthedocs.io/en/stable/
+Project-URL: repository, https://github.com/sunpy/streamtracer
 
 # streamtracer
 
 Fast streamline tracing in python
 
 [![Documentation Status](https://readthedocs.org/projects/streamtracer/badge/?version=latest)](https://streamtracer.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://dev.azure.com/dstansby/streamtracer/_apis/build/status/dstansby.streamtracer?branchName=master)](https://dev.azure.com/dstansby/dstansby/_build/latest?definitionId=1&branchName=master)
```

