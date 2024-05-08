# Comparing `tmp/auroris-0.1.1.tar.gz` & `tmp/auroris-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auroris-0.1.1.tar", last modified: Wed May  8 00:37:58 2024, max compression
+gzip compressed data, was "auroris-0.1.2.tar", last modified: Wed May  8 00:57:25 2024, max compression
```

## Comparing `auroris-0.1.1.tar` & `auroris-0.1.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.506966 auroris-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.490965 auroris-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.494966 auroris-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/ISSUE_TEMPLATE/default-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/changelog_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.494966 auroris-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 00:36:55.000000 auroris-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-08 00:36:55.000000 auroris-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 00:36:55.000000 auroris-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-08 00:37:58.502966 auroris-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-08 00:36:55.000000 auroris-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.494966 auroris-0.1.1/auroris/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.494966 auroris-0.1.1/auroris/curation/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/curation/_curator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.494966 auroris-0.1.1/auroris/curation/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/curation/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-08 00:36:55.000000 auroris-0.1.1/auroris/curation/actions/_ac_stereoisomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/actions/_outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/curation/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/auroris/report/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/auroris/report/broadcaster/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/broadcaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/broadcaster/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/broadcaster/_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/broadcaster/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/auroris/report/broadcaster/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/report/broadcaster/templates/report.html.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/auroris/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/visualization/_chemspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/visualization/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 00:36:56.000000 auroris-0.1.1/auroris/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.502966 auroris-0.1.1/auroris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 00:37:58.000000 auroris-0.1.1/auroris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/api/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/actions/deduplication.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/actions/discretization.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/actions/mol.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/actions/outlier_detection.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/actions/stereo_ac.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/curator.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/functional.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/types.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/api/visualization.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.490965 auroris-0.1.1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/assets/css/custom-alchemy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.498966 auroris-0.1.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)   168635 2024-05-08 00:36:56.000000 auroris-0.1.1/docs/tutorials/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-08 00:36:56.000000 auroris-0.1.1/env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-08 00:36:56.000000 auroris-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-08 00:36:56.000000 auroris-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:37:58.506966 auroris-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:37:58.502966 auroris-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_deduplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_mol_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 00:36:56.000000 auroris-0.1.1/tests/test_stereoisomer_ac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/default-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/changelog_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 00:53:38.000000 auroris-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-08 00:53:38.000000 auroris-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 00:53:38.000000 auroris-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 00:57:25.059462 auroris-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 00:53:38.000000 auroris-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/curation/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/_curator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/curation/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_ac_stereoisomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/actions/_outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/curation/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.051462 auroris-0.1.2/auroris/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/report/broadcaster/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/report/broadcaster/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/report/broadcaster/templates/report.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/auroris/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/_chemspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 00:53:38.000000 auroris-0.1.2/auroris/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/auroris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 00:57:25.000000 auroris-0.1.2/auroris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 00:57:24.000000 auroris-0.1.2/auroris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/api/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/deduplication.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/discretization.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/mol.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/outlier_detection.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/actions/stereo_ac.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/curator.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/functional.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/types.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/api/visualization.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.047462 auroris-0.1.2/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/assets/css/custom-alchemy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.055462 auroris-0.1.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   168635 2024-05-08 00:53:38.000000 auroris-0.1.2/docs/tutorials/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-08 00:53:38.000000 auroris-0.1.2/env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-08 00:53:38.000000 auroris-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-08 00:53:38.000000 auroris-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:57:25.059462 auroris-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:57:25.059462 auroris-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_mol_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 00:53:38.000000 auroris-0.1.2/tests/test_stereoisomer_ac.py
```

### Comparing `auroris-0.1.1/.github/CODE_OF_CONDUCT.md` & `auroris-0.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `auroris-0.1.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/ISSUE_TEMPLATE/default-template.md` & `auroris-0.1.2/.github/ISSUE_TEMPLATE/default-template.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/ISSUE_TEMPLATE/feature-request.md` & `auroris-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `auroris-0.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/workflows/code-check.yml` & `auroris-0.1.2/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/workflows/doc.yml` & `auroris-0.1.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/workflows/release.yml` & `auroris-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.github/workflows/test.yml` & `auroris-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/.gitignore` & `auroris-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/LICENSE` & `auroris-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/cli.py` & `auroris-0.1.2/auroris/cli.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/_curator.py` & `auroris-0.1.2/auroris/curation/_curator.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_ac_stereoisomer.py` & `auroris-0.1.2/auroris/curation/actions/_ac_stereoisomer.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_base.py` & `auroris-0.1.2/auroris/curation/actions/_base.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_deduplicate.py` & `auroris-0.1.2/auroris/curation/actions/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_discretize.py` & `auroris-0.1.2/auroris/curation/actions/_discretize.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_distribution.py` & `auroris-0.1.2/auroris/curation/actions/_distribution.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_mol.py` & `auroris-0.1.2/auroris/curation/actions/_mol.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/curation/actions/_outlier.py` & `auroris-0.1.2/auroris/curation/actions/_outlier.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/report/_report.py` & `auroris-0.1.2/auroris/report/_report.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/report/broadcaster/_html.py` & `auroris-0.1.2/auroris/report/broadcaster/_html.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/report/broadcaster/_logger.py` & `auroris-0.1.2/auroris/report/broadcaster/_logger.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/report/broadcaster/templates/report.html.jinja` & `auroris-0.1.2/auroris/report/broadcaster/templates/report.html.jinja`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/utils.py` & `auroris-0.1.2/auroris/utils.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/visualization/_chemspace.py` & `auroris-0.1.2/auroris/visualization/_chemspace.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/visualization/_distribution.py` & `auroris-0.1.2/auroris/visualization/_distribution.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris/visualization/utils.py` & `auroris-0.1.2/auroris/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/auroris.egg-info/SOURCES.txt` & `auroris-0.1.2/auroris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/docs/assets/css/custom-alchemy.css` & `auroris-0.1.2/docs/assets/css/custom-alchemy.css`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/docs/tutorials/getting_started.ipynb` & `auroris-0.1.2/docs/tutorials/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/env.yml` & `auroris-0.1.2/env.yml`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   - seaborn
 
   # Chemistry
   - datamol >=0.12.1
 
   # Visualization
   - umap-learn
-  # - tmap
 
   # Optional
   - gcsfs
 
   # Dev
   - pytest
   - pytest-xdist
```

### Comparing `auroris-0.1.1/mkdocs.yml` & `auroris-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/pyproject.toml` & `auroris-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Lu Zhu", email = "lu@valencediscovery.com" },
     { name = "Julien St-Laurent", email = "julien.stl@valencediscovery.com" },
     { name = "Cas Wognum", email = "cas@valencediscovery.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
@@ -38,14 +38,15 @@
     "numpy",
     "pandas < 2.2.0",
     "scipy",
     "scikit-learn",
     "seaborn",
     "datamol >=0.12.1",
     "pillow",
+    "fsspec",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-xdist",
     "pytest-cov",
```

### Comparing `auroris-0.1.1/tests/test_curator.py` & `auroris-0.1.2/tests/test_curator.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/tests/test_deduplication.py` & `auroris-0.1.2/tests/test_deduplication.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/tests/test_discretization.py` & `auroris-0.1.2/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/tests/test_mol_curation.py` & `auroris-0.1.2/tests/test_mol_curation.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/tests/test_outlier_detection.py` & `auroris-0.1.2/tests/test_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `auroris-0.1.1/tests/test_stereoisomer_ac.py` & `auroris-0.1.2/tests/test_stereoisomer_ac.py`

 * *Files identical despite different names*

