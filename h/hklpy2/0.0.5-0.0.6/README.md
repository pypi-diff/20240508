# Comparing `tmp/hklpy2-0.0.5.tar.gz` & `tmp/hklpy2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hklpy2-0.0.5.tar", last modified: Fri May  3 23:06:43 2024, max compression
+gzip compressed data, was "hklpy2-0.0.6.tar", last modified: Wed May  8 20:10:22 2024, max compression
```

## Comparing `hklpy2-0.0.5.tar` & `hklpy2-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.852792 hklpy2-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.844792 hklpy2-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 23:06:35.000000 hklpy2-0.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-03 23:06:35.000000 hklpy2-0.0.5/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 23:06:35.000000 hklpy2-0.0.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-03 23:06:35.000000 hklpy2-0.0.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 23:06:35.000000 hklpy2-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-03 23:06:35.000000 hklpy2-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 23:06:35.000000 hklpy2-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-03 23:06:43.852792 hklpy2-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-03 23:06:35.000000 hklpy2-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 23:06:35.000000 hklpy2-0.0.5/docs/source/substitutions.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 23:06:35.000000 hklpy2-0.0.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/hklpy2/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/hklpy2/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/backends/hkl_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/hklpy2/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/backends/tests/test_hkl_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/hklpy2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 23:06:35.000000 hklpy2-0.0.5/hklpy2/tests/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:06:43.848792 hklpy2-0.0.5/hklpy2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-03 23:06:43.000000 hklpy2-0.0.5/hklpy2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-03 23:06:43.000000 hklpy2-0.0.5/hklpy2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:06:43.000000 hklpy2-0.0.5/hklpy2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 23:06:43.000000 hklpy2-0.0.5/hklpy2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 23:06:43.000000 hklpy2-0.0.5/hklpy2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-03 23:06:35.000000 hklpy2-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:06:43.852792 hklpy2-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.442913 hklpy2-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.442913 hklpy2-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 20:10:14.000000 hklpy2-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-08 20:10:14.000000 hklpy2-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 20:10:14.000000 hklpy2-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-08 20:10:22.450913 hklpy2-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-08 20:10:14.000000 hklpy2-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/docs/source/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/hkl_soleil.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends/no_op.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/lattice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/reflection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api/z_misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 20:10:14.000000 hklpy2-0.0.6/docs/source/substitutions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 20:10:14.000000 hklpy2-0.0.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.446913 hklpy2-0.0.6/hklpy2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/no_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/backends/tests/test_hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 20:10:14.000000 hklpy2-0.0.6/hklpy2/tests/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:10:22.450913 hklpy2-0.0.6/hklpy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 20:10:22.000000 hklpy2-0.0.6/hklpy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-08 20:10:14.000000 hklpy2-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:10:22.450913 hklpy2-0.0.6/setup.cfg
```

### Comparing `hklpy2-0.0.5/.github/workflows/code.yml` & `hklpy2-0.0.6/.github/workflows/code.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,69 +12,75 @@
 
 defaults:
   run:
     shell: bash -l {0}
 
 jobs:
 
-  # lint:
-  #   name: Code style
-  #   runs-on: ubuntu-latest
+  lint:
+    name: Code style
+    runs-on: ubuntu-latest
 
-  #   steps:
-  #     - uses: actions/checkout@v4
+    steps:
+      - uses: actions/checkout@v4
 
-  #     - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
+        with:
+          python-version: "3.11"
 
-  #     - name: Install Dependencies
-  #       run: |
-  #         python -m pip install --upgrade pip
-  #         pip install flake8
+      - name: Install package
+        run: |
+          set -vxeuo pipefail
+          python -m pip install --upgrade pip
 
-  #     - name: Run flake8
-  #       run: |
-  #         flake8
+      - name: Run ruff
+        uses: davidslusser/actions_python_ruff@v1.0.1
+        with:
+          python_version: "3.11"
 
-  test-matrix:
+  tests:
     name: Python ${{ matrix.python-version }}
-    # needs: lint
+    needs: lint
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
           - "3.10"  # not 3.10 which truncates to 3.1
           - "3.11"
           - "3.12"
       max-parallel: 5
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Create Python ${{ matrix.python-version }} environment
-      uses: mamba-org/provision-with-micromamba@main
-      # use main branch to enable choice of channel-priority
+      uses: mamba-org/setup-micromamba@v1
       with:
