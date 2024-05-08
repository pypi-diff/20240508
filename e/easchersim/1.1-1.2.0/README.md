# Comparing `tmp/easchersim-1.1.tar.gz` & `tmp/easchersim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easchersim-1.1.tar", last modified: Thu Feb  3 03:41:32 2022, max compression
+gzip compressed data, was "easchersim-1.2.0.tar", last modified: Wed May  8 21:05:17 2024, max compression
```

## Comparing `easchersim-1.1.tar` & `easchersim-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.270467 easchersim-1.1/
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-02-03 03:40:52.000000 easchersim-1.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      226 2022-02-03 03:40:52.000000 easchersim-1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-02-03 03:40:52.000000 easchersim-1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1522 2022-02-03 03:40:52.000000 easchersim-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3531 2022-02-03 03:41:32.270467 easchersim-1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2761 2022-02-03 03:40:52.000000 easchersim-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.261467 easchersim-1.1/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.261467 easchersim-1.1/docs/UserGuide/
--rw-rw-rw-   0 root         (0) root         (0)    11039 2022-02-03 03:40:52.000000 easchersim-1.1/docs/UserGuide/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.263467 easchersim-1.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    14461 2022-02-03 03:40:52.000000 easchersim-1.1/docs/_static/GSSI_logo.jpeg
--rw-rw-rw-   0 root         (0) root         (0)    23392 2022-02-03 03:40:52.000000 easchersim-1.1/docs/_static/PennStateLogo.jpeg
--rw-rw-rw-   0 root         (0) root         (0)   305491 2022-02-03 03:40:52.000000 easchersim-1.1/docs/_static/UChicago_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   422272 2022-02-03 03:40:52.000000 easchersim-1.1/docs/_static/usage_demo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.264467 easchersim-1.1/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)     2749 2022-02-03 03:40:52.000000 easchersim-1.1/docs/_templates/footer.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.264467 easchersim-1.1/docs/api/
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-02-03 03:40:52.000000 easchersim-1.1/docs/api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3242 2022-02-03 03:40:52.000000 easchersim-1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2022-02-03 03:40:52.000000 easchersim-1.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-02-03 03:40:52.000000 easchersim-1.1/docs/requirements
--rw-rw-rw-   0 root         (0) root         (0)      687 2022-02-03 03:40:52.000000 easchersim-1.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.264467 easchersim-1.1/recipe/
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-02-03 03:40:52.000000 easchersim-1.1/recipe/conda_build_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2022-02-03 03:40:52.000000 easchersim-1.1/recipe/meta.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1309 2022-02-03 03:41:32.273468 easchersim-1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.260467 easchersim-1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.266467 easchersim-1.1/src/easchersim/
--rw-rw-rw-   0 root         (0) root         (0)     2810 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    11151 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/atmosphere.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/cher_func.py
--rw-rw-rw-   0 root         (0) root         (0)     2614 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.270467 easchersim-1.1/src/easchersim/data/
--rw-rw-rw-   0 root         (0) root         (0)   806059 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/data/Example_CORSIKA_proton_1e17eV.long
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10186 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/data/alpha_values_typical_atmosphere_updated.txt
--rw-rw-rw-   0 root         (0) root         (0)     1909 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/data/default_conf.ini
--rw-rw-rw-   0 root         (0) root         (0)    13953 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/eas_cher_sim.py
--rw-rw-rw-   0 root         (0) root         (0)    17167 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/electron_func.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/fit_func.py
--rw-rw-rw-   0 root         (0) root         (0)    10410 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)    13120 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/io_func.py
--rw-rw-rw-   0 root         (0) root         (0)    12022 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    24249 2022-02-03 03:40:52.000000 easchersim-1.1/src/easchersim/spatial_cherenkov_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 03:41:32.268467 easchersim-1.1/src/easchersim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3531 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1165 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 03:41:31.000000 easchersim-1.1/src/easchersim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       71 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-02-03 03:41:32.000000 easchersim-1.1/src/easchersim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.523588 easchersim-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-05-08 21:04:57.000000 easchersim-1.2.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-08 21:04:57.000000 easchersim-1.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2024-05-08 21:04:57.000000 easchersim-1.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-08 21:04:57.000000 easchersim-1.2.0/CHANGELOG
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-08 21:04:57.000000 easchersim-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-05-08 21:05:17.523588 easchersim-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2024-05-08 21:04:57.000000 easchersim-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.515588 easchersim-1.2.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.515588 easchersim-1.2.0/docs/UserGuide/
+-rw-rw-rw-   0 root         (0) root         (0)    12323 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/UserGuide/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.516588 easchersim-1.2.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    14461 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/_static/GSSI_logo.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)    23392 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/_static/PennStateLogo.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)   305491 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/_static/UChicago_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   422272 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/_static/usage_demo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.517588 easchersim-1.2.0/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2749 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/_templates/footer.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.517588 easchersim-1.2.0/docs/api/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/api/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-08 21:04:57.000000 easchersim-1.2.0/docs/requirements
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-08 21:04:57.000000 easchersim-1.2.0/my_config_file.ini
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-05-08 21:04:57.000000 easchersim-1.2.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.517588 easchersim-1.2.0/recipe/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-08 21:04:57.000000 easchersim-1.2.0/recipe/conda_build_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-08 21:04:57.000000 easchersim-1.2.0/recipe/meta.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-08 21:05:17.523588 easchersim-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.512588 easchersim-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.520588 easchersim-1.2.0/src/easchersim/
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11159 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/atmosphere.py
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/cher_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.522588 easchersim-1.2.0/src/easchersim/data/
+-rw-rw-rw-   0 root         (0) root         (0)   806059 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/data/Example_CORSIKA_proton_1e17eV.long
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10186 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/data/alpha_values_typical_atmosphere_updated.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/data/default_conf.ini
+-rw-rw-rw-   0 root         (0) root         (0)    15652 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/eas_cher_sim.py
+-rw-rw-rw-   0 root         (0) root         (0)    25271 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/electron_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/fit_func.py
+-rw-rw-rw-   0 root         (0) root         (0)    10492 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    15808 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/io_func.py
+-rw-rw-rw-   0 root         (0) root         (0)    12235 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    30414 2024-05-08 21:04:57.000000 easchersim-1.2.0/src/easchersim/spatial_cherenkov_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:17.523588 easchersim-1.2.0/src/easchersim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-08 21:05:17.000000 easchersim-1.2.0/src/easchersim.egg-info/top_level.txt
```

### Comparing `easchersim-1.1/.gitlab-ci.yml` & `easchersim-1.2.0/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -61,15 +61,15 @@
   stage: deploy
   image: continuumio/miniconda3:latest
   before_script: []
   script:
     - conda config --append channels conda-forge
     - conda install conda-build anaconda-client conda-verify
     - conda build --no-anaconda-upload --output-folder=dist/ recipe/
