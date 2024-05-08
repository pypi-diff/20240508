# Comparing `tmp/splinebox-0.0.1a0.tar.gz` & `tmp/splinebox-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splinebox-0.0.1a0.tar", last modified: Wed Mar 27 14:00:11 2024, max compression
+gzip compressed data, was "splinebox-0.0.2a0.tar", last modified: Wed May  8 07:55:23 2024, max compression
```

## Comparing `splinebox-0.0.1a0.tar` & `splinebox-0.0.2a0.tar`

### file list

```diff
@@ -1,47 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.320928 splinebox-0.0.1a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.312928 splinebox-0.0.1a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.312928 splinebox-0.0.1a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-27 14:00:11.320928 splinebox-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/basis_functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/docs/pyplots/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_catmullrom.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_cubichermite.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/pyplots/plot_exponentialhermite.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/docs/spline_curves.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/examples/plot_example1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:00:11.320928 splinebox-0.0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.312928 splinebox-0.0.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/src/splinebox/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/src/splinebox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    23704 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/src/splinebox/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27259 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/src/splinebox/spline_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/src/splinebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 14:00:11.000000 splinebox-0.0.1a0/src/splinebox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:00:11.316928 splinebox-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/tests/test_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/tests/test_spline_curves.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-27 13:59:55.000000 splinebox-0.0.1a0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.855112 splinebox-0.0.2a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.843112 splinebox-0.0.2a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.843112 splinebox-0.0.2a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-08 07:55:23.855112 splinebox-0.0.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.847112 splinebox-0.0.2a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.847112 splinebox-0.0.2a0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/_static/EPFL_Unités_Center-for-imaging.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   158821 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21228 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/_static/imaging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   206340 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252458 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.847112 splinebox-0.0.2a0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/b1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/b2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/b3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/basis_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/catmullrom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/cubichermite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/exponential.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/exponentialhermite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/hermite_spline_curves.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/api/spline_curves.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.847112 splinebox-0.0.2a0/docs/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/definitions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.851112 splinebox-0.0.2a0/docs/pyplots/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_catmullrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_cubichermite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/docs/pyplots/plot_exponentialhermite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.851112 splinebox-0.0.2a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/examples/plot_active_contours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/examples/plot_example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/examples/plot_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/examples/plot_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:55:23.855112 splinebox-0.0.2a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.843112 splinebox-0.0.2a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.851112 splinebox-0.0.2a0/src/splinebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/src/splinebox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/src/splinebox/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22756 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/src/splinebox/spline_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.851112 splinebox-0.0.2a0/src/splinebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 07:55:23.000000 splinebox-0.0.2a0/src/splinebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:55:23.851112 splinebox-0.0.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/tests/test_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/tests/test_spline_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 07:55:10.000000 splinebox-0.0.2a0/tox.ini
```

### Comparing `splinebox-0.0.1a0/.github/workflows/test_and_deploy.yml` & `splinebox-0.0.2a0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/.gitignore` & `splinebox-0.0.2a0/.gitignore`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/.pre-commit-config.yaml` & `splinebox-0.0.2a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/.readthedocs.yaml` & `splinebox-0.0.2a0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/LICENSE` & `splinebox-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/PKG-INFO` & `splinebox-0.0.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splinebox
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: A python package for fitting splines.
 Author-email: Florian Aymanns <florian.aymanns@epfl.ch>, Virginie Uhlmann <uhlmann@ebi.ac.uk>, Edward Andò <edward.ando@epfl.ch>
 Maintainer-email: Florian Aymanns <flroian.aymanns@epfl.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, EPFL Center for Imaging
         
@@ -57,14 +57,16 @@
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
+Requires-Dist: scikit-image; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
 
 <img style="float: right;" src="https://imaging.epfl.ch/resources/logo-for-gitlab.svg">
 
 # splinebox
 A python package for fitting splines.
 Developed by the [EPFL Center for Imaging](https://imaging.epfl.ch/) as part of a collaboration with the [Uhlmann Group at EMBL-EBI](https://www.ebi.ac.uk/research/uhlmann/) in Feb 2024.
```

### Comparing `splinebox-0.0.1a0/README.md` & `splinebox-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/docs/Makefile` & `splinebox-0.0.2a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/docs/make.bat` & `splinebox-0.0.2a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/docs/pyplots/plot_b2.py` & `splinebox-0.0.2a0/docs/pyplots/plot_b2.py`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/docs/pyplots/plot_b3.py` & `splinebox-0.0.2a0/docs/pyplots/plot_b3.py`

 * *Files identical despite different names*

### Comparing `splinebox-0.0.1a0/docs/pyplots/plot_catmullrom.py` & `splinebox-0.0.2a0/docs/pyplots/plot_catmullrom.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 x = np.linspace(-3, 3, 100)
 
 basis_0th = basis.eval(x)
 basis_1st = basis.eval(x, derivative=1)
 basis_2nd = basis.eval(x, derivative=2)
 
-fig.suptitle("Keys basis function and its derivatives")
+fig.suptitle("Catmull Rom basis function and its derivatives")
 axes[0].plot(x, basis_0th, label=r"$f(x)$")
 axes[0].legend()
 axes[1].plot(x, basis_1st, label=r"$\frac{df}{dx}(x)$")
 axes[1].legend()
 axes[2].plot(x, basis_2nd, label=r"$\frac{d^2f}{dx^2}(x)$")
 axes[2].legend()
 axes[2].set_xlabel(r"$x$")
```

### Comparing `splinebox-0.0.1a0/docs/pyplots/plot_cubichermite.py` & `splinebox-0.0.2a0/docs/pyplots/plot_cubichermite.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 basis = splinebox.basis_functions.CubicHermite()
 
 x = np.linspace(-3, 3, 100)
 
 basis_0th = basis.eval(x)
 basis_1st = basis.eval(x, derivative=1)
 
-fig.suptitle("H3 basis function and its derivatives")
+fig.suptitle("Cubic Hermite basis function and its derivatives")
 axes[0][0].plot(x, basis_0th[0], label=r"$f_1(x)$")
 axes[0][0].legend()
 axes[1][0].plot(x, basis_1st[0], label=r"$\frac{df_1}{dx}(x)$")
 axes[1][0].legend()
 axes[1][0].set_xlabel(r"$x$")
 axes[0][1].plot(x, basis_0th[1], label=r"$f_2(x)$")
 axes[0][1].legend()
```

### Comparing `splinebox-0.0.1a0/docs/pyplots/plot_exponentialhermite.py` & `splinebox-0.0.2a0/docs/pyplots/plot_exponentialhermite.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 basis = splinebox.basis_functions.ExponentialHermite(alpha=alpha)
 
 x = np.linspace(-3, 3, 100)
 
 basis_0th = basis.eval(x)
 basis_1st = basis.eval(x, derivative=1)
 
-fig.suptitle(f"HE3 basis function and its derivatives for $\\alpha={alpha}$")
+fig.suptitle(f"Exponential Hermite basis function and its derivatives for $\\alpha={alpha}$")
 axes[0][0].plot(x, basis_0th[0], label=r"$f_1(x)$")
 axes[0][0].legend()
 axes[1][0].plot(x, basis_1st[0], label=r"$\frac{df_1}{dx}(x)$")
 axes[1][0].legend()
 axes[1][0].set_xlabel(r"$x$")
 axes[0][1].plot(x, basis_0th[1], label=r"$f_2(x)$")
 axes[0][1].legend()
```

### Comparing `splinebox-0.0.1a0/examples/plot_example1.py` & `splinebox-0.0.2a0/examples/plot_example1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Closed interpolating splines
 ============================
 
 This example shows different closed interpolating splines.
 """
 
-import math
-
 import matplotlib.pyplot as plt
 import numpy as np
 import splinebox.basis_functions
 import splinebox.spline_curves
 
 n, m = 2, 2
 fig, axes = plt.subplots(n, m, sharex=True, sharey=True)
@@ -25,20 +23,20 @@
 # The parameter values at which the spline is evaluated
 x = np.linspace(0, len(coordinates), 1000)
 
 for i, (name, basis_function) in enumerate(
     (
         ("B1", splinebox.basis_functions.B1()),
         ("B3", splinebox.basis_functions.B3()),
-        ("Exponential", splinebox.basis_functions.Exponential(len(coordinates), 2.0 * math.pi / len(coordinates))),
+        ("Exponential", splinebox.basis_functions.Exponential(len(coordinates))),
         ("CatmullRom", splinebox.basis_functions.CatmullRom()),
     )
 ):
     curve = splinebox.spline_curves.Spline(len(coordinates), basis_function, True)
-    curve.getCoefsFromKnots(coordinates)
+    curve.knots = coordinates
     discreteContour = curve.eval(x)
 
     axes[i // n, i % n].plot(discreteContour[:, 0], discreteContour[:, 1])
     axes[i // n, i % n].set_title(name)
     axes[i // n, i % n].set_aspect("equal", adjustable="box")
 
 plt.show()
```

### Comparing `splinebox-0.0.1a0/pyproject.toml` & `splinebox-0.0.2a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -95,11 +95,13 @@
     "tox",
     "pytest",
     "pytest-cov",
 ]
 docs = [
     "matplotlib",
     "sphinx-gallery",
+    "scikit-image",
+    "pydata-sphinx-theme",
 ]
 
 [project.urls]
 Repository = "https://github.com/EPFL-Center-for-Imaging/splinebox"
```

### Comparing `splinebox-0.0.1a0/src/splinebox/basis_functions.py` & `splinebox-0.0.2a0/src/splinebox/basis_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,23 +99,23 @@
     """
 
     def __init__(self):
         super().__init__(False, 2)
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _func(x):
+    def _func(x):  # pragma: no cover
         val = 0
         if abs(x) >= 0 and abs(x) < 1:
             val = 1 - abs(x)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_1(x):
