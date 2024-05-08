# Comparing `tmp/pz_rail_sklearn-0.0.6.tar.gz` & `tmp/pz_rail_sklearn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_sklearn-0.0.6.tar", last modified: Wed Apr 17 23:58:01 2024, max compression
+gzip compressed data, was "pz_rail_sklearn-0.0.7.tar", last modified: Wed May  8 15:55:31 2024, max compression
```

## Comparing `pz_rail_sklearn-0.0.6.tar` & `pz_rail_sklearn-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.528747 pz_rail_sklearn-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:58:01.528747 pz_rail_sklearn-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/k_nearneigh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12447 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/nz_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/estimation/algos/sklearn_neurnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/src/rail/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/src/rail/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 23:58:01.000000 pz_rail_sklearn-0.0.6/src/rail/sklearn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.520747 pz_rail_sklearn-0.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:58:01.524747 pz_rail_sklearn-0.0.6/tests/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-17 23:57:54.000000 pz_rail_sklearn-0.0.6/tests/sklearn/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/k_nearneigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12447 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/nz_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/sklearn_neurnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/rail/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/rail/sklearn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/tests/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/tests/sklearn/test_algos.py
```

### Comparing `pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/pull_request_template.md` & `pz_rail_sklearn-0.0.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/workflows/linting.yml` & `pz_rail_sklearn-0.0.7/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/workflows/publish-to-pypi.yml` & `pz_rail_sklearn-0.0.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/workflows/smoke-test.yml` & `pz_rail_sklearn-0.0.7/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.github/workflows/testing-and-coverage.yml` & `pz_rail_sklearn-0.0.7/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.gitignore` & `pz_rail_sklearn-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/.pre-commit-config.yaml` & `pz_rail_sklearn-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/LICENSE` & `pz_rail_sklearn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/PKG-INFO` & `pz_rail_sklearn-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.6
+Version: 0.0.7
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_sklearn-0.0.6/README.md` & `pz_rail_sklearn-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/pyproject.toml` & `pz_rail_sklearn-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/PKG-INFO` & `pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.6
+Version: 0.0.7
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_sklearn-0.0.6/src/pz_rail_sklearn.egg-info/SOURCES.txt` & `pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/k_nearneigh.py` & `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/k_nearneigh.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,10 +188,11 @@
             else:
                 knn_df.loc[np.isclose(knn_df[col], self.config.nondetect_val), col] = self.config.mag_limits[col]
 
         testcolordata = _computecolordata(knn_df, self.config.ref_band, self.config.bands)
         dists, idxs = self.kdtree.query(testcolordata, k=self.numneigh)
         dists += TEENY
         test_ens = _makepdf(dists, idxs, self.trainszs, self.sigma)
+        
         zmode = test_ens.mode(grid=self.zgrid)
         test_ens.set_ancil(dict(zmode=zmode))
         self._do_chunk_output(test_ens, start, end, first)
```

### Comparing `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/nz_dir.py` & `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/nz_dir.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/random_forest.py` & `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/random_forest.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/src/rail/estimation/algos/sklearn_neurnet.py` & `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/sklearn_neurnet.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.6/tests/sklearn/test_algos.py` & `pz_rail_sklearn-0.0.7/tests/sklearn/test_algos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import os
 import pytest
 import scipy.special
 
-from rail.core.algo_utils import one_algo
+from rail.utils.testing_utils import one_algo
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.core.data import TableHandle
 from rail.estimation.algos import k_nearneigh, sklearn_neurnet, random_forest
 
 sci_ver_str = scipy.__version__.split(".")
 
 
 DS = RailStage.data_store
```

