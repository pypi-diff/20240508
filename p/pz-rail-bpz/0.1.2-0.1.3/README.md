# Comparing `tmp/pz-rail-bpz-0.1.2.tar.gz` & `tmp/pz_rail_bpz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-bpz-0.1.2.tar", last modified: Fri Oct 27 19:17:51 2023, max compression
+gzip compressed data, was "pz_rail_bpz-0.1.3.tar", last modified: Wed May  8 20:28:07 2024, max compression
```

## Comparing `pz-rail-bpz-0.1.2.tar` & `pz_rail_bpz-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.137491 pz-rail-bpz-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.121491 pz-rail-bpz-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.125491 pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.125491 pz-rail-bpz-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-10-27 19:17:51.137491 pz-rail-bpz-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.129490 pz-rail-bpz-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    33371 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/examples/BPZ_lite_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22586 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/examples/BPZ_lite_with_custom_SEDs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   460800 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/examples/nonphysical_dc2_templates.tar
--rw-r--r--   0 runner    (1001) docker     (127)    83848 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/examples/test_dc2_train_customtemp_broadttypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    83848 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/examples/test_dc2_training_9816_broadtypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 19:17:51.137491 pz-rail-bpz-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.117490 pz-rail-bpz-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.133491 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-10-27 19:17:51.000000 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-27 19:17:51.000000 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 19:17:51.000000 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-27 19:17:51.000000 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-27 19:17:51.000000 pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.117490 pz-rail-bpz-0.1.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.133491 pz-rail-bpz-0.1.2/src/rail/bpz/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/src/rail/bpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-27 19:17:50.000000 pz-rail-bpz-0.1.2/src/rail/bpz/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/src/rail/bpz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.117490 pz-rail-bpz-0.1.2/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.133491 pz-rail-bpz-0.1.2/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    26654 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.117490 pz-rail-bpz-0.1.2/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.117490 pz-rail-bpz-0.1.2/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.133491 pz-rail-bpz-0.1.2/src/rail/examples_data/estimation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/src/rail/examples_data/estimation_data/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 19:17:51.137491 pz-rail-bpz-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2023-10-27 19:17:36.000000 pz-rail-bpz-0.1.2/tests/validation_10gal.pq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    33376 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22592 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   460800 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/nonphysical_dc2_templates.tar
+-rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/test_dc2_train_customtemp_broadttypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/test_dc2_training_9816_broadtypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/bpz/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/bpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/rail/bpz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/bpz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    26660 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/pull_request_template.md` & `pz_rail_bpz-0.1.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/workflows/linting.yml` & `pz_rail_bpz-0.1.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/workflows/publish-to-pypi.yml` & `pz_rail_bpz-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/workflows/smoke-test.yml` & `pz_rail_bpz-0.1.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.github/workflows/testing-and-coverage.yml` & `pz_rail_bpz-0.1.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.gitignore` & `pz_rail_bpz-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.pre-commit-config.yaml` & `pz_rail_bpz-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/.prepare_project.sh` & `pz_rail_bpz-0.1.3/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/LICENSE` & `pz_rail_bpz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/PKG-INFO` & `pz_rail_bpz-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.1.2
+Version: 0.1.3
 Author-email: LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-bpz-0.1.2/README.md` & `pz_rail_bpz-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/examples/BPZ_lite_demo.ipynb` & `pz_rail_bpz-0.1.3/examples/BPZ_lite_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977379241926656%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(9, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -25,15 +25,15 @@
                 "import pickle\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import desc_bpz\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b04c8503-74ee-4de7-b0f7-a2d8d1398db7",
             "metadata": {},
@@ -689,13 +689,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-bpz-0.1.2/examples/BPZ_lite_with_custom_SEDs.ipynb` & `pz_rail_bpz-0.1.3/examples/BPZ_lite_with_custom_SEDs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977331349206349%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(0, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -53,15 +53,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "064164cf-c923-4f34-96ba-5549f6b6df10",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "import os\n",
                 "custom_data_path = RAILDIR + '/rail/examples_data/estimation_data/data'\n",
                 "sedpath = RAILDIR + '/rail/examples_data/estimation_data/data/SED'\n",
                 "tarpath = RAILDIR + '/rail/examples_data/estimation_data/data/nonphysical_dc2_templates.tar'\n",
                 "\n",
                 "#os.environ['tempbpzsedpath'] = sedpath\n",
                 "#os.environ['tempbpztarpath'] = tarpath\n",
@@ -566,13 +566,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-bpz-0.1.2/examples/nonphysical_dc2_templates.tar` & `pz_rail_bpz-0.1.3/examples/nonphysical_dc2_templates.tar`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/examples/test_dc2_train_customtemp_broadttypes.hdf5` & `pz_rail_bpz-0.1.3/examples/test_dc2_train_customtemp_broadttypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/examples/test_dc2_training_9816_broadtypes.hdf5` & `pz_rail_bpz-0.1.3/examples/test_dc2_training_9816_broadtypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/pyproject.toml` & `pz_rail_bpz-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/PKG-INFO` & `pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.1.2
+Version: 0.1.3
 Author-email: LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-bpz-0.1.2/src/pz_rail_bpz.egg-info/SOURCES.txt` & `pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/src/rail/estimation/algos/bpz_lite.py` & `pz_rail_bpz-0.1.3/src/rail/estimation/algos/bpz_lite.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pandas as pd
 import scipy.integrate
 import glob
 import qp
 import tables_io
 from ceci.config import StageParameter as Param
 from rail.estimation.estimator import CatEstimator, CatInformer
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.bpz.utils import RAIL_BPZ_DIR
 from rail.core.common_params import SHARED_PARAMS
 
 
 
 def nzfunc(z, z0, alpha, km, m, m0):  # pragma: no cover
     zm = z0 + (km * (m - m0))
```

### Comparing `pz-rail-bpz-0.1.2/src/rail/examples_data/estimation_data/configs/test_bpz.columns` & `pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.2/tests/test_algos.py` & `pz_rail_bpz-0.1.3/tests/test_algos.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import glob
 import pickle
 import pytest
 import yaml
 import tables_io
 from rail.core.stage import RailStage
 from rail.core.data import DataStore, TableHandle
-from rail.core.utils import RAILDIR
-from rail.core.algo_utils import one_algo
+from rail.utils.path_utils import RAILDIR
+from rail.utils.testing_utils import one_algo
 from rail.estimation.algos import bpz_lite
 from rail.bpz.utils import RAIL_BPZ_DIR
 
 import scipy.special
 sci_ver_str = scipy.__version__.split('.')
 
 parquetdata = "./tests/validation_10gal.pq"
@@ -67,19 +67,19 @@
                          'p_min': 0.005,
                          'gauss_kernel': 0.0,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': 'photometry',
                          'nt_array': [8],
                          'model': 'testmodel_bpz.pkl'}
-    zb_expected = np.array([0.16, 0.12, 0.14, 0.14, 0.06, 0.14, 0.12, 0.14, 0.06, 0.16])
+    zb_expected = np.array([0.16, 0.12, 0.0, 0.12, 0.05, 0.14, 0.11, 0.14, 0.05, 0.16])
     train_algo = None
     pz_algo = bpz_lite.BPZliteEstimator
     results, rerun_results, rerun3_results = one_algo("BPZ_lite", train_algo, pz_algo, train_config_dict, estim_config_dict)
-    assert np.isclose(results.ancil['zmode'], zb_expected).all()
+    assert np.isclose(results.ancil['zmode'], zb_expected, atol=0.03).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
 @pytest.mark.parametrize(
     "inputdata, groupname",
     [
         (parquetdata, ""),
         (validdata, "photometry")
```

### Comparing `pz-rail-bpz-0.1.2/tests/validation_10gal.pq` & `pz_rail_bpz-0.1.3/tests/validation_10gal.pq`

 * *Files identical despite different names*