+    def _derivative_1(x):  # pragma: no cover
         val = 0
         if x > -1 and x < 0:
             val = 1
         elif x > 0 and x < 1:
             val = -1
         elif x == 0 or x == -1 or x == 1:
             # This is the gradient you'll get at exactly 0
@@ -150,39 +150,39 @@
     """
 
     def __init__(self):
         super().__init__(False, 3)
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _func(x):
+    def _func(x):  # pragma: no cover
         val = 0
         if x >= -1.5 and x <= -0.5:
             val = 0.5 * (x**2) + 1.5 * x + 1.125
         elif x > -0.5 and x <= 0.5:
             val = -x * x + 0.75
         elif x > 0.5 and x <= 1.5:
             val = 0.5 * (x**2) - 1.5 * x + 1.125
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_1(x):
+    def _derivative_1(x):  # pragma: no cover
         val = 0
         if x >= -1.5 and x <= -0.5:
             val = x + 1.5
         elif x > -0.5 and x <= 0.5:
             val = -2 * x
         elif x > 0.5 and x <= 1.5:
             val = x - 1.5
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_2(x):
+    def _derivative_2(x):  # pragma: no cover
         val = 0
         if x >= -1.5 and x <= -0.5:
             val = 1
         elif x > -0.5 and x <= 0.5:
             val = -2
         elif x > 0.5 and x <= 1.5:
             val = 1
@@ -207,39 +207,39 @@
     """
 
     def __init__(self):
         super().__init__(False, 4)
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _func(x):
+    def _func(x):  # pragma: no cover
         val = 0
         if abs(x) >= 0 and abs(x) < 1:
             val = 2 / 3 - (abs(x) ** 2) + (abs(x) ** 3) / 2
         elif abs(x) >= 1 and abs(x) <= 2:
             val = ((2 - abs(x)) ** 3) / 6
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_1(x):
+    def _derivative_1(x):  # pragma: no cover
         val = 0
         if x >= 0 and x < 1:
             val = -2 * x + 1.5 * x * x
         elif x > -1 and x < 0:
             val = -2 * x - 1.5 * x * x
         elif x >= 1 and x <= 2:
             val = -0.5 * ((2 - x) ** 2)
         elif x >= -2 and x <= -1:
             val = 0.5 * ((2 + x) ** 2)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_2(x):
+    def _derivative_2(x):  # pragma: no cover
         val = 0
         if x >= 0 and x < 1:
             val = -2 + 3 * x
         elif x > -1 and x < 0:
             val = -2 - 3 * x
         elif x >= 1 and x <= 2:
             val = 2 - x
@@ -248,163 +248,179 @@
         return val
 
     @staticmethod
     def filter_symmetric(s):
         M = len(s)
         pole = -2 + np.sqrt(3)
 
-        cp = np.zeros(M)
+        ndim = 1 if s.ndim == 1 else s.shape[1]
+
+        cp = np.zeros((M, ndim))
         eps = 1e-8
         k0 = np.min(((2 * M) - 2, int(np.ceil(np.log(eps) / np.log(np.abs(pole))))))
         for k in range(k0):
             k = k % (2 * M - 2)
             val = s[2 * M - 2 - k] if k >= M else s[k]
             cp[0] += val * (pole**k)
         cp[0] *= 1 / (1 - (pole ** (2 * M - 2)))
 
         for k in range(1, M):
             cp[k] = s[k] + pole * cp[k - 1]
 
-        cm = np.zeros(M)
+        cm = np.zeros((M, ndim))
         cm[M - 1] = cp[M - 1] + (pole * cp[M - 2])
         cm[M - 1] *= pole / ((pole**2) - 1)
         for k in range(M - 2, -1, -1):
             cm[k] = pole * (cm[k + 1] - cp[k])
 
         c = cm * 6
 
         c[np.where(abs(c) < eps)] = 0
-        return c
+        return np.squeeze(c)
 
     @staticmethod
     def filter_periodic(s):
         M = len(s)
         pole = -2 + np.sqrt(3)
 
-        cp = np.zeros(M)
+        ndim = 1 if s.ndim == 1 else s.shape[1]
+
+        cp = np.zeros((M, ndim))
         for k in range(M):
             cp[0] += s[(M - k) % M] * (pole**k)
         cp[0] *= 1 / (1 - (pole**M))
 
         for k in range(1, M):
             cp[k] = s[k] + pole * cp[k - 1]
 
-        cm = np.zeros(M)
+        cm = np.zeros((M, ndim))
         for k in range(M):
             cm[M - 1] += (pole**k) * cp[k]
         cm[M - 1] *= pole / (1 - (pole**M))
         cm[M - 1] += cp[M - 1]
         cm[M - 1] *= -pole
 
         for k in range(M - 2, -1, -1):
             cm[k] = pole * (cm[k + 1] - cp[k])
 
         c = cm * 6
 
         eps = 1e-8
         c[np.where(abs(c) < eps)] = 0
-        return c
+        return np.squeeze(c)
 
     def refinement_mask(self):
         order = int(self.support)
         mask = np.zeros(order + 1)
         _multinomial(order, 2, np.zeros(2), 0, 2, order, mask)
         return mask
 
 
 class Exponential(BasisFunction):
     r"""
     ???
 
     .. math::
         f(x) = \begin{cases}
-        \frac{L}{\alpha^2} 2 \sin(\frac{\alpha}{2} x) & \text{for } 0 \leq x < 1 \\
+        \frac{L}{\alpha^2} 2 \sin(\frac{\alpha}{2} x)^2 & \text{for } 0 \leq x < 1 \\
         \frac{L}{\alpha^2} (\cos(\alpha (x - 2)) + \cos(\alpha (x - 1)) - 2 \cos(\alpha)) & \text{for } 1 \leq x < 2 \\
         \frac{L}{\alpha^2} 2 \sin(\frac{\alpha}{2} (x- 3))^2 & \text{for } 2 \leq x \leq 3 \\
         0 & \text{otherwise}\end{cases}
 
     .. math::
-        \text{where } L=(\frac{\sin(\pi / M)}{\pi / M})^{-2}
+        \text{where } L=(\frac{\sin(\pi / M)}{\pi / M})^{-2}\text{ and }x = x + \frac{support}{2}
+
+    .. math::
+        f(x) = \begin{cases}
+        2 L \sin(\alpha x)^2 & \text{for } 0 \leq x < 1 \\
+        L (\cos(2\alpha (x - 2)) + \cos(2\alpha (x - 1)) - 2 \cos(2\alpha)) & \text{for } 1 \leq x < 2 \\
+        2 L \sin(\alpha (x - 3))^2 & \text{for } 2 \leq x \leq 3 \\
+        0 & \text{otherwise}\end{cases}
+
+    .. math::
+        \text{where } \alpha=\frac{\pi}{M}, L=\frac{1}{4 \sin(\alpha)^2} \text{ and }x = x + \frac{3}{2}
     """
 
-    def __init__(self, M, alpha):
+    def __init__(self, M):
         super().__init__(False, 3)
         self.M = M
-        self.alpha = alpha
 
     def _func(self, x):
-        return self.__func(x, self.support / 2, self.M, self.alpha)
+        return self.__func(x, self.support / 2, self.M)
 
     @staticmethod
-    @numba.vectorize(
-        [numba.float64(numba.float64, numba.float64, numba.float64, numba.float64)], nopython=True, cache=True
-    )
-    def __func(x, half_support, M, alpha):
+    @numba.vectorize([numba.float64(numba.float64, numba.float64, numba.float64)], nopython=True, cache=True)
+    def __func(x, half_support, M):  # pragma: no cover
         x += half_support
-        L = (np.sin(np.pi / M) / (np.pi / M)) ** (-2)
+
+        alpha = np.pi / M
+        L = 1 / (4 * np.sin(alpha) ** 2)
 
         val = 0
         if x >= 0 and x < 1:
