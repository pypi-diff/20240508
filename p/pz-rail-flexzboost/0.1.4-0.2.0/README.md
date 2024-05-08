# Comparing `tmp/pz-rail-flexzboost-0.1.4.tar.gz` & `tmp/pz_rail_flexzboost-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-flexzboost-0.1.4.tar", last modified: Tue Oct 31 22:14:32 2023, max compression
+gzip compressed data, was "pz_rail_flexzboost-0.2.0.tar", last modified: Wed May  8 20:29:45 2024, max compression
```

## Comparing `pz-rail-flexzboost-0.1.4.tar` & `pz_rail_flexzboost-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.458120 pz-rail-flexzboost-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.450120 pz-rail-flexzboost-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.450120 pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-31 22:14:32.458120 pz-rail-flexzboost-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/archive/x_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.446120 pz-rail-flexzboost-0.1.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 22:14:32.458120 pz-rail-flexzboost-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.446120 pz-rail-flexzboost-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.446120 pz-rail-flexzboost-0.1.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.446120 pz-rail-flexzboost-0.1.4/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    14067 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/src/rail/flexzboost/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/src/rail/flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-31 22:14:32.000000 pz-rail-flexzboost-0.1.4/src/rail/flexzboost/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:14:32.454120 pz-rail-flexzboost-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2023-10-31 22:14:15.000000 pz-rail-flexzboost-0.1.4/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/x_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/pull_request_template.md` & `pz_rail_flexzboost-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/workflows/linting.yml` & `pz_rail_flexzboost-0.2.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/workflows/publish-to-pypi.yml` & `pz_rail_flexzboost-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/workflows/smoke-test.yml` & `pz_rail_flexzboost-0.2.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.github/workflows/testing-and-coverage.yml` & `pz_rail_flexzboost-0.2.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.gitignore` & `pz_rail_flexzboost-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.pre-commit-config.yaml` & `pz_rail_flexzboost-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/.prepare_project.sh` & `pz_rail_flexzboost-0.2.0/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/LICENSE` & `pz_rail_flexzboost-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/PKG-INFO` & `pz_rail_flexzboost-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.1.4
+Version: 0.2.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-flexzboost-0.1.4/README.md` & `pz_rail_flexzboost-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/archive/README.md` & `pz_rail_flexzboost-0.2.0/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/archive/pypi.yaml` & `pz_rail_flexzboost-0.2.0/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/pyproject.toml` & `pz_rail_flexzboost-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/PKG-INFO` & `pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.1.4
+Version: 0.2.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-flexzboost-0.1.4/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 archive/README.md
 archive/pypi.yaml
 archive/x_requirements.txt
 archive/x_setup.py
-docs/notebooks/fzboost_pdf_representation_comparison.ipynb
 src/pz_rail_flexzboost.egg-info/PKG-INFO
 src/pz_rail_flexzboost.egg-info/SOURCES.txt
 src/pz_rail_flexzboost.egg-info/dependency_links.txt
 src/pz_rail_flexzboost.egg-info/requires.txt
 src/pz_rail_flexzboost.egg-info/top_level.txt
 src/rail/estimation/algos/flexzboost.py
 src/rail/flexzboost/__init__.py
```

### Comparing `pz-rail-flexzboost-0.1.4/src/rail/estimation/algos/flexzboost.py` & `pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/flexzboost.py`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.4/tests/test_algos.py` & `pz_rail_flexzboost-0.2.0/tests/test_algos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 from rail.core.stage import RailStage
-from rail.core.algo_utils import one_algo
-from rail.core.utils import RAILDIR
+from rail.utils.testing_utils import one_algo
+from rail.utils.path_utils import RAILDIR
 from rail.estimation.algos import flexzboost
 import scipy.special
 sci_ver_str = scipy.__version__.split('.')
 
 
 def test_flexzboost():
     train_config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
```