-        cache-env: true
-        cache-env-key: env-key-${{ matrix.python-version }}
-        channel-priority: flexible
+        cache-environment: true
+        cache-environment-key: env-key-${{ matrix.python-version }}
+        condarc: |
+          channel-priority: flexible
         environment-file: environment.yml
         environment-name: anaconda-test-env-py-${{ matrix.python-version }}
-        extra-specs: |
+        create-args: >-
           pytest
           python=${{ matrix.python-version }}
           pyyaml
           ruamel_yaml
           yaml
           setuptools-scm
 
     - name: Install code coverage requirements by pip
       run: |
         # https://github.com/pradyunsg/furo/discussions/308#discussioncomment-3064061
         pip install coverage coveralls
 
+    - name: Install source code
+      run: pip install -e . --no-deps
+
     - name: Diagnostic
       run: |
         micromamba info
         micromamba list
         conda config --show-sources
         conda config --show
         micromamba env list
@@ -99,15 +105,15 @@
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
         COVERALLS_PARALLEL: true
 
   # https://coveralls-python.readthedocs.io/en/latest/usage/configuration.html#github-actions-support
   coveralls:
     name: Report unit test coverage to coveralls
-    needs: test-matrix
+    needs: tests
     runs-on: ubuntu-latest
     container: python:3-slim
 
     steps:
       - name: Gather coverage and report to Coveralls
         run: |
           echo "Finally!"
```

### Comparing `hklpy2-0.0.5/.github/workflows/docs.yml` & `hklpy2-0.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/.github/workflows/pypi.yml` & `hklpy2-0.0.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/.gitignore` & `hklpy2-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/LICENSE` & `hklpy2-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/PKG-INFO` & `hklpy2-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.5
+Version: 0.0.6
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -52,16 +52,17 @@
         represents that its use would not infringe privately owned rights.
         
         ****************************************************************************
         
 Project-URL: Homepage, https://prjemian.github.io/hklpy2
 Project-URL: Bug Tracker, https://github.com/prjemian/hklpy2/issues
 Keywords: bluesky,diffraction,diffractometer
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
+Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
@@ -76,28 +77,28 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ophyd
 Requires-Dist: pint
-Provides-Extra: libhkl
-Requires-Dist: pygobject; extra == "libhkl"
+Provides-Extra: hkl-soleil
+Requires-Dist: pygobject; extra == "hkl-soleil"
 Provides-Extra: tests
 Requires-Dist: packaging; extra == "tests"
 Provides-Extra: all
-Requires-Dist: hklpy2[libhkl,tests]; extra == "all"
+Requires-Dist: hklpy2[hkl_soleil,tests]; extra == "all"
 
 # hklpy2
 
 NOTE:  this project at initial development
 