-            val = 2 * np.sin(alpha * 0.5 * x) * np.sin(alpha * 0.5 * x)
+            val = 2 * np.sin(alpha * x) ** 2
         elif x >= 1 and x < 2:
-            val = np.cos(alpha * (x - 2)) + np.cos(alpha * (x - 1)) - 2 * np.cos(alpha)
+            val = np.cos(2 * alpha * (x - 2)) + np.cos(2 * alpha * (x - 1)) - 2 * np.cos(2 * alpha)
         elif x >= 2 and x <= 3:
-            val = 2 * np.sin(alpha * 0.5 * (x - 3)) * np.sin(alpha * 0.5 * (x - 3))
+            val = 2 * np.sin(alpha * (x - 3)) ** 2
 
-        return (L * val) / (alpha * alpha)
+        return L * val
 
     def _derivative_1(self, x):
-        return self.__derivative_1(x, self.support / 2, self.M, self.alpha)
+        return self.__derivative_1(x, self.support / 2, self.M)
 
     @staticmethod
-    @numba.vectorize(
-        [numba.float64(numba.float64, numba.float64, numba.float64, numba.float64)], nopython=True, cache=True
-    )
-    def __derivative_1(x, half_support, M, alpha):
+    @numba.vectorize([numba.float64(numba.float64, numba.float64, numba.float64)], nopython=True, cache=True)
+    def __derivative_1(x, half_support, M):  # pragma: no cover
         x += half_support
-        L = (np.sin(np.pi / M) / (np.pi / M)) ** (-2)
+
+        alpha = np.pi / M
+        L = 1 / (4 * np.sin(alpha) ** 2)
 
         val = 0
         if x >= 0 and x <= 1:
-            val = alpha * np.sin(alpha * x)
+            val = 4 * alpha * np.sin(alpha * x) * np.cos(alpha * x)
         elif x > 1 and x <= 2:
-            val = alpha * (np.sin(alpha * (1 - x)) + np.sin(alpha * (2 - x)))
+            val = 2 * alpha * (np.sin(2 * alpha * (2 - x)) + np.sin(2 * alpha * (1 - x)))
         elif x > 2 and x <= 3:
-            val = alpha * np.sin(alpha * (x - 3))
+            val = 4 * alpha * np.sin(alpha * (x - 3)) * np.cos(alpha * (x - 3))
 
-        return (L * val) / (alpha * alpha)
+        return L * val
 
     def _derivative_2(self, x):
-        return self.__derivative_2(x, self.support / 2, self.M, self.alpha)
+        return self.__derivative_2(x, self.support / 2, self.M)
 
     @staticmethod
-    @numba.vectorize(
-        [numba.float64(numba.float64, numba.float64, numba.float64, numba.float64)], nopython=True, cache=True
-    )
-    def __derivative_2(x, half_support, M, alpha):
+    @numba.vectorize([numba.float64(numba.float64, numba.float64, numba.float64)], nopython=True, cache=True)
+    def __derivative_2(x, half_support, M):  # pragma: no cover
         x += half_support
-        L = (np.sin(np.pi / M) / (np.pi / M)) ** (-2)
+
+        alpha = np.pi / M
+        L = 1 / (4 * np.sin(alpha) ** 2)
 
         val = 0
         if x >= 0 and x <= 1:
-            val = alpha * alpha * np.cos(alpha * x)
+            val = 4 * alpha**2 * (np.cos(alpha * x) ** 2 - np.sin(alpha * x) ** 2)
         elif x > 1 and x <= 2:
-            val = alpha * alpha * (-np.cos(alpha * (1 - x)) - np.cos(alpha * (2 - x)))
+            val = -4 * alpha**2 * (np.cos(2 * alpha * (2 - x)) + np.cos(2 * alpha * (1 - x)))
         elif x > 2 and x <= 3:
-            val = alpha * alpha * np.cos(alpha * (x - 3))
+            val = 4 * alpha**2 * (np.cos(alpha * (x - 3)) ** 2 - np.sin(alpha * (x - 3)) ** 2)
 
-        return (L * val) / (alpha * alpha)
+        return L * val
 
     def filter_symmetric(self, s):
         self.M = len(s)
+
+        ndim = 1 if s.ndim == 1 else s.shape[1]
+
         b0 = self._func(0)
         b1 = self._func(1)
         pole = (-b0 + np.sqrt(2 * b0 - 1)) / (1 - b0)
 
-        cp = np.zeros(self.M)
+        cp = np.zeros((self.M, ndim))
         eps = 1e-8
         k0 = np.min(
             (
                 (2 * self.M) - 2,
                 int(np.ceil(np.log(eps) / np.log(np.abs(pole)))),
             )
         )
@@ -413,54 +429,57 @@
             val = s[2 * self.M - 2 - k] if k >= self.M else s[k]
             cp[0] += val * (pole**k)
         cp[0] *= 1 / (1 - (pole ** (2 * self.M - 2)))
 
         for k in range(1, self.M):
             cp[k] = s[k] + pole * cp[k - 1]
 
-        cm = np.zeros(self.M)
+        cm = np.zeros((self.M, ndim))
         cm[self.M - 1] = cp[self.M - 1] + (pole * cp[self.M - 2])
         cm[self.M - 1] *= pole / ((pole * pole) - 1)
         for k in range(self.M - 2, -1, -1):
             cm[k] = pole * (cm[k + 1] - cp[k])
 
         c = cm / b1
 
         c[np.where(np.abs(c) < eps)] = 0
-        return c
+        return np.squeeze(c)
 
     def filter_periodic(self, s):
         self.M = len(s)
+
+        ndim = 1 if s.ndim == 1 else s.shape[1]
+
         b0 = self._func(0)
         pole = (-b0 + np.sqrt(2 * b0 - 1)) / (1 - b0)
 
-        cp = np.zeros(self.M)
+        cp = np.zeros((self.M, ndim))
         cp[0] = s[0]
-        for k in range(self.M):
+        for k in range(1, self.M):
             cp[0] += s[k] * (pole ** (self.M - k))
         cp[0] *= 1 / (1 - (pole**self.M))
 
         for k in range(1, self.M):
             cp[k] = s[k] + (pole * cp[k - 1])
 
-        cm = np.zeros(self.M)
+        cm = np.zeros((self.M, ndim))
         cm[self.M - 1] = cp[self.M - 1]
         for k in range(self.M - 1):
             cm[self.M - 1] += cp[k] * (pole ** (k + 1))
         cm[self.M - 1] *= 1 / (1 - (pole**self.M))
         cm[self.M - 1] *= (1 - pole) ** 2
 
         for k in range(self.M - 2, -1, -1):
             cm[k] = (pole * cm[k + 1]) + (((1 - pole) ** 2) * cp[k])
 
         c = cm
 
         eps = 1e-8
         c[np.where(np.abs(c) < eps)] = 0
-        return c
+        return np.squeeze(c)
 
     def refinement_mask(self):
         order = int(self.support)
         mask = np.zeros(order + 1)
 
         denominator = 2 ** (order - 1)
         mask[0] = 1 / denominator
