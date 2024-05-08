# Comparing `tmp/skerch-0.6.1.tar.gz` & `tmp/skerch-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skerch-0.6.1.tar", last modified: Mon Mar 25 12:42:14 2024, max compression
+gzip compressed data, was "skerch-0.7.0.tar", last modified: Wed May  8 02:08:09 2024, max compression
```

## Comparing `skerch-0.6.1.tar` & `skerch-0.7.0.tar`

### file list

```diff
@@ -1,83 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.432381 skerch-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.416381 skerch-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.416381 skerch-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-25 12:42:06.000000 skerch-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-25 12:42:06.000000 skerch-0.6.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-25 12:42:06.000000 skerch-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-25 12:42:06.000000 skerch-0.6.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.416381 skerch-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-03-25 12:42:06.000000 skerch-0.6.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-25 12:42:06.000000 skerch-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 12:42:06.000000 skerch-0.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-25 12:42:06.000000 skerch-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-25 12:42:06.000000 skerch-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-03-25 12:42:14.432381 skerch-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-03-25 12:42:06.000000 skerch-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.412381 skerch-0.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.416381 skerch-0.6.1/docs/materials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.416381 skerch-0.6.1/docs/materials/apidoc_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/apidoc_templates/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/apidoc_templates/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/apidoc_templates/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.420381 skerch-0.6.1/docs/materials/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33219 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   390456 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_full.png
--rw-r--r--   0 runner    (1001) docker     (127)   465260 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_full.svg
--rw-r--r--   0 runner    (1001) docker     (127)   465555 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)   465555 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_horizontal_inv.svg
--rw-r--r--   0 runner    (1001) docker     (127)   371874 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   168786 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_qr.png
--rw-r--r--   0 runner    (1001) docker     (127)   199726 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_qr.svg
--rw-r--r--   0 runner    (1001) docker     (127)   103496 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/assets/skerch_text.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.424381 skerch-0.6.1/docs/materials/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/examples/example_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/examples/example_decompositions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/examples/example_deep_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/examples/example_distributed_decompositions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/for_developers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-25 12:42:06.000000 skerch-0.6.1/docs/materials/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-25 12:42:06.000000 skerch-0.6.1/makefile
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-25 12:42:06.000000 skerch-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-25 12:42:14.432381 skerch-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      412 2024-03-25 12:42:06.000000 skerch-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.424381 skerch-0.6.1/skerch/
--rwxr-xr-x   0 runner    (1001) docker     (127)      807 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8716 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8524 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/a_posteriori.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2423 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/a_priori.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.428381 skerch-0.6.1/skerch/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1424 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/cli/create_hdf5_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/cli/merge_hdf5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/cli/post_bounds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1032 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/cli/prio_hpars.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7281 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/decompositions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11663 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/distributed_decompositions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21311 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/distributed_measurements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11649 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/linops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5782 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/ssrft.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7694 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/synthmat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4068 2024-03-25 12:42:06.000000 skerch-0.6.1/skerch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.428381 skerch-0.6.1/skerch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 12:42:14.000000 skerch-0.6.1/skerch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:42:14.428381 skerch-0.6.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-03-25 12:42:06.000000 skerch-0.6.1/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-03-25 12:42:06.000000 skerch-0.6.1/test/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3883 2024-03-25 12:42:06.000000 skerch-0.6.1/test/dseigh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-03-25 12:42:06.000000 skerch-0.6.1/test/dssvd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7446 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_a_posteriori.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5156 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_a_priori.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34756 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_decompositions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    36169 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_distributed_decompositions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11099 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_distributed_measurements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11369 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_linops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2007 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_qr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6422 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_ssrft.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17586 2024-03-25 12:42:06.000000 skerch-0.6.1/test/test_synthetic_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.986387 skerch-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.966387 skerch-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.966387 skerch-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 02:08:04.000000 skerch-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 02:08:04.000000 skerch-0.7.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 02:08:04.000000 skerch-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-08 02:08:04.000000 skerch-0.7.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.966387 skerch-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-08 02:08:04.000000 skerch-0.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-08 02:08:04.000000 skerch-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 02:08:04.000000 skerch-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 02:08:04.000000 skerch-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 02:08:04.000000 skerch-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-05-08 02:08:09.986387 skerch-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-08 02:08:04.000000 skerch-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.962387 skerch-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.966387 skerch-0.7.0/docs/materials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.970387 skerch-0.7.0/docs/materials/apidoc_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/apidoc_templates/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/apidoc_templates/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/apidoc_templates/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.974387 skerch-0.7.0/docs/materials/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33219 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   390456 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_full.png
+-rw-r--r--   0 runner    (1001) docker     (127)   465260 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   465555 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   465555 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_horizontal_inv.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   371874 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   168786 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_qr.png
+-rw-r--r--   0 runner    (1001) docker     (127)   199726 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_qr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   103496 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/assets/skerch_text.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.974387 skerch-0.7.0/docs/materials/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_deep_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_diagonals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_distributed_decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/examples/example_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/for_developers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-08 02:08:04.000000 skerch-0.7.0/docs/materials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-08 02:08:04.000000 skerch-0.7.0/makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 02:08:04.000000 skerch-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 02:08:09.986387 skerch-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      412 2024-05-08 02:08:04.000000 skerch-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.978387 skerch-0.7.0/skerch/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8716 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8524 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/a_posteriori.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2423 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/a_priori.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.978387 skerch-0.7.0/skerch/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1424 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/cli/create_hdf5_layout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/cli/merge_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/cli/post_bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1032 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/cli/prio_hpars.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7281 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/decompositions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11663 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/distributed_decompositions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21426 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/distributed_measurements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14343 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/linops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6099 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/ssrft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8743 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/subdiagonals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7813 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/synthmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13112 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/triangles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4575 2024-05-08 02:08:04.000000 skerch-0.7.0/skerch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.982387 skerch-0.7.0/skerch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 02:08:09.000000 skerch-0.7.0/skerch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:08:09.982387 skerch-0.7.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-05-08 02:08:04.000000 skerch-0.7.0/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-05-08 02:08:04.000000 skerch-0.7.0/test/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3883 2024-05-08 02:08:04.000000 skerch-0.7.0/test/dseigh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-05-08 02:08:04.000000 skerch-0.7.0/test/dssvd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7446 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_a_posteriori.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5156 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_a_priori.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34756 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_decompositions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36169 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_distributed_decompositions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11099 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_distributed_measurements.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11369 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_linops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6255 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_proj_linops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2007 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_qr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6422 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_ssrft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11546 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_subdiagonals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17741 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_synthetic_matrices.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23087 2024-05-08 02:08:04.000000 skerch-0.7.0/test/test_triangular_linop.py
```

### Comparing `skerch-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `skerch-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md` & `skerch-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/.github/pull_request_template.md` & `skerch-0.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/.github/workflows/ci.yaml` & `skerch-0.7.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/.gitignore` & `skerch-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/.readthedocs.yaml` & `skerch-0.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/LICENSE` & `skerch-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/PKG-INFO` & `skerch-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skerch
-Version: 0.6.1
+Version: 0.7.0
 Summary: Sketched matrix decompositions for PyTorch
 Home-page: https://github.com/andres-fr/skerch
 Author: aferro
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -61,53 +61,55 @@
 |                                                             PyPI                                                                 |                                                                             Docs                                                                             |                                                                                                  CI                                                                                                  |                                                                                    Tests                                                                                    |
 |:--------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
 | [![PyPI - Downloads](https://img.shields.io/pypi/dm/skerch?style=flat&label=skerch)](https://pypi.org/project/skerch/) | [![Documentation Status](https://readthedocs.org/projects/skerch/badge/?version=latest)](https://skerch.readthedocs.io/en/latest/?badge=latest) | [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andres-fr/skerch/ci.yaml)](https://github.com/andres-fr/skerch/actions) | [![Coverage Status](https://coveralls.io/repos/github/andres-fr/skerch/badge.svg?branch=main)](https://coveralls.io/github/andres-fr/skerch?branch=main) |
 
 </div>
 
 
-`skerch` is a Python package to compute diagonal decompositions (SVD, Hermitian Eigendecomposition) of linear operators via sketched methods.
+`skerch` is a Python package to compute different decompositions (SVD, Hermitian Eigendecomposition, diagonal, subdiagonal, triangular, block-triangular) of linear operators via sketched methods.
 
 * Built on top of PyTorch, with natural support for CPU and CUDA interoperability, and very few dependencies otherwise
 * Works on matrices and matrix-free operators of potentially very large dimensionality
 * Support for sketched measurements in a fully distributed fashion via [HDF5 databases](https://www.h5py.org/)
 
 
 References:
 
 * [Streaming Low-Rank Matrix Approximation with an Application to Scientific Simulation](https://arxiv.org/abs/1902.08651) Joel A. Tropp, Alp Yurtsever, Madeleine Udell, and Volkan Cevher. 2019. SIAM Journal on Scientific Computing 41 (4): A2430–63.
+* [Stochastic diagonal estimation: probabilistic bounds and an improved algorithm](https://arxiv.org/abs/2201.10684) Robert A. Baston and Yuji Nakatsukasa. 2022. CoRR abs/2201.10684.
 
 
-See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details.
+See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details, including examples for other decompositions and use cases.
 
 
 # Installation and basic usage
 
 Install via:
 
 ```bash
 pip install skerch
 ```
 
-The sketched SVD of a linear operator `op` can be then computed simply via:
+The sketched SVD of a linear operator `op` of shape `(h, w)` can be then computed simply via:
 
 
 ```python
 from skerch.decompositions import ssvd
 
 q, u, s, vt, pt = ssvd(
     op,
     op_device=DEVICE,
     op_dtype=DTYPE,
     outer_dim=NUM_OUTER,
     inner_dim=NUM_INNER,
 )
 ```
 
-Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`.
+Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`, where `q, p` are *thin* orthonormal matrices of shape `(h, NUM_OUTER)` and `(NUM_OUTER, w)` respectively, and `u, vt` are *small* orthogonal matrices of shape `(NUM_OUTER, NUM_OUTER)`.
+
 The `op` object must simply satify the following criteria:
 
 * It must have a `op.shape = (height, width)` attribute
 * It must implement the `w = op @ v` right-matmul operator, receiving and returning PyTorch vectors/matrices
 * It must implement the `w = v @ op` left-matmul operator, receiving and returning PyTorch vectors/matrices
 
 `skerch` provides a convenience PyTorch wrapper for the cases where `op` interacts with NumPy arrays instead (e.g. [SciPy linear operators](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.LinearOperator.html) like the ones used in [CurvLinOps](https://github.com/f-dangel/curvlinops)).
```

