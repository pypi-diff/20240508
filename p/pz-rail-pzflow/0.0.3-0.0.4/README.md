# Comparing `tmp/pz-rail-pzflow-0.0.3.tar.gz` & `tmp/pz_rail_pzflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-pzflow-0.0.3.tar", last modified: Tue Oct 31 21:15:10 2023, max compression
+gzip compressed data, was "pz_rail_pzflow-0.0.4.tar", last modified: Wed May  8 20:28:56 2024, max compression
```

## Comparing `pz-rail-pzflow-0.0.3.tar` & `pz_rail_pzflow-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.899206 pz-rail-pzflow-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-10-31 21:15:10.899206 pz-rail-pzflow-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 21:15:10.899206 pz-rail-pzflow-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.891206 pz-rail-pzflow-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.891206 pz-rail-pzflow-0.0.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.891206 pz-rail-pzflow-0.0.3/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/src/rail/creation/engines/flowEngine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.891206 pz-rail-pzflow-0.0.3/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/src/rail/estimation/algos/pzflow_nf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/src/rail/pzflow/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/src/rail/pzflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-31 21:15:10.000000 pz-rail-pzflow-0.0.3/src/rail/pzflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/src/rail/tools/flow_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.891206 pz-rail-pzflow-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:15:10.895206 pz-rail-pzflow-0.0.3/tests/pzflow/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/tests/pzflow/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2023-10-31 21:14:58.000000 pz-rail-pzflow-0.0.3/tests/pzflow/test_flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/creation/engines/flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/estimation/algos/pzflow_nf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/pzflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:28:55.000000 pz_rail_pzflow-0.0.4/src/rail/pzflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/tools/flow_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/tests/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/tests/pzflow/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/tests/pzflow/test_flowEngine.py
```

### Comparing `pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/pull_request_template.md` & `pz_rail_pzflow-0.0.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/workflows/linting.yml` & `pz_rail_pzflow-0.0.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_pzflow-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/workflows/smoke-test.yml` & `pz_rail_pzflow-0.0.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_pzflow-0.0.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.gitignore` & `pz_rail_pzflow-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/.pre-commit-config.yaml` & `pz_rail_pzflow-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/LICENSE` & `pz_rail_pzflow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/PKG-INFO` & `pz_rail_pzflow-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pzflow
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-pzflow-0.0.3/README.md` & `pz_rail_pzflow-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/pyproject.toml` & `pz_rail_pzflow-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/PKG-INFO` & `pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pzflow
-Version: 0.0.3
+Version: 0.0.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-pzflow-0.0.3/src/pz_rail_pzflow.egg-info/SOURCES.txt` & `pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/src/rail/creation/engines/flowEngine.py` & `pz_rail_pzflow-0.0.4/src/rail/creation/engines/flowEngine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/src/rail/estimation/algos/pzflow_nf.py` & `pz_rail_pzflow-0.0.4/src/rail/estimation/algos/pzflow_nf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/src/rail/tools/flow_handle.py` & `pz_rail_pzflow-0.0.4/src/rail/tools/flow_handle.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.3/tests/pzflow/test_algos.py` & `pz_rail_pzflow-0.0.4/tests/pzflow/test_algos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 import scipy.special
 
-from rail.core.algo_utils import one_algo
+from rail.utils.testing_utils import one_algo
 from rail.core.stage import RailStage
 from rail.estimation.algos import pzflow_nf
 
 sci_ver_str = scipy.__version__.split(".")
 
 
 DS = RailStage.data_store
@@ -53,14 +53,15 @@
         n_error_samples=3,
         soft_sharpness=10,
         soft_idx_col=0,
         redshift_column_name="redshift",
         num_training_epochs=50,
         hdf5_groupname="photometry",
         model="PZflowPDF.pkl",
+        output_mode = "skip_write"
     )
     estim_config_dict = dict(hdf5_groupname="photometry", model="PZflowPDF.pkl")
 
     # zb_expected = np.array([0.15, 0.14, 0.11, 0.14, 0.12, 0.14, 0.15, 0.16, 0.11, 0.12])
     train_algo = pzflow_nf.PZFlowInformer
     pz_algo = pzflow_nf.PZFlowEstimator
     results, rerun_results, rerun3_results = one_algo(
```

### Comparing `pz-rail-pzflow-0.0.3/tests/pzflow/test_flowEngine.py` & `pz_rail_pzflow-0.0.4/tests/pzflow/test_flowEngine.py`

 * *Files identical despite different names*