@@ -477,39 +496,39 @@
     """
 
     def __init__(self):
         super().__init__(False, 4)
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _func(x):
+    def _func(x):  # pragma: no cover
         val = 0
         if np.abs(x) >= 0 and np.abs(x) <= 1:
             val = (3 / 2) * (np.abs(x) ** 3) - (5 / 2) * (np.abs(x) ** 2) + 1
         elif np.abs(x) > 1 and np.abs(x) <= 2:
             val = (-1 / 2) * (np.abs(x) ** 3) + (5 / 2) * (np.abs(x) ** 2) - 4 * np.abs(x) + 2
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_1(x):
+    def _derivative_1(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = x * (4.5 * x - 5)
         elif x >= -1 and x < 0:
             val = -x * (4.5 * x + 5)
         elif x > 1 and x <= 2:
             val = -1.5 * x * x + 5 * x - 4
         elif x >= -2 and x < -1:
             val = 1.5 * x * x + 5 * x + 4
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def _derivative_2(x):
+    def _derivative_2(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = 9 * x - 5
         elif x >= -1 and x < 0:
             val = -9 * x - 5
         elif x > 1 and x <= 2:
             val = -3 * x + 5
@@ -535,48 +554,48 @@
         super().__init__(True, 2)
 
     def _func(self, x):
         return np.array([self.h31(x), self.h32(x)])
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def h31(x):
+    def h31(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = (1 + (2 * x)) * (x - 1) * (x - 1)
         elif x < 0 and x >= -1:
             val = (1 - (2 * x)) * (x + 1) * (x + 1)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def h32(x):
+    def h32(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = x * (x - 1) * (x - 1)
         elif x < 0 and x >= -1:
             val = x * (x + 1) * (x + 1)
         return val
 
     def _derivative_1(self, x):
         return np.array([self.h31prime(x), self.h32prime(x)])
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def h31prime(x):
+    def h31prime(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = 6 * x * (x - 1)
         elif x < 0 and x >= -1:
             val = -6 * x * (x + 1)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64)], nopython=True, cache=True)
-    def h32prime(x):
+    def h32prime(x):  # pragma: no cover
         val = 0
         if x >= 0 and x <= 1:
             val = 3 * x * x - 4 * x + 1
         elif x < 0 and x >= -1:
             val = 3 * x * x + 4 * x + 1
         return val
 
@@ -667,14 +686,22 @@
             if M != 2:
                 val = 13 / (M * 420)
         elif nmod == M - 1:
             val = -13 / (M * 420)
 
         return val
 
+    @staticmethod
+    def filter_symmetric(s):
+        return s
+
+    @staticmethod
+    def filter_periodic(s):
+        return s
+
 
 class ExponentialHermite(BasisFunction):
     """
     ???
     """
 
     def __init__(self, alpha):
@@ -682,15 +709,15 @@
         self.alpha = alpha
 
     def _func(self, x):
         return np.array([self._he31(x, self.alpha), self._he32(x, self.alpha)])
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64, numba.float64)], nopython=True, cache=True)
-    def _he31(x, alpha):
+    def _he31(x, alpha):  # pragma: no cover
         def _g1(x, alpha):
             val = 0
             if x >= 0 and x <= 1:
                 denom = (0.5 * alpha * np.cos(0.5 * alpha)) - np.sin(0.5 * alpha)
                 num = (
                     (0.5 * ((alpha * np.cos(0.5 * alpha)) - np.sin(0.5 * alpha)))
                     - (0.5 * alpha * np.cos(0.5 * alpha) * x)
@@ -700,15 +727,15 @@
             return val
 
         val = _g1(x, alpha) if x >= 0 else _g1(-x, alpha)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64, numba.float64)], nopython=True, cache=True)
-    def _he32(x, alpha):
+    def _he32(x, alpha):  # pragma: no cover
         def _g2(x, alpha):
             val = 0
             if x >= 0 and x <= 1:
                 denom = ((0.5 * alpha * np.cos(0.5 * alpha)) - np.sin(0.5 * alpha)) * (4 * alpha) * np.sin(0.5 * alpha)
                 num = (
                     -((alpha * np.cos(alpha)) - np.sin(alpha))
                     - (2 * alpha * np.sin(0.5 * alpha) * np.sin(0.5 * alpha) * x)
@@ -722,29 +749,29 @@
         return val
 
     def _derivative_1(self, x):
         return np.array([self._he31prime(x, self.alpha), self._he32prime(x, self.alpha)])
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64, numba.float64)], nopython=True, cache=True)
-    def _he31prime(x, alpha):
+    def _he31prime(x, alpha):  # pragma: no cover
         def _g1prime(x, alpha):
             val = 0
             if x >= 0 and x <= 1:
                 denom = (0.5 * alpha * np.cos(0.5 * alpha)) - np.sin(0.5 * alpha)
                 num = -(0.5 * alpha * np.cos(0.5 * alpha)) + (0.5 * alpha * np.cos(0.5 * alpha - (alpha * x)))
                 val = num / denom
             return val
 
         val = _g1prime(x, alpha) if x >= 0 else -1 * _g1prime(-x, alpha)
         return val
 
     @staticmethod
     @numba.vectorize([numba.float64(numba.float64, numba.float64)], nopython=True, cache=True)
-    def _he32prime(x, alpha):
+    def _he32prime(x, alpha):  # pragma: no cover
         def _g2prime(x, alpha):
             val = 0
             if x >= 0 and x <= 1:
                 denom = ((0.5 * alpha * np.cos(0.5 * alpha)) - np.sin(0.5 * alpha)) * (4 * alpha) * np.sin(0.5 * alpha)
                 num = (
                     -(2 * alpha * np.sin(0.5 * alpha) * np.sin(0.5 * alpha))
                     + (2 * alpha * np.sin(0.5 * alpha) * np.sin(alpha * (x - 0.5)))
@@ -757,14 +784,22 @@
         return val
 
     @staticmethod
     def _derivative_2(x):
         raise RuntimeError("ExponentialHermite isn't twice differentiable.")
         return
 
+    @staticmethod
+    def filter_symmetric(s):
+        return s
+
+    @staticmethod
+    def filter_periodic(s):
+        return s
+
 
 def _multinomial(
     maxValue,
     numberOfCoefficiens,
     kArray,
     iteration,
     dilationFactor,
```

### Comparing `splinebox-0.0.1a0/src/splinebox/spline_curves.py` & `splinebox-0.0.2a0/src/splinebox/spline_curves.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import collections
 import copy
-import itertools
 import math
-import warnings
 
 import numba
 import numpy as np
 import scipy.integrate
 
 
 class Spline:
@@ -34,386 +32,314 @@
         else:
             raise RuntimeError("M must be greater or equal than the spline generator support size.")
 
         self.basis_function = basis_function
         self.halfSupport = self.basis_function.support / 2
         # Number of additional knots used for padding the ends
         # of an open spline
-        self.pad = math.ceil(self.halfSupport)
+        self.pad = math.ceil(self.halfSupport) - 1
         self.closed = closed
         self.coeffs = coeffs
 
+    def _check_coeffs(self):
+        """
+        Most methods require coefficients to be set before they
+        can be used. This helper function checks if the coefficients have been
+        set.
+        """
+        if self.coeffs is None:
+            raise RuntimeError(self._no_coeffs_msg)
+
     @property
     def coeffs(self):
         return self._coeffs
 
     @coeffs.setter
     def coeffs(self, values):
         if values is not None:
             n = len(values)
             if self.closed and n != self.M:
                 raise ValueError(
                     f"The number of coefficients must match the number of knots for a closed spline. You provided {n} coefficients for a spline with M={self.M} knots."
                 )
-            support = self.basis_function.support
-            padded_M = int(self.M + support)
+            padded_M = self.M + 2 * self.pad
             if not self.closed and n != padded_M:
                 raise ValueError(
-                    f"Non-closed splines are padded at the ends with additional knots, i.e. the effective number of knots is M + support of the basis function. You provided {n} coefficients for a spline with M={self.M} and a basis function with support={support}, expected {padded_M}."
+                    f"Non-closed splines are padded at the ends with additional knots, i.e. the effective number of knots is M + 2 * (ceil(support/2) - 1) of the basis function. You provided {n} coefficients for a spline with M={self.M} and a basis function with support={self.basis_function.support}, expected {padded_M}."
                 )
         self._coeffs = values
 
     @property
+    def knots(self):
+        t = np.arange(self.M) if self.closed else np.arange(-self.pad, self.M + self.pad)
+        return self.eval(t)
+
+    @knots.setter
+    def knots(self, values):
+        knots = np.array(values)
+        if self.closed:
+            self.coeffs = self.basis_function.filter_periodic(knots)
+        else:
+            # Add constant padding for the ends of the spline
+            if knots.ndim == 1:
+                knots = knots[:, np.newaxis]
+            knots = np.pad(knots, ((self.pad, self.pad), (0, 0)), mode="edge")
+            knots = np.squeeze(knots)
+
+            self.coeffs = self.basis_function.filter_symmetric(knots)
+
+    @property
     def basis_function(self):
         return self._basis_function
 
     @basis_function.setter
     def basis_function(self, value):
         if value.multigenerator:
             raise ValueError(
                 "You are trying to construct a Hermite spline using the ordinary `Spline` class. Use the `HermiteSpline` class instead."
             )
         self._basis_function = value
 
     def copy(self):
         return copy.deepcopy(self)
 
-    def draw(self, dimensions):
+    def draw(self, x, y):
         """
         Computes a whether a point is inside or outside a closed
         spline on a regular grid of points.
 
         I would ask the user to provide a grid of points directly instead
         of asking for the dimensions. Like that the user can choose how densly
         they want to sample the grid.
         """
-        if self.coeffs is None:
-            raise RuntimeError(self._no_coeffs_msg)
+        self._check_coeffs()
 
-        if len(self.coeffs.shape) == 2 and self.coeffs.shape[1] == 2:
-            if self.closed:
-                warnings.warn(
-                    "draw() will take ages, go get yourself a coffee.",
-                    stacklevel=1,
-                )
+        if self.coeffs.ndim != 2 or self.coeffs.shape[1] != 2:
+            raise RuntimeError("draw() can only be used with 2D curves")
 
-                if len(dimensions) != 2:
-                    raise RuntimeError("dimensions must be a triplet.")
+        if not self.closed:
+            raise RuntimeError("draw() can only be used with closed curves.")
 
-                xvals = range(dimensions[1])
-                yvals = range(dimensions[0])
-                pointsList = list(itertools.product(xvals, yvals))
-
-                vals = [self.isInside(p) for p in pointsList]
-                vals = np.asarray(vals)
-
-                area = np.zeros(dimensions, dtype=np.int8)
-                for i in range(len(pointsList)):
-                    p = pointsList[i]
-                    area[p[1], p[0]] = int(255 * vals[i])
+        xx, yy = np.meshgrid(x, y)
+        result = self.is_inside(xx.flatten(), yy.flatten())
+        return result.reshape(xx.shape)
 
-                return area
+    def dtheta(self, t):
+        r"""
+        Helper function for calculating the winding number.
 
