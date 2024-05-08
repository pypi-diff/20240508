# Comparing `tmp/pz-rail-som-0.0.5.tar.gz` & `tmp/pz_rail_som-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-som-0.0.5.tar", last modified: Wed Nov  1 01:55:15 2023, max compression
+gzip compressed data, was "pz_rail_som-0.0.6.tar", last modified: Wed May  8 15:56:07 2024, max compression
```

## Comparing `pz-rail-som-0.0.5.tar` & `pz_rail_som-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.362233 pz-rail-som-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.366233 pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.366233 pz-rail-som-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.358233 pz-rail-som-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.366233 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/pz_rail_som.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.358233 pz-rail-som-0.0.5/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.358233 pz-rail-som-0.0.5/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    16358 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/src/rail/estimation/algos/minisom_som.py
--rw-r--r--   0 runner    (1001) docker     (127)    27326 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/src/rail/estimation/algos/somoclu_som.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/src/rail/som/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/src/rail/som/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-01 01:55:15.000000 pz-rail-som-0.0.5/src/rail/som/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.358233 pz-rail-som-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 01:55:15.370233 pz-rail-som-0.0.5/tests/som/
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/tests/som/test_som_summarizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-11-01 01:55:02.000000 pz-rail-som-0.0.5/tests/som/test_somoclu_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.443110 pz_rail_som-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.443110 pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.443110 pz_rail_som-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.439110 pz_rail_som-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/pz_rail_som.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.439110 pz_rail_som-0.0.6/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.439110 pz_rail_som-0.0.6/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    16358 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/src/rail/estimation/algos/minisom_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27326 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/src/rail/estimation/algos/somoclu_som.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/src/rail/som/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/src/rail/som/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:56:07.000000 pz_rail_som-0.0.6/src/rail/som/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.443110 pz_rail_som-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:56:07.447110 pz_rail_som-0.0.6/tests/som/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/tests/som/test_som_summarizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-08 15:56:00.000000 pz_rail_som-0.0.6/tests/som/test_somoclu_summarizers.py
```

### Comparing `pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_som-0.0.6/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/pull_request_template.md` & `pz_rail_som-0.0.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/workflows/linting.yml` & `pz_rail_som-0.0.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/workflows/publish-to-pypi.yml` & `pz_rail_som-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/workflows/smoke-test.yml` & `pz_rail_som-0.0.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.github/workflows/testing-and-coverage.yml` & `pz_rail_som-0.0.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.gitignore` & `pz_rail_som-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/.pre-commit-config.yaml` & `pz_rail_som-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/LICENSE` & `pz_rail_som-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/PKG-INFO` & `pz_rail_som-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-som
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-som-0.0.5/README.md` & `pz_rail_som-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/pyproject.toml` & `pz_rail_som-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/src/pz_rail_som.egg-info/PKG-INFO` & `pz_rail_som-0.0.6/src/pz_rail_som.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-som
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-som-0.0.5/src/pz_rail_som.egg-info/SOURCES.txt` & `pz_rail_som-0.0.6/src/pz_rail_som.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/src/rail/estimation/algos/minisom_som.py` & `pz_rail_som-0.0.6/src/rail/estimation/algos/minisom_som.py`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/src/rail/estimation/algos/somoclu_som.py` & `pz_rail_som-0.0.6/src/rail/estimation/algos/somoclu_som.py`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.5/tests/som/test_som_summarizers.py` & `pz_rail_som-0.0.6/tests/som/test_som_summarizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import numpy as np
 import qp
 
 from rail.core.data import TableHandle
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.estimation.algos import minisom_som
 
 testszdata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 testphotdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
```

### Comparing `pz-rail-som-0.0.5/tests/som/test_somoclu_summarizers.py` & `pz_rail_som-0.0.6/tests/som/test_somoclu_summarizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import numpy as np
 import qp
 
 from rail.core.data import TableHandle
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.estimation.algos import somoclu_som
 
 testszdata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 testphotdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
```