-    - conda install -c $PWD/dist easchersim
+    - conda create -n dummy -c $PWD/dist easchersim
     - conda convert --platform osx-64 dist/linux-64/easchersim* -o dist/
     - anaconda -t "$ANACONDA_TOKEN" upload -u easchersim dist/*/*.tar.bz2
 
   only:
     - tags
 
 pages:
```

### Comparing `easchersim-1.1/LICENSE` & `easchersim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/PKG-INFO` & `easchersim-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: easchersim
-Version: 1.1
+Version: 1.2.0
 Summary: A Simulator for Cherenkov photon production and atmopheric transport for Extensive Air Showers
 Home-page: https://gitlab.com/c4341/easchersim
 Author: Austin Cummings, Johannes Eser
 Author-email: alc6658@psu.edu, jeser@uchicago.edu
 License: BSD-3-Clause-Clear
 Keywords: Extensive Air Shower,Cherenkov,neutrinos,Simulation
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: importlib_resources
+Requires-Dist: matplotlib-label-lines
+Requires-Dist: rich
 
 # EASCherSim
 
 ![GitLab Release (latest by date)](https://img.shields.io/gitlab/v/release/c4341/easchersim)
 [![PyPI](https://img.shields.io/pypi/v/easchersim)](https://pypi.org/project/easchersim/)
 [![Conda](https://img.shields.io/conda/v/easchersim/easchersim)](https://anaconda.org/easchersim/easchersim)
 [![pipeline status](https://gitlab.com/c4341/easchersim/badges/main/pipeline.svg)](https://gitlab.com/c4341/easchersim/-/commits/main)
@@ -95,9 +100,7 @@
 # Download & Build
 
 ### Clone the Repository (for development)
 
 1. `git clone https://gitlab.com/c4341/easchersim.git`
 2. `cd easchersim`
 3. `python3 -m pip install -e .`
-
-
```

### Comparing `easchersim-1.1/README.md` & `easchersim-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/UserGuide/index.rst` & `easchersim-1.2.0/docs/UserGuide/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -50,32 +50,35 @@
 .. code-block:: none
 
     $ easchersim make-config -h
 
     usage: easchersim make-config [OPTIONS] CONFIGFILE
 
     OPTIONS:
-    -h, --help            show this help message and exit
-    --det-alt DET_ALT     Set detection plane altitude in km
-    -e ENG, --energy ENG  Set shower energy in eV
-    -a ANGLE GEOMETRY-DEF, --angle ANGLE GEOMETRY-DEF
+      -h, --help            show this help message and exit
+      --det-alt DET_ALT     Set detection plane altitude in km
+      -e ENG, --energy ENG  Set shower energy in eV
+      -a ANGLE GEOMETRY-DEF, --angle ANGLE GEOMETRY-DEF
                             Set shower angle and geometry definition (viewing/emergence)
-    -d FIRST_INTERACTION_DISTANCE DISTANCE-DEF, --dist-first-int FIRST_INTERACTION_DISTANCE DISTANCE-DEF
+      -X0 X0                Set starting grammage (X0) in g/cm^2
+      -d FIRST_INTERACTION_DISTANCE DISTANCE-DEF, --dist-first-int FIRST_INTERACTION_DISTANCE DISTANCE-DEF
                             Set distance to first interaction (linear distance/altitude(only for below limb events))
-    -s {yes,no,on,off}, --scattering {yes,no,on,off}
+      -s {yes,no,on,off}, --scattering {yes,no,on,off}
                             Turn atmospheric scattering on/off
-    -m {yes,no,on,off}, --use-mag-field {yes,no,on,off}
+      -m {yes,no,on,off}, --use-mag-field {yes,no,on,off}
                             Turn magnetic field on/off
-    -g {yes,no,on,off}, --use-greisen {yes,no,on,off}
+      -g {yes,no,on,off}, --use-greisen {yes,no,on,off}
                             Use Greisen parametrization for longitudianal profile instead of CORSIKA file
-    -o OUTPUT_NAME, --output OUTPUT_NAME
+      --lat_dist {Lafebre,NKG}
+                            Choice of parameterization of lateral distribution of electrons
+      -o OUTPUT_NAME, --output OUTPUT_NAME
                             Name of the output file. Supported formats are root, npz
-    -p {none,basic,general,all}, --plots {none,basic,general,all}
+      -p {none,basic,general,all}, --plots {none,basic,general,all}
                             Set the type of plots to be created
-    --save-plots          Set the type of plots to be created
+      --save-plots          Set the type of plots to be created
 
 Run cherenkov simulation
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 Simulate cherenkov photons at detection plane and save plots to disk
 
 .. code-block:: bash
@@ -88,23 +91,26 @@
 .. code-block:: none
 
     $ easchersim run -h
     
     usage: easchersim run [OPTIONS] CONFIGFILE
 
     OPTIONS:
-    -h, --help            show this help message and exit
-    -e ENG, --energy ENG  Set shower energy in eV
-    -a ANGLE GEOMETRY-DEF, --angle ANGLE GEOMETRY-DEF
-                            Set shower angle and geometry definition (viewing/emergence)
-    -d FIRST_INTERACTION_DISTANCE DISTANCE-DEF, --dist-first-int FIRST_INTERACTION_DISTANCE DISTANCE-DEF
-                            Set distance to first interaction (linear distance/altitude(only for below limb events))
-    --save-plots          Set the type of plots to be created
-    -o OUTPUT_NAME, --output OUTPUT_NAME
-                        Name of the output file. Supported formats are root, npz
+      -h, --help            show this help message and exit
+      -e ENG, --energy ENG  Set shower energy in eV
+      -a ANGLE GEOMETRY-DEF, --angle ANGLE GEOMETRY-DEF
+                             Set shower angle and geometry definition (viewing/emergence)
+      -d FIRSTINTERACTIONDISTANCE DISTANCE-DEF, --dist-first-int FIRSTINTERACTIONDISTANCE DISTANCE-DEF
+                             Set distance to first interaction
+      -X0 X0                 Set starting grammage (X0) in g/cm^2
+      --save-plots           Set the type of plots to be created
+      -o OUTPUT_NAME, --output OUTPUT_NAME
+                             Name of the output file. Supported formats are root, npz
+      -i INPUT-FILE SHOWER-INDEX, --input INPUT-FILE SHOWER-INDEX
+                             Name of the input file. Only CORSIKA showers supported
 
 Output files
 ------------
 There are two types of output files that can be generated by EASCherSim. We support the Cern ROOT format as well as 
 a the .npz file format to store the simulation results.
 
 .npz format
@@ -116,88 +122,98 @@
 * *wavelengths*: wavelength bin edges
 * *wavelength_counts*: photon count in each wavelength bin
 * *dist_bins*: distance bin edges
 * *dist_counts*: photon count in each distance bin
 * *time_bins*: timing bin edges
 * *time_counts*: photon count per distance bin in each time bin (arr[dist][time])
 * *time_offset*: time offset to be added for each distance bin
-* *angle_bins*: angular bin edges
-* *angle_counts*: photon count per distance bin in each angular bin (arr[dist][ang])
-* *angle_offset*: angular offset to be added for each distance bin
+* *phZenith_bins*: Zenith angular bin edges
+* *phZenith_counts*: photon count per distance bin in each Zenith bin (arr[dist][zen])
+* *phZenith_offset*: Zenith offset to be added for each distance bin
+* *phAzi_bins*: Azimuth angular bin edges
+* *phAzi_counts*: photon count per distance bin in each Azimuth bin (arr[dist][azi])
 
 Example how to access array from .npz file:
 
 .. code-block:: python
         
     import numpy as np
 
     npzfile = np.load("outfile.npz")
     npzfile.files
-    >>>>['shower_prop', 'wavelengths', 'wavelength_counts', 'dist_bins', 'dist_counts', 'time_bins', 'time_counts', 'time_offset', 'angle_bins', 'angle_counts', 'angle_offset']
+    >>>>['shower_prop', 'wavelengths', 'wavelength_counts', 'dist_bins', 'dist_counts', 'time_bins', 'time_counts', 'time_offset', 'phZenith_bins', 'phZenith_counts', 'phZenith_offset', 'phAzi_bins', 'phAzi_counts', 't_counts']
         
     npzfile['shower_prop']
-    >>>>[1.0e+17 8.5e+01 0.0e+00]
+    >>>>[1.0e+17 8.5e+01 0.0e+00, 0.0e+00]
 
 ROOT format
 ^^^^^^^^^^^
 In the ROOT file you can find two TTrees. **cherPhProp** contains the simulation results while **showerProp** holds 
 the shower properties (energy, angle and distance to first interaction) used in the simulation.
 
 .. tabs::
 
     .. code-tab:: bash showerProp
 
         ******************************************************************************
         *Tree    :showerProp: Shower Properties                                      *
-        *Entries :        1 : Total =            2129 bytes  File  Size =        808 *
+        *Entries :        1 : Total =            2703 bytes  File  Size =        987 *
         *        :          : Tree compression factor =   1.00                       *
         ******************************************************************************
         *Br    0 :energy    : eng/D                                                  *
         *Entries :        1 : Total  Size=        575 bytes  File Size  =         87 *
         *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.00     *
         *............................................................................*
         *Br    1 :zenith    : zen/D                                                  *
         *Entries :        1 : Total  Size=        575 bytes  File Size  =         87 *
         *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.00     *
         *............................................................................*
-        *Br    2 :startalt  : startalt/D                                             *
-        *Entries :        1 : Total  Size=        594 bytes  File Size  =         89 *
+        *Br    2 :startdist : startdist/D                                            *
+        *Entries :        1 : Total  Size=        599 bytes  File Size  =         90 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.00     *
+        *............................................................................*
+        *Br    3 :X0        : X0/D                                                   *
+        *Entries :        1 : Total  Size=        564 bytes  File Size  =         83 *
         *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.00     *
         *............................................................................*
 
     .. code-tab:: bash cherPhProp
 
         ******************************************************************************
         *Tree    :cherPhProp: Cherenkov Photon Properties                            *
-        *Entries :        1 : Total =          756226 bytes  File  Size =     114166 *
-        *        :          : Tree compression factor =   6.65                       *
+        *Entries :        1 : Total =         6210816 bytes  File  Size =    3044722 *
+        *        :          : Tree compression factor =   2.04                       *
         ******************************************************************************
         *Br    0 :wavelength : TH1D                                                  *
-        *Entries :        1 : Total  Size=       2742 bytes  File Size  =       1740 *
+        *Entries :        1 : Total  Size=       2742 bytes  File Size  =       1738 *
         *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.28     *
         *............................................................................*
         *Br    1 :distance  : TH1D                                                   *
-        *Entries :        1 : Total  Size=       2729 bytes  File Size  =       1653 *
-        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.35     *
+        *Entries :        1 : Total  Size=       4329 bytes  File Size  =       3023 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.27     *
         *............................................................................*
         *Br    2 :time_offset : TH1D                                                 *
-        *Entries :        1 : Total  Size=       2751 bytes  File Size  =       1684 *
-        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.33     *
+        *Entries :        1 : Total  Size=       4351 bytes  File Size  =       3007 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.28     *
         *............................................................................*
-        *Br    3 :angle_offset : TH1D                                                *
-        *Entries :        1 : Total  Size=       2759 bytes  File Size  =       1677 *
-        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.34     *
+        *Br    3 :phZenith_offset : TH1D                                             *
+        *Entries :        1 : Total  Size=       4382 bytes  File Size  =       3010 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.28     *
         *............................................................................*
         *Br    4 :time_dist : vector<TH1D>                                           *
-        *Entries :        1 : Total  Size=     372136 bytes  File Size  =      10335 *
-        *Baskets :        1 : Basket Size=      32000 bytes  Compression=  35.96     *
+        *Entries :        1 : Total  Size=     747634 bytes  File Size  =     302507 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   2.47     *
         *............................................................................*
-        *Br    5 :angle_dist : vector<TH1D>                                          *
-        *Entries :        1 : Total  Size=     372438 bytes  File Size  =      96107 *
-        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   3.87     *
+        *Br    5 :phZenith_dist : vector<TH1D>                                       *
+        *Entries :        1 : Total  Size=     749843 bytes  File Size  =     245904 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   3.05     *
+        *............................................................................*
+        *Br    6 :phAzimuth_dist : vector<TH1D>                                      *
+        *Entries :        1 : Total  Size=    4696814 bytes  File Size  =    2484447 *
+        *Baskets :        1 : Basket Size=      32000 bytes  Compression=   1.89     *
         *............................................................................*
 
 For the vector variables each entry represents the corresponding distance bin.
 Examples of how to read the photon properties and show the distribution for a given distance bin. 
 First in C++ syntax and second using pyroot.
 
 .. tabs::
```

### Comparing `easchersim-1.1/docs/_static/GSSI_logo.jpeg` & `easchersim-1.2.0/docs/_static/GSSI_logo.jpeg`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/_static/PennStateLogo.jpeg` & `easchersim-1.2.0/docs/_static/PennStateLogo.jpeg`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/_static/UChicago_logo.png` & `easchersim-1.2.0/docs/_static/UChicago_logo.png`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/_static/usage_demo.svg` & `easchersim-1.2.0/docs/_static/usage_demo.svg`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/_templates/footer.html` & `easchersim-1.2.0/docs/_templates/footer.html`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/conf.py` & `easchersim-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/docs/index.rst` & `easchersim-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/pyproject.toml` & `easchersim-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/recipe/meta.yaml` & `easchersim-1.2.0/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/setup.cfg` & `easchersim-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/__init__.py` & `easchersim-1.2.0/src/easchersim/__init__.py`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/atmosphere.py` & `easchersim-1.2.0/src/easchersim/atmosphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,18 +270,18 @@
 
     wavelength_bins, altitude_bins = np.meshgrid(wavelength_bins, altitude_bins)
 
     # 2D interpolation of the extinction coefficients
     # If Rayleigh_flag == True, above 50km, consider ONLY Rayleigh scattering
     # If False, no scattering above 50km
     if Rayleigh_flag:
-        extinction_coefficients = np.where(altitude_bins > 50, rayleigh_extinction_coefficient(altitude_bins[:, 0], wavelength_bins[0]), np.exp(griddata((data_wavelength.flatten(), data_altitude.flatten()), data_extinction_coefficients.flatten(), (wavelength_bins, altitude_bins), method='cubic', fill_value=0)))
+        extinction_coefficients = np.where(altitude_bins > 50, rayleigh_extinction_coefficient(altitude_bins[:, 0], wavelength_bins[0]), np.exp(griddata((data_wavelength.flatten(), data_altitude.flatten()), data_extinction_coefficients.flatten(), (wavelength_bins, altitude_bins), method='cubic', fill_value = -20)))
         extinction_coefficients[altitude_bins > const.alt_max] = 0
     else:
-        extinction_coefficients = np.exp(griddata((data_wavelength.flatten(), data_altitude.flatten()), data_extinction_coefficients.flatten(), (wavelength_bins, altitude_bins), method='cubic', fill_value=0))
+        extinction_coefficients = np.exp(griddata((data_wavelength.flatten(), data_altitude.flatten()), data_extinction_coefficients.flatten(), (wavelength_bins, altitude_bins), method='cubic', fill_value = -20))
         extinction_coefficients[altitude_bins > 50] = 0
 
     # Cumulatively integrate the extinction coefficients along the trajectory
     optical_depth = -integrate.cumtrapz(extinction_coefficients.T, L_bins * 1e3, axis=1, initial=0)
     optical_depth = np.flip(optical_depth, axis=1)
 
     return optical_depth
```

### Comparing `easchersim-1.1/src/easchersim/cher_func.py` & `easchersim-1.2.0/src/easchersim/cher_func.py`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/constants.py` & `easchersim-1.2.0/src/easchersim/constants.py`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/data/Example_CORSIKA_proton_1e17eV.long` & `easchersim-1.2.0/src/easchersim/data/Example_CORSIKA_proton_1e17eV.long`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/data/alpha_values_typical_atmosphere_updated.txt` & `easchersim-1.2.0/src/easchersim/data/alpha_values_typical_atmosphere_updated.txt`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/data/default_conf.ini` & `easchersim-1.2.0/src/easchersim/data/default_conf.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 [shower]
 # shower energy in eV
 energy: 1e17
 # shower and geometry definition (viewing or emergence angle)
 angle: 0, viewing
+# grammage to the first interaction in g/cm^2
+X0: 0
 # distance to the first interaction in km
 distFirstInteraction: 0., distance
 
 [runSettings]
 numShowers: 1
 # use Geiseren parametrization for profile or CORSIKA
 useGreisenParametrization: no
+# use NKG parameterization for lateral distribution of electrons
+lat_dist: NKG
 # proto shower for longitudial profile(CORSIKA.long file)
-protoShowerPofile:
+protoShowerProfile:
 # energy of proto shower (CORSIKA.long file)
 protoShowerEnergy: 1.e17
 # slant depth bins: number of bins , upper value (in g/cm^2: starts at 0)
 slantDepth: 1000, 2000.
 # wavelength: number of bins, lower (in nm), upper (in nm)
 wavelength: 100, 270., 1000.
 # electron energy bins: number of bins (log space), upper value (in MeV: starts at the Cherenkov threshold)
 elEnergy: 30, 1e5
 # electron zenith bins: number of bins (log space), log10(lower value), log10(upper value) (scaled values, see A.M. Hillas. Air. J. Phys. G, 8:1461-1473, 1982)
 elZenith: 200, -4., 1.
 # azimuth bins about the Cherenkov ring: number of bins (from 0 to 2pi)
 ringAzimuthNumBin: 50
 # photon spatial bins: number of bins, percentile of total photon data to capture
-phSpatial: 100, 10.
+phSpatial: 200, 50.
 # photon zenith bins: number of bins, log10(lower value), log10(upper value) (in degrees)
 phZenith: 200, -3., 2.
 # photon timing bins: number of bins, log10(lower value), log10(upper value) (in ns)
 phTime: 200, -1., 4.
+# photon azimuth bins: number of bins, lower value, upper value (in degrees)
+phAzimuth: 1440, -180, 180
 
 [detector]
 # detection plane height in km
 altitude: 33.
 
 [atmosphere]
 # turn atmospheric scattering on/off
```

### Comparing `easchersim-1.1/src/easchersim/eas_cher_sim.py` & `easchersim-1.2.0/src/easchersim/eas_cher_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # The Clear BSD License
 #
 # Copyright (c) 2021 Austin Cummings
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted (subject to the limitations in the disclaimer
@@ -51,15 +50,14 @@
 
 from . import io_func
 from . import plot
 from . import geometry as geo
 from . import constants as const
 from . import spatial_cherenkov_profile as sp_cher_prof
 
-
 def cli():
     """Command line interface
 
     Returns
     -------
     parser Obj
         command line arguments
@@ -90,25 +88,35 @@
                          )
     run_par.add_argument('-d', '--dist-first-int',
                          nargs=2,
                          metavar=("FIRSTINTERACTIONDISTANCE", "DISTANCE-DEF"),
                          dest='distFirstInt',
                          help='Set distance to first interaction'
                          )
+    run_par.add_argument('-X0',
+                         type=float,
+                         dest='X0',
+                         help='Set starting grammage (X0) in g/cm^2'
+                         )
     run_par.add_argument('--save-plots',
                           dest='savefig',
                           action='store_true',
                           help='Set the type of plots to be created'
                           )
     run_par.add_argument('-o', '--output',
                           type=str,
-                          default='',
                           dest='output_name',
                           help='Name of the output file. Supported formats are root, npz'
                           )
+    run_par.add_argument('-i', '--input',
+                         nargs=2,
+                         metavar=("INPUT-FILE", "SHOWER-INDEX"),
+                         dest='input_name',
+                         help='Name of the input file. Only CORSIKA showers supported'
+                         )
     run_par.set_defaults(func=run)
 
     # create the configuration file
     make_cfg = subparsers.add_parser('make-config',
                                      help='Produce configuration file from default \
                                      and/or given parameters.',
                                      prog='easchersim make-config',
@@ -133,14 +141,20 @@
     make_cfg.add_argument('-a', '--angle',
                           nargs=2,
                           default=[0., 'viewing'],
                           metavar=("ANGLE", "GEOMETRY-DEF"),
                           dest='angle',
                           help='Set shower angle and geometry definition (viewing/emergence)'
                           )
+    make_cfg.add_argument('-X0',
+                         type=float,
+                         default = 0.,
+                         dest='X0',
+                         help='Set starting grammage (X0) in g/cm^2'
+                         )
     make_cfg.add_argument('-d', '--dist-first-int',
                           nargs=2,
                           default=[0., 'distance'],
                           metavar=("FIRST_INTERACTION_DISTANCE", "DISTANCE-DEF"),
                           dest='distFirstInt',
                           help='Set distance to first interaction (linear distance/altitude(only for below limb events))'
                           )
@@ -162,14 +176,21 @@
                           type=str,
                           choices=('yes', 'no', 'on', 'off'),
                           default='no',
                           dest='useGreisen',
                           help='Use Greisen parametrization for longitudianal profile \
                                 instead of CORSIKA file'
                           )
+    make_cfg.add_argument('--lat_dist',
+                          type=str,
+                          choices=('Lafebre', 'NKG'),
+                          default='NKG',
+                          dest='lat_dist',
+                          help='Choice of parameterization of lateral distribution of electrons'
+                          )
     make_cfg.add_argument('-o', '--output',
                           type=str,
                           default='',
                           dest='output_name',
                           help='Name of the output file. Supported formats are root, npz'
                           )
     make_cfg.add_argument('-p', '--plots',
@@ -222,14 +243,19 @@
         io_func.flog(f'''[bold blue]WARN:[/] You entered an unkown shower geometry ({geo_view})! \n'''
                      '''Allowed options are\n'''
                      '''   - emergence for emergence angle shower definition\n'''
                      '''   - viewing for detector viewing angle shower definition\n'''
                      '''Please change your configuration accordingly.\n''')
         sys.exit(-1)
 
+    if user_args.X0 is None:
+        X0 = float(cfg.getfloat('shower', 'X0'))
+    else:
+        X0 = float(user_args.X0)
+
     if user_args.distFirstInt is None:
         dist_def = cfg.getlist('shower', 'distFirstInt')[1]
         dist = float(cfg.getlist('shower', 'distFirstInt')[0])
     else:
         dist_def = user_args.distFirstInt[1]
         dist = float(user_args.distFirstInt[0])
     if dist_def == 'distance':
@@ -246,81 +272,94 @@
                      '''Allowed options are\n'''
                      '''   - distance for linear distance to first interaction of shower\n'''
                      '''   - altitude for altitude of first interaction of shower (only valid for below-limb geometries)\n'''
                      '''Please change your configuration accordingly.\n''')
         sys.exit(-1)
 
     ## Calculating the path lengths to the detector and the top of the atmosphere
-    [L_detector, L_atmosphere] = [geo.L_from_z(z, theta_D, detector_altitude)
+    if theta_D > 90:
+        [L_detector, L_atmosphere] = [geo.L_from_z(detector_altitude, theta_D, detector_altitude), 1e20]
+    else:
+        [L_detector, L_atmosphere] = [geo.L_from_z(z, theta_D, detector_altitude)
                                   for z in [detector_altitude, const.z_max]]
 
     ## Disallowing for unobservable trajectories
     if np.isnan(L_detector) or np.isnan(L_atmosphere) or L_particle > min([L_detector, L_atmosphere]):
         io_func.flog('''[bold red] ERROR: [/]EAS begins past either the detector or the atmosphere and is unobservable.''')
         # change to try next shower in the future
         sys.exit(-1)
     if user_args.eng is None:
         energy = cfg.getfloat('shower', 'energy')
     else:
         energy = float(user_args.eng)
-    
-    # save or not to save fig
-    if user_args.savefig or cfg.getboolean('output', 'saveFigures'):
-        savefig = True
-    else:
-        savefig = False
 
+    # save or not to save fig
+    savefig = bool(user_args.savefig or cfg.getboolean('output', 'saveFigures'))
     # set up output file
-    out_file = cfg.get('output', 'name') if (user_args.output_name == None) else user_args.output_name
+    out_file = (
+        cfg.get('output', 'name')
+        if user_args.output_name is None
+        else user_args.output_name
+    )
     if ".root" in out_file and io_func.root_found or ".npz" in out_file:
         output = io_func.IO(out_file)
     elif".root" in out_file:
         io_func.flog('''[bold red] ERROR: [/]Output format root requested but no root install found!\n'''
                      '''Please make sure root is installed and sourced.\n'''
                      '''ROOT can be installed via cond *conda install -c conda-forge root*'''
                      )
         sys.exit(-1)
     elif out_file != '':
         io_func.flog(f'''[bold red]ERROR: {cfg.get('output', 'name')} is an unknown format.\n'''
                      '''       Please change to one of the supported formats: root, npz'''
                      )
         sys.exit(-1)
-    elif out_file == '':
-        io_func.flog('''[bold blue]WARN:[/] No output file will be created. \n''')
     else:
-        io_func.flog(f'''Simulation result will be written to {cfg.get('output', 'name')} \n''')
+        io_func.flog('''[bold blue]WARN:[/] No output file will be created. \n''')
 
     # create plot folder
     if savefig:
         i = 1
         while os.path.exists(plot.plot_out_dir):
             plot.plot_out_dir = f"plots({i})/"
             i += 1
         io_func.flog(f'''Plots will be saved in {plot.plot_out_dir[:-1]}.''')
         os.mkdir(plot.plot_out_dir)
 
+    # Check for an input file
+    if user_args.input_name is None:
+        input_file = None
+        shower_index = None
+    else:
+        input_file = user_args.input_name[0]
+        # For averaging over all showers in an input file
+        # give a second argument "all"
+        if(user_args.input_name[1] == "all"):
+            shower_index = None
+        else:
+            shower_index = int(user_args.input_name[1])
     sim_result = sp_cher_prof.cherenkov_from_particle_profile(detector_altitude,
                                                               energy, theta_D,
-                                                              L_particle, L_detector, L_atmosphere,
+                                                              X0, L_particle, L_detector, L_atmosphere,
                                                               cfg['atmosphere'], cfg['magField'],
                                                               cfg['runSettings'],
                                                               cfg.get('output', 'plots'),
-                                                              savefig
-                                                              )
+                                                              savefig,
+                                                              input_file=input_file,
+                                                              shower_index=shower_index)
     if "output" in locals():
         # write shower prop
-        output.write_shower_prop(energy, float(theta_D), L_particle)
+        output.write_shower_prop(energy, float(theta_D), L_particle, X0)
         # write cher ph prop
         output.write_cher_ph_prop(sim_result)
 
     # new check here as previous part needs to move to loop for multiple showers
     if "output" in locals():
         output.close()
 
-
 def main():
     io_func.get_console(log_time=False, log_path=False).rule("[bold blue]EASCherSim")
     args = cli()
     args.func(args)
 
 
 if __name__ == "__main__":
```

### Comparing `easchersim-1.1/src/easchersim/electron_func.py` & `easchersim-1.2.0/src/easchersim/io_func.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,401 +24,409 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-''' Electron Functions
+# TODO: make Showerfile actually configurable, requires calculation of X_0 and energy of shower file
+
+''' IO Functions
 
 .. autosummary::
    :toctree:
    :recursive:
 
-    Lorentz_factor
-    particle_velocity
-    gyroradius
-    geomagnetic_deflection_correction
-    Hillas_Energy_Distribution
-    Hillas_Angular_Distribution
-    Lafebre_Lateral_Distribution
-    Lafebre_Lag_Time_Distribution
-    Greisen_Longitudinal_Profile
-    CORSIKA_interpolation
+   CORSIKA_Shower_Reader
+   average_CORSIKA_profile
+   read_config
 
 '''
 
-import numpy as np
-from scipy import interpolate
-import scipy.stats as st
+from rich.console import Console
+from rich.table import Column
+from rich.progress import Progress, BarColumn, TextColumn, TimeElapsedColumn
+from importlib_resources import files
+from os.path import exists as file_exists
 
-from . import io_func
-from . import constants as const
-from . import atmosphere as atm
+import configparser as cp
+import numpy as np
+import io
+import sys
 
+import matplotlib.pyplot as plt
 
-def Lorentz_factor(energy):
-    """Calculate the Lorentz factor of an electron with a given energy in MeV
+try:
+    from ROOT import TFile, TTree, TH1D, vector
+except ImportError:
+    root_found = False
+else:
+    root_found = True
 
-    Parameters
-    ----------
-    energy : float
-        e- energy in MeV
 
-    Returns
-    -------
-    float
-        Lorentz factor
+class IO:
+    """root IO class
     """
-    gamma = energy / const.electron_mass
-
-    return gamma
+    def __init__(self, file_name='CherSim.root'):
+        self.check_file_exist(file_name)
+        self.__filename = file_name
+        self.__root = False
+        if ".root" in file_name:
+            self.__root = True
+            self.__vec_time = vector("TH1D")()
+            self.__vec_phZenith = vector("TH1D")()
+            self.__vec_phAzi = vector("TH1D")()
+            self.create_root_file(file_name)
+
+    def check_file_exist(self, file_name):
+        if file_exists(file_name):
+            overwrite = get_console().input(f'''[bold blue]WARN:[/] A file with the same name'''
+                                            f''' [italic]{file_name}[/] already exist.'''
+                                            f''' Do you want to overwrite it? (yes/no) ''')
+            if 'y' not in overwrite.lower():
+                sys.exit(0)
+        flog(f'''Simulation result will be written to {file_name} \n''')
+
+    def create_root_file(self, filename):
+        self.__file = TFile(filename, 'recreate')
+        self.__tcher_ph = TTree("cherPhProp", "Cherenkov Photon Properties")
+        self.__tshower = TTree("showerProp", "Shower Properties")
+
+        # create branches for tshower
+        self.__eng = np.zeros(1, dtype=float)
+        self.__zen = np.zeros(1, dtype=float)
+        self.__startdist = np.zeros(1, dtype=float)
+        self.__X0 = np.zeros(1, dtype=float)
+
+        self.__tshower.Branch("energy", self.__eng, 'eng/D')
+        self.__tshower.Branch("zenith", self.__zen, 'zen/D')
+        self.__tshower.Branch("startdist", self.__startdist, 'startdist/D')
+        self.__tshower.Branch("X0", self.__X0, 'X0/D')
+
+        # define histograms
+        histo_w = TH1D()
+        histo_r = TH1D()
+        histo_t_off = TH1D()
+        histo_phZenith_off = TH1D()
+
+        # set branch for histograms
+        self.__tcher_ph.Branch("wavelength", 'TH1D', histo_w)
+        self.__tcher_ph.Branch("distance", 'TH1D', histo_r)
+        self.__tcher_ph.Branch("time_offset", 'TH1D', histo_t_off)
+        self.__tcher_ph.Branch("phZenith_offset", 'TH1D', histo_phZenith_off)
+        self.__tcher_ph.Branch("time_dist", self.__vec_time)
+        self.__tcher_ph.Branch("phZenith_dist", self.__vec_phZenith)
+        self.__tcher_ph.Branch("phAzimuth_dist", self.__vec_phAzi)
+
+    def write_shower_prop(self, energy, theta_D, L_particle, X0):
+        # add shower properties
+        self.__shower_settings = np.array([energy, theta_D, L_particle, X0], dtype=float)
+        if self.__root:
+            self.__eng[0] = energy
+            self.__zen[0] = theta_D
+            self.__startdist[0] = L_particle
+            self.__X0[0] = X0
+            self.__tshower.Fill()
+
+    def write_cher_ph_prop(self, cher_ph):
+
+        if self.__root:
+            num_wl_bin = len(cher_ph["wavelengths"]) - 1
+            num_dist_bin = len(cher_ph["r_bins"]) - 1
+            num_time_bin = len(cher_ph["time_bins"]) - 1
+            num_phZenith_bin = len(cher_ph["phZenith_bins"]) - 1
+            num_phAzi_bin = len(cher_ph["phAzi_bins"]) - 1
+
+            # define histograms
+            histo_w = TH1D("wl", "wavelength", num_wl_bin, cher_ph["wavelengths"])
+            histo_r = TH1D("r", "distance", num_dist_bin, cher_ph["r_bins"])
+            histo_t_off = TH1D("t_off", "time offset",
+                                num_dist_bin, cher_ph["r_bins"])
+            histo_phZenith_off = TH1D("phZenith_off", "phZenith offset",
+                                    num_dist_bin, cher_ph["r_bins"])
+            histo_t = [
+                TH1D(
+                    f"t_dist_{str(i)}",
+                    f"time_dist_{str(i)}",
+                    num_time_bin,
+                    cher_ph["time_bins"],
+                )
+                for i in range(num_dist_bin)
+            ]
+            histo_phZenith = [
+                TH1D(
+                    f"phZenith_dist_{str(i)}",
+                    f"phZenith_dist_{str(i)}",
+                    num_phZenith_bin,
+                    cher_ph["phZenith_bins"],
+                )
+                for i in range(num_dist_bin)
+            ]
+
+            histo_phAzi = [
+                TH1D(
+                    f"phAzi_dist_{str(i)}",
+                    f"phAzi_dist_{str(i)}",
+                    num_phAzi_bin,
+                    cher_ph["phAzi_bins"],
+                )
+                for i in range(num_dist_bin)
+            ]
+
+            # fill histograms
+            for wl_bin, counts in enumerate(cher_ph["wavelength_counts"]):
+                histo_w.SetBinContent(wl_bin + 1, counts)
+            for r_bin, counts in enumerate(cher_ph["r_counts"]):
+                histo_r.SetBinContent(r_bin + 1, counts)
+                histo_t_off.SetBinContent(r_bin + 1, cher_ph["lower_times"][r_bin])
+                histo_phZenith_off.SetBinContent(r_bin + 1, cher_ph["lower_phZenith"][r_bin])
+                for t_bin, counts_t in enumerate(cher_ph["time_counts"][r_bin]):
+                    histo_t[r_bin].SetBinContent(t_bin + 1, counts_t)
+                for phZenith_bin, counts_phZenith in enumerate(cher_ph["phZenith_counts"][r_bin]):
+                    histo_phZenith[r_bin].SetBinContent(phZenith_bin + 1, counts_phZenith)
+                for phAzi_bin, counts_phAzi in enumerate(cher_ph["phAzi_counts"][r_bin]):
+                    histo_phAzi[r_bin].SetBinContent(phAzi_bin + 1, counts_phAzi)
+
+            self.__tcher_ph.SetBranchAddress("wavelength", histo_w)
+            self.__tcher_ph.SetBranchAddress("distance", histo_r)
+            self.__tcher_ph.SetBranchAddress("phZenith_offset", histo_phZenith_off)
+            self.__tcher_ph.SetBranchAddress("time_offset", histo_t_off)
+            self.__vec_time.assign(histo_t)
+            self.__vec_phZenith.assign(histo_phZenith)
+            self.__vec_phAzi.assign(histo_phAzi)
+            self.__tcher_ph.Fill()
+        else:
+            np.savez(self.__filename, shower_prop=self.__shower_settings,
+                     wavelengths=cher_ph["wavelengths"], wavelength_counts=cher_ph["wavelength_counts"],
+                     dist_bins=cher_ph["r_bins"], dist_counts=cher_ph["r_counts"],
+                     time_bins=cher_ph["time_bins"], time_counts=cher_ph["time_counts"],
+                     time_offset=cher_ph["lower_times"],
+                     phZenith_bins=cher_ph["phZenith_bins"], phZenith_counts=cher_ph["phZenith_counts"],
+                     phZenith_offset=cher_ph["lower_phZenith"],
+                     phAzi_bins=cher_ph["phAzi_bins"], phAzi_counts=cher_ph["phAzi_counts"],
+                     t_counts=cher_ph["t_counts"],
+                    )
+
+    def close(self):
+        if self.__root:
+            self.__tshower.Write("", TFile.kOverwrite)
+            self.__tcher_ph.Write("", TFile.kOverwrite)
+            self.__file.Close()
 
 
-def particle_velocity(energy):
-    """Calculate the speed of an electron relative to the speed of light with a given energy in MeV
+def is_float(s):
+    """Determines if an input value is a float
 
     Parameters
     ----------
-    energy : float
-        e- energy in MeV
+    s : str
+        input string
 
     Returns
     -------
-    float
-        beta: speed of e- relative to c
+    Boolean
+        True: if string is float, False otherwise
     """
-    # Calculate the particle's Lorentz factor
-    particle_Lorentz_factor = Lorentz_factor(energy)
 
-    beta = np.sqrt(1 - 1 / (particle_Lorentz_factor**2))
+    try:
+        float(s)
+        return True
+    except ValueError:
+        return False
 
-    return beta
 
-
-def gyroradius(electron_energy, electron_zenith, electron_azimuth, magnetic_field_strength, magnetic_field_zenith):
-    """Calculates the gyroradius (in km) of an electron with a given energy (in MeV), zenith angle (with respect to trajectory: in degrees)
-    and azimuth angle (in degrees) inside a magnetic field with a given strength (in uT) and zenith angle(in degrees)
+def CORSIKA_Shower_Reader(filename):
+    """Reads in longitudinal charged particle profiles (.long files) generated by CORSIKA simulations
 
     Parameters
     ----------
-    electron_energy : ArrayLike
-        e- energy in MeV
-    electron_zenith : ArrayLike
-        e- zenith in degrees
-    electron_azimuth : ArrayLike
-        e- azimuth in degrees
-    magnetic_field_strength : float
-        magnetic field strength in uT
-    magnetic_field_zenith : float
-        magnetic field inclination with respect to shower axis in degrees
+    filename : str
+        CORSIKA .long file path
 
     Returns
     -------
     ArrayLike
-        gyroradius in km
+        longitudial charged particle profile of showers array of lists (depth, number of electrons)
     """
-    # Calculates the normalized pointing array of the magnetic field, aligning the incident particle along the z axis
-    magnetic_field_zenith = (np.pi / 180) * magnetic_field_zenith
-    magnetic_field_direction = np.array([np.sin(magnetic_field_zenith), 0, np.cos(magnetic_field_zenith)])
-
-    # Initializes the normalized velocity vector of the particle (aligned along the z axis)
-    electron_zenith = (np.pi / 180) * electron_zenith
-    particle_direction = np.array([np.cos(electron_azimuth[None, None, :]) * np.sin(electron_zenith[:, :, None]), np.sin(electron_azimuth[None, None, :]) * np.sin(electron_zenith[:, :, None]), np.cos(electron_zenith[:, :, None] * np.ones(len(electron_azimuth))[None, None, :])])
-
-    # Calculating the Lorentz factor and particle relative velocity
-    particle_Lorentz_factor, particle_relative_velocity = Lorentz_factor(electron_energy), particle_velocity(electron_energy)
+    # Initialize an array to contain all the simulated showers and arrays to contain the depths (g/cm^2) and particle content for each shower
+    showers = []
+    depths, electrons = [], []
+
+    with open(filename) as f:
+        # Flag for whether to output the lines which follow, initialize as false
+        readout_flag = False
+
+        # Loop through the given file line by line
+        for line in f:
+            if readout_flag:
+
+                # Split the line on the " " delimiter
+                data = line.split()
+                # If the first value is a float, can continue
+                if is_float(data[0]):
+                    # Append the depth to the depth array, and the sum of electrons and positrons to the electron array
+                    # If other particle types are desired:
+                    # [0]: depths, [1]: gammas, [2]: electrons, [3]: positrons, [4]: anti-muons, [5]: muons, [6]: hadrons, [7]: charged particles, [8]: nuclei
+                    depths.append(float(data[0]))
+                    electrons.append(float(data[2]) + float(data[3]))
+
+            # Determine if charged particle info follows.
+            # CORSIKA outputs charged particle profiles, followed by energy information, so flag must switch every instance of header
+            if ("ELECTRONS" in line) or ("EM CUT" in line):
+                # Append shower info to container array
+                if len(depths) > 0:
+                    showers.append([depths, electrons])
+
+                readout_flag = not readout_flag
+                # Reinitialize arrays
+                depths, electrons = [], []
 
-    particle_gyroradius = particle_Lorentz_factor[None, :, None] * const.electron_mass * const.MeV_to_kg * particle_relative_velocity[None, :, None] * const.cl / (const.electron_charge * np.linalg.norm(np.cross(particle_direction, magnetic_field_strength * 1e-6 * magnetic_field_direction, axis=0), axis=0))
+    return np.array(showers)
 
-    return particle_gyroradius
 
-
-def geomagnetic_deflection_correction(Ls, L_detector, electron_energy, electron_zenith, electron_azimuth, magnetic_field_strength, magnetic_field_zenith):
-    """Calculates the deflection correction (in km) of an electron with a given energy (in MeV), zenith angle (with respect to trajectory: in degrees)
-    and azimuth angle (in degrees) inside a magnetic field with a given strength (in uT) and zenith angle(in degrees)
-
-    TODO: RECONSIDER THIS WHOLE CONCEPT...
+def average_CORSIKA_profile(showers):
+    """Calculates the average charged particle longitudinal profile from the CORSIKA data
 
     Parameters
     ----------
-    Ls : ArrayLike
-        distance bins along the shower trajectory in km
-    L_detector : float
-        distance from the start of the shower to the detector in km
-    electron_energy : ArrayLike
-        e- energy in MeV
-    electron_zenith : ArrayLike
-        e- zenith in degrees
-    electron_azimuth : ArrayLike
-        e- azimuth in degrees
-    magnetic_field_strength : float
-        magnetic field strength in uT
-    magnetic_field_zenith : float
-        magnetic field inclination with respect to shower axis in degrees
-
-    Returns
-    -------
-    float
-        deflection correction in km
-    """
-    # Calculate the gyroradius of the electrons
-    particle_gyroradius = gyroradius(electron_energy, electron_zenith, electron_azimuth, magnetic_field_strength, magnetic_field_zenith)
-
-    # Calculate the deflected angle inside the given distance bins and the corresponding projection on the detection plane
-    dLs = np.append(np.diff(Ls), Ls[-1] - Ls[-2])
-    added_distance = np.reshape(np.random.choice([-1, 1], size=particle_gyroradius.shape), particle_gyroradius.shape) * (L_detector - Ls[None, :, None]) * (dLs[None, :, None] / particle_gyroradius) / np.sqrt(1 - (dLs[None, :, None] / particle_gyroradius)**2)
-
-    return added_distance
-
-
-def Hillas_Energy_Distribution(electron_energy, shower_age):
-    """Calculates the total fraction of electrons present at a given shower age above an energy (in MeV) as given by:
-    A.M. Hillas. Air. J. Phys. G, 8:1461-1473, 1982
-
-    Parameters
-    ----------
-    electron_energy : ArrayLike
-        e- energy in MeV
-    shower_age : ArrayLike
-        shower age
+    showers : ArrayLike
+        array of showers returned by the CORSIKA_Shower_Reader function
 
     Returns
     -------
     ArrayLike
-        e- fraction above input energy at shower age
+        the average longitudinal charged particle profile of many showers
     """
-    E0 = np.where(shower_age < 0.4, 26, 44 - 17 * (shower_age - 1.46)**2)
-
-    if isinstance(shower_age, np.ndarray):
-        part1 = 0.89 * E0 - 1.2
-        part2 = E0[:, None] + electron_energy
-        part3 = 1 + (electron_energy * shower_age[:, None]) * 1e-4
-
-        electron_fraction = ((part1[:, None] / part2)**shower_age[:, None]) * (part3)**(-2)
-    else:
-        part1 = 0.89 * E0 - 1.2
-        part2 = E0 + electron_energy
-        part3 = 1 + (electron_energy * shower_age) * 1e-4
-
-        electron_fraction = ((part1 / part2)**shower_age) * (part3)**(-2)
-
-    return electron_fraction
+    return np.average(showers, axis=0)
 
-
-def Hillas_Angular_Distribution(electron_energy, shower_age, us):
-    """e- angular distribution (Hillas)
-
-    Calculates (i) the corresponding angle (in degrees) of the scaled angular bin (u) and
-    (ii) the fraction of electrons within the scaled angular bins
-    for a given energy (in MeV) and shower age as given by: A.M. Hillas. Air. J. Phys. G, 8:1461-1473, 1982
+def average_CORSIKA_profile_2(showers):
+    """Calculates the average charged particle longitudinal profile from the CORSIKA data
 
     Parameters
     ----------
-    electron_energy : ArrayLike
-        e- energy in MeV
-    shower_age : ArrayLike
-        shower age
-    us : ArrayLike
-        scaled angular bins, following Hillas 1982
+    showers : ArrayLike
+        array of showers returned by the CORSIKA_Shower_Reader function
 
     Returns
     -------
-    list of arrays
-        angular distribution of electrons (bins in degrees, fraction of electrons per bin)
+    ArrayLike
+        the average longitudinal charged particle profile of many showers
     """
-    # Calculate the midpoint of the angular bins
-    lower_us, upper_us = us[:-1], us[1:]
-    mid_us = (lower_us + upper_us) / 2
-
-    # Calculate the corresponding angle of the given bins
-    v = electron_energy / (1150 + 454 * np.log(shower_age))
-    average_w = 0.0054 * electron_energy * (1 + v) / (1 + 13 * v + 8.3 * v * v)
-    w = mid_us[:, None] * average_w[None, :]
-    theta = (180 / np.pi) * np.arccos(1 - w / (2 * (electron_energy[None, :] / 21)**2))
-
-    # Calculate the fraction of electrons within each scaled angular bin
-    A = np.where(electron_energy < 350, 0.777, 1.318)
-    z0 = np.where(electron_energy < 350, 0.59, 0.37)
-    z_values = [np.sqrt(lower_us), np.sqrt(upper_us)]
-    lambda_ls = [np.where((electron_energy[None, :] < 350) & (z[:, None] < 0.59), 0.478, np.where((electron_energy[None, :] < 350) & (z[:, None] >= 0.59), 0.380, np.where((electron_energy[None, :] >= 350) & (z[:, None] < 0.37), 0.413, 0.380))) for z in z_values]
-
-    # Must consider the bins in z which cross z0 and have different behavior
-    [n_lower, n_upper] = [-2 * A[None, :] * np.exp((-z_values[i][:, None] + z0[None, :]) / lambda_ls[i]) * lambda_ls[i] * (lambda_ls[i] + z_values[i][:, None]) for i in (0, 1)]
-    [n_z0_lower, n_z0_upper] = [-2 * A[None, :] * lambda_ls[i] * (lambda_ls[i] + z0[None, :]) for i in (0, 1)]
-
-    dn = np.where((z_values[0][:, None] < z0[None, :]) & (z_values[1][:, None] >= z0[None, :]), n_upper - n_z0_upper + n_z0_lower - n_lower, n_upper - n_lower)
-
-    # Do not return NaN values
-    NaN_values = np.isnan(theta)
-    theta[NaN_values] = 0
-    dn[NaN_values] = 0
-
-    return [theta, dn]
-
-
-def Lafebre_Lateral_Distribution(electron_energies, radiation_lengths, zs, coordinates):
-    """Lateral distribution Lafebre
-
-    Randomly samples lateral offsets of electrons (in km) from the shower axis, given their primary energy (in MeV),
-    their modified shower age (radiation length measured from shower maximum), their altitudes, and the desired shape of the output array
-    as parameterized by: S. Lafebre, R. Engel, H. Falcke, J. Horandel, T. Huege, J. Kuijpers, and R. Ulrich. Astropart. Phys., 31:243-254, 2009
+    indices = np.argmax(showers[:,1,:], axis = 1)
+    min_index = np.min(indices)
 
-    Parameters
-    ----------
-    electron_energies : ArrayLike
-        e- energy in MeV
-    radiation_lengths : ArrayLike
-        radiation length (X-Xmax)/X0
-    zs : ArrayLike
-        altitudes in km
-    coordinates : ArrayLike
-        coordinates of ellipse about which to sample lateral offsets
+    shifts = indices-min_index
+    new_parts = np.array([np.roll(showers[i,1,:], -shifts[i]) for i in range(len(shifts))])
+    
+    showers[:, 1, :] = new_parts
+    
+    fig = plt.figure()
+    for i in range(len(shifts)):
+        
+        plt.plot(showers[i,0,:], showers[i, 1, :], color = 'red')
+    
+    #average_shower = np.array([showers[loc_min_index, 0, :], showers[loc_min_index, 1, :]])
+    average_shower = np.average(showers, axis=0)
+    plt.plot(showers[i,0,:], average_shower[1,:], label = 'Average Profile', color = 'black')
+    plt.xlabel('Grammage '+r'$(\mathrm{g}/\mathrm{cm}^{2})$')
+    plt.ylabel('Charged Particles')
+    plt.yscale('log')
+    #plt.show()
+    
+    #
+    '''
+    plt.plot(average_shower[0], average_shower[1], color = 'black')
+    plt.yscale('log')
+    plt.show()
+'''
+    return average_shower
 
-    Returns
-    -------
-    ArrayLike
-        sampled lateral offsets for each point about the input ellipse
-    """
-    # Model is only parameterized within energy range 1MeV-1GeV
-    modified_electron_energies = np.copy(electron_energies)
-    modified_electron_energies[modified_electron_energies < 1] = 1
-    modified_electron_energies[modified_electron_energies > 1000] = 1000
-
-    # Model is only parameterized within shower age range -9-9
-    radiation_lengths[radiation_lengths < -9] = -9
-    radiation_lengths[radiation_lengths > 9] = 9
-
-    # Model parameters
-    logE = np.log(modified_electron_energies)
-    x1 = 0.859 - 0.0461 * (logE**2) + 0.00428 * (logE**3)
-    Lt = 0.0263 * radiation_lengths
-    L0 = Lt + 1.34 + 0.160 * logE - 0.0404 * (logE**2) + 0.00276 * (logE**3)
-    L1 = Lt - 4.33
-
-    # Loading the desired shape of the samples
-    zenith_shape, azimuth_shape = coordinates.shape[0], coordinates.shape[2]
-
-    # Calculating Moliere Radius
-    moliere = atm.moliere_radius(zs)
-
-    # Randomly sample the lateral offsets using a scaled betaprime distribution
-    sampled_offsets = np.transpose(np.array([moliere[i] * x1[i] * st.betaprime.rvs(L0[i], -L0[i] - L1[i], size=zenith_shape * azimuth_shape).reshape(zenith_shape, azimuth_shape) for i in range(0, len(modified_electron_energies))]), (1, 0, 2))
-
-    return sampled_offsets
-
-
-def Lafebre_Lag_Time_Distribution(electron_energies, radiation_lengths, zs, coordinates):
-    """Randomly samples lag times of electrons (in s) from an imaginary particle travelling along the shower axis at the speed of light, given their primary energy (in MeV),
-    their modified shower age (radiation length measured from shower maximum), their altitudes, and the desired shape of the output array
-    as parameterized by: S. Lafebre, R. Engel, H. Falcke, J. Horandel, T. Huege, J. Kuijpers, and R. Ulrich. Astropart. Phys., 31:243-254, 2009
+def read_config(cfg_file):
+    """Read configuration file.
 
     Parameters
     ----------
-    electron_energies : ArrayLike
-        e- energies in MeV
-    radiation_lengths : ArrayLike
-        radiation length (X-Xmax)/X0
-    zs : ArrayLike
-        altitudes in km
-    coordinates : ArrayLike
-        coordinates of ellipse about which to sample lateral offsets
+    cfg_file : str
+        name of User config file
 
     Returns
     -------
-    ArrayLike
-        sampled lag times of electrons in s for each point about the input ellipse
+    ConfigParser
+        Settings for simulation (defualt & user specified)
     """
-    # Model is only parameterized within energy range 1MeV-1GeV
-    modified_electron_energies = np.copy(electron_energies)
-    modified_electron_energies[modified_electron_energies < 1] = 1
-    modified_electron_energies[modified_electron_energies > 1000] = 1000
-
-    # Model is only parameterized within shower age range -4.5 to 9
-    # lower limit adjusted to respected domains scaled betaprime distribution
-    radiation_lengths[radiation_lengths < -4.45] = -4.45
-    radiation_lengths[radiation_lengths > 9] = 9
+    cfg = cp.ConfigParser(allow_no_value=True,
+                          converters={'list': lambda x: [i.strip() for i in x.split(',')]})
+    cfg.optionxform = lambda option: option
+    # read default settings
+    default_cfg = files("easchersim.data")/"default_conf.ini"
+    cfg.read(default_cfg)
 
-    # Model parameters
-    logE = np.log(modified_electron_energies)
-    tau1 = np.exp(-2.71 + 0.0823 * logE - 0.114 * (logE**2))
-    L0 = 1.70 + 0.160 * radiation_lengths - 0.142 * logE
-    L1 = -3.21
+    # read user settings (overwrittes defaults)
+    cfg.read(cfg_file)
 
-    # Loading the desired shape of the samples
-    zenith_shape, azimuth_shape = coordinates.shape[0], coordinates.shape[2]
+    return cfg
 
-    # Calculating Moliere Radius
-    moliere = atm.moliere_radius(zs)
 
-    # Randomly sample the lateral offsets using a scaled betaprime distribution
-    sampled_lag_times = (1 / const.cl) * np.transpose(np.array([moliere[i] * tau1[i] * st.betaprime.rvs(L0[i], -L0[i] - L1, size=zenith_shape * azimuth_shape).reshape(zenith_shape, azimuth_shape) for i in range(0, len(modified_electron_energies))]), (1, 0, 2))
+def create_config(user_args):
+    """Creates example configuration file
 
-    return sampled_lag_times
-
-
-def Greisen_Longitudinal_Profile(energy, slant_depth):
-    """Calculates the number of charged particles for a given slant depth (in g/cm^2) and a given shower energy (in eV)
-    as parameterized by Greisen, found in: Cosmic Rays and Particle Physics: 2nd Edition.
+    Values can be specified by user via command line all not specified parameter will be default
 
     Parameters
     ----------
-    energy : float
-        primary energy of shower in eV
-    slant_depth : float
-        slant depth along shower trajectory in g/cm^2
-
-    Returns
-    -------
-    float
-        the number of charged particles at the input slant depth for a shower with a given energy
+    user_args : namespace
+        User inputs parsed by argparse
     """
-    # Convert the slant depth to radiation lengths
-    radiation_length = slant_depth / 36.7
-
-    # Convert the radiation lengths to shower age
-    shower_age = 3 * radiation_length / (radiation_length + 2 * np.log(energy / 87e6))
-
-    # Calculate the number of charged particles and filter out and NaN values
-    charged_particles = (0.31 / ((np.log(1e17 / 87e6))**0.5)) * np.exp(radiation_length * (1 - 1.5 * np.log(shower_age)))
-    charged_particles[np.isnan(charged_particles)] = 0
+    cfg = cp.ConfigParser()
+    cfg.optionxform = lambda option: option
+    cfg['shower'] = {'energy': user_args.eng,
+                     'X0': user_args.X0,
+                     'angle': f"""{user_args.angle[0]}, {user_args.angle[1]}""",
+                     'distFirstInt': f"""{user_args.distFirstInt[0]}, {user_args.distFirstInt[1]}"""}
+    cfg['detector'] = {'altitude': user_args.det_alt}
+    cfg['atmosphere'] = {'scattering': user_args.atm_scatter}
+    cfg['magField'] = {'useField': user_args.mag_field}
+    cfg['runSettings'] = {'useGreisenParametrization': user_args.useGreisen,
+                          'lat_dist': user_args.lat_dist}
+    cfg['output'] = {'name': user_args.output_name,
+                     'plots': user_args.plots,
+                     'saveFigures': "yes" if user_args.savefig else "no"}
 
-    return charged_particles
+    with open(user_args.filename, 'w') as cfg_file:
+        cfg.write(cfg_file)
 
 
-def CORSIKA_interpolation(energy, slant_depth, filename, simulated_energy):
-    """Calculates the number of charged particles for a given slant depth (in g/cm^2) and a given shower energy (in eV)
-    interpolating from a given charged particle longitudinal profile generated by CORSIKA and scaled linearly
-
-    Parameters
-    ----------
-    energy : float
-        primary energy of shower in eV
-    slant_depth : float
-        slant depth along shower trajectory in g/cm^2
-    filename : str
-        name of CORSIKA file to interpolate
-    simulated_energy : float
-        shower energy used for CORSIKA simualtion in eV
-
-    Returns
-    -------
-    ArrayLike
-        charged particle profile scaled to shower energy
+def dump_default_conf():
+    """Print default configuration to screen
     """
-    # Load in the CORSIKA showers
-    CORSIKA_showers = io_func.CORSIKA_Shower_Reader(filename)
-
-    # Calculate the average of these showers
-    average_shower = io_func.average_CORSIKA_profile(CORSIKA_showers)
-    del CORSIKA_showers
-
-    # Create an interpolation object of the average shower
-    charged_particles_from_slant_depth = interpolate.interp1d(average_shower[0], average_shower[1], fill_value='extrapolate')
-    del average_shower
-
-    # Calculate the number of charged particles and filter out NaN and negative values
-    charged_particles = (energy / simulated_energy) * charged_particles_from_slant_depth(slant_depth)
-    charged_particles[np.isnan(charged_particles)] = 0
-    charged_particles[charged_particles < 0] = 0
-
-    return charged_particles
+    cfg = cp.ConfigParser()
+    # read default settings
+    default_cfg = files("easchersim.data")/"default_conf.ini"
+    cfg.read(default_cfg)
+    with io.StringIO() as str_stream:
+        cfg.write(str_stream)
+        print(str_stream.getvalue())
+
+
+def get_console(**kargs):
+    return (
+        Console(**kargs, width=100)
+        if kargs
+        else Console(width=100, log_path=False)
+    )
+
+
+def flog(*args):
+    get_console().log(*args)
+
+
+def get_progress():
+    text_col = TextColumn("[bold red]{task.description}", table_column=Column(ratio=1))
+    bar_col = BarColumn(bar_width=40, table_column=Column(ratio=4))
+
+    return Progress(
+        text_col,
+        bar_col,
+        "[progress.percentage]{task.percentage:>3.0f}%",
+        TimeElapsedColumn(),
+        console=get_console(),
+    )
```

### Comparing `easchersim-1.1/src/easchersim/fit_func.py` & `easchersim-1.2.0/src/easchersim/fit_func.py`

 * *Files identical despite different names*

### Comparing `easchersim-1.1/src/easchersim/geometry.py` & `easchersim-1.2.0/src/easchersim/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,18 @@
         theta_EE = theta_EE_from_theta_D(det_alt, theta_D) * (np.pi / 180)
         a = 1
         b = 2 * const.R_Earth * np.sin(theta_EE)
         c = const.R_Earth**2 - (z + const.R_Earth)**2
         root_1 = (-b - np.sqrt(b**2 - 4 * a * c)) / (2 * a)
         root_2 = (-b + np.sqrt(b**2 - 4 * a * c)) / (2 * a)
 
-    return max(np.array([root_1, root_2]))
+    if theta_D > 90:
+        return min(np.array([root_1, root_2]))
+    else:
+        return max(np.array([root_1, root_2]))
 
 
 def ellipse_focii(Ls, L_detector, electron_zenith, Cherenkov_angle):
     """Calculates the minor and major focii (in km) of the ellipse generated on the detection plane (assuming the plane normal to the shower incidence)
     given the distance of the emission point from the shower starting point (in km), the detection plane distance (in km),
     the electron zenith angle with respect to the shower axis (in degrees), and the Cherenkov angle (in degrees)
```

### Comparing `easchersim-1.1/src/easchersim/plot.py` & `easchersim-1.2.0/src/easchersim/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,27 +159,29 @@
     plt.xlabel('Distance From Shower Axis (km)')
     plt.ylabel('90% Time Spread (ns)')
     plt.grid(which='both')
 
     return fig
 
 
-def plot_photon_angular_spread(r_bins, angular_bins, angular_counts):
+def plot_photon_angular_spread(r_bins, angular_bins, angular_counts, type):
     """Plots the angular distribution.
 
     Plots the angular spread within which 90% of the arriving Cherenkov photons arrive (in degrees), per spatial bin
 
     Parameters
     ----------
     r_bins: ArrayLike
         spatial bins within which to bin the photons
     angular_bins : ArrayLike
         angular bins within which to bin the photons
     angular_counts : ArrayLike
         photons within each spatial and angular bin
+    type : str
+        the type of angular spread to plot (azimuth or zenith)
 
     Returns
     -------
     matplot.figure
         plot of the time distribution of the arriving Cherenkov photons
     """
 
@@ -187,16 +189,18 @@
     cumulative_counts = np.cumsum(angular_counts, axis=1) / np.sum(angular_counts, axis=1)[:, None]
     low_bin, high_bin = np.argmax(cumulative_counts >= 0.05, axis=1), np.argmax(cumulative_counts >= 0.95, axis=1)
     angular_diffs = angular_bins[high_bin] - angular_bins[low_bin]
 
     fig = plt.figure()
     plt.plot(r_bins[:-1], angular_diffs)
     plt.yscale('log')
+    if (type == 'azimuth'):
+        plt.yscale('linear')
     plt.xlabel('Distance From Shower Axis (km)')
-    plt.ylabel('90% Angular Spread (degrees)')
+    plt.ylabel(f'90% {type} Angular Spread (degrees)')
     plt.grid(which='both')
 
     return fig
 
 ###################################################################
 # General Plots
 
@@ -357,30 +361,35 @@
     matplot.figure
         plot of the extinction coefficient
     """
 
     # Loads in data
     zs, wavelengths = np.meshgrid(alpha[1],alpha[0])
     alphas = alpha[2]
-    
+
     # External array to interpolate over
     z_grid = np.linspace(0,50,11)
     w_grid = np.linspace(270,1000,100)
     stretched_z_grid, stretched_w_grid = np.meshgrid(z_grid,w_grid)
 
     # Interpolating values
     alpha_array = 1000*np.exp(griddata((zs.flatten(), wavelengths.flatten()), alphas.flatten(), (stretched_z_grid, stretched_w_grid), method='cubic', fill_value = 0))
 
     cm_subsection = np.linspace(0,1,len(z_grid))
     colors = [ cm.jet(x) for x in cm_subsection ]
-    
+
     fig = plt.figure()
-    for i in range(0, len(z_grid)):
+    for i in range(len(z_grid)):
         if z_grid[i]%5 == 0:
-            plt.plot(w_grid, alpha_array[:,i], color = colors[i], label =str(z_grid[i])+'km')
+            plt.plot(
+                w_grid,
+                alpha_array[:, i],
+                color=colors[i],
+                label=f'{str(z_grid[i])}km',
+            )
     plt.xlabel('Wavelength (nm)')
     plt.ylabel('Extinction coefficient '+r'$(\mathrm{km}^{-1})$')
     plt.yscale('log')
     plt.grid(which = 'both')
     labelLines(plt.gca().get_lines(),xvals=(310, 1000),zorder=2.5)
-    
+
     return fig
```

### Comparing `easchersim-1.1/src/easchersim/spatial_cherenkov_profile.py` & `easchersim-1.2.0/src/easchersim/spatial_cherenkov_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,39 +49,44 @@
 from . import atmosphere as atm
 from . import geometry as geo
 from . import cher_func as chf
 from . import electron_func as elef
 from . import fit_func as fitf
 from . import plot
 
+from matplotlib  import cm
+
 try:
     from importlib.resources import files
 except ImportError:
     from importlib_resources import files
 
 np.seterr(divide='ignore', invalid='ignore')
 np.set_printoptions(threshold=sys.maxsize)
 
 
 def cherenkov_from_particle_profile(detector_altitude,
                                     energy, theta_D,
-                                    L_particle, L_detector, L_atmosphere,
+                                    X0, L_particle, L_detector, L_atmosphere,
                                     atmo, mag_field, run_set,
-                                    plots, save_fig
-                                    ):
+                                    plots, save_fig,
+                                    input_file=None,
+                                    shower_index=None):
     """Calculates Spatial Cherenkov Profile given geometric constraints
 
     Parameters
     ----------
     detector_altitude : float
         Altitude of the detection plane in km
     energy : float
         primary energy of the shower in eV
     theta_D : float
         detector viewing angle in degrees
+    X0 : float
+        propagated grammage of the particle (in g/cm^2) before interaction
     L_particle : float
         propagated distance of the particle (in km) before interaction
     L_detector : float
         path length to the detector in km
     L_atmosphere : float
         path length to the top of the atmosphere in km
     atmo : configparse_section Obj
@@ -97,48 +102,58 @@
 
     Returns
     -------
     dict
         Dictionary of simulation results
     """
     # Calculating slant depth profile as a function of propagation distance
-    slant_depth_data = atm.slant_X_from_L_table([L_particle, min([L_detector, L_atmosphere])], detector_altitude, theta_D)
-
+    if theta_D > 90:
+        slant_depth_data = atm.slant_X_from_L_table([L_particle, L_detector], detector_altitude, theta_D)
+    else:
+        slant_depth_data = atm.slant_X_from_L_table([L_particle, min([L_detector, L_atmosphere])], detector_altitude, theta_D)
+    
     # Creating interpolation objects to get slant depth from propagation distance and vice-versa
     L_from_slant_depth = interpolate.interp1d(slant_depth_data[1], slant_depth_data[0], fill_value='extrapolate')
 
     ################################################################
     # Initializing Atmosphere
 
     # Initializing the slant depth bins to calculate photon content
     max_x = float(run_set.getlist('slantDepth')[1])
     x_bins = int(run_set.getlist('slantDepth')[0])
+    
+    if X0 >= slant_depth_data[1][-1]:
+        print('Starting grammage (X0) greater than total grammage provided by trajectory, exiting...')
+        sys.exit(-1)
+    
     if max_x > 0:
         slant_depths = np.linspace(0, min(slant_depth_data[1][-1], max_x), x_bins)
     else:
         slant_depths = np.linspace(0, slant_depth_data[1][-1], x_bins)
 
     dx = slant_depths[1] - slant_depths[0]
 
-    # Deleting the slant depth data object to save memory
-    del slant_depth_data
-
     # Calculating the distance along the trajectory for each slant depth value
     Ls = L_from_slant_depth(slant_depths)
+    
+    # Deleting the slant depth data object to save memory
+    del slant_depth_data
 
     # Calculating the altitude of each slant depth value
     zs = geo.z_from_L(Ls, theta_D, detector_altitude)
 
     # Integral calculation for time it takes photon to reach detector plane along shower axis
     # Take points along the path from the emission point to the detection plane
+    
+    #todo: make much faster and more accurate
     Ls_t_value_calc = np.array([np.linspace(L_bottom, L_detector, 1000) for L_bottom in Ls])
 
     # Calculate the index of refraction at these points (using a reference 450nm wavelength)
     zs_t_value_calc = geo.z_from_L(Ls_t_value_calc, theta_D, detector_altitude)
-    ns_t_value_calc = np.array([atm.index_of_refraction(zs_t_value_calc[i], 450) for i in range(0, len(Ls))])
+    ns_t_value_calc = np.array([atm.index_of_refraction(zs_t_value_calc[i], 450) for i in range(len(Ls))])
 
     # Integrate the traversal time taking into account the changing speed of light and clear unneeded values
     t0s = np.trapz(ns_t_value_calc / const.cl, Ls_t_value_calc, axis=1)
     del Ls_t_value_calc, zs_t_value_calc, ns_t_value_calc
 
     # Initialize Wavelength Grid
     wavelength_bins, wavelength_lower, wavelength_upper = run_set.getlist('wavelength')
@@ -183,28 +198,41 @@
     del alpha
 
     ################################################################
     # Initializing shower
 
     # Calculating the number of electrons and positrons for each point in the shower
     if run_set.getboolean('useGreisenParametrization'):
-        charged_parts = elef.Greisen_Longitudinal_Profile(energy, slant_depths)
+        charged_parts = elef.Greisen_Longitudinal_Profile(energy, slant_depths-X0)
     else:
-        if run_set.get('protoShowerPofile') == '':
-            filename = str(files("easchersim.data") / "Example_CORSIKA_proton_1e17eV.long")
+        if run_set.get('protoShowerProfile') == '':
+            if isinstance(input_file, str):
+                filename = input_file
+            else:
+                filename = str(files("easchersim.data") / "Example_CORSIKA_proton_1e17eV.long")
             simulated_energy = 1e17
         else:
-            filename = run_set.get('protoShowerPofile')
+            filename = run_set.get('protoShowerProfile')
             simulated_energy = run_set.getfloat('protoShowerEnergy')
-        charged_parts = elef.CORSIKA_interpolation(energy, slant_depths, filename, simulated_energy)
+        charged_parts = elef.CORSIKA_interpolation(
+            energy,
+            slant_depths-X0,
+            filename,
+            simulated_energy,
+            index=shower_index
+        )
 
     # Calculating the position of the shower maximum, and the corresponding shower ages and radiation lenghts
     shower_xmax = slant_depths[np.argmax(charged_parts)]
     shower_age = 3 / (1 + 2 * shower_xmax / slant_depths)
+    shower_age[shower_age == 0] = 0.001
     radiation_lengths = (slant_depths - shower_xmax) / 36.7
+    
+    zmax = zs[np.argmax(charged_parts)]
+    ch_max = chf.Cherenkov_angle(zmax, 450, 1)
 
     ################################################################
     # Initializing Cherenkov photons
 
     # Calculating the threshold energy for Cherenkov production for each point,
     # using a reference 450nm wavelength
     Cherenkov_thresholds = chf.Cherenkov_threshold(zs, 450)
@@ -265,36 +293,40 @@
     # Initializing the bins in azimuth about which to calculate photon content
     azimuth_bins = run_set.getint('ringAzimuthNumBin')
     Cherenkov_ring_azimuth = np.linspace(0, 2 * np.pi, azimuth_bins)
 
     ################################################################
     # Initializing the arrays to be used for the spatial, timing, and angular distributions of the arriving photons
 
-    spatial_counts, time_counts, angle_counts = 0, 0 , 0
+    spatial_counts, time_counts, phZenith_counts, phAzi_counts, t_counts = 0, 0, 0, 0, 0
 
     spatial_bins = int(run_set.getlist('phSpatial')[0])
     bins, start, stop = run_set.getlist('phTime')
     time_bins = np.logspace(float(start), float(stop), num=int(bins))
     bins, start, stop = run_set.getlist('phZenith')
-    angle_bins = np.logspace(float(start), float(stop), num=int(bins))
+    phZenith_bins = np.logspace(float(start), float(stop), num=int(bins))
+    bins, start, stop = run_set.getlist('phAzimuth')
+    bin_size = (float(stop) - float(start)) / float(bins)
+    phAzi_bins = np.arange(float(start), float(stop), bin_size) 
 
     # If generating plots, initialize the 2D spatial array
-    if plot.Plot[plots] > 0:
+    if plot.Plot[plots] > 0 or mag_field.getboolean('useField'):
         det_array = 0
 
     ################################################################
     # Beginning main loop
     # Loop over electron energy bins (start with the bin at the Cherenkov threshold for each altitude and move up to considered upper bound)
 
     with io_func.get_progress() as progress:
         io_func.flog(f'''Computing the Cherenkov Photon properties at an altitude of '''
                      f'''{detector_altitude}km for one EAS \n''')
-        task = progress.add_task(f"1.Shower({energy}eV,{theta_D}deg,{L_particle}km)",
+        task = progress.add_task(f"1.Shower({energy}eV,{theta_D}deg,{L_particle}km,{X0}g/cm^2)",
                                  total=electron_energies.shape[1])
-        for i in range(0, electron_energies.shape[1]):
+
+        for i in range(electron_energies.shape[1]):
             # Selecting the electron energies and the Cherenkov photons emitted at this energy
             electron_energy, transmitted_photons = electron_energies[:, i], W_integrated_photons[:, i]
 
             # Calculate Lorentz factor and particle relative velocity to the speed of light
             electron_velocity = elef.particle_velocity(electron_energy)
 
             # Calculate the Cherenkov angle for each point and electron energy for a reference wavelength of 450nm
@@ -305,155 +337,237 @@
             Cherenkov_angles[undefined_Cherenkov_angle] = 0
             transmitted_photons[undefined_Cherenkov_angle] = 0
 
             # Calculate Zenith angles and dn values at angles
             [electron_zenith_angle, electron_angular_content] = elef.Hillas_Angular_Distribution(electron_energy,
                                                                                                  shower_age,
                                                                                                  scaled_angle_u)
+            #[electron_zenith_angle, electron_angular_content] = elef.Lafebre_Angular_Distribution(electron_energy,
+            #                                                                                     scaled_angle_u)
 
             # Dividing the generated Cherenkov photons into the corresponding bins in zenith angle
             angular_transmitted_photons = transmitted_photons[None, :] * electron_angular_content
 
             # Calculating the coordinates of the projected Cherenkov ring on the detection plane
             [ellipse_x, ellipse_y] = geo.ellipse_coordinates(Ls, L_detector,
                                                              electron_zenith_angle,
                                                              Cherenkov_angles, Cherenkov_ring_azimuth)
 
             # Calculating the arrival angle of the photons on the detection plane
             photon_arrival_angles = (180 / np.pi) * \
                 np.arctan(np.sqrt(ellipse_x**2 + ellipse_y**2) / (L_detector - Ls[None, :, None]))
+                
+            photon_azimuth_angles = (180/np.pi)*np.arctan2(ellipse_y, ellipse_x)
 
             # Randomly sampling lateral offsets and lag times for each Cherenkov photon generated
-            lateral_offsets = elef.Lafebre_Lateral_Distribution(electron_energy, radiation_lengths, zs, ellipse_x)
+            if run_set.get('lat_dist') == 'Lafebre':
+                lateral_offsets = elef.Lafebre_Lateral_Distribution(electron_energy, radiation_lengths, zs, ellipse_x)
+            elif run_set.get('lat_dist') == 'NKG':
+                # The NKG parameterization has no energy dependence so there is no need to calculate multiple times
+                if i == 0:
+                    lateral_offsets = elef.NKG_Lateral_Distribution(shower_age, zs, ellipse_x)
+            else:
+                print('Unknown lateral distribution, exiting...')
+                sys.exit(-1)
             lag_times = elef.Lafebre_Lag_Time_Distribution(electron_energy, radiation_lengths, zs, ellipse_x)
 
             # Smearing sampled lateral offsets by randomly sampled azimuth angle
             sampled_angles = np.random.uniform(0, 2 * np.pi, size=ellipse_x.shape)
             x_offsets, y_offsets = lateral_offsets * np.cos(sampled_angles), lateral_offsets * np.sin(sampled_angles)
 
-            del sampled_angles, lateral_offsets
+            del sampled_angles
+            
+            if run_set.get('lat_dist') == 'Lafebre':
+                del lateral_offsets
 
             # Adding the randomly sampled offsets to each point about the Cherenkov ring
             ellipse_x += x_offsets
             ellipse_y += y_offsets
+            
+            photon_azimuth_angles_new = (180/np.pi)*np.arctan2(ellipse_y, ellipse_x)
+            azimuth_angles = photon_azimuth_angles_new - photon_azimuth_angles
+            
+            azi_below = azimuth_angles<-180
+            azi_above = azimuth_angles>180
+            azimuth_angles[azi_below] = 360+azimuth_angles[azi_below]
+            azimuth_angles[azi_above] = -360+azimuth_angles[azi_above]
 
-            del x_offsets, y_offsets
+            del x_offsets, y_offsets, photon_azimuth_angles, photon_azimuth_angles_new, azi_below, azi_above
 
             # Calculating the distance from the shower axis for each point (in order to consider azimuthal symmetry)
             r_coordinates = np.sqrt(ellipse_x**2 + ellipse_y**2)
 
             del ellipse_x, ellipse_y
             total_propagation_times = (Ls[None, :, None] / const.cl + t0s[None, :, None] / np.cos((np.pi / 180) * photon_arrival_angles) + lag_times) / 1e-9
             total_propagation_times -= np.nanmin(total_propagation_times)
 
             # Calculating the number of Cherenkov photons arriving on the detection plane at each point along the Cherenkov ring
             photons_on_plane = (1 / azimuth_bins) * angular_transmitted_photons[:, :, None] * np.ones(azimuth_bins)[None, None, :]
 
             # Ignoring points which do not intersect the plane
-            nan_indexes = np.isnan(r_coordinates)
+            nan_indexes = np.logical_or(np.isnan(r_coordinates), np.isnan(total_propagation_times))
             r_coordinates[nan_indexes] = 0
             total_propagation_times[nan_indexes] = 0
             photon_arrival_angles[nan_indexes] = 0
             photons_on_plane[nan_indexes] = 0
 
             # The first iteration of the loop has the maximum photon content, so at this step, the bounds are determined for the 2D histograms
             # that will be carried out for futher iterations in the loop
             if i == 0:
                 # Find r bins such that a certain percentage of the total photon content is captured
                 # We recommend 30% for near ring behavior
                 pct_cap = float(run_set.getlist('phSpatial')[1])
                 r_percentiles = fitf.weighted_percentile(r_coordinates.flatten(), pct_cap, weights=photons_on_plane.flatten())
+                r_bins_3d = np.linspace(0, r_percentiles, spatial_bins)
                 r_bins = np.linspace(0, r_percentiles, spatial_bins)
+                #r_bins = np.linspace(0,np.tan(10*ch_max*np.pi/180)*(L_detector-L_particle), spatial_bins)
+                #r_bins = np.tan(np.logspace(-3, 1, 200)*np.pi/180)*(L_detector-L_particle)
 
                 # Calculate the size of one spatial bin in m^2
-                pixel_size = ((r_bins[1] - r_bins[0]) * 1000)**2
+                pixel_size = ((r_bins_3d[1] - r_bins_3d[0]) * 1000)**2
 
                 # Initializing the arrays to store the upper and lower bounds for the timing and angular photon distributions
                 time_bounds, zenith_bounds = [], []
 
                 # Loop over the spatial bins
-                for j in range(0, len(r_bins) - 1):
+                for j in range(len(r_bins) - 1):
                     # Find coordinates which are inside each spatial bin
+                    
                     r_lower, r_upper = r_bins[j], r_bins[j + 1]
                     in_range = (r_coordinates >= r_lower) & (r_coordinates <= r_upper)
                     in_range_time, in_range_zenith, in_range_photons = total_propagation_times[in_range], photon_arrival_angles[in_range], photons_on_plane[in_range]
+                    
 
-                    # Calculate the 1% and 99% weighted percentiles of the arrival time and arrival angle inside the bin
-                    time_percentiles = fitf.weighted_percentile(in_range_time.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
-                    zenith_percentiles = fitf.weighted_percentile(in_range_zenith.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
+                    '''
+                    in_range_azimuth, in_range_azimuth_new = photon_azimuth_angles[in_range], photon_azimuth_angles_new[in_range]
+                    delta_azi = in_range_azimuth_new-in_range_azimuth
+                    fig = plt.figure()
+                    to_plot_angle = in_range_zenith-min(in_range_zenith)
+                    #plt.hist(to_plot_angle, weights = in_range_photons, bins = phZenith_bins)
+                    print(min(np.abs(delta_azi)))
+                    plt.hist(delta_azi, weights = in_range_photons, bins = np.arange(-360, 360, 1))
+                    #plt.hist(to_plot_angle, weights = in_range_photons, bins = np.linspace(0,4,70))
+                    #plt.xscale('log')
+                    plt.show()
+                    '''
+                    
+                    if len(in_range_time.flatten()>0):
+                        # Calculate the 1% and 99% weighted percentiles of the arrival time and arrival angle inside the bin
+                        time_percentiles = fitf.weighted_percentile(in_range_time.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
+                        zenith_percentiles = fitf.weighted_percentile(in_range_zenith.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
+                    else:
+                        print(r_bins[j])
+                        #r_lower, r_upper = r_bins[max(j-10,0)], r_bins[min(j + 10, len(r_bins)- 1)]
+                        #in_range = (r_coordinates >= r_lower) & (r_coordinates <= r_upper)
+                        #in_range_time, in_range_zenith, in_range_photons = total_propagation_times[in_range], photon_arrival_angles[in_range], photons_on_plane[in_range]
+                        
+                        #time_percentiles = fitf.weighted_percentile(in_range_time.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
+                        #zenith_percentiles = fitf.weighted_percentile(in_range_zenith.flatten(), np.array([1, 99]), weights=in_range_photons.flatten())
+                        time_percentiles = [0, 0]
+                        zenith_percentiles = [0, 0]
+                    #print(time_percentiles)
 
                     time_bounds.append(time_percentiles)
                     zenith_bounds.append(zenith_percentiles)
+                    
 
                 # Calculate the lower bound time and zenith offsets as a function of r (in km)
                 time_offset = interpolate.interp1d(r_bins[:-1], np.array(time_bounds)[:, 0], kind='cubic', bounds_error=False, fill_value=0)
                 angle_offset = interpolate.interp1d(r_bins[:-1], np.array(zenith_bounds)[:, 0], kind='cubic', bounds_error=False, fill_value=0)
 
             # Plot the photon intensity (in photons/m^2) in 2 dimensions
-            if plot.Plot[plots] > 0:
+            if plot.Plot[plots] > 0 or mag_field.getboolean('useField'):
                 # Smear the calculated distances from shower axis about the axis random;y
                 random_azimuth_angles = np.random.uniform(0, 2 * np.pi, size=r_coordinates.shape)
                 x_coordinates, y_coordinates = r_coordinates * np.cos(random_azimuth_angles), r_coordinates * np.sin(random_azimuth_angles)
 
                 # Shift the x coordinates by the calculated offset due to geomagnetic deflection (axis is arbitrary)
                 if mag_field.getboolean('useField'):
-                    x_coordinates += elef.geomagnetic_deflection_correction(Ls, L_detector,
-                                                                            electron_energy,
-                                                                            electron_zenith_angle,
-                                                                            Cherenkov_ring_azimuth,
-                                                                            mag_field.getfloat('strength'),
-                                                                            mag_field.getfloat('angle'))
+                    x_coordinates += elef.updated_geomagnetic_deflection_correction(Ls, L_detector, zs, scaled_angle_u, shower_age, electron_energy, photon_arrival_angles, 
+                                                                         random_azimuth_angles, mag_field.getfloat('strength'), 
+                                                                         mag_field.getfloat('angle'))
 
                 # Update the 2D array stored in memory
-                current_array = np.histogram2d(np.abs(x_coordinates.flatten()), np.abs(y_coordinates.flatten()), bins=(r_bins, r_bins), weights=photons_on_plane.flatten() / (4 * pixel_size))[0]
+                current_array = np.histogram2d(np.abs(x_coordinates.flatten()), np.abs(y_coordinates.flatten()), bins=(r_bins_3d, r_bins_3d), weights=photons_on_plane.flatten() / (4 * pixel_size))[0]
                 det_array += current_array
 
                 del random_azimuth_angles, x_coordinates, y_coordinates
 
             # Shifting the calculated values by the lower offset
             total_propagation_times -= time_offset(r_coordinates.flatten()).reshape(total_propagation_times.shape)
             photon_arrival_angles -= angle_offset(r_coordinates.flatten()).reshape(photon_arrival_angles.shape)
+            
+
 
             # Calculating the 1D histogram for the spatial counts and the 2D histogram for the arrival times and arrival angles
             spatial_counts += np.histogram(r_coordinates.flatten(), r_bins, weights=photons_on_plane.flatten())[0]
             time_counts += np.histogram2d(r_coordinates.flatten(), total_propagation_times.flatten(), bins=(r_bins, time_bins), weights=photons_on_plane.flatten())[0]
-            angle_counts += np.histogram2d(r_coordinates.flatten(), photon_arrival_angles.flatten(), bins=(r_bins, angle_bins), weights=photons_on_plane.flatten())[0]
+            phZenith_counts += np.histogram2d(r_coordinates.flatten(), photon_arrival_angles.flatten(), bins=(r_bins, phZenith_bins), weights=photons_on_plane.flatten())[0]
+            phAzi_counts += np.histogram2d(r_coordinates.flatten(), azimuth_angles.flatten(), bins=(r_bins, phAzi_bins), weights=photons_on_plane.flatten())[0]
+            t_counts += np.histogramdd(
+                [r_coordinates.flatten(), photon_arrival_angles.flatten(), total_propagation_times.flatten()],
+                bins=(r_bins, phZenith_bins, time_bins), weights=photons_on_plane.flatten())[0]
 
             del r_coordinates, total_propagation_times, photon_arrival_angles, photons_on_plane
             progress.advance(task)
     io_func.flog("[bold blue]Shower 1 done! :heavy_check_mark:")
-
+    
     # Plotting Wavelength, Angular, Time, and Spatial Distributions of the arriving Cherenkov photons
     if plot.Plot[plots] > 0:
         wl = plot.plot_wavelength_distribution(wavelengths, X_integrated_photons)
-        ph_as = plot.plot_photon_angular_spread(r_bins, angle_bins, angle_counts)
+        ph_thetas = plot.plot_photon_angular_spread(r_bins, phZenith_bins, phZenith_counts, "zenith")
+        ph_azis = plot.plot_photon_angular_spread(r_bins, phAzi_bins, phAzi_counts, "azimuth")
         ph_ts = plot.plot_photon_time_spread(r_bins, time_bins, time_counts)
         ph_3d_sd = plot.plot_3D_spatial_distribution(r_bins, det_array)
         if save_fig:
             wl.savefig(plot.plot_out_dir + "wavelen_dist.png")
-            ph_as.savefig(plot.plot_out_dir +"ph_angular_spread.png")
+            ph_thetas.savefig(plot.plot_out_dir +"ph_theta_spread.png")
+            ph_azis.savefig(plot.plot_out_dir +"ph_azimuth_spread.png")
             ph_ts.savefig(plot.plot_out_dir +"ph_time_spread.png")
             ph_3d_sd.savefig(plot.plot_out_dir +"ph_3D_spatial_dist.png")
 
     # Correcting the spatial counts to account for the area of the ring (photons/m^2)
     ring_area = np.pi * ((r_bins[1:] * 1000)**2 - (r_bins[:-1] * 1000)**2)
     spatial_counts = spatial_counts / (ring_area)
 
+    # r_bins = (180/np.pi)*np.arctan(r_bins/(L_detector-L_particle))
+
     ################################################################
+    if mag_field.getboolean('useField'):
+        cher_res = {
+            "wavelengths" : wavelengths,
+            "wavelength_counts" : X_integrated_photons[:-1],
+            "r_bins" : r_bins,
+            "r_counts" : np.array([spatial_counts, (det_array[0,:]+det_array[1,:]+det_array[2,:])/3, (det_array[:,0]+det_array[:,1]+det_array[:,2])/3]),
+            "time_bins" : time_bins,
+            "time_counts" : time_counts,
+            "lower_times" : np.array(time_bounds)[:, 0],
+            "phZenith_bins" : phZenith_bins,
+            "phZenith_counts" : phZenith_counts,
+            "phAzi_bins" : phAzi_bins,
+            "phAzi_counts" : phAzi_counts,
+            "t_counts" : t_counts,
+            "lower_phZenith" : np.array(zenith_bounds)[:, 0],
+        }
+
+    else:
+        cher_res = {
+            "wavelengths" : wavelengths,
+            "wavelength_counts" : X_integrated_photons[:-1],
+            "r_bins" : r_bins,
+            "r_counts" : spatial_counts,
+            "time_bins" : time_bins,
+            "time_counts" : time_counts,
+            "lower_times" : np.array(time_bounds)[:, 0],
+            "phZenith_bins" : phZenith_bins,
+            "phZenith_counts" : phZenith_counts,
+            "phAzi_bins" : phAzi_bins,
+            "phAzi_counts" : phAzi_counts,
+            "t_counts" : t_counts,
+            "lower_phZenith" : np.array(zenith_bounds)[:, 0],
+        }
 
-    cher_res = {
-        "wavelengths" : wavelengths,
-        "wavelength_counts" : X_integrated_photons[:-1],
-        "r_bins" : r_bins,
-        "r_counts" : spatial_counts,
-        "time_bins" : time_bins,
-        "time_counts" : time_counts,
-        "lower_times" : np.array(time_bounds)[:, 0],
-        "angle_bins" : angle_bins,
-        "angle_counts" : angle_counts,
-        "lower_angles" : np.array(zenith_bounds)[:, 0],
-    }
 
     if plot.Plot[plots] > 0 and not save_fig:
         plt.show()
 
     return cher_res
```

### Comparing `easchersim-1.1/src/easchersim.egg-info/PKG-INFO` & `easchersim-1.2.0/src/easchersim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: easchersim
-Version: 1.1
+Version: 1.2.0
 Summary: A Simulator for Cherenkov photon production and atmopheric transport for Extensive Air Showers
 Home-page: https://gitlab.com/c4341/easchersim
 Author: Austin Cummings, Johannes Eser
 Author-email: alc6658@psu.edu, jeser@uchicago.edu
 License: BSD-3-Clause-Clear
 Keywords: Extensive Air Shower,Cherenkov,neutrinos,Simulation
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: importlib_resources
+Requires-Dist: matplotlib-label-lines
+Requires-Dist: rich
 
 # EASCherSim
 
 ![GitLab Release (latest by date)](https://img.shields.io/gitlab/v/release/c4341/easchersim)
 [![PyPI](https://img.shields.io/pypi/v/easchersim)](https://pypi.org/project/easchersim/)
 [![Conda](https://img.shields.io/conda/v/easchersim/easchersim)](https://anaconda.org/easchersim/easchersim)
 [![pipeline status](https://gitlab.com/c4341/easchersim/badges/main/pipeline.svg)](https://gitlab.com/c4341/easchersim/-/commits/main)
@@ -95,9 +100,7 @@
 # Download & Build
 
 ### Clone the Repository (for development)
 
 1. `git clone https://gitlab.com/c4341/easchersim.git`
 2. `cd easchersim`
 3. `python3 -m pip install -e .`
-
-
```

### Comparing `easchersim-1.1/src/easchersim.egg-info/SOURCES.txt` & `easchersim-1.2.0/src/easchersim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .flake8
 .gitignore
 .gitlab-ci.yml
+CHANGELOG
 LICENSE
 README.md
+my_config_file.ini
 pyproject.toml
 setup.cfg
 docs/conf.py
 docs/index.rst
 docs/requirements
 docs/UserGuide/index.rst
 docs/_static/GSSI_logo.jpeg
```