-            else:
-                raise RuntimeError("draw() can only be used with closed curves.")
-        else:
-            raise RuntimeError("draw() can only be used with 2D curves.")
+        `dtheta` is the derivative of the polar coordinate :math:`\theta(t)`
 
-    def windingNumber(self, t):
-        """
-        ???
+        .. math::
+            \theta(t) = arctan \left( \frac{y(t)}{x(t)} \right)
+
+        Differentiation yields:
 
-        Number that can be integrated along the entire spline
-        to determine where it wraps around the origin or not.
+        .. math::
+            \frac{d \theta}{dt} = \frac{1}{r^2} \left( x\frac{dy}{dt} - y\frac{dx}{dt} \right) \text{, where } r^2 = x^2 + y^2
         """
+        self._check_coeffs()
         r = self.eval(t)
-        dr = self.eval(t, dt=True)
+        dr = self.eval(t, derivative=1)
+        if r.ndim == 1:
+            r = r[np.newaxis, :]
+            dr = dr[np.newaxis, :]
+        r2 = np.linalg.norm(r, axis=1) ** 2
+        if np.any(np.isnan(dr)) or np.isclose(r2, 0):
+            # Happens the the spline is not differentiable in this location
+            # or when the point is at the origin
+            # The solution to return 0 is a bit of a hack but works in practice with
+            # the numerical integration
+            return np.squeeze(np.zeros(r.shape[0]))
+        val = (1.0 / r2) * (r[:, 0] * dr[:, 1] - r[:, 1] * dr[:, 0])
+        return np.squeeze(val)
+
+    def is_inside(self, x, y):
+        r"""
+        Determines if a point with coordinates `x`, `y` is inside the spline.
+        Only works for closed 2D curves.
 
-        r2 = np.linalg.norm(r) ** 2
-        val = (1.0 / r2) * (r[0] * dr[1] - r[1] * dr[0])
-        return val
-
-    def isInside(self, point):
-        """
-        Determines if a point is inside the closed spline
-        or not. Is it fair game to change the coeff of the
-        object or should it be cloned first?
-        The :meth:`splinebox.splines.Spline.translate` method should
-        be used instead of subtracting the point.
+        To determine whether a point is inside or outside the spline, the winding number
+        is used:
+
+        .. math::
+            wind(\gamma, 0) = \frac{1}{2\pi} \oint_\gamma d\theta = \frac{1}{2\pi} \oint_\gamma \left( \frac{x}{r^2}dy - \frac{y}{r^2}dx \right).
+
+        For a description of :math:`d\theta` check :meth:`splinebox.splines_curves.Spline.dtheta`.
 
         Parameters
         ----------
-        point : numpy.array
+        x : numpy.ndarray or float
+            x coordinate(s) of point(s)
+        y : numpy.ndarray or float
+            y coordinate(s) of point(s)
+
+        Returns
+        -------
+        val : float
+            1 if the point is inside, 0.5 if its on the curve and 0 if it is outside the curve.
         """
-        if self.closed:
-            originalCoefs = copy.deepcopy(self.coeffs)
-            self.coeffs = originalCoefs - point
-
-            res = scipy.integrate.quad(self.windingNumber, 0, self.M)
-
-            self.coeffs = originalCoefs
-
-            val = res[0]
-            if np.abs(val - 2.0 * np.pi) < 1e-6:
-                return 1
-            elif np.abs(val - np.pi) < 1e-6:
-                return 0.5
-            else:
-                return 0
-        else:
+        if not self.closed:
             raise RuntimeError("isInside() can only be used with closed curves.")
-
-    def getKnotsFromCoefs(self):
-        if len(self.coeffs.shape) == 1:
-            if self.closed:
-                knots = np.zeros(self.M)
-                for k in range(self.M):
-                    knots[k] = self.eval(k)
+        self._check_coeffs()
+        if self.coeffs.ndim != 2 or self.coeffs.shape[1] != 2:
+            raise RuntimeError("isInside() can only be used with 2D curves.")
+
+        if isinstance(x, float):
+            x = np.array([x])
+        if isinstance(y, float):
+            y = np.array([y])
+        if not np.allclose(x.shape, y.shape):
+            raise ValueError("x and y need to have the same shape")
+
+        results = np.zeros(x.shape)
+        for coord, point in enumerate(np.stack([x, y], axis=-1)):
+            spline_copy = self.copy()
+            spline_copy.translate(-point)
+            winding_number = scipy.integrate.quad(spline_copy.dtheta, 0, spline_copy.M)[0]
+            for ref in np.array([[1, 1], [1, 2], [2, 2], [2, 1]]):
+                if np.allclose(point, ref):
+                    print(ref, winding_number)
+            if np.abs(np.abs(winding_number) - 2 * np.pi) < 1e-6:
+                results[coord] = 1
+            elif np.abs(winding_number) > 1e-6:
+                results[coord] = 0.5
             else:
-                knots = np.zeros(self.M + 2 * self.pad)
-                for kn, k in enumerate(range(-self.pad, self.M + self.pad)):
-                    knots[kn] = self.eval(k)
-        elif len(self.coeffs.shape) == 2 and (self.coeffs.shape[1] == 2):
-            if self.closed:
-                knots = np.zeros((self.M, 2))
-                for k in range(self.M):
-                    knots[k] = self.eval(k)
-            else:
-                knots = np.zeros((self.M + 2 * self.pad, 2))
-                for kn, k in enumerate(range(-self.pad, self.M + self.pad)):
-                    knots[kn] = self.eval(k)
-        return knots
-
-    def getCoefsFromKnots(self, knots):
-        """
-        ???
+                results[coord] = 0
+        return np.squeeze(results)
 
-        Fits the spline to go through the knots.
-        get is a bad name since nothing is returned.
-        fit would be better.
+    def fit(self, points, arc_length_parameterization=False):
         """
-        knots = np.array(knots)
-        if len(knots.shape) == 1:
-            if self.closed:
-                self.coeffs = self.basis_function.filter_periodic(knots)
-            else:
-                for _i in range(int(self.pad)):
-                    # knots = np.append(knots, knots[-1-_i] + (knots[-1-_i]-knots[-(_i+1)*2]) )
-                    knots = np.append(knots, knots[-1])
-                for _i in range(int(self.pad)):
-                    # knots = np.append(knots[0+_i] + (knots[0+_i]-knots[2*(_i+1)-1]), knots)
-                    knots = np.append(knots[0], knots)
-                self.coeffs = self.basis_function.filter_symmetric(knots)
-        elif len(knots.shape) == 2:
-            if knots.shape[1] == 2:
-                if self.closed:
-                    coeffsX = self.basis_function.filter_periodic(knots[:, 0])
-                    coeffsY = self.basis_function.filter_periodic(knots[:, 1])
-                else:
-                    for _i in range(int(self.pad)):
-                        knots = np.vstack((knots, knots[-1]))
-                    for _i in range(int(self.pad)):
-                        knots = np.vstack((knots[0], knots))
-                    coeffsX = self.basis_function.filter_symmetric(knots[:, 0])
-                    coeffsY = self.basis_function.filter_symmetric(knots[:, 1])
-                self.coeffs = np.hstack(
-                    (
-                        np.array([coeffsX]).transpose(),
-                        np.array([coeffsY]).transpose(),
-                    )
-                )
-            else:
-                raise RuntimeError(self._wrong_dimension_msg)
-        else:
-            raise RuntimeError(self._wrong_array_size_msg)
-
-    def getCoefsFromDenseContour(self, contourPoints, arcLengthParameterization=False):
-        """
-        ???
-
-        Fits the spline to match a contour.
-        get is a bad name since nothing is returned.
-        fit would be better.
-        Presumably the this is different from getCoefsFromKnots
-        because the spline does not have to go through the points.
-        """
-        N = len(contourPoints)
-
-        phi = np.zeros((N, self.M)) if self.closed else np.zeros((N, self.M + int(self.basis_function.support)))
+        Fit the provided points with the spline using
+        least squares.
 
-        if len(contourPoints.shape) == 1:
-            r = np.zeros(N)
-        elif len(contourPoints.shape) == 2 and (contourPoints.shape[1] == 2):
-            r = np.zeros((N, 2))
-
-        if arcLengthParameterization:
-            dist = [np.linalg.norm(contourPoints[i] - contourPoints[i - 1]) for i in range(1, len(contourPoints))]
-            if self.closed:
-                dist.append(np.linalg.norm(contourPoints[0] - contourPoints[-1]))
-            arclengths = np.hstack(([0], np.cumsum(dist, 0)))
+        Parameters
+        ----------
+        points : numpy.ndarray
+            The data points that should be fit.
+        arc_length_parameterization : bool
+            Whether or not to space the knots based on the distance
+            between the provided points. This is usefull when the
+            points are not equally spaced. Default is `False`.
+        """
+        if len(points) < self.M:
+            raise RuntimeError(
+                "You provided fewer data points than you spline has knots. For the fit to have a unique solution you need to provide at least as many data points as your spline has knots. Consider adding more data or reducing the number of knots M."
+            )
+        if arc_length_parameterization:
+            raise NotImplementedError
         else:
