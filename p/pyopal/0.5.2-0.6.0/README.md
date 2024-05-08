# Comparing `tmp/pyopal-0.5.2.tar.gz` & `tmp/pyopal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopal-0.5.2.tar", last modified: Wed Feb 28 00:16:18 2024, max compression
+gzip compressed data, was "pyopal-0.6.0.tar", last modified: Wed May  8 16:23:07 2024, max compression
```

## Comparing `pyopal-0.5.2.tar` & `pyopal-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.807437 pyopal-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-02-28 00:15:42.000000 pyopal-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-28 00:15:42.000000 pyopal-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-28 00:15:42.000000 pyopal-0.5.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-28 00:15:42.000000 pyopal-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-02-28 00:16:18.807437 pyopal-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-02-28 00:15:42.000000 pyopal-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.803437 pyopal-0.5.2/pyopal/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/_align.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/_patch.pxi
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/lib.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    49046 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/lib.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/opal.h
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/opal.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.803437 pyopal-0.5.2/pyopal/platform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/platform/pxd.in
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/platform/pyx.in
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/shared_mutex.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.807437 pyopal-0.5.2/pyopal/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_aligner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-28 00:15:42.000000 pyopal-0.5.2/pyopal/tests/test_score_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.803437 pyopal-0.5.2/pyopal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyopal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-28 00:16:18.000000 pyopal-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-28 00:16:18.807437 pyopal-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    23360 2024-02-28 00:15:42.000000 pyopal-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.799437 pyopal-0.5.2/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.807437 pyopal-0.5.2/vendor/opal/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.807437 pyopal-0.5.2/vendor/opal/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/ScoreMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/ScoreMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    86516 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/opal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/opal.h
--rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/opal_aligner.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 00:16:18.807437 pyopal-0.5.2/vendor/opal/src/score_matrices/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/blosum45.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/blosum50.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/blosum62.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/blosum80.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/pam120.mat
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/score_matrices/pam250.mat
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-02-28 00:15:42.000000 pyopal-0.5.2/vendor/opal/src/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.159912 pyopal-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-08 16:22:53.000000 pyopal-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-08 16:22:53.000000 pyopal-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 16:22:53.000000 pyopal-0.6.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-08 16:22:53.000000 pyopal-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-08 16:23:07.159912 pyopal-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-05-08 16:22:53.000000 pyopal-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.155912 pyopal-0.6.0/pyopal/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/_align.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/_patch.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/lib.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47588 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/lib.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-08 16:22:55.000000 pyopal-0.6.0/pyopal/opal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/opal.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.155912 pyopal-0.6.0/pyopal/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/platform/pxd.in
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/platform/pyx.in
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/shared_mutex.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.155912 pyopal-0.6.0/pyopal/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-08 16:22:53.000000 pyopal-0.6.0/pyopal/tests/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.155912 pyopal-0.6.0/pyopal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyopal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 16:23:07.000000 pyopal-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-08 16:23:07.159912 pyopal-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-05-08 16:22:53.000000 pyopal-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.151912 pyopal-0.6.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.155912 pyopal-0.6.0/vendor/opal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.159912 pyopal-0.6.0/vendor/opal/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/ScoreMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/ScoreMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    86516 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/opal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/opal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/opal_aligner.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:23:07.159912 pyopal-0.6.0/vendor/opal/src/score_matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/blosum45.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/blosum50.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/blosum62.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/blosum80.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/pam120.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/score_matrices/pam250.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-08 16:22:55.000000 pyopal-0.6.0/vendor/opal/src/test.cpp
```

### Comparing `pyopal-0.5.2/CHANGELOG.md` & `pyopal-0.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pyopal/compare/v0.5.2...HEAD
+[Unreleased]: https://github.com/althonos/pyopal/compare/v0.6.0...HEAD
+
+
+## [v0.6.0] - 2024-05-08
+[v0.6.0]: https://github.com/althonos/pyopal/compare/v0.5.2...v0.6.0
+
+### Changed
+- Use `scoring-matrices` package to handle scoring matrices.
+- Import Cython classes from `pyopal.lib` in the main `pyopal` namespace.
+
+### Fixed
+- Patching of architecture flags of MacOS compilers.
+
+### Removed
+- The `ScoreMatrix` class from `pyopal.lib`.
 
 
 ## [v0.5.2] - 2024-02-28
 [v0.5.2]: https://github.com/althonos/pyopal/compare/v0.5.1...v0.5.2
 
 ### Fixed
 - Segmentation fault when attempting to align to an empty `Database` ([#6](https://github.com/althonos/pyopal/issues/6)).
```

### Comparing `pyopal-0.5.2/CONTRIBUTING.md` & `pyopal-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/COPYING` & `pyopal-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/MANIFEST.in` & `pyopal-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/PKG-INFO` & `pyopal-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.5.2
+Version: 0.6.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
```

### Comparing `pyopal-0.5.2/README.md` & `pyopal-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/__init__.py` & `pyopal-0.6.0/pyopal/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 __author__ = "Martin Larralde <martin.larralde@embl.de>"
 __license__ = "MIT"
 __all__ = [
     "Alphabet",
     "Aligner",
     "BaseDatabase",
     "Database",
-    "ScoreMatrix",
     "ScoreResult",
     "EndResult",
     "FullResult",
     "align",
 ]
 
 from . import lib
 from ._align import align
 from .lib import (
     Alphabet,
     Aligner,
     BaseDatabase,
     Database,
-    ScoreMatrix,
     ScoreResult,
     EndResult,
     FullResult,
 )
 
 # Use the library documentation
 __doc__ = lib.__doc__
```

### Comparing `pyopal-0.5.2/pyopal/_align.py` & `pyopal-0.6.0/pyopal/_align.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import contextlib
 import functools
 import multiprocessing.pool
 import os
 
+from scoring_matrices import ScoringMatrix
+
 from .lib import (
     Aligner,
     BaseDatabase,
     Database,
-    ScoreMatrix,
     ScoreResult,
     FullResult,
     EndResult,
 )
 
 @contextlib.contextmanager
 def nullcontext(enter_result):
@@ -23,15 +24,15 @@
     """
     yield enter_result
 
 
 def align(
     query,
     database,
-    score_matrix = None,
+    scoring_matrix = None,
     *,
     gap_open = 3,
     gap_extend = 1,
     mode = "score",
     overflow = "buckets",
     algorithm = "sw",
     threads = 0,
@@ -41,16 +42,18 @@
     """Align the query sequence to every database sequence in parallel.
 
     Arguments:
         query (`str` or byte-like object): The sequence to query the
             database with.
         database (iterable of `str` or byte-like objects): The database 
             sequences to align the query to. 
-        score_matrix (`~pyopal.ScoreMatrix`): The scoring matrix
-            to use for the alignment.
+        scoring_matrix (`~scoring_matrices.ScoringMatrix` or `str`): The 
+            scoring matrix to use for the alignment, either as a 
+            `ScoringMatrix` object, or as the name of a matrix to load
+            with the `ScoringMatrix.from_name` class method.
 
     Keyword Arguments:
         gap_open(`int`): The gap opening penalty :math:`G` for
             scoring the alignments.
         gap_extend (`int`): The gap extension penalty :math:`E`
             for scoring the alignments.
         mode (`str`): The search mode to use for querying the database:
@@ -109,25 +112,30 @@
 
     .. versionadded:: 0.5.0
 
     """
     # derive default parameters
     if threads == 0:
         threads = os.cpu_count() or 1
-    if score_matrix is None:
-        score_matrix = ScoreMatrix.aa()
+    if scoring_matrix is None:
+        scoring_matrix = Aligner._DEFAULT_SCORING_MATRIX
+    elif isinstance(scoring_matrix, str):
+        scoring_matrix = ScoringMatrix.from_name(scoring_matrix)
+    elif not isinstance(scoring_matrix, ScoringMatrix):
+        ty = type(scoring_matrix).__name__
+        raise TypeError(f"expected str or ScoringMatrix, got {ty}")
     if not isinstance(database, BaseDatabase):
-        database = Database(database, score_matrix.alphabet)
+        database = Database(database, scoring_matrix.alphabet)
 
     # avoid using more threads than necessary
     if threads > len(database):
         threads = len(database) or 1
 
     # align query to database
-    aligner = Aligner(score_matrix, gap_open=gap_open, gap_extend=gap_extend)
+    aligner = Aligner(scoring_matrix, gap_open=gap_open, gap_extend=gap_extend)
     if threads == 1:
         # use main thread if a single thread is needed
         yield from aligner.align(
             query, 
             database, 
             mode=mode, 
             overflow=overflow,
```

### Comparing `pyopal-0.5.2/pyopal/_align.pyi` & `pyopal-0.6.0/pyopal/_align.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import contextlib
 import functools
 import multiprocessing.pool
 import os
 import typing
 
+from scoring_matrices import ScoringMatrix
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 from .lib import (
     Aligner,
     BaseDatabase,
     Database,
-    ScoreMatrix,
     ScoreResult,
     FullResult,
     EndResult,
 )
 
 ALIGN_MODE = Literal["score", "end", "full"]
 ALIGN_OVERFLOW = Literal["simple", "buckets"]
@@ -29,45 +30,45 @@
 def nullcontext(enter_result: T) -> typing.Iterator[T]: ...
 
 
 @typing.overload
 def align(
     query: typing.Union[str, bytes, bytearray],
     database: typing.Union[BaseDatabase, typing.Iterable[typing.Union[str, bytes, bytearray]]],
-    score_matrix: typing.Optional[ScoreMatrix] = None,
+    scoring_matrix: typing.Union[ScoringMatrix, str, None] = None,
     *,
     gap_open: int = 3,
     gap_extend: int = 1,
     mode: Literal["end"],
     overflow: Literal["simple", "buckets"] = "buckets",
     algorithm: Literal["nw", "hw", "ov", "sw"] = "sw",
     threads: int = 0,
 ) -> typing.Iterator[EndResult]:
     ...
 
 @typing.overload
 def align(
     query: typing.Union[str, bytes, bytearray],
     database: typing.Union[BaseDatabase, typing.Iterable[typing.Union[str, bytes, bytearray]]],
-    score_matrix: typing.Optional[ScoreMatrix] = None,
+    scoring_matrix: typing.Union[ScoringMatrix, str, None] = None,
     *,
     gap_open: int = 3,
     gap_extend: int = 1,
     mode: Literal["full"],
     overflow: Literal["simple", "buckets"] = "buckets",
     algorithm: Literal["nw", "hw", "ov", "sw"] = "sw",
     threads: int = 0,
 ) -> typing.Iterator[FullResult]:
     ...
 
 @typing.overload
 def align(
     query: typing.Union[str, bytes, bytearray],
     database: typing.Union[BaseDatabase, typing.Iterable[typing.Union[str, bytes, bytearray]]],
-    score_matrix: typing.Optional[ScoreMatrix] = None,
+    scoring_matrix: typing.Union[ScoringMatrix, str, None] = None,
     *,
     gap_open: int = 3,
     gap_extend: int = 1,
     mode: Literal["score", "end", "full"] = "score",
     overflow: Literal["simple", "buckets"] = "buckets",
     algorithm: Literal["nw", "hw", "ov", "sw"] = "sw",
     threads: int = 0,
```

### Comparing `pyopal-0.5.2/pyopal/lib.pxd` & `pyopal-0.6.0/pyopal/lib.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # --- C imports ----------------------------------------------------------------
 
 from libc.limits cimport UCHAR_MAX
 from libcpp cimport bool, nullptr
 from libcpp.vector cimport vector
 from libcpp.memory cimport shared_ptr
 
+from scoring_matrices cimport ScoringMatrix
+
 from . cimport opal
 from .opal cimport OpalSearchResult
 from .shared_mutex cimport shared_mutex
 
 # --- Constants ----------------------------------------------------------------
 
 cdef extern from * nogil:
@@ -75,19 +77,14 @@
 
     cpdef void encode_into(self, const unsigned char[:] sequence, digit_t[:] encoded)
     cpdef void decode_into(self, const digit_t[:] encoded, unsigned char[:] sequence)
 
     cpdef bytes encode(self, object sequence)
     cpdef str decode(self, object encoded)
 
-cdef class ScoreMatrix:
-    cdef vector[int]       _matrix
-    cdef Py_ssize_t        _shape[2]
-    cdef readonly Alphabet alphabet
-
 # --- Sequence storage ---------------------------------------------------------
 
 cdef class BaseDatabase:
     cdef readonly SharedMutex      lock
     cdef readonly Alphabet         alphabet
 
     cdef const digit_t** get_sequences(self) except? NULL
@@ -125,12 +122,14 @@
     cdef int _target_length
 
     cpdef str cigar(self)
     cpdef float identity(self)
     cpdef float coverage(self, str reference=*)
 
 cdef class Aligner:
-    cdef readonly Alphabet    alphabet
-    cdef readonly ScoreMatrix score_matrix
-    cdef readonly int         gap_open
-    cdef readonly int         gap_extend
-    cdef          searchfn_t  _search
+    cdef readonly Alphabet      alphabet
+    cdef readonly ScoringMatrix scoring_matrix
+    cdef readonly int           gap_open
+    cdef readonly int           gap_extend
+    
+    cdef          searchfn_t    _search
+    cdef          int*          _int_matrix
```

### Comparing `pyopal-0.5.2/pyopal/lib.pyi` & `pyopal-0.6.0/pyopal/lib.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sys
 import typing
 
+from scoring_matrices import ScoringMatrix
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 ALIGN_MODE = Literal["score", "end", "full"]
 ALIGN_OVERFLOW = Literal["simple", "buckets"]
@@ -21,28 +23,14 @@
     def __reduce__(self) -> typing.Tuple[typing.Type[Alphabet], typing.Tuple[str]]: ...
     def __repr__(self) -> str: ...
     def __eq__(self, obj: object) -> bool: ...
     def __str__(self) -> str: ...
     def encode(self, sequence: typing.Union[bytes, bytearray, memoryview]) -> bytes: ...
     def decode(self, encoded: typing.Union[bytes, bytearray, memoryview]) -> str: ...
 
-class ScoreMatrix:
-    @classmethod
-    def aa(cls) -> ScoreMatrix: ...
-    def __init__(
-        self, 
-        alphabet: typing.Union[str, Alphabet], 
-        matrix: typing.Iterable[typing.Iterable[int]],
-    ) -> None: ...
-    def __repr__(self) -> str: ...
-    def __reduce__(self) -> typing.Tuple[object, ...]: ...
-    @property
-    def alphabet(self) -> Alphabet: ...
-    @property
-    def matrix(self) -> typing.List[typing.List[int]]: ...
 
 # --- Sequence storage ---------------------------------------------------------
 
 class BaseDatabase(typing.Sequence[str]):
     @property
     def alphabet(self) -> Alphabet: ...
     def __len__(self) -> int: ...
@@ -121,21 +109,21 @@
     def cigar(self) -> str: ...
     def identity(self) -> float: ...
     def coverage(self, reference: COVERAGE_REFERENCE = "query") -> float: ...
 
 class Aligner:
     def __init__(
         self,
-        score_matrix: typing.Optional[ScoreMatrix] = None,
+        scoring_matrix: typing.Union[ScoringMatrix, str, None] = None,
         *,
         gap_open: int = 3,
         gap_extend: int = 10
     ) -> None: ...
     @property
-    def score_matrix(self) -> ScoreMatrix: ...
+    def scoring_matrix(self) -> ScoringMatrix: ...
     @property
     def alphabet(self) -> Alphabet: ...
     @property
     def gap_open(self) -> int: ...
     @property
     def gap_extend(self) -> int: ...
     @typing.overload
```

### Comparing `pyopal-0.5.2/pyopal/lib.pyx` & `pyopal-0.6.0/pyopal/lib.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
       PLoS One. 2015;10(12):e0145857. Published 2015 Dec 31.
       :doi:`10.1371/journal.pone.0145857`.
 
 """
 
 # --- C imports ----------------------------------------------------------------
 
+from libc.stdlib cimport calloc, free
 from libc.string cimport memset, memcpy, memcmp
 from libc.stdint cimport uint32_t, UINT32_MAX
 from libc.limits cimport UCHAR_MAX
 from libcpp cimport bool
 from libcpp.numeric cimport accumulate
 from libcpp.vector cimport vector
 from libcpp.memory cimport shared_ptr
@@ -31,14 +32,16 @@
     PyUnicode_KIND,
     PyUnicode_DATA,
     PyUnicode_READ,
     PyUnicode_GET_LENGTH,
     PyUnicode_1BYTE_KIND
 )
 
+from scoring_matrices cimport ScoringMatrix
+
 from . cimport opal
 from .opal cimport OpalSearchResult
 from .shared_mutex cimport shared_mutex
 
 if NEON_BUILD_SUPPORT:
     from pyopal.platform.neon cimport opalSearchDatabaseNEON
 if SSE2_BUILD_SUPPORT:
@@ -69,15 +72,14 @@
 # --- Python imports -----------------------------------------------------------
 
 import operator
 from string import ascii_lowercase
 
 include "_version.py"
 include "_patch.pxi"
-include "matrices.pxi"
 
 # --- Constants ----------------------------------------------------------------
 
 cdef dict _OPAL_SEARCH_MODES = {
     "score": opal.OPAL_SEARCH_SCORE,
     "end": opal.OPAL_SEARCH_SCORE_END,
     "full": opal.OPAL_SEARCH_ALIGNMENT,
@@ -313,142 +315,14 @@
 
         """
         cdef bytearray decoded = bytearray(len(encoded))
         self.decode_into(encoded, decoded)
         return decoded.decode('ascii')
 
 
-cdef class ScoreMatrix:
-    """A score matrix for comparing character matches in sequences.
-
-    Attributes:
-        alphabet (`~pyopal.Alphabet`): The alphabet object storing the
-            letters corresponding to column and row indices of the
-            scoring matrix.
-
-    """
-
-    @classmethod
-    def aa(cls, name: str = "BLOSUM50"):
-        """Create a scoring matrix from a built-in matrix.
-
-        Arguments:
-            name (`str`): The name of the built-in scoring matrix
-                to use. Supported values are: ``BLOSUM45``, ``BLOSUM50``,
-                ``BLOSUM62``, ``PAM120`` and ``PAM250``.
-
-        Note:
-            Only ``BLOSUM50`` is configured to support unknown alphabet
-            symbols.
-
-        .. versionchanged:: 0.5.0
-           Support for additional scoring matrices from Opal.
-
-        """
-        if not name in _SCORE_MATRICES:
-            raise ValueError(f"unknown scoring matrix: {name!r}")
-        letters, matrix = _SCORE_MATRICES[name]
-        return cls(letters, matrix)
-
-    def __init__(self, object alphabet not None, object matrix not None):
-        """Create a new score matrix from the given alphabet and scores.
-
-        Arguments:
-            alphabet (`str` or `~pyopal.Alphabet`): The alphabet of the
-                similarity matrix.
-            matrix (`~numpy.typing.ArrayLike` of `int`): The scoring matrix,
-                as a square matrix indexed by the alphabet characters.
-
-        Example:
-            Create a new similarity matrix using the HOXD70 scores by
-            Chiaromonte, Yap and Miller (:pmid:`11928468`)::
-
-                >>> matrix = ScoreMatrix(
-                ...     "ATCG",
-                ...     [[  91, -114,  -31, -123],
-                ...      [-114,  100, -125,  -31],
-                ...      [ -31, -125,  100, -114],
-                ...      [-123,  -31, -114,   91]]
-                ... )
-
-            Create a new similarity matrix using one of the matrices from
-            the `Bio.Align.substitution_matrices` module::
-
-                >>> jones = Bio.Align.substitution_matrices.load('JONES')
-                >>> matrix = ScoreMatrix(jones.alphabet, jones)
-
-        """
-        cdef int           i
-        cdef int           j
-        cdef object        row
-        cdef int           value
-        cdef int           length    = len(matrix)
-
-        if isinstance(alphabet, Alphabet):
-            self.alphabet = alphabet
-        elif isinstance(alphabet, str):
-            self.alphabet = Alphabet(alphabet)
-        else:
-            raise TypeError(f"expected str or Alphabet, found {type(alphabet).__name__!r}")
-
-        if len(self.alphabet) != length:
-            raise ValueError("Alphabet must have the same length as matrix")
-        if not all(len(row) == length for row in matrix):
-            raise ValueError("`matrix` must be a square matrix")
-
-        # record shape
-        self._shape[0] = self._shape[1] = self.alphabet.length
-        # copy the scores
-        self._matrix = vector[int](length * length, 0)
-        for i, row in enumerate(matrix):
-            for j, value in enumerate(row):
-                self._matrix[i*length+j] = value
-
-    def __eq__(self, object other):
-        if not isinstance(other, ScoreMatrix):
-            return NotImplemented
-        return self.alphabet == other.alphabet and self.matrix == other.matrix
-
-    def __repr__(self):
-        cdef str ty = type(self).__name__
-        return f"{ty}({self.alphabet!r}, {self.matrix!r})"
-
-    def __reduce__(self):
-        return (type(self), (self.alphabet, self.matrix))
-
-    def __getbuffer__(self, Py_buffer* buffer, int flags):
-        if flags & PyBUF_FORMAT:
-            buffer.format = b"i"
-        else:
-            buffer.format = NULL
-        buffer.buf = &self._matrix[0]
-        buffer.internal = NULL
-        buffer.itemsize = sizeof(int)
-        buffer.len = self._shape[0] * self._shape[1] * sizeof(int)
-        buffer.ndim = 2
-        buffer.obj = self
-        buffer.readonly = 1
-        buffer.shape = <Py_ssize_t*> &self._shape
-        buffer.suboffsets = NULL
-        buffer.strides = NULL
-
-    @property
-    def matrix(self):
-        """`list` of `list` of `int`: The score matrix.
-        """
-        cdef int        i
-        cdef int        j
-        cdef int        length = self.alphabet.length
-        cdef const int* scores = self._matrix.data()
-
-        return [
-            [ scores[i*length + j] for j in range(length) ]
-            for i in range(length)
-        ]
-
 # --- Sequence storage ---------------------------------------------------------
 
 cdef class BaseDatabase:
     """The base class for views of database sequences.
 
     To allow reusing the rest of the code, this class can be inherited
     from a Cython extension and used with `Aligner.align`. Child classes
@@ -470,16 +344,21 @@
     _DEFAULT_ALPHABET = Alphabet()
 
     # --- Magic methods --------------------------------------------------------
 
     def __cinit__(self):
         self.lock = SharedMutex()
 
-    def __init__(self, object sequences = (), Alphabet alphabet = None):
-        self.alphabet = self._DEFAULT_ALPHABET if alphabet is None else alphabet
+    def __init__(self, object sequences = (), object alphabet = None):
+        if alphabet is None:
+            self.alphabet = self._DEFAULT_ALPHABET
+        elif isinstance(alphabet, Alphabet):
+            self.alphabet = alphabet
+        else:
+            self.alphabet = Alphabet(alphabet)
         if sequences:
             raise TypeError("cannot create a `BaseDatabase` with sequences")
 
     @property
     def lengths(self):
         """`list` of `int`: The length of each sequence in the database.
         """
@@ -580,15 +459,15 @@
     """
 
     # --- Magic methods --------------------------------------------------------
 
     def __cinit__(self):
         self._sequences.clear()
 
-    def __init__(self, object sequences=(), Alphabet alphabet = None):
+    def __init__(self, object sequences=(), object alphabet = None):
         super().__init__(alphabet=alphabet)
         # reset the collection if `__init__` is called more than once
         self.clear()
         # add the sequences to the database
         self.extend(sequences)
 
     def __reduce__(self):
@@ -1201,45 +1080,99 @@
         # compute the final coverage
         return 0.0 if length < 0 else (<float> length) / reflength
 
 
 cdef class Aligner:
     """The Opal aligner.
 
+    The `Aligner` implements an accelerated pipeline for computing pairwise
+    alignments between a query sequence and a database of target sequences
+    in parallel, using :wiki:`Single instruction, multiple data` capacities
+    of modern processors.
+
+    Note:
+        The Opal algorithm requires scoring matrices to be integer
+        matrices, as all computations are handled with integer vectors.
+        Only matrices where the `~scoring_matrices.ScoringMatrix.is_integer`
+        returns `True` can be given to the `Aligner` constructor.
+
+    Attributes:
+        scoring_matrix (`~scoring_matrices.ScoringMatrix`): The scoring
+            matrix to use for scoring the alignments.
+        alphabet (`~pyopal.Alphabet`): The alphabet for encoding sequences
+            before alignment.
+        gap_open(`int`): The gap opening penalty :math:`G` for
+            scoring the alignments.
+        gap_extend (`int`): The gap extension penalty :math:`E`
+            for scoring the alignments.
+
     .. versionadded:: 0.5.0
 
+    .. versionchanged:: 0.6.0
+       Use the external `ScoringMatrix` class to handle scoring matrices.
+
     """
 
-    _DEFAULT_SCORE_MATRIX = ScoreMatrix.aa()
+    _DEFAULT_SCORING_MATRIX = ScoringMatrix.from_name("BLOSUM50")
     _DEFAULT_GAP_OPEN = 3
     _DEFAULT_GAP_EXTEND = 1
 
+    def __cinit__(self):
+        self._int_matrix = NULL
+
+    def __dealloc__(self):
+        free(self._int_matrix)
+
     def __init__(
         self,
-        ScoreMatrix score_matrix = None,
+        object scoring_matrix = None,
         int gap_open = _DEFAULT_GAP_OPEN,
         int gap_extend = _DEFAULT_GAP_EXTEND,
     ):
         """Create a new Aligner with the given parameters.
 
         Arguments:
-            score_matrix (`~pyopal.ScoreMatrix`): The score
-                matrix to use for scoring the alignments.
+            scoring_matrix (`~scoring_matrices.ScoringMatrix` or `str`): The
+                scoring matrix to use for scoring the alignments, either as
+                a `ScoringMatrix` object, or as the name of a matrix to load
+                with the `ScoringMatrix.from_name` class method. The aligner
+                will use the matrix columns to instantiate an `Alphabet`.
             gap_open(`int`): The gap opening penalty :math:`G` for
                 scoring the alignments.
             gap_extend (`int`): The gap extension penalty :math:`E`
                 for scoring the alignments.
 
         Hint:
             A gap of length :math:`N` will receive a penalty of
             :math:`E + (N - 1)G`.
 
-        """
-        self.score_matrix = score_matrix or self._DEFAULT_SCORE_MATRIX
-        self.alphabet = self.score_matrix.alphabet
+        Raises:
+            `ValueError`: When the given scoring matrix is not an integer
+                matrix.
+            `RuntimeError`: When no supported SIMD backend could be detected
+                on the host platform.
+            `MemoryError`: When some internal buffers could not be allocated
+                properly.
+
+        """
+        cdef size_t       i
+        cdef size_t       size
+        cdef const float* data
+
+        if scoring_matrix is None:
+            self.scoring_matrix = self._DEFAULT_SCORING_MATRIX
+        elif isinstance(scoring_matrix, str):
+            self.scoring_matrix = ScoringMatrix.from_name(scoring_matrix)
+        elif isinstance(scoring_matrix, ScoringMatrix):
+            self.scoring_matrix = scoring_matrix
+        else:
+            ty = type(scoring_matrix).__name__
+            raise TypeError(f"expected str or ScoringMatrix, found {ty}")
+
+        self.alphabet = Alphabet(self.scoring_matrix.alphabet)
         self.gap_open = gap_open
         self.gap_extend = gap_extend
 
         # Select the best available SIMD backend
         if SSE2_BUILD_SUPPORT and _SSE2_RUNTIME_SUPPORT:
             self._search = opalSearchDatabaseSSE2
         if SSE4_BUILD_SUPPORT and _SSE4_RUNTIME_SUPPORT:
@@ -1247,26 +1180,38 @@
         if AVX2_BUILD_SUPPORT and _AVX2_RUNTIME_SUPPORT:
             self._search = opalSearchDatabaseAVX2
         if NEON_BUILD_SUPPORT and _NEON_RUNTIME_SUPPORT:
             self._search = opalSearchDatabaseNEON
         if self._search is NULL:
             raise RuntimeError("no supported SIMD backend available")
 
+        # copy alignment weights
+        if not self.scoring_matrix.is_integer():
+            raise ValueError("Integer scoring matrix is expected")
+        with nogil:
+            size = self.scoring_matrix.size()
+            data = self.scoring_matrix.data_ptr()
+            self._int_matrix = <int*> calloc(size*size, sizeof(int))
+            if self._int_matrix == NULL:
+                raise MemoryError("Failed to allocate scoring matrix")
+            for i in range(size*size):
+                self._int_matrix[i] = <int> data[i]
+
     def __repr__(self):
         args = []
-        if self.score_matrix != self._DEFAULT_SCORE_MATRIX:
-            args.append(f"{self.score_matrix!r}")
+        if self.scoring_matrix != self._DEFAULT_SCORING_MATRIX:
+            args.append(f"{self.scoring_matrix!r}")
         if self.gap_open != self._DEFAULT_GAP_OPEN:
             args.append(f"gap_open={self.gap_open!r}")
         if self.gap_extend != self._DEFAULT_GAP_EXTEND:
             args.append(f"gap_extend={self.gap_extend!r}")
         return f"{type(self).__name__}({', '.join(args)})"
 
     def __reduce__(self):
-        return type(self), (self.score_matrix, self.gap_open, self.gap_extend)
+        return type(self), (self.scoring_matrix, self.gap_open, self.gap_extend)
 
     def __eq__(self, object other):
         if not isinstance(other, Aligner):
             return NotImplemented
         return self.__reduce__()[1] == other.__reduce__()[1]
 
     def align(
@@ -1404,15 +1349,15 @@
                         view,
                         length,
                         <digit_t**> &sequences[start],
                         size,
                         <int*> &lengths[start],
                         self.gap_open,
                         self.gap_extend,
-                        self.score_matrix._matrix.data(),
+                        self._int_matrix,
                         self.alphabet.length,
                         results_raw.data(),
                         _mode,
                         _algo,
                         _overflow,
                     )
```

### Comparing `pyopal-0.5.2/pyopal/opal.h` & `pyopal-0.6.0/pyopal/opal.h`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/opal.pxd` & `pyopal-0.6.0/pyopal/opal.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/platform/pxd.in` & `pyopal-0.6.0/pyopal/platform/pxd.in`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/platform/pyx.in` & `pyopal-0.6.0/pyopal/platform/pyx.in`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/tests/__init__.py` & `pyopal-0.6.0/pyopal/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from . import (
     test_aligner,
     test_align,
     test_alphabet,
     test_database,
     test_doctest,
     test_result,
-    test_score_matrix,
 )
 
 
 def load_tests(loader, suite, pattern):
     test_doctest.load_tests(loader, suite, pattern)
     suite.addTests(loader.loadTestsFromModule(test_aligner))
     suite.addTests(loader.loadTestsFromModule(test_align))
     suite.addTests(loader.loadTestsFromModule(test_alphabet))
     suite.addTests(loader.loadTestsFromModule(test_database))
     suite.addTests(loader.loadTestsFromModule(test_result))
-    suite.addTests(loader.loadTestsFromModule(test_score_matrix))
     return suite
```

### Comparing `pyopal-0.5.2/pyopal/tests/test_align.py` & `pyopal-0.6.0/pyopal/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/tests/test_aligner.py` & `pyopal-0.6.0/pyopal/tests/test_aligner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 import random
 import unittest
 
 import pyopal
+from scoring_matrices import ScoringMatrix
+
+
+class TestAligner(unittest.TestCase):
+
+    def test_init_scoring_matrix_str(self):
+        matrix = ScoringMatrix.from_name("VTML80")
+        aligner = pyopal.Aligner("VTML80")
+        self.assertEqual(aligner.scoring_matrix, matrix)
+
+    def test_init_scoring_matrix_object(self):
+        matrix = ScoringMatrix.from_name("VTML80")
+        aligner = pyopal.Aligner(matrix)
+        self.assertEqual(aligner.scoring_matrix, matrix)
+
+    def test_init_scoring_matrix_error(self):
+        self.assertRaises(TypeError, pyopal.Aligner, 1)
 
 
 class _TestSearchOverflow(object):
 
     algorithm = NotImplemented
 
     def test_overflow(self):
```

### Comparing `pyopal-0.5.2/pyopal/tests/test_alphabet.py` & `pyopal-0.6.0/pyopal/tests/test_alphabet.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/tests/test_database.py` & `pyopal-0.6.0/pyopal/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/tests/test_doctest.py` & `pyopal-0.6.0/pyopal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal/tests/test_result.py` & `pyopal-0.6.0/pyopal/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/pyopal.egg-info/PKG-INFO` & `pyopal-0.6.0/pyopal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.5.2
+Version: 0.6.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
```

### Comparing `pyopal-0.5.2/pyopal.egg-info/SOURCES.txt` & `pyopal-0.6.0/pyopal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CONTRIBUTING.md
 COPYING
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+pyopal/__init__.pxd
 pyopal/__init__.py
 pyopal/_align.py
 pyopal/_align.pyi
 pyopal/_patch.pxi
 pyopal/_version.py
 pyopal/lib.pxd
 pyopal/lib.pyi
@@ -30,15 +31,14 @@
 pyopal/tests/__init__.py
 pyopal/tests/test_align.py
 pyopal/tests/test_aligner.py
 pyopal/tests/test_alphabet.py
 pyopal/tests/test_database.py
 pyopal/tests/test_doctest.py
 pyopal/tests/test_result.py
-pyopal/tests/test_score_matrix.py
 vendor/opal/LICENSE
 vendor/opal/README.md
 vendor/opal/src/ScoreMatrix.cpp
 vendor/opal/src/ScoreMatrix.hpp
 vendor/opal/src/opal.cpp
 vendor/opal/src/opal.h
 vendor/opal/src/opal_aligner.cpp
```

### Comparing `pyopal-0.5.2/setup.cfg` & `pyopal-0.6.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,18 @@
 zip_safe = false
 packages = pyopal, pyopal.tests
 include_package_data = false
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
 	cython ~=3.0
+	scoring-matrices ~=0.2
 install_requires = 
 	archspec ~=0.2      ; os_name != 'nt'
+	scoring-matrices ~=0.2
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
 [options.package_data]
 pyopal = py.typed, *.pyi, *.pxd, *.h
 pyopal.tests = requirements.txt
 pyopal.tests.data = *
```

### Comparing `pyopal-0.5.2/setup.py` & `pyopal-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,25 @@
 _HEADER_PATTERN = re.compile("^@@ -(\d+),?(\d+)? \+(\d+),?(\d+)? @@$")
 
 
 def _eprint(*args, **kwargs):
     print(*args, **kwargs, file=sys.stderr)
 
 
-def _patch_osx_compiler(compiler):
+def _patch_osx_compiler(compiler, machine):
     # On newer OSX, Python has been compiled as a universal binary, so
     # it will attempt to pass universal binary flags when building the
     # extension. This will not work because the code makes use of SSE2.
     for tool in ("compiler", "compiler_so", "linker_so"):
         flags = getattr(compiler, tool)
         i = next(
             (
                 i
                 for i in range(1, len(flags))
-                if flags[i - 1] == "-arch" and flags[i] != platform.machine()
+                if flags[i - 1] == "-arch" and flags[i] != machine
             ),
             None,
         )
         if i is not None:
             flags.pop(i)
             flags.pop(i - 1)
 
@@ -116,53 +116,14 @@
         c.set("build-system", "build-backend", '"setuptools.build_meta"')
         with open("pyproject.toml", "w") as pyproject:
             c.write(pyproject)
         # run the rest of the packaging
         _sdist.run(self)
 
 
-class build_matrices(setuptools.Command):
-
-    user_options = [
-        ('force', 'f', 'force generation of files')
-    ]
-
-    def initialize_options(self) -> None:
-        self.force = False
-        self.folder = None
-        self.output = None
-
-    def finalize_options(self) -> None:
-        self.folder = os.path.join("vendor", "opal", "src", "score_matrices")
-        self.output = os.path.join("pyopal", "matrices.pxi")
-
-    def run(self):
-        matrix_files = glob.glob(os.path.join(self.folder, "*.mat"))
-        self.make_file(matrix_files, self.output, self._generate_matrices, (matrix_files, self.output))
-
-    def _parse_matrix_file(self, matrix_file):
-        with open(matrix_file) as f:
-            letters = ''.join(f.readline().strip().split())
-            matrix = [
-                list(map(int, line.strip().split()))
-                for line in map(str.strip, f)
-                if line
-            ]
-            return letters, matrix
-
-    def _generate_matrices(self, matrix_files, output_file):
-        matrices = {}
-        for matrix_file in matrix_files:
-            matrix_name = os.path.splitext(os.path.basename(matrix_file))[0].upper()
-            matrices[matrix_name] = self._parse_matrix_file(matrix_file)
-
-        with open(output_file, "w") as dst:
-            dst.write("cdef dict _SCORE_MATRICES = {}".format(json.dumps(matrices, indent=4)))
-
-
 class build_ext(_build_ext):
     """A `build_ext` that adds various SIMD flags and defines."""
 
     # --- Compatibility with `setuptools.Command`
 
     user_options = _build_ext.user_options + [
         (
@@ -432,21 +393,15 @@
         if isinstance(cythonize, ImportError):
             raise RuntimeError(
                 "Cython is required to run `build_ext` command"
             ) from cythonize
 
         # remove universal compilation flags for OSX
         if platform.system() == "Darwin":
-            _patch_osx_compiler(self.compiler)
-
-        # generate score matrices
-        if not self.distribution.have_run.get("build_matrices", False):
-            _build_cmd = self.get_finalized_command("build_matrices")
-            _build_cmd.force = self.force
-            _build_cmd.run()
+            _patch_osx_compiler(self.compiler, self.target_machine)
 
         # generate files from templates:
         for i, ext in enumerate(self.extensions):
             if isinstance(ext, ExtensionTemplate):
                 self.generate_extension(ext)
 
         # use debug directives with Cython if building in debug mode
@@ -581,15 +536,14 @@
                 os.path.join("pyopal", "platform", "neon.pxd"): os.path.join("pyopal", "platform", "pxd.in"),
                 os.path.join("pyopal", "platform", "neon.pyx"): os.path.join("pyopal", "platform", "pyx.in"),
             },
             sources=[
                 os.path.join("vendor", "opal", "src", "opal.cpp"),
                 os.path.join("pyopal", "platform", "neon.pyx"),
             ],
-            
         ),
         ExtensionTemplate(
             "pyopal.platform.sse2",
             language="c++",
             simd="SSE2",
             define_macros=[("__SSE2__", 1)],
             include_dirs=["pyopal"],
@@ -638,11 +592,10 @@
             sources=[os.path.join("pyopal", "lib.pyx")],
             include_dirs=["pyopal"],
         ),
     ],
     cmdclass={
         "sdist": sdist,
         "build_ext": build_ext,
-        "build_matrices": build_matrices,
         "clean": clean,
     },
 )
```

### Comparing `pyopal-0.5.2/vendor/opal/LICENSE` & `pyopal-0.6.0/vendor/opal/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/README.md` & `pyopal-0.6.0/vendor/opal/README.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/ScoreMatrix.cpp` & `pyopal-0.6.0/vendor/opal/src/ScoreMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/ScoreMatrix.hpp` & `pyopal-0.6.0/vendor/opal/src/ScoreMatrix.hpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/opal.cpp` & `pyopal-0.6.0/vendor/opal/src/opal.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/opal.h` & `pyopal-0.6.0/vendor/opal/src/opal.h`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/opal_aligner.cpp` & `pyopal-0.6.0/vendor/opal/src/opal_aligner.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/blosum45.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/blosum45.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/blosum50.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/blosum50.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/blosum62.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/blosum62.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/blosum80.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/blosum80.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/pam120.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/pam120.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/score_matrices/pam250.mat` & `pyopal-0.6.0/vendor/opal/src/score_matrices/pam250.mat`

 * *Files identical despite different names*

### Comparing `pyopal-0.5.2/vendor/opal/src/test.cpp` & `pyopal-0.6.0/vendor/opal/src/test.cpp`

 * *Files identical despite different names*