-| Name | Downloads | Version | Platforms | PyPI |
-| --- | --- | --- | --- | --- |
-| [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) |
+| Name | Downloads | Version | Platforms | PyPI | Coverage |
+| --- | --- | --- | --- | --- | --- |
+| [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) | [![Coverage Status](https://coveralls.io/repos/github/prjemian/hklpy2/badge.svg?branch=main)](https://coveralls.io/github/prjemian/hklpy2?branch=main) |
 
 Controls for using diffractometers within the [Bluesky
 Framework](https://blueskyproject.io).
 
 ## References
 
 - hklpy2 documentation: <https://prjemian.github.io/hklpy2>
```

### Comparing `hklpy2-0.0.5/docs/Makefile` & `hklpy2-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/docs/make.bat` & `hklpy2-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.5/docs/source/conf.py` & `hklpy2-0.0.6/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     # 'member-order': 'bysource',
     "private-members": True,
     # "special-members": "__init__",
     # 'undoc-members': True,
     "exclude-members": autodoc_exclude_members,
 }
 autodoc_mock_imports = [
+    "gi",
     "pint",
 ]
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 inheritance_graph_attrs = {"rankdir": "LR"}
 inheritance_node_attrs = {"fontsize": 24}
```

### Comparing `hklpy2-0.0.5/docs/source/index.rst` & `hklpy2-0.0.6/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 .. caution:: Development in progress.
 
 .. toctree::
    :glob:
    :hidden:
 
-   license
+   api
 
 .. TODO remove from comment
     .. icons: https://fonts.google.com/icons
 
     .. grid:: 2
 
         .. grid-item-card:: :material-outlined:`summarize;3em` User Guide
@@ -34,11 +34,11 @@
 
 :home: https://prjemian.github.io/hklpy2
 :source: https://github.com/prjemian/hklpy2
 :license: :ref:`license`
 :full version: |release|
 :published: |today|
 :index: :ref:`genindex`
-:module: :ref:`modindex`
+:modules: :ref:`modindex`
 :1st gen: |hklpy|
 :acknowledgement: "This product includes software produced by UChicago Argonne,
     LLC under Contract No. DE-AC02-06CH11357 with the Department of Energy."
```

### Comparing `hklpy2-0.0.5/hklpy2.egg-info/PKG-INFO` & `hklpy2-0.0.6/hklpy2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.5
+Version: 0.0.6
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -52,16 +52,17 @@
         represents that its use would not infringe privately owned rights.
         
         ****************************************************************************
         
 Project-URL: Homepage, https://prjemian.github.io/hklpy2
 Project-URL: Bug Tracker, https://github.com/prjemian/hklpy2/issues
 Keywords: bluesky,diffraction,diffractometer
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
+Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
@@ -76,28 +77,28 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ophyd
 Requires-Dist: pint
-Provides-Extra: libhkl
-Requires-Dist: pygobject; extra == "libhkl"
+Provides-Extra: hkl-soleil
+Requires-Dist: pygobject; extra == "hkl-soleil"
 Provides-Extra: tests
 Requires-Dist: packaging; extra == "tests"
 Provides-Extra: all
-Requires-Dist: hklpy2[libhkl,tests]; extra == "all"
+Requires-Dist: hklpy2[hkl_soleil,tests]; extra == "all"
 
 # hklpy2
 
 NOTE:  this project at initial development
 
-| Name | Downloads | Version | Platforms | PyPI |
-| --- | --- | --- | --- | --- |
-| [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) |
+| Name | Downloads | Version | Platforms | PyPI | Coverage |
+| --- | --- | --- | --- | --- | --- |
+| [![Conda Package](https://img.shields.io/badge/package-hklpy2-green.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/hklpy2.svg)](https://anaconda.org/conda-forge/hklpy2) | [![PyPi](https://img.shields.io/pypi/v/hklpy2.svg)](https://pypi.python.org/pypi/hklpy2) | [![Coverage Status](https://coveralls.io/repos/github/prjemian/hklpy2/badge.svg?branch=main)](https://coveralls.io/github/prjemian/hklpy2?branch=main) |
 
 Controls for using diffractometers within the [Bluesky
 Framework](https://blueskyproject.io).
 
 ## References
 
 - hklpy2 documentation: <https://prjemian.github.io/hklpy2>
```

### Comparing `hklpy2-0.0.5/pyproject.toml` & `hklpy2-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["bluesky", "diffraction", "diffractometer"]
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/?highlight=license
 license = {file = "LICENSE"}
 # https://pypi.org/classifiers/
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
+    "Environment :: OpenStack",
     "Intended Audience :: Science/Research",
     "License :: Freely Distributable",
     "License :: Public Domain",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
@@ -44,22 +45,26 @@
 
 dependencies = [
   "numpy",
   "ophyd",
   "pint",
 ]
 
+[project.entry-points."hklpy2.solver"]
+no_op = "hklpy2.backends.no_op:NoOpSolver"
+hkl_soleil = "hklpy2.backends.hkl_soleil:HklSolver"
+
 [project.optional-dependencies]
-libhkl = [
+hkl_soleil = [
   "pygobject",
 ]
 tests = [
   "packaging",
 ]
-all = ["hklpy2[libhkl,tests]"]
+all = ["hklpy2[hkl_soleil,tests]"]
 
 [project.urls]
 "Homepage" = "https://prjemian.github.io/hklpy2"
 "Bug Tracker" = "https://github.com/prjemian/hklpy2/issues"
 
 [tool.black]
 line-length = 115  # matches the value of 'max-line-length' in .flake8
```