-            if self.closed:
-                samplingRate = int(N / self.M)
-                extraPoints = N % self.M
-            else:
-                samplingRate = int(N / (self.M - 1))
-                extraPoints = N % (self.M - 1)
-
-        for i in range(N):
-            r[i] = contourPoints[i]
-
-            if arcLengthParameterization:
-                if self.closed:
-                    t = arclengths[i] * self.M / arclengths[-1]
-                else:
-                    t = arclengths[i] * (self.M - 1) / arclengths[-1]
-            else:
-                t = i / (samplingRate + 1.0) if i / samplingRate < extraPoints else i / samplingRate
-
-            if self.closed:
-                for k in range(self.M):
-                    tval = self.wrapIndex(t, k)
-                    if tval > -self.halfSupport and tval < self.halfSupport:
-                        basisFactor = self.basis_function.eval(tval)
-                    else:
-                        basisFactor = 0.0
-                    phi[i, k] += basisFactor
-            else:
-                for k in range(self.M + int(self.basis_function.support)):
-                    tval = t - (k - self.halfSupport)
-                    if tval > -self.halfSupport and tval < self.halfSupport:
-                        basisFactor = self.basis_function.eval(tval)
-                    else:
-                        basisFactor = 0.0
-                    phi[i, k] += basisFactor
-
-        if len(contourPoints.shape) == 1:
-            c = np.linalg.lstsq(phi, r, rcond=None)
-
-            if self.closed:
-                self.coeffs = np.zeros([self.M])
-                for k in range(self.M):
-                    self.coeffs[k] = c[0][k]
-            else:
-                self.coeffs = np.zeros([self.M + int(self.basis_function.support)])
-                for k in range(self.M + int(self.basis_function.support)):
-                    self.coeffs[k] = c[0][k]
-
-        elif len(contourPoints.shape) == 2 and contourPoints.shape[1] == 2:
-            cX = np.linalg.lstsq(phi, r[:, 0], rcond=None)
-            cY = np.linalg.lstsq(phi, r[:, 1], rcond=None)
-
-            if self.closed:
-                self.coeffs = np.zeros([self.M, 2])
-                for k in range(self.M):
-                    self.coeffs[k] = np.array([cX[0][k], cY[0][k]])
-            else:
-                self.coeffs = np.zeros([self.M + int(self.basis_function.support), 2])
-                for k in range(self.M + int(self.basis_function.support)):
-                    self.coeffs[k] = np.array([cX[0][k], cY[0][k]])
+            t = np.linspace(0, self.M, len(points) + 1)[:-1] if self.closed else np.linspace(0, self.M - 1, len(points))
+        tval = self._get_tval(t)
+        basis_function_values = self.basis_function.eval(tval, derivative=0)
+        self.coeffs = np.linalg.lstsq(basis_function_values, points, rcond=None)[0]
 
-    def arcLength(self, t0, tf=None):
+    def arc_length(self, stop=None, start=0):
         """
-        Integrate along the arc length.
-
-        Can probably be made faster if the basis functions
-        accept arrays directly.
+        Compute the arc length of the spline between
+        the two parameter value specified. if
 
         Parameters
         ----------
-        t0 : float
+        stop : float (optional)
+            Stop point in parameter space.
+        start : float (optional)
             Start point in parameter space.
-        tf : float (optional)
-            End point in parameter space.
         """
-        if t0 == tf:
-            return 0.0
+        self._check_coeffs()
+        if stop is None:
+            stop = self.M if self.closed else self.M - 1
 
-        if tf is None:
-            tf = self.M if self.closed else self.M - 1
+        if start == stop:
+            return 0
 
-        if t0 > tf:
-            temp = tf
-            tf = t0
-            t0 = temp
+        if start > stop:
+            start, stop = stop, start
 
         integral = scipy.integrate.quad(
-            lambda t: np.linalg.norm(self.eval(t, dt=True)),
-            t0,
-            tf,
+            lambda t: np.linalg.norm(self.eval(t, derivative=1)),
+            start,
+            stop,
             epsabs=1e-6,
             epsrel=1e-6,
             maxp1=50,
             limit=100,
         )
 
         return integral[0]
 
-    def lengthToParameterRecursion(self, s, currentValue, lowerBound, upperBound, precisionDecimals=4):
+    def _length_to_parameter_recursion(self, s, current_value, lower_bound, upper_bound, atol=1e-4):
         """
         Convert the given arc length s on the curve to a value in parameters space.
         This is done recursively, i.e. check if the point is before or after halfway
-        and repeat.
-
-        Some intelegent default can probably be set so the user only has to provide s.
-        Or this function should be made private entirely,
-        because there is :meth:`splinebox.splines.Spline.lengthToParameter`
+        and repeat. It uses binary search.
 
         Parameters
         ----------
         s : float
             Arc length on the spline.
-        currentValue : float
+        current_value : float
             The arc length to the lower bound.
-        lowerBound : float
+        lower_bound : float
             Lower limit in parameter space.
-        upperBound : float
+        upper_bound : float
             Upper limit in parameters space.
-        precisionDecimals : int
-            Precision to which the length is matched.
+        atol : float
+            Absolute precision to which the length is matched.
         """
-        midPoint = lowerBound + (upperBound - lowerBound) / 2
-        midPointLength = currentValue + self.arcLength(lowerBound, midPoint)
+        self._check_coeffs()
+        midpoint = lower_bound + (upper_bound - lower_bound) / 2
+        midpoint_length = current_value + self.arc_length(lower_bound, midpoint)
 
-        if (np.round(currentValue, precisionDecimals) == np.round(midPointLength, precisionDecimals)) or (
-            np.round(s, precisionDecimals) == np.round(midPointLength, precisionDecimals)
-        ):
-            return np.round(midPoint, precisionDecimals)
-
-        elif np.round(s, precisionDecimals) < np.round(midPointLength, precisionDecimals):
-            return self.lengthToParameterRecursion(s, currentValue, lowerBound, midPoint, precisionDecimals)
+        if np.isclose(s, midpoint_length, atol=atol, rtol=0):
+            return midpoint
+        elif s < midpoint_length:
+            return self._length_to_parameter_recursion(s, current_value, lower_bound, midpoint, atol)
         else:
-            return self.lengthToParameterRecursion(s, midPointLength, midPoint, upperBound, precisionDecimals)
+            return self._length_to_parameter_recursion(s, midpoint_length, midpoint, upper_bound, atol)
 
-    def lengthToParameter(self, s):
+    def arc_length_to_parameter(self, s, atol=1e-4):
         """
         Convert the arc length `s` to the coresponding value in parameter space.
 
         Parameters
         ----------
-        s : float
+        s : float or np.array
             Length on curve.
+        atol : float
+            The ablsolute error tolerance.
         """
-        if self.closed:
-            return self.lengthToParameterRecursion(s, 0, 0, self.M)
-        else:
-            return self.lengthToParameterRecursion(s, 0, 0, self.M - 1)
+        self._check_coeffs()
+        if not isinstance(s, np.ndarray):
+            s = np.array([s])
+        sort_indices = np.argsort(s)
+        results = np.zeros_like(s)
+
+        current_value = 0
+        lower_bound = 0
+        upper_bound = self.M if self.closed else self.M - 1
+
+        for i in sort_indices:
+            results[i] = self._length_to_parameter_recursion(s[i], current_value, lower_bound, upper_bound, atol=atol)
+            lower_bound = results[i]
+            current_value = self.arc_length(0, lower_bound)
+
+        return np.squeeze(results)
 
     def sampleArcLength(self, numSamples, dt=False):
         """
         Evaluate the spline equidistantly spaced along its trajectory.
         Perhaps it makes sense to ask the user to provide an array of distances
         instead of the numSamples.
         """
-        if self.coeffs is None:
-            raise RuntimeError(self.noCoefsMessage)
+        self._check_coeffs()
 
         if len(self.coeffs.shape) == 1 or (len(self.coeffs.shape) == 2 and self.coeffs.shape[1] == 2):
             N = numSamples if self.closed else numSamples - 1