### Comparing `skerch-0.6.1/README.md` & `skerch-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,53 +14,55 @@
 |                                                             PyPI                                                                 |                                                                             Docs                                                                             |                                                                                                  CI                                                                                                  |                                                                                    Tests                                                                                    |
 |:--------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
 | [![PyPI - Downloads](https://img.shields.io/pypi/dm/skerch?style=flat&label=skerch)](https://pypi.org/project/skerch/) | [![Documentation Status](https://readthedocs.org/projects/skerch/badge/?version=latest)](https://skerch.readthedocs.io/en/latest/?badge=latest) | [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andres-fr/skerch/ci.yaml)](https://github.com/andres-fr/skerch/actions) | [![Coverage Status](https://coveralls.io/repos/github/andres-fr/skerch/badge.svg?branch=main)](https://coveralls.io/github/andres-fr/skerch?branch=main) |
 
 </div>
 
 
-`skerch` is a Python package to compute diagonal decompositions (SVD, Hermitian Eigendecomposition) of linear operators via sketched methods.
+`skerch` is a Python package to compute different decompositions (SVD, Hermitian Eigendecomposition, diagonal, subdiagonal, triangular, block-triangular) of linear operators via sketched methods.
 
 * Built on top of PyTorch, with natural support for CPU and CUDA interoperability, and very few dependencies otherwise
 * Works on matrices and matrix-free operators of potentially very large dimensionality
 * Support for sketched measurements in a fully distributed fashion via [HDF5 databases](https://www.h5py.org/)
 
 
 References:
 
 * [Streaming Low-Rank Matrix Approximation with an Application to Scientific Simulation](https://arxiv.org/abs/1902.08651) Joel A. Tropp, Alp Yurtsever, Madeleine Udell, and Volkan Cevher. 2019. SIAM Journal on Scientific Computing 41 (4): A2430–63.
+* [Stochastic diagonal estimation: probabilistic bounds and an improved algorithm](https://arxiv.org/abs/2201.10684) Robert A. Baston and Yuji Nakatsukasa. 2022. CoRR abs/2201.10684.
 
 
-See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details.
+See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details, including examples for other decompositions and use cases.
 
 
 # Installation and basic usage
 
 Install via:
 
 ```bash
 pip install skerch
 ```
 
-The sketched SVD of a linear operator `op` can be then computed simply via:
+The sketched SVD of a linear operator `op` of shape `(h, w)` can be then computed simply via:
 
 
 ```python
 from skerch.decompositions import ssvd
 
 q, u, s, vt, pt = ssvd(
     op,
     op_device=DEVICE,
     op_dtype=DTYPE,
     outer_dim=NUM_OUTER,
     inner_dim=NUM_INNER,
 )
 ```
 
-Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`.
+Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`, where `q, p` are *thin* orthonormal matrices of shape `(h, NUM_OUTER)` and `(NUM_OUTER, w)` respectively, and `u, vt` are *small* orthogonal matrices of shape `(NUM_OUTER, NUM_OUTER)`.
+
 The `op` object must simply satify the following criteria:
 
 * It must have a `op.shape = (height, width)` attribute
 * It must implement the `w = op @ v` right-matmul operator, receiving and returning PyTorch vectors/matrices
 * It must implement the `w = v @ op` left-matmul operator, receiving and returning PyTorch vectors/matrices
 
 `skerch` provides a convenience PyTorch wrapper for the cases where `op` interacts with NumPy arrays instead (e.g. [SciPy linear operators](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.LinearOperator.html) like the ones used in [CurvLinOps](https://github.com/f-dangel/curvlinops)).
```

### Comparing `skerch-0.6.1/docs/materials/apidoc_templates/package.rst_t` & `skerch-0.7.0/docs/materials/apidoc_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/favicon.ico` & `skerch-0.7.0/docs/materials/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_full.png` & `skerch-0.7.0/docs/materials/assets/skerch_full.png`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_full.svg` & `skerch-0.7.0/docs/materials/assets/skerch_full.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_horizontal.svg` & `skerch-0.7.0/docs/materials/assets/skerch_horizontal.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_horizontal_inv.svg` & `skerch-0.7.0/docs/materials/assets/skerch_horizontal_inv.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_logo.svg` & `skerch-0.7.0/docs/materials/assets/skerch_logo.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_qr.png` & `skerch-0.7.0/docs/materials/assets/skerch_qr.png`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_qr.svg` & `skerch-0.7.0/docs/materials/assets/skerch_qr.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/assets/skerch_text.svg` & `skerch-0.7.0/docs/materials/assets/skerch_text.svg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/examples/example_cli.py` & `skerch-0.7.0/docs/materials/examples/example_cli.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/examples/example_decompositions.py` & `skerch-0.7.0/docs/materials/examples/example_decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/examples/example_deep_learning.py` & `skerch-0.7.0/docs/materials/examples/example_deep_learning.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/examples/example_distributed_decompositions.py` & `skerch-0.7.0/docs/materials/examples/example_distributed_decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/for_developers.rst` & `skerch-0.7.0/docs/materials/for_developers.rst`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/docs/materials/index.rst` & `skerch-0.7.0/docs/materials/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,20 @@
 
 This package implements functionality to perform such sketched decompositions
 for any arbitrary matrix or linear operator :math:`A`.
 **This includes non-square, non-PSD, and matrix-free operators**. Furthermore,
 operations are implemented using ``PyTorch``, which means that **CPU/CUDA can
 be used in a device-agnostic way and automatic differentiation is available**.
 
-It also implements efficient *a priori* methods to choose meaningful hyperparameters
-for the sketched algorithms, and efficient *a posteriori* methods to estimate the
-quality and rank of the sketched approximations.
+It also implements:
+
+* Efficient *a priori* methods to choose meaningful hyperparameters for the sketched algorithms
+* Efficient *a posteriori* methods to estimate the quality and rank of the sketched approximations
+* Matrix-free estimation of (sub-)diagonals for square linear operators
+* Matrix-free estimation of matrix-vector products for upper- and lower-triangular portions of square linear operators.
 
 .. seealso::
 
   The contents of this repository are based on the following publications:
 
   * `[HMT2009] <https://arxiv.org/abs/0909.4061>`_: Nathan Halko, Per-Gunnar
     Martinsson, Joel A. Tropp. 2011. *“Finding Structure with Randomness:
@@ -44,14 +47,17 @@
     SIAM Review, 53 (2): 217-288.
 
   * `[TYUC2019] <https://arxiv.org/abs/1902.08651>`_: Joel A. Tropp, Alp
     Yurtsever, Madeleine Udell, and Volkan Cevher. 2019. *“Streaming Low-rank
     Matrix Approximation with an Application to Scientific Simulation”*. SIAM
     Journal on Scientific Computing 41 (4): A2430–63.
 
+  * `[BN2022] <https://arxiv.org/abs/2201.10684>`_: Robert A. Baston and Yuji
+    Nakatsukasa. 2022. *“Stochastic diagonal estimation: probabilistic bounds and
+    an improved algorithm”*.  CoRR abs/2201.10684.
 
 .. toctree::
    :maxdepth: 2
    :caption: Getting Started
 
    getting_started
```

### Comparing `skerch-0.6.1/makefile` & `skerch-0.7.0/makefile`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/pyproject.toml` & `skerch-0.7.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 match_dir = '^(?!(docs|.eggs)).*'
 match = '(?!example_).*\.py'
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
-version = "0.6.1"
+version = "0.7.0"
 update_changelog_on_bump = true
 major_version_zero = true
```

### Comparing `skerch-0.6.1/setup.cfg` & `skerch-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/__init__.py` & `skerch-0.7.0/skerch/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 This implementation is based on the following publications, referenced
 throughout the documentation:
 
 * `[TYUC2019] <https://arxiv.org/abs/1902.08651>`_: Joel A. Tropp, Alp
   Yurtsever, Madeleine Udell, and Volkan Cevher. 2019. *“Streaming Low-rank
   Matrix Approximation with an Application to Scientific Simulation”*. SIAM
   Journal on Scientific Computing 41 (4): A2430–63.
+* `[BN2022] <https://arxiv.org/abs/2201.10684>`_: Robert A. Baston and Yuji
+  Nakatsukasa. 2022. *“Stochastic diagonal estimation: probabilistic bounds and
+  an improved algorithm”*.  CoRR abs/2201.10684.
 """
 
 
 # ##############################################################################
 # # GLOBALS
 # ##############################################################################
```

### Comparing `skerch-0.6.1/skerch/__main__.py` & `skerch-0.7.0/skerch/__main__.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/a_posteriori.py` & `skerch-0.7.0/skerch/a_posteriori.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/a_priori.py` & `skerch-0.7.0/skerch/a_priori.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/cli/create_hdf5_layout.py` & `skerch-0.7.0/skerch/cli/create_hdf5_layout.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/cli/merge_hdf5.py` & `skerch-0.7.0/skerch/cli/merge_hdf5.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/cli/post_bounds.py` & `skerch-0.7.0/skerch/cli/post_bounds.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/cli/prio_hpars.py` & `skerch-0.7.0/skerch/cli/prio_hpars.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/decompositions.py` & `skerch-0.7.0/skerch/decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/distributed_decompositions.py` & `skerch-0.7.0/skerch/distributed_decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/skerch/distributed_measurements.py` & `skerch-0.7.0/skerch/distributed_measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,16 +442,17 @@
       tensor or a ``numpy`` or a ``HDF5`` array, accepting in-place  writing
       via ``out_vals[:] = ...``.
     :param flag: An array-like object of shape (1,) and string datatype,
       optionally used by this function to keep track of current state by
       setting it to the ``processing_flag, success_flag`` values via
       the ``flag[0] = "..."`` assignment.
     :param bool adjoint: See above.
-    :returns: Nothing, result is written to ``out_vals``, and optionally
-      ``flag`` is also written.
+    :returns: the SSRFT matrix-free linear operator used for the measurement.
+      Note that the measurement is not returned, but written to ``out_vals``,
+      and optionally ``flag`` is also written.
     """
     assert (
         0 <= idx <= total_measurements
     ), "OOB index for number of measurements!"
     vals_shape = out_vals.shape
     lop_h, lop_w = lop.shape
     if adjoint:
@@ -469,14 +470,15 @@
         # try to assign as-is (covers torch-to-torch and CPU cases)
         out_vals[:] = result
     except Exception:
         # if anything happens, try to copy to CPU
         out_vals[:] = result.cpu()
     if flag is not None:
         flag[0] = success_flag
+    return ssrft
 
 
 # ##############################################################################
 # # DISTRIBUTED INNER MEASUREMENTS
 # ##############################################################################
 def innermeas_idx_torch(
     idx,
```

### Comparing `skerch-0.6.1/skerch/linops.py` & `skerch-0.7.0/skerch/linops.py`

 * *Files 13% similar despite different names*

```diff
@@ -258,14 +258,94 @@
         if len(self.diag) > self.MAX_PRINT_ENTRIES:
             diagstr += "..."
         s = f"<{clsname}({self.shape[0]}x{self.shape[1]})[{diagstr}]>"
         return s
 
 
 # ##############################################################################
+# # DIAGONAL LINEAR OPERATOR
+# ##############################################################################
+class OrthProjLinOp(BaseLinOp):
+    r"""Linear operator for an orthogonal projector.
+
+    Given a "thin" matrix (i.e. height >= width) :math:`Q` of orthonormal
+    columns, this class implements the orthogonal projector onto its span,
+    i.e. :math:`Q Q^T`.
+    """
+
+    def __init__(self, Q):
+        """Object initialization.
+
+        :param Q: Linear operator of shape ``(h, w)`` with ``h >= w``, expected
+          to be orthonormal (i.e. columns with unit Euclidean norm and all
+          orthogonal to each other). It must implement the left and right
+          matmul operations via the ``@`` operator.
+
+        .. warning::
+
+          This class assumes ``Q`` is orthonormal, but this is not checked.
+        """
+        self.Q = Q
+        #
+        h, w = Q.shape
+        if w > h:
+            raise BadShapeError("Projector matrix must be thin!")
+        super().__init__((h, h))  # this sets self.shape also
+
+    def __matmul__(self, x):
+        """Forward (right) matrix-vector multiplication ``self @ x``.
+
+        See parent class for more details.
+        """
+        self.check_input(x, adjoint=False)
+        result = self.Q @ (x.T @ self.Q).T
+        return result
+
+    def __rmatmul__(self, x):
+        """Adjoint (left) matrix-vector multiplication ``x @ self``.
+
+        See parent class for more details.
+        """
+        self.check_input(x, adjoint=True)
+        result = self.Q @ (x @ self.Q).T
+        return result.T
+
+    def __repr__(self):
+        """Returns a string in the form <OrthProjLinOp(Q_shape)>."""
+        clsname = self.__class__.__name__
+        s = f"<{clsname}({self.Q.shape})>"
+        return s
+
+
+class NegOrthProjLinOp(OrthProjLinOp):
+    """Linear operator for a negative orthogonal projector.
+
+    Given a "thin" matrix (i.e. height >= width) :math:`Q` of orthonormal
+    columns, this class implements the orthogonal projector :math:`Q Q^T`.
+    Given a "thin" matrix (i.e. height >= width) :math:`Q` of orthonormal
+    columns, this class implements the orthogonal projector onto the space
+    orthogonal to its span, i.e. :math:`(I - Q Q^T)`.
+    """
+
+    def __matmul__(self, x):
+        """Forward (right) matrix-vector multiplication ``self @ x``.
+
+        See parent class for more details.
+        """
+        return x - super().__matmul__(x)
+
+    def __rmatmul__(self, x):
+        """Forward (right) matrix-vector multiplication ``self @ x``.
+
+        See parent class for more details.
+        """
+        return x - super().__rmatmul__(x)
+
+
+# ##############################################################################
 # # TORCH INTEROPERABILITY
 # ##############################################################################
 class TorchLinOpWrapper:
     """Linear operator that always accepts and produces PyTorch tensors.
 
     Since this library operates mainly with PyTorch tensors, but some useful
     LinOps interface with e.g. NumPy arrays instead, this mixin class acts as a
```

### Comparing `skerch-0.6.1/skerch/ssrft.py` & `skerch-0.7.0/skerch/ssrft.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
-"""Scrambled Subsampled Randomized Fourier Transform (SSRFT) utilities.
+"""Scrambled Subsampled Randomized Fourier Transform (SSRFT).
 
-PyTorch-compatible implementation of the SSRFT, from
+PyTorch-compatible implementation of the SSRFT (as a matrix-free linear operator
+and other utilities), from
 `[TYUC2019, 3.2] <https://arxiv.org/abs/1902.08651>`_.
 """
 
 
 import torch
 import torch_dct as dct
 
 from .linops import BaseRandomLinOp
-from .utils import BadShapeError, NoFlatError, rademacher, randperm
+from .utils import BadShapeError, NoFlatError, rademacher_flip, randperm
 
 
 # ##############################################################################
 # # SSRFT
 # ##############################################################################
 def ssrft(x, out_dims, seed=0b1110101001010101011, dct_norm="ortho"):
     r"""Right (forward) matrix multiplication of the SSRFT.
@@ -42,20 +43,20 @@
     if len(x.shape) != 1:
         raise NoFlatError("Only flat tensors supported!")
     x_len = len(x)
     assert out_dims <= x_len, "Projection to larger dimensions not supported!"
     seeds = [seed + i for i in range(5)]
     # first scramble: permute, rademacher, and DCT
     perm1 = randperm(x_len, seed=seeds[0], device="cpu")
-    x, rad1 = rademacher(x[perm1], seed=seeds[1], inplace=False)
+    x, rad1 = rademacher_flip(x[perm1], seed=seeds[1], inplace=False)
     del perm1, rad1
     x = dct.dct(x, norm=dct_norm)
     # second scramble: permute, rademacher and DCT
     perm2 = randperm(x_len, seed=seeds[2], device="cpu")
-    x, rad2 = rademacher(x[perm2], seeds[3], inplace=False)
+    x, rad2 = rademacher_flip(x[perm2], seeds[3], inplace=False)
     del perm2, rad2
     x = dct.dct(x, norm=dct_norm)
     # extract random indices and return
     out_idxs = randperm(x_len, seed=seeds[4], device="cpu")[:out_dims]
     x = x[out_idxs]
     return x
 
@@ -100,21 +101,21 @@
     ).to(x.device)
     # first embed signal into original indices
     out_idxs = randperm(out_dims, seed=seeds[4], device="cpu")[:x_len]
     result[out_idxs] = x
     del x
     # then do the idct, followed by rademacher and inverse permutation
     result = dct.idct(result, norm=dct_norm)
-    rademacher(result, seeds[3], inplace=True)
+    rademacher_flip(result, seeds[3], inplace=True)
     perm2_inv = randperm(out_dims, seed=seeds[2], device="cpu", inverse=True)
     result = result[perm2_inv]
     del perm2_inv
     # second inverse pass
     result = dct.idct(result, norm=dct_norm)
-    rademacher(result, seeds[1], inplace=True)
+    rademacher_flip(result, seeds[1], inplace=True)
     perm1_inv = randperm(out_dims, seed=seeds[0], device="cpu", inverse=True)
     result = result[perm1_inv]
     #
     return result
 
 
 class SSRFT(BaseRandomLinOp):
@@ -145,7 +146,13 @@
 
     def rmatmul(self, x):
         """Adjoint (left) matrix-vector multiplication ``x @ SSRFT``.
 
         See parent class for more details.
         """
         return ssrft_adjoint(x, self.shape[1], seed=self.seed, dct_norm="ortho")
+
+    def get_row(self, idx, dtype, device):
+        """Returns SSRFT[idx, :] via left-matmul with a one-hot vector."""
+        in_buff = torch.zeros(self.shape[0], dtype=dtype, device=device)
+        in_buff[idx] = 1
+        return in_buff @ self
```

### Comparing `skerch-0.6.1/skerch/synthmat.py` & `skerch-0.7.0/skerch/synthmat.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Optionally, the decaying spectrum is multiplied by Rademacher noise, to test
   also with non-PSD matrices
 """
 
 
 import torch
 
-from .utils import gaussian_noise, rademacher
+from .utils import gaussian_noise, rademacher_flip
 
 
 # ##############################################################################
 # # SYNTH MATRIX FACTORY
 # ##############################################################################
 class SynthMat:
     """Static class to produce different families of synthetic matrices."""
@@ -147,24 +147,25 @@
         :param int rank: Entries in ``S[:rank]`` will have a magnitude of 1.
         :param float decay: Parameter determining how quickly magnitudes in
           ``S[rank:]`` decay to zero, following :math:`2^d, 3^d, 4^d, \dots`
           for decay :math:`d`. In
           `[TYUC2019, 7.3.1] <https://arxiv.org/abs/1902.08651>`_ the following
           values are used: 0.5 for slow decay, 1 for medium, 2 for fast.
         :param bool symmetric: If true, ``V == U``.
-        :param psd: If true, ``S`` will be multiplied with Rademacher noise
-          to create a non-PSD matrix (assuming symmetric).
+        :param psd: If false, and matrix is symmetric, the "tail" singular
+          values will be multiplied with Rademacher noise to create a non-PSD
+          matrix.
         """
         min_shape = min(shape)
         # a few ones, followed by a poly decay
         svals = torch.zeros(min_shape, dtype=dtype).to(device)
         svals[:rank] = 1
         svals[rank:] = torch.arange(2, min_shape - rank + 2) ** (-float(decay))
-        if not psd:
-            rademacher(svals[rank:], seed=seed + 1, inplace=True)
+        if (not psd) and symmetric:
+            rademacher_flip(svals[rank:], seed=seed + 1, inplace=True)
         #
         result = cls._decay_helper(
             svals, shape, rank, decay, symmetric, seed, dtype, device
         )
         return result
 
     @classmethod
@@ -189,22 +190,23 @@
         :param int rank: Entries in ``S[:rank]`` will have a magnitude of 1.
         :param float decay: Parameter determining how quickly magnitudes in
           ``S[rank:]`` decay to zero, following :math:`10^{-d}, 10^{-2d}, \dots`
           for decay :math:`d`. In
           `[TYUC2019, 7.3.1] <https://arxiv.org/abs/1902.08651>`_ the following
           values are used: 0.01 for slow decay, 0.1 for medium, 0.5 for fast.
         :param bool symmetric: If true, ``V == U``.
-        :param psd: If true, ``S`` will be multiplied with Rademacher noise
-          to create a non-PSD matrix (assuming symmetric).
+        :param psd: If false, and matrix is symmetric, the "tail" singular
+          values will be multiplied with Rademacher noise to create a non-PSD
+          matrix.
         """
         min_shape = min(shape)
         # a few ones, followed by exp decay
         svals = torch.zeros(min_shape, dtype=dtype).to(device)
         svals[:rank] = 1
         svals[rank:] = 10 ** -(decay * torch.arange(1, min_shape - rank + 1))
-        if not psd:
-            rademacher(svals[rank:], seed=seed + 1, inplace=True)
+        if (not psd) and symmetric:
+            rademacher_flip(svals[rank:], seed=seed + 1, inplace=True)
         #
         result = cls._decay_helper(
             svals, shape, rank, decay, symmetric, seed, dtype, device
         )
         return result
```

### Comparing `skerch-0.6.1/skerch/utils.py` & `skerch-0.7.0/skerch/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,40 @@
     rng.manual_seed(seed)
     #
     noise = torch.zeros(shape, dtype=dtype, device=device)
     noise.normal_(mean=mean, std=std, generator=rng)
     return noise
 
 
+def rademacher_noise(shape, seed=None, device="cpu"):
+    """Reproducible Rademacher noise.
+
+    .. note::
+      This function makes use of :func:`uniform_noise` to sample the Rademacher
+      noise. If ``x`` itself has been generated using ``uniform_noise``, make
+      sure to use a different seed to mitigate correlations.
+
+    .. warning::
+      PyTorch does not ensure RNG reproducibility across
+      devices. This parameter determines the device to generate the noise from.
+      If you want cross-device reproducibility, make sure that the noise is
+      always generated from the same device.
+
+    :param shape: Shape of the output tensor with Rademacher noise.
+    :param seed: Seed for the randomness.
+    :param device: Device of the output tensor and also source for the noise.
+      See warning.
+    """
+    noise = (
+        uniform_noise(shape, seed=seed, dtype=torch.float32, device=device)
+        > 0.5
+    ) * 2 - 1
+    return noise
+
+
 def randperm(n, seed=None, device="cpu", inverse=False):
     """Reproducible randperm of ``n`` integers from  0 to (n-1) (both included).
 
     :param bool inverse: If False, a random permutation ``P`` is provided. If
       true, an inverse permutation ``Q`` is provided, such that both
       permutations are inverse to each other, i.e. ``v == v[P][Q] == v[Q][P]``.
     """
@@ -86,36 +112,24 @@
         # we take the O(N) approach since we anticipate large N
         inv = torch.empty_like(perm)
         inv[perm] = torch.arange(perm.size(0), device=perm.device)
         perm = inv
     return perm
 
 
-def rademacher(x, seed=None, inplace=True, rng_device="cpu"):
-    """Reproducible sign-flipping via Rademacher noise.
+def rademacher_flip(x, seed=None, inplace=True, rng_device="cpu"):
+    """Reproducible random sign flip using Rademacher noise.
 
     .. note::
       This function makes use of :func:`uniform_noise` to sample the Rademacher
       noise. If ``x`` itself has been generated using ``uniform_noise``, make
       sure to use a different seed to mitigate correlations.
 
     .. warning::
-      PyTorch does not ensure RNG reproducibility across
-      devices. This parameter determines the device to generate the noise from.
-      If you want cross-device reproducibility, make sure that the noise is
-      always generated from the same device.
-
-    :param rng_device: While result will be returned on the same device as
-      ``x``, the Rademacher noise used to flip entries will be sampled on
-      this device (see reproducibility note).
+      See :func:`rademacher_noise` for notes on reproducibility and more info.
     """
-    mask = (
-        uniform_noise(
-            x.shape, seed=seed, dtype=torch.float32, device=rng_device
-        )
-        > 0.5
-    ).to(x.device) * 2 - 1
+    mask = rademacher_noise(x.shape, seed, device=rng_device).to(x.device)
     if inplace:
         x *= mask
         return x, mask
     else:
         return x * mask, mask
```

### Comparing `skerch-0.6.1/skerch.egg-info/PKG-INFO` & `skerch-0.7.0/skerch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skerch
-Version: 0.6.1
+Version: 0.7.0
 Summary: Sketched matrix decompositions for PyTorch
 Home-page: https://github.com/andres-fr/skerch
 Author: aferro
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -61,53 +61,55 @@
 |                                                             PyPI                                                                 |                                                                             Docs                                                                             |                                                                                                  CI                                                                                                  |                                                                                    Tests                                                                                    |
 |:--------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
 | [![PyPI - Downloads](https://img.shields.io/pypi/dm/skerch?style=flat&label=skerch)](https://pypi.org/project/skerch/) | [![Documentation Status](https://readthedocs.org/projects/skerch/badge/?version=latest)](https://skerch.readthedocs.io/en/latest/?badge=latest) | [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/andres-fr/skerch/ci.yaml)](https://github.com/andres-fr/skerch/actions) | [![Coverage Status](https://coveralls.io/repos/github/andres-fr/skerch/badge.svg?branch=main)](https://coveralls.io/github/andres-fr/skerch?branch=main) |
 
 </div>
 
 
-`skerch` is a Python package to compute diagonal decompositions (SVD, Hermitian Eigendecomposition) of linear operators via sketched methods.
+`skerch` is a Python package to compute different decompositions (SVD, Hermitian Eigendecomposition, diagonal, subdiagonal, triangular, block-triangular) of linear operators via sketched methods.
 
 * Built on top of PyTorch, with natural support for CPU and CUDA interoperability, and very few dependencies otherwise
 * Works on matrices and matrix-free operators of potentially very large dimensionality
 * Support for sketched measurements in a fully distributed fashion via [HDF5 databases](https://www.h5py.org/)
 
 
 References:
 
 * [Streaming Low-Rank Matrix Approximation with an Application to Scientific Simulation](https://arxiv.org/abs/1902.08651) Joel A. Tropp, Alp Yurtsever, Madeleine Udell, and Volkan Cevher. 2019. SIAM Journal on Scientific Computing 41 (4): A2430–63.
+* [Stochastic diagonal estimation: probabilistic bounds and an improved algorithm](https://arxiv.org/abs/2201.10684) Robert A. Baston and Yuji Nakatsukasa. 2022. CoRR abs/2201.10684.
 
 
-See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details.
+See the [documentation](https://skerch.readthedocs.io/en/latest/index.html) for more details, including examples for other decompositions and use cases.
 
 
 # Installation and basic usage
 
 Install via:
 
 ```bash
 pip install skerch
 ```
 
-The sketched SVD of a linear operator `op` can be then computed simply via:
+The sketched SVD of a linear operator `op` of shape `(h, w)` can be then computed simply via:
 
 
 ```python
 from skerch.decompositions import ssvd
 
 q, u, s, vt, pt = ssvd(
     op,
     op_device=DEVICE,
     op_dtype=DTYPE,
     outer_dim=NUM_OUTER,
     inner_dim=NUM_INNER,
 )
 ```
 
-Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`.
+Where the number of outer and inner measurements for the sketch is specified, and `q @ u @ diag(s) @ vt @ pt` is a PyTorch matrix that approximates `op`, where `q, p` are *thin* orthonormal matrices of shape `(h, NUM_OUTER)` and `(NUM_OUTER, w)` respectively, and `u, vt` are *small* orthogonal matrices of shape `(NUM_OUTER, NUM_OUTER)`.
+
 The `op` object must simply satify the following criteria:
 
 * It must have a `op.shape = (height, width)` attribute
 * It must implement the `w = op @ v` right-matmul operator, receiving and returning PyTorch vectors/matrices
 * It must implement the `w = v @ op` left-matmul operator, receiving and returning PyTorch vectors/matrices
 
 `skerch` provides a convenience PyTorch wrapper for the cases where `op` interacts with NumPy arrays instead (e.g. [SciPy linear operators](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.linalg.LinearOperator.html) like the ones used in [CurvLinOps](https://github.com/f-dangel/curvlinops)).
```

### Comparing `skerch-0.6.1/skerch.egg-info/SOURCES.txt` & `skerch-0.7.0/skerch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,29 @@
 docs/materials/assets/skerch_qr.png
 docs/materials/assets/skerch_qr.svg
 docs/materials/assets/skerch_text.svg
 docs/materials/examples/README.txt
 docs/materials/examples/example_cli.py
 docs/materials/examples/example_decompositions.py
 docs/materials/examples/example_deep_learning.py
+docs/materials/examples/example_diagonals.py
 docs/materials/examples/example_distributed_decompositions.py
+docs/materials/examples/example_triangles.py
 skerch/__init__.py
 skerch/__main__.py
 skerch/a_posteriori.py
 skerch/a_priori.py
 skerch/decompositions.py
 skerch/distributed_decompositions.py
 skerch/distributed_measurements.py
 skerch/linops.py
 skerch/ssrft.py
+skerch/subdiagonals.py
 skerch/synthmat.py
+skerch/triangles.py
 skerch/utils.py
 skerch.egg-info/PKG-INFO
 skerch.egg-info/SOURCES.txt
 skerch.egg-info/dependency_links.txt
 skerch.egg-info/not-zip-safe
 skerch.egg-info/requires.txt
 skerch.egg-info/top_level.txt
@@ -60,10 +64,13 @@
 test/dssvd.py
 test/test_a_posteriori.py
 test/test_a_priori.py
 test/test_decompositions.py
 test/test_distributed_decompositions.py
 test/test_distributed_measurements.py
 test/test_linops.py
+test/test_proj_linops.py
 test/test_qr.py
 test/test_ssrft.py
-test/test_synthetic_matrices.py
+test/test_subdiagonals.py
+test/test_synthetic_matrices.py
+test/test_triangular_linop.py
```

### Comparing `skerch-0.6.1/test/__init__.py` & `skerch-0.7.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/conftest.py` & `skerch-0.7.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/dseigh.py` & `skerch-0.7.0/test/dseigh.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/dssvd.py` & `skerch-0.7.0/test/dssvd.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_a_posteriori.py` & `skerch-0.7.0/test/test_a_posteriori.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_a_priori.py` & `skerch-0.7.0/test/test_a_priori.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_decompositions.py` & `skerch-0.7.0/test/test_decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_distributed_decompositions.py` & `skerch-0.7.0/test/test_distributed_decompositions.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_distributed_measurements.py` & `skerch-0.7.0/test/test_distributed_measurements.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_linops.py` & `skerch-0.7.0/test/test_linops.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_qr.py` & `skerch-0.7.0/test/test_qr.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_ssrft.py` & `skerch-0.7.0/test/test_ssrft.py`

 * *Files identical despite different names*

### Comparing `skerch-0.6.1/test/test_synthetic_matrices.py` & `skerch-0.7.0/test/test_synthetic_matrices.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Pytest for synthetic matrix utilities."""
 
 
 import pytest
 import torch
 
 from skerch.synthmat import SynthMat
-from skerch.utils import rademacher
+from skerch.utils import rademacher_flip
 
 from . import exp_decay, poly_decay, rng_seeds, snr_lowrank_noise, torch_devices
 
 
 # ##############################################################################
 # # FIXTURES
 # ##############################################################################
@@ -276,15 +276,17 @@
                                 ew[:r], torch.ones_like(ew[:r]), rtol=rtol
                             ), "ew[:rank] should be == 1"
                             ew_dec = 10.0 ** -(
                                 dec * torch.arange(1, dim - r + 1, dtype=dtype)
                             ).to(device)
                             if not psd:
                                 # apply rademacher to the decay
-                                rademacher(ew_dec, seed=seed + 1, inplace=True)
+                                rademacher_flip(
+                                    ew_dec, seed=seed + 1, inplace=True
+                                )
                                 # sort recovered eigenvals by descending mag
                                 _, perm = ew.abs().sort(descending=True)
                                 ew = ew[perm]
                                 # check that we actually have negatives
                                 if ew_dec.numel() > 0:
                                     assert (
                                         ew_dec < -abs(decay_ew_atol[dtype])
@@ -324,15 +326,17 @@
                             ), "ew[:rank] should be == 1"
                             ew_dec = (
                                 torch.arange(2, dim - r + 2, dtype=dtype)
                                 ** (-float(dec))
                             ).to(device)
                             if not psd:
                                 # apply rademacher to the decay
-                                rademacher(ew_dec, seed=seed + 1, inplace=True)
+                                rademacher_flip(
+                                    ew_dec, seed=seed + 1, inplace=True
+                                )
                                 # sort recovered eigenvals by descending mag
                                 _, perm = ew.abs().sort(descending=True)
                                 ew = ew[perm]
                                 # check that we actually have negatives
                                 if ew_dec.numel() > 0:
                                     assert (
                                         ew_dec < -abs(decay_ew_atol[dtype])
```