-            L = self.arcLength(0)
+            L = self.arc_length()
 
             ts = [0]
             for n in range(1, N):
                 s = n * L / N
                 t = self.lengthToParameter(s)
                 ts.append(t)
             if self.closed:
@@ -439,53 +365,53 @@
         ----------
         t : numpy.array, float
             A 1D numpy array or a single float value.
         derivative : int
             Can be 0, 1, 2 for the spline, and its
             first and second derivative respectively.
         """
-        if self.coeffs is None:
-            raise RuntimeError(self._no_coeffs_msg)
+        self._check_coeffs()
         # Get values at which the basis functions have to be evaluated
         tval = self._get_tval(t)
         basis_function_values = self.basis_function.eval(tval, derivative=derivative)
         value = np.matmul(basis_function_values, self.coeffs)
-        return value
+        return np.squeeze(value)
 
     def _get_tval(self, t):
         """
         This is a helper method for `eval`. It is its own method
         to allow :class:`splinebox.spline_curves.HermiteSpline` to
         overwrite the `eval` method using `_get_tval`.
+        It is also used in :meth:`splinebox.spline_curves.Spline.fit`
         """
         if not isinstance(t, collections.abc.Iterable):
             t = np.array([t])
         if self.closed:
             # all knot indices
             k = np.arange(self.M)
             # output array for the helper function _wrap_index
             tval = np.full((len(t), len(k)), np.nan)
             # compute the positions at which the basis functions have to be evaluated
             # and save them in tval
             self._wrap_index(t, k, self.halfSupport, self.M, tval)
         else:
             # take into account the padding with additional basis functions
             # for non-closed splines
-            k = np.arange(self.M + int(self.basis_function.support))
+            k = np.arange(self.M + 2 * self.pad) - self.pad
             k = k[np.newaxis, :]
             t = t[:, np.newaxis]
             # positions at which the basis functions have to be evaluated
-            tval = t - (k - self.halfSupport)
+            tval = t - k
         return tval
 
     @staticmethod
     @numba.guvectorize(
         [(numba.float64[:], numba.float64[:], numba.float64, numba.int64, numba.float64[:, :])], "(n),(m),(),()->(n,m)"
     )
-    def _wrap_index(ts, ks, halfSupport, M, wrapped_tval):
+    def _wrap_index(ts, ks, halfSupport, M, wrapped_tval):  # pragma: no cover
         """
         Fill the wrapped_tval array whenever a value t
         is affected by the basis function at knot k, taking
         into account that basis functions at the begging/end
         affect positions on the opposite end for closed splines.
         """
         outside_tvalue = halfSupport + 1
@@ -502,55 +428,69 @@
                 elif t > k + halfSupport or t < k - halfSupport:
                     # t is outside the support of the k-th basis function
                     # this can be any value outside the support
                     wrapped_tval[j, i] = outside_tvalue
                 else:
                     wrapped_tval[j, i] = t - k
 
-    def centroid(self):
+    def _coeffs_centroid(self):
         """
-        Does this correspond to the geometric centroid?
-        Probably not, since the coefficient values are used.
-        Why is centroid always 2D? Should there be a check for
-        dimensionality here?
+        Helper method for :meth:`splinebox.spline_curves.Spline.scale`
+        and :meth:`splinebox.spline_curves.Spline.rotate`.
+        Computes the centroid of the coefficients.
         """
-        centroid = np.zeros(2)
+        self._check_coeffs()
+        return np.mean(self.coeffs, axis=0)
 
-        for k in range(self.M):
-            centroid += self.coeffs[k]
-
-        return centroid / self.M
-
-    def translate(self, translationVector):
+    def translate(self, vector):
         """
-        Translates the spline by a vector.
-        Is vector the right name here or can it also be a scalar?
+        Translates the spline by a `vector`.
+
+        Parameters
+        ----------
+        vector : numpy.ndarray
+            Displacement vector added to the coefficients.
         """
-        for k in range(self.M):
-            self.coeffs[k] += translationVector
+        self._check_coeffs()
+        self.coeffs = self.coeffs + vector
 
-    def scale(self, scalingFactor):
+    def scale(self, scaling_factor):
         """
         Enlarge or shrink the spline.
-        This should probably use :meth:`splinebox.splines.Spline.translate`
+        This should probably use :meth:`splinebox.spline_curves.Spline.translate`
         `scalingFactor` can be renamed to `factor`.
         """
-        centroid = self.centroid()
+        self._check_coeffs()
+        centroid = self._coeffs_centroid()
+        self.translate(-centroid)
+        self.coeffs *= scaling_factor
+        self.translate(centroid)
 
-        for k in range(self.M):
-            vectorToCentroid = self.coeffs[k] - centroid
-            self.coeffs[k] = centroid + scalingFactor * vectorToCentroid
-
-    def rotate(self, rotationMatrix):
+    def rotate(self, rotation_matrix, centred=True):
         """
-        Rotate the spline.
-        Should the dimensionality be checked here?
+        Rotate the spline with the provided rotation matrix.
+
+        Parameters
+        ----------
+        rotation_matrix : numpy.ndarray
+            The rotation matrix applied to the spline.
         """
-        for k in range(self.M):
-            self.coeffs[k] = np.matmul(rotationMatrix, self.coeffs[k])
+        self._check_coeffs()
+        if self.coeffs.ndim == 1:
+            raise RuntimeError("1D splines can not be rotated.")
+
+        if centred:
+            centroid = self._coeffs_centroid()
+            self.translate(-centroid)
+
+        for k in range(len(self.coeffs)):
+            self.coeffs[k] = np.matmul(rotation_matrix, self.coeffs[k])
+
+        if centred:
+            self.translate(centroid)
 
 
 class HermiteSpline(Spline):
     """
     Class for the construction of a Hermite spline.
 
     Parameters
@@ -566,31 +506,41 @@
     _coef_tangent_mismatch_msg = "It looks like coeffs and tangents have different shapes."
     _no_tangents_msg = "This spline doesn't have any tangents."
 
     def __init__(self, M, basis_function, closed=False, coeffs=None, tangents=None):
         super().__init__(M, basis_function, closed, coeffs=coeffs)
         self.tangents = tangents
 
+    def _check_coeffs_and_tangents(self):
+        """
+        Most methods require coefficients to be set before they
+        can be used. This helper function checks if the coefficients have been
+        set.
+        """
+        self._check_coeffs()
+        if self.tangents is None:
+            raise RuntimeError(self._no_tangents_msg)
+
     @property
     def tangents(self):
         return self._tangents
 
     @tangents.setter
     def tangents(self, values):
         if values is not None:
             n = len(values)
             if self.closed and n != self.M:
                 raise ValueError(
                     f"The number of tangents must match the number of knots for a closed spline. You provided {n} tangents for a spline with M={self.M} knots."
                 )
             support = self.basis_function.support
-            padded_M = int(self.M + support)
+            padded_M = self.M + 2 * self.pad
             if not self.closed and n != padded_M:
                 raise ValueError(
-                    f"Non-closed splines are padded at the ends with additional knots, i.e. the effective number of knots is M + support of the basis function. You provided {n} tangents for a spline with M={self.M} and a basis function with support={support}, expected {padded_M}."
+                    f"Non-closed splines are padded at the ends with additional knots, i.e. the effective number of knots is M + 2 * (ceil(support / 2) - 1) of the basis function. You provided {n} tangents for a spline with M={self.M} and a basis function with support={support}, expected {padded_M}."
                 )
         self._tangents = values
 
     @property
     def basis_function(self):
         return self._basis_function
 
@@ -598,127 +548,56 @@
     def basis_function(self, value):
         if not value.multigenerator:
             raise ValueError(
                 "It looks like you are trying to use a single generator to build a multigenerator spline model."
             )
         self._basis_function = value
 
-    def getCoefsFromKnots(self, knots, tangentAtKnots):
-        knots = np.array(knots)
-        tangentAtKnots = np.array(tangentAtKnots)
-
-        if knots.shape != tangentAtKnots.shape:
-            raise RuntimeError(self.coefTangentMismatchMessage)
-
-        if len(knots.shape) == 1:
-            self.coeffs = knots
-            self.tangents = tangentAtKnots
-        elif len(knots.shape) == 2:
-            if knots.shape[1] == 2:
-                self.coeffs = knots
-                self.tangents = tangentAtKnots
-            else:
-                raise RuntimeError(self._wrong_dimension_msg)
-        else:
-            raise RuntimeError(self._wrong_array_size_msg)
-
-    def getCoefsFromDenseContour(self, contourPoints, arcLengthParameterization=False):
-        N = len(contourPoints)
-        phi = np.zeros((N, 2 * self.M))
-
-        if len(contourPoints.shape) == 1:
-            r = np.zeros(N)
-        elif len(contourPoints.shape) == 2 and (contourPoints.shape[1] == 2):
-            r = np.zeros((N, 2))
-
-        if arcLengthParameterization:
-            dist = [np.linalg.norm(contourPoints[i] - contourPoints[i - 1]) for i in range(1, len(contourPoints))]
-            if self.closed:
-                dist.append(np.linalg.norm(contourPoints[0] - contourPoints[-1]))
-            arclengths = np.hstack(([0], np.cumsum(dist, 0)))
+    def fit(self, points, arc_length_parameterization=False):
+        if len(points) < self.M:
+            raise RuntimeError(
+                "You provided fewer data points than you spline has knots. For the fit to have a unique solution you need to provide at least as many data points as your spline has knots. Consider adding more data or reducing the number of knots M."
+            )
+        if arc_length_parameterization:
+            raise NotImplementedError
         else:
-            if self.closed:
-                samplingRate = int(N / self.M)
-                extraPoints = N % self.M
-            else:
-                samplingRate = int(N / (self.M - 1))
-                extraPoints = N % (self.M - 1)
-
-        for i in range(N):
-            r[i] = contourPoints[i]
-
-            if arcLengthParameterization:
-                if self.closed:
-                    t = arclengths[i] * self.M / arclengths[-1]
-                else:
-                    t = arclengths[i] * (self.M - 1) / arclengths[-1]
-            else:
-                if i == 0:
-                    t = 0
-                elif t < extraPoints:
-                    t += 1.0 / (samplingRate + 1.0)
-                else:
-                    t += 1.0 / samplingRate
-
-            for k in range(self.M):
-                tval = self.wrapIndex(t, k) if self.closed else t - k
-                if tval > -self.halfSupport and tval < self.halfSupport:
-                    basisFactor = self.basis_function.eval(tval)
-                else:
-                    basisFactor = [0.0, 0.0]
-
-                phi[i, k] += basisFactor[0]
-                phi[i, k + self.M] += basisFactor[1]
-
-        if len(contourPoints.shape) == 1:
-            c = np.linalg.lstsq(phi, r, rcond=None)
-
-            self.coeffs = np.zeros([self.M])
-            self.tangents = np.zeros([self.M])
-            for k in range(self.M):
-                self.coeffs[k] = c[0][k]
-                self.tangents[k] = c[0][k + self.M]
-
-        elif len(contourPoints.shape) == 2 and (contourPoints.shape[1] == 2):
-            cX = np.linalg.lstsq(phi, r[:, 0], rcond=None)
-            cY = np.linalg.lstsq(phi, r[:, 1], rcond=None)
-
-            self.coeffs = np.zeros([self.M, 2])
-            self.tangents = np.zeros([self.M, 2])
-            for k in range(self.M):
-                self.coeffs[k] = np.array([cX[0][k], cY[0][k]])
-                self.tangents[k] = np.array([cX[0][k + self.M], cY[0][k + self.M]])
+            t = np.linspace(0, self.M, len(points) + 1)[:-1] if self.closed else np.linspace(0, self.M - 1, len(points))
+        tval = self._get_tval(t)
+        basis_function_values = self.basis_function.eval(tval, derivative=0)
+        basis_function_values = np.concatenate([basis_function_values[0], basis_function_values[1]], axis=1)
+        half = self.M if self.closed else self.M + 2 * self.pad
+        solution = np.linalg.lstsq(basis_function_values, points, rcond=None)[0]
+        self.coeffs = solution[:half]
+        self.tangents = solution[half:]
 
     def eval(self, t, derivative=0):
         """
         Evalute the spline or one of its derivatives at
         parameter value(s) `t`.
 
         Parameters
         ----------
         t : numpy.array, float
             A 1D numpy array or a single float value.
         derivative : int
             Can be 0, 1, 2 for the spline, and its
             first and second derivative respectively.
         """
-        if self.coeffs is None:
-            raise RuntimeError(self._no_coeffs_msg)
-        if self.tangents is None:
-            raise RuntimeError(self._no_tangents_msg)
+        self._check_coeffs_and_tangents()
 
         tval = self._get_tval(t)
         basis_function_values = self.basis_function.eval(tval, derivative=derivative)
-        value = np.matmul(basis_function_values, self.coeffs) + np.matmul(basis_function_values, self.tangents)
+        value = np.matmul(basis_function_values[0], self.coeffs) + np.matmul(basis_function_values[1], self.tangents)
         return value
 
-    def scale(self, scalingFactor):
-        Spline.scale(self, scalingFactor)
+    def scale(self, scaling_factor):
+        self._check_coeffs_and_tangents()
+        Spline.scale(self, scaling_factor)
+        self.tangents *= scaling_factor
 
-        for k in range(self.M):
-            self.tangents[k] *= scalingFactor
+    def rotate(self, rotation_matrix, centred=True):
+        self._check_coeffs_and_tangents()
 
-    def rotate(self, rotationMatrix):
-        Spline.rotate(self, rotationMatrix)
+        Spline.rotate(self, rotation_matrix, centred=centred)
 
-        for k in range(self.M):
-            self.tangents[k] = np.matmul(rotationMatrix, self.tangents[k])
+        for k in range(len(self.tangents)):
+            self.tangents[k] = np.matmul(rotation_matrix, self.tangents[k])
```

### Comparing `splinebox-0.0.1a0/src/splinebox.egg-info/PKG-INFO` & `splinebox-0.0.2a0/src/splinebox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splinebox
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: A python package for fitting splines.
 Author-email: Florian Aymanns <florian.aymanns@epfl.ch>, Virginie Uhlmann <uhlmann@ebi.ac.uk>, Edward Andò <edward.ando@epfl.ch>
 Maintainer-email: Florian Aymanns <flroian.aymanns@epfl.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, EPFL Center for Imaging
         
@@ -57,14 +57,16 @@
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
+Requires-Dist: scikit-image; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
 
 <img style="float: right;" src="https://imaging.epfl.ch/resources/logo-for-gitlab.svg">
 
 # splinebox
 A python package for fitting splines.
 Developed by the [EPFL Center for Imaging](https://imaging.epfl.ch/) as part of a collaboration with the [Uhlmann Group at EMBL-EBI](https://www.ebi.ac.uk/research/uhlmann/) in Feb 2024.
```

### Comparing `splinebox-0.0.1a0/tests/test_basis_functions.py` & `splinebox-0.0.2a0/tests/test_basis_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import math
+
 import numpy as np
 import pytest
 import splinebox.basis_functions
 
 
 def test_base_class_eval(derivative):
     basis_function = splinebox.basis_functions.BasisFunction(False, 2)
@@ -24,37 +26,27 @@
 def test_filters(basis_function, is_interpolating, knot_gen):
     s = knot_gen()
     if is_interpolating(basis_function):
         assert np.allclose(basis_function.filter_symmetric(s), s)
         assert np.allclose(basis_function.filter_periodic(s), s)
 
 
-def test_derivatives(basis_function, derivative):
+def test_derivatives(basis_function, derivative, not_differentiable_twice):
     if derivative == 0:
         return
 
     support = basis_function.support
     x = np.linspace(-support / 2 - 1, support / 2 + 1, 100000)
     y = basis_function.eval(x, derivative=derivative - 1)
 
     dx = np.diff(x)
     dy = np.diff(y)
     estimated_derivative = dy / dx
 
-    if (
-        isinstance(
-            basis_function,
-            (
-                splinebox.basis_functions.B1,
-                splinebox.basis_functions.CubicHermite,
-                splinebox.basis_functions.ExponentialHermite,
-            ),
-        )
-        and derivative == 2
-    ):
+    if not_differentiable_twice(basis_function) and derivative == 2:
         # B1, CubicHermite, and ExponentialHermite basis functions are not differentiable twice.
         with pytest.raises(RuntimeError):
             basis_function.eval(x[:-1] + dx / 2, derivative=2)
     else:
         # Check where the estimated derivative is close to the
         # derivative value returned by the method
         close = np.isclose(
@@ -71,7 +63,21 @@
             # the output of CubicHermite and ExponentialHermite basis functions is 2D
             for i in range(2):
                 close[i] = np.convolve(close[i], kernel, mode="same")
         else:
             close = np.convolve(close, kernel, mode="same")
 
         assert np.all(close > 0)
+
+
+def test_partition_of_unity(basis_function):
+    support = math.ceil(basis_function.support)
+    x = np.linspace(0, 1, 10000)
+    summed = np.zeros_like(x)
+    for k in range(-support, support):
+        vals = basis_function.eval(x - k)
+        if basis_function.multigenerator:
+            vals = vals[0]
+        if vals.ndim == 2:
+            vals = vals[:, 0]
+        summed += vals
+    assert np.allclose(summed, np.ones_like(summed))
```

