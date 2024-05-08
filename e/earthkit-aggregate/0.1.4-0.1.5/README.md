# Comparing `tmp/earthkit-aggregate-0.1.4.tar.gz` & `tmp/earthkit_aggregate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-aggregate-0.1.4.tar", last modified: Mon Mar 25 10:33:02 2024, max compression
+gzip compressed data, was "earthkit_aggregate-0.1.5.tar", last modified: Wed May  8 13:53:12 2024, max compression
```

## Comparing `earthkit-aggregate-0.1.4.tar` & `earthkit_aggregate-0.1.5.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.699657 earthkit-aggregate-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.683657 earthkit-aggregate-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.687657 earthkit-aggregate-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/.github/workflows/on-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-03-25 10:33:02.695657 earthkit-aggregate-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.687657 earthkit-aggregate-0.1.4/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/ci/combined-environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.691657 earthkit-aggregate-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.691657 earthkit-aggregate-0.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.691657 earthkit-aggregate-0.1.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.691657 earthkit-aggregate-0.1.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   201951 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/notebooks/aggregate-climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   650734 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/notebooks/aggregate-spatial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   346392 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/notebooks/aggregate-temporal.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/notebooks/requirements-for-notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.687657 earthkit-aggregate-0.1.4/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.695657 earthkit-aggregate-0.1.4/earthkit/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/climatology.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit/aggregate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.695657 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 10:33:02.000000 earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 10:33:02.699657 earthkit-aggregate-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:33:02.695657 earthkit-aggregate-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/tests/test_10_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/tests/test_20_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-25 10:32:49.000000 earthkit-aggregate-0.1.4/tests/test_30_spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.979419 earthkit_aggregate-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.983419 earthkit_aggregate-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/.github/workflows/on-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.983419 earthkit_aggregate-0.1.5/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/ci/combined-environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.983419 earthkit_aggregate-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.983419 earthkit_aggregate-0.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.983419 earthkit_aggregate-0.1.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.987419 earthkit_aggregate-0.1.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   650734 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/aggregate-spatial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.987419 earthkit_aggregate-0.1.5/docs/notebooks/climatology/
+-rw-r--r--   0 runner    (1001) docker     (127)   169307 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/climatology/01-era5-climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/requirements-for-notebooks.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.987419 earthkit_aggregate-0.1.5/docs/notebooks/temporal/
+-rw-r--r--   0 runner    (1001) docker     (127)   345207 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/temporal/01-era5-general-methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   315330 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/temporal/02-era5-daily-monthly-statistics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   389728 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/notebooks/temporal/03-seas5-daily-statistics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.979419 earthkit_aggregate-0.1.5/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/earthkit/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30668 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/climatology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31967 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit/aggregate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 13:53:12.000000 earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:53:12.991419 earthkit_aggregate-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/tests/test_10_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/tests/test_20_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/tests/test_30_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-08 13:52:58.000000 earthkit_aggregate-0.1.5/tests/test_30_temporal.py
```

### Comparing `earthkit-aggregate-0.1.4/.github/workflows/on-push.yml` & `earthkit_aggregate-0.1.5/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/.github/workflows/on-release.yml` & `earthkit_aggregate-0.1.5/.github/workflows/on-release.yml`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/.gitignore` & `earthkit_aggregate-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/.pre-commit-config.yaml` & `earthkit_aggregate-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/.readthedocs.yaml` & `earthkit_aggregate-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/LICENSE` & `earthkit_aggregate-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/Makefile` & `earthkit_aggregate-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/PKG-INFO` & `earthkit_aggregate-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-aggregate
-Version: 0.1.4
+Version: 0.1.5
 Summary: Aggregation tools for meteorological and climate data.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `earthkit-aggregate-0.1.4/README.md` & `earthkit_aggregate-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/docs/Makefile` & `earthkit_aggregate-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/docs/conf.py` & `earthkit_aggregate-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/docs/make.bat` & `earthkit_aggregate-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/docs/notebooks/aggregate-climatology.ipynb` & `earthkit_aggregate-0.1.5/docs/notebooks/climatology/01-era5-climatology.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937732835509208%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from earthkit.data.testing import "*

 * *            'earthkit_remote_test_data_file\\n\'), (4, \'ek_data.settings.set("cache-policy", '*

 * *            '"user")\')], delete: [3]}}, 2: {\'source\': {insert: [(6, \'All `earthkit-aggregate` '*

 * *            'methods can be called with `earthkit-data` objects (Readers and Wrappers) or with a '*

 * *            'pre-loaded `xarray`. To reduce the number of conversions in the example, we will '*

 * *            'convert to xarray in the firs […]*

```diff
@@ -13,485 +13,41 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Imports\n",
                 "from earthkit import aggregate as ek_aggregate\n",
                 "from earthkit import data as ek_data\n",
-                "from earthkit.data.testing import earthkit_remote_test_data_file"
+                "from earthkit.data.testing import earthkit_remote_test_data_file\n",
+                "ek_data.settings.set(\"cache-policy\", \"user\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "## Load some test data\n",
                 "\n",
-                "All `earthkit-aggregate` methods can be called with `earthkit-data` objects (Readers and Wrappers) or with the \n",
-                "pre-loaded `xarray`.\n",
-                "\n",
                 "In this example we will use hourly ERA5 2m temperature data on a 0.5x0.5 spatial grid for the year 2015 as\n",
                 "our physical data; and we will use the NUTS geometries which are stored in a geojson file.\n",
                 "\n",
-                "First we lazily load the ERA5 data  and NUTS geometries from our test-data repository.\n",
-                "\n",
-                "Note the data is only downloaded when\n",
-                "we use it, e.g. at the `.to_xarray` line, additionally, the download is cached so the next time you run this\n",
-                "cell you will not need to re-download the file (unless it has been a very long time since you have run the\n",
-                "code, please see tutorials in `earthkit-data` for more details in cache management)."
+                "All `earthkit-aggregate` methods can be called with `earthkit-data` objects (Readers and Wrappers) or with a pre-loaded `xarray`. To reduce the number of conversions in the example, we will convert to xarray in the first cell and use that data object for all subsequent steps."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
-                            "<defs>\n",
-                            "<symbol id=\"icon-database\" viewBox=\"0 0 32 32\">\n",
-                            "<path d=\"M16 0c-8.837 0-16 2.239-16 5v4c0 2.761 7.163 5 16 5s16-2.239 16-5v-4c0-2.761-7.163-5-16-5z\"></path>\n",
-                            "<path d=\"M16 17c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
-                            "<path d=\"M16 26c-8.837 0-16-2.239-16-5v6c0 2.761 7.163 5 16 5s16-2.239 16-5v-6c0 2.761-7.163 5-16 5z\"></path>\n",
-                            "</symbol>\n",
-                            "<symbol id=\"icon-file-text2\" viewBox=\"0 0 32 32\">\n",
-                            "<path d=\"M28.681 7.159c-0.694-0.947-1.662-2.053-2.724-3.116s-2.169-2.030-3.116-2.724c-1.612-1.182-2.393-1.319-2.841-1.319h-15.5c-1.378 0-2.5 1.121-2.5 2.5v27c0 1.378 1.122 2.5 2.5 2.5h23c1.378 0 2.5-1.122 2.5-2.5v-19.5c0-0.448-0.137-1.23-1.319-2.841zM24.543 5.457c0.959 0.959 1.712 1.825 2.268 2.543h-4.811v-4.811c0.718 0.556 1.584 1.309 2.543 2.268zM28 29.5c0 0.271-0.229 0.5-0.5 0.5h-23c-0.271 0-0.5-0.229-0.5-0.5v-27c0-0.271 0.229-0.5 0.5-0.5 0 0 15.499-0 15.5 0v7c0 0.552 0.448 1 1 1h7v19.5z\"></path>\n",
-                            "<path d=\"M23 26h-14c-0.552 0-1-0.448-1-1s0.448-1 1-1h14c0.552 0 1 0.448 1 1s-0.448 1-1 1z\"></path>\n",
-                            "<path d=\"M23 22h-14c-0.552 0-1-0.448-1-1s0.448-1 1-1h14c0.552 0 1 0.448 1 1s-0.448 1-1 1z\"></path>\n",
-                            "<path d=\"M23 18h-14c-0.552 0-1-0.448-1-1s0.448-1 1-1h14c0.552 0 1 0.448 1 1s-0.448 1-1 1z\"></path>\n",
-                            "</symbol>\n",
-                            "</defs>\n",
-                            "</svg>\n",
-                            "<style>/* CSS stylesheet for displaying xarray objects in jupyterlab.\n",
-                            " *\n",
-                            " */\n",
-                            "\n",
-                            ":root {\n",
-                            "  --xr-font-color0: var(--jp-content-font-color0, rgba(0, 0, 0, 1));\n",
-                            "  --xr-font-color2: var(--jp-content-font-color2, rgba(0, 0, 0, 0.54));\n",
-                            "  --xr-font-color3: var(--jp-content-font-color3, rgba(0, 0, 0, 0.38));\n",
-                            "  --xr-border-color: var(--jp-border-color2, #e0e0e0);\n",
-                            "  --xr-disabled-color: var(--jp-layout-color3, #bdbdbd);\n",
-                            "  --xr-background-color: var(--jp-layout-color0, white);\n",
-                            "  --xr-background-color-row-even: var(--jp-layout-color1, white);\n",
-                            "  --xr-background-color-row-odd: var(--jp-layout-color2, #eeeeee);\n",
-                            "}\n",
-                            "\n",
-                            "html[theme=dark],\n",
-                            "body[data-theme=dark],\n",
-                            "body.vscode-dark {\n",
-                            "  --xr-font-color0: rgba(255, 255, 255, 1);\n",
-                            "  --xr-font-color2: rgba(255, 255, 255, 0.54);\n",
-                            "  --xr-font-color3: rgba(255, 255, 255, 0.38);\n",
-                            "  --xr-border-color: #1F1F1F;\n",
-                            "  --xr-disabled-color: #515151;\n",
-                            "  --xr-background-color: #111111;\n",
-                            "  --xr-background-color-row-even: #111111;\n",
-                            "  --xr-background-color-row-odd: #313131;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-wrap {\n",
-                            "  display: block !important;\n",
-                            "  min-width: 300px;\n",
-                            "  max-width: 700px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-text-repr-fallback {\n",
-                            "  /* fallback to plain text repr when CSS is not injected (untrusted notebook) */\n",
-                            "  display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-header {\n",
-                            "  padding-top: 6px;\n",
-                            "  padding-bottom: 6px;\n",
-                            "  margin-bottom: 4px;\n",
-                            "  border-bottom: solid 1px var(--xr-border-color);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-header > div,\n",
-                            ".xr-header > ul {\n",
-                            "  display: inline;\n",
-                            "  margin-top: 0;\n",
-                            "  margin-bottom: 0;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-obj-type,\n",
-                            ".xr-array-name {\n",
-                            "  margin-left: 2px;\n",
-                            "  margin-right: 10px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-obj-type {\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-sections {\n",
-                            "  padding-left: 0 !important;\n",
-                            "  display: grid;\n",
-                            "  grid-template-columns: 150px auto auto 1fr 20px 20px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-item {\n",
-                            "  display: contents;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-item input {\n",
-                            "  display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-item input + label {\n",
-                            "  color: var(--xr-disabled-color);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-item input:enabled + label {\n",
-                            "  cursor: pointer;\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-item input:enabled + label:hover {\n",
-                            "  color: var(--xr-font-color0);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary {\n",
-                            "  grid-column: 1;\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "  font-weight: 500;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary > span {\n",
-                            "  display: inline-block;\n",
-                            "  padding-left: 0.5em;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in:disabled + label {\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in + label:before {\n",
-                            "  display: inline-block;\n",
-                            "  content: '\u25ba';\n",
-                            "  font-size: 11px;\n",
-                            "  width: 15px;\n",
-                            "  text-align: center;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in:disabled + label:before {\n",
-                            "  color: var(--xr-disabled-color);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in:checked + label:before {\n",
-                            "  content: '\u25bc';\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in:checked + label > span {\n",
-                            "  display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary,\n",
-                            ".xr-section-inline-details {\n",
-                            "  padding-top: 4px;\n",
-                            "  padding-bottom: 4px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-inline-details {\n",
-                            "  grid-column: 2 / -1;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-details {\n",
-                            "  display: none;\n",
-                            "  grid-column: 1 / -1;\n",
-                            "  margin-bottom: 5px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-section-summary-in:checked ~ .xr-section-details {\n",
-                            "  display: contents;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-array-wrap {\n",
-                            "  grid-column: 1 / -1;\n",
-                            "  display: grid;\n",
-                            "  grid-template-columns: 20px auto;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-array-wrap > label {\n",
-                            "  grid-column: 1;\n",
-                            "  vertical-align: top;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-preview {\n",
-                            "  color: var(--xr-font-color3);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-array-preview,\n",
-                            ".xr-array-data {\n",
-                            "  padding: 0 5px !important;\n",
-                            "  grid-column: 2;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-array-data,\n",
-                            ".xr-array-in:checked ~ .xr-array-preview {\n",
-                            "  display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-array-in:checked ~ .xr-array-data,\n",
-                            ".xr-array-preview {\n",
-                            "  display: inline-block;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-dim-list {\n",
-                            "  display: inline-block !important;\n",
-                            "  list-style: none;\n",
-                            "  padding: 0 !important;\n",
-                            "  margin: 0;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-dim-list li {\n",
-                            "  display: inline-block;\n",
-                            "  padding: 0;\n",
-                            "  margin: 0;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-dim-list:before {\n",
-                            "  content: '(';\n",
-                            "}\n",
-                            "\n",
-                            ".xr-dim-list:after {\n",
-                            "  content: ')';\n",
-                            "}\n",
-                            "\n",
-                            ".xr-dim-list li:not(:last-child):after {\n",
-                            "  content: ',';\n",
-                            "  padding-right: 5px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-has-index {\n",
-                            "  font-weight: bold;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-list,\n",
-                            ".xr-var-item {\n",
-                            "  display: contents;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-item > div,\n",
-                            ".xr-var-item label,\n",
-                            ".xr-var-item > .xr-var-name span {\n",
-                            "  background-color: var(--xr-background-color-row-even);\n",
-                            "  margin-bottom: 0;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-item > .xr-var-name:hover span {\n",
-                            "  padding-right: 5px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-list > li:nth-child(odd) > div,\n",
-                            ".xr-var-list > li:nth-child(odd) > label,\n",
-                            ".xr-var-list > li:nth-child(odd) > .xr-var-name span {\n",
-                            "  background-color: var(--xr-background-color-row-odd);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-name {\n",
-                            "  grid-column: 1;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-dims {\n",
-                            "  grid-column: 2;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-dtype {\n",
-                            "  grid-column: 3;\n",
-                            "  text-align: right;\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-preview {\n",
-                            "  grid-column: 4;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-index-preview {\n",
-                            "  grid-column: 2 / 5;\n",
-                            "  color: var(--xr-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-name,\n",
-                            ".xr-var-dims,\n",
-                            ".xr-var-dtype,\n",
-                            ".xr-preview,\n",
-                            ".xr-attrs dt {\n",
-                            "  white-space: nowrap;\n",
-                            "  overflow: hidden;\n",
-                            "  text-overflow: ellipsis;\n",
-                            "  padding-right: 10px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-name:hover,\n",
-                            ".xr-var-dims:hover,\n",
-                            ".xr-var-dtype:hover,\n",
-                            ".xr-attrs dt:hover {\n",
-                            "  overflow: visible;\n",
-                            "  width: auto;\n",
-                            "  z-index: 1;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-attrs,\n",
-                            ".xr-var-data,\n",
-                            ".xr-index-data {\n",
-                            "  display: none;\n",
-                            "  background-color: var(--xr-background-color) !important;\n",
-                            "  padding-bottom: 5px !important;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-attrs-in:checked ~ .xr-var-attrs,\n",
-                            ".xr-var-data-in:checked ~ .xr-var-data,\n",
-                            ".xr-index-data-in:checked ~ .xr-index-data {\n",
-                            "  display: block;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-data > table {\n",
-                            "  float: right;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-var-name span,\n",
-                            ".xr-var-data,\n",
-                            ".xr-index-name div,\n",
-                            ".xr-index-data,\n",
-                            ".xr-attrs {\n",
-                            "  padding-left: 25px !important;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-attrs,\n",
-                            ".xr-var-attrs,\n",
-                            ".xr-var-data,\n",
-                            ".xr-index-data {\n",
-                            "  grid-column: 1 / -1;\n",
-                            "}\n",
-                            "\n",
-                            "dl.xr-attrs {\n",
-                            "  padding: 0;\n",
-                            "  margin: 0;\n",
-                            "  display: grid;\n",
-                            "  grid-template-columns: 125px auto;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-attrs dt,\n",
-                            ".xr-attrs dd {\n",
-                            "  padding: 0;\n",
-                            "  margin: 0;\n",
-                            "  float: left;\n",
-                            "  padding-right: 10px;\n",
-                            "  width: auto;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-attrs dt {\n",
-                            "  font-weight: normal;\n",
-                            "  grid-column: 1;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-attrs dt:hover span {\n",
-                            "  display: inline-block;\n",
-                            "  background: var(--xr-background-color);\n",
-                            "  padding-right: 10px;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-attrs dd {\n",
-                            "  grid-column: 2;\n",
-                            "  white-space: pre-wrap;\n",
-                            "  word-break: break-all;\n",
-                            "}\n",
-                            "\n",
-                            ".xr-icon-database,\n",
-                            ".xr-icon-file-text2,\n",
-                            ".xr-no-icon {\n",
-                            "  display: inline-block;\n",
-                            "  vertical-align: middle;\n",
-                            "  width: 1em;\n",
-                            "  height: 1.5em !important;\n",
-                            "  stroke-width: 0;\n",
-                            "  stroke: currentColor;\n",
-                            "  fill: currentColor;\n",
-                            "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
-                            "Dimensions:     (number: 1, time: 4384, step: 1, surface: 1, latitude: 201,\n",
-                            "                 longitude: 281)\n",
-                            "Coordinates:\n",
-                            "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2015-01-01 ... 2017-12-31T18:00:00\n",
-                            "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) float64 0.0\n",
-                            "  * latitude    (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude   (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "    valid_time  (time, step) datetime64[ns] ...\n",
-                            "Data variables:\n",
-                            "    t2m         (number, time, step, surface, latitude, longitude) float32 ...\n",
-                            "Attributes:\n",
-                            "    GRIB_edition:            1\n",
-                            "    GRIB_centre:             ecmf\n",
-                            "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
-                            "    GRIB_subCentre:          0\n",
-                            "    Conventions:             CF-1.7\n",
-                            "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-e62e4645-368a-4e35-a479-8b64d1a69780' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-e62e4645-368a-4e35-a479-8b64d1a69780' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 4384</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-1a88de29-fbd6-4000-adf9-d1d7167f3079' class='xr-section-summary-in' type='checkbox'  checked><label for='section-1a88de29-fbd6-4000-adf9-d1d7167f3079' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-81451edd-bae1-40fb-bead-d6ae56d59e15' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-81451edd-bae1-40fb-bead-d6ae56d59e15' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dfd95309-c335-4c9a-ac21-f2a36a651f4e' class='xr-var-data-in' type='checkbox'><label for='data-dfd95309-c335-4c9a-ac21-f2a36a651f4e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2015-01-01 ... 2017-12-31T18:00:00</div><input id='attrs-15f39318-2f4d-428f-9b4d-52ae5f6b4d66' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-15f39318-2f4d-428f-9b4d-52ae5f6b4d66' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-239d3322-695a-4828-9890-87bcd6049e83' class='xr-var-data-in' type='checkbox'><label for='data-239d3322-695a-4828-9890-87bcd6049e83' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2015-01-01T00:00:00.000000000&#x27;, &#x27;2015-01-01T06:00:00.000000000&#x27;,\n",
-                            "       &#x27;2015-01-01T12:00:00.000000000&#x27;, ..., &#x27;2017-12-31T06:00:00.000000000&#x27;,\n",
-                            "       &#x27;2017-12-31T12:00:00.000000000&#x27;, &#x27;2017-12-31T18:00:00.000000000&#x27;],\n",
-                            "      dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-c771d9a0-048f-4ce9-8d90-b5237610ae91' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c771d9a0-048f-4ce9-8d90-b5237610ae91' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-aa7b1879-b26d-45e8-a0e9-3482ac9101a4' class='xr-var-data-in' type='checkbox'><label for='data-aa7b1879-b26d-45e8-a0e9-3482ac9101a4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-034bd2f3-5ab1-4f25-8e2b-d2e6d210c1dd' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-034bd2f3-5ab1-4f25-8e2b-d2e6d210c1dd' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3d657516-d413-4670-a841-a680c05714f1' class='xr-var-data-in' type='checkbox'><label for='data-3d657516-d413-4670-a841-a680c05714f1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-e32d2dcb-6ff5-4d2b-85c5-12819e08aa48' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e32d2dcb-6ff5-4d2b-85c5-12819e08aa48' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ddf2bba4-9f1c-4285-aaf3-dd035d3fd2d8' class='xr-var-data-in' type='checkbox'><label for='data-ddf2bba4-9f1c-4285-aaf3-dd035d3fd2d8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-72270b35-216a-471d-a7b2-dfa7bf0ba403' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-72270b35-216a-471d-a7b2-dfa7bf0ba403' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d4d95312-7502-4cfc-b7ab-47bff1f836fc' class='xr-var-data-in' type='checkbox'><label for='data-d4d95312-7502-4cfc-b7ab-47bff1f836fc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-6e1411a4-d5a4-4c23-b5c2-4398418817b0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6e1411a4-d5a4-4c23-b5c2-4398418817b0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c05088cc-bb79-4676-885a-10cdf74bca6c' class='xr-var-data-in' type='checkbox'><label for='data-c05088cc-bb79-4676-885a-10cdf74bca6c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[4384 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-867c55fb-0200-42ff-ac18-74609df3a887' class='xr-section-summary-in' type='checkbox'  checked><label for='section-867c55fb-0200-42ff-ac18-74609df3a887' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(number, time, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-9c991bf9-9941-407c-bdf6-90d9c7502ef4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9c991bf9-9941-407c-bdf6-90d9c7502ef4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c7187a2d-7915-4046-a474-754a85b03ad9' class='xr-var-data-in' type='checkbox'><label for='data-c7187a2d-7915-4046-a474-754a85b03ad9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>[247612704 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-6d67a886-058c-456d-ac31-9dbb67860bbe' class='xr-section-summary-in' type='checkbox'  ><label for='section-6d67a886-058c-456d-ac31-9dbb67860bbe' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-49b1a6cf-07c8-4983-b1cf-db15a8c2a8e9' class='xr-index-data-in' type='checkbox'/><label for='index-49b1a6cf-07c8-4983-b1cf-db15a8c2a8e9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d8dafdb8-3350-4282-aa6a-c7e824dbc649' class='xr-index-data-in' type='checkbox'/><label for='index-d8dafdb8-3350-4282-aa6a-c7e824dbc649' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2015-01-01 00:00:00&#x27;, &#x27;2015-01-01 06:00:00&#x27;,\n",
-                            "               &#x27;2015-01-01 12:00:00&#x27;, &#x27;2015-01-01 18:00:00&#x27;,\n",
-                            "               &#x27;2015-01-02 00:00:00&#x27;, &#x27;2015-01-02 06:00:00&#x27;,\n",
-                            "               &#x27;2015-01-02 12:00:00&#x27;, &#x27;2015-01-02 18:00:00&#x27;,\n",
-                            "               &#x27;2015-01-03 00:00:00&#x27;, &#x27;2015-01-03 06:00:00&#x27;,\n",
-                            "               ...\n",
-                            "               &#x27;2017-12-29 12:00:00&#x27;, &#x27;2017-12-29 18:00:00&#x27;,\n",
-                            "               &#x27;2017-12-30 00:00:00&#x27;, &#x27;2017-12-30 06:00:00&#x27;,\n",
-                            "               &#x27;2017-12-30 12:00:00&#x27;, &#x27;2017-12-30 18:00:00&#x27;,\n",
-                            "               &#x27;2017-12-31 00:00:00&#x27;, &#x27;2017-12-31 06:00:00&#x27;,\n",
-                            "               &#x27;2017-12-31 12:00:00&#x27;, &#x27;2017-12-31 18:00:00&#x27;],\n",
-                            "              dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, length=4384, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1ed664ea-c414-4deb-b699-ccae7f05d423' class='xr-index-data-in' type='checkbox'/><label for='index-1ed664ea-c414-4deb-b699-ccae7f05d423' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-eb6dcca4-316b-4119-838a-2fa6b04b5af1' class='xr-index-data-in' type='checkbox'/><label for='index-eb6dcca4-316b-4119-838a-2fa6b04b5af1' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-61b66e33-bd32-48cf-b417-efc0e4365dd1' class='xr-index-data-in' type='checkbox'/><label for='index-61b66e33-bd32-48cf-b417-efc0e4365dd1' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
-                            "       ...\n",
-                            "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-412cd2f7-8bb8-4ec0-815a-d1185f6b2748' class='xr-index-data-in' type='checkbox'/><label for='index-412cd2f7-8bb8-4ec0-815a-d1185f6b2748' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
-                            "       ...\n",
-                            "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7f2f6346-20a1-476c-827b-7824ff8a2996' class='xr-section-summary-in' type='checkbox'  checked><label for='section-7f2f6346-20a1-476c-827b-7824ff8a2996' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
-                        ],
-                        "text/plain": [
-                            "<xarray.Dataset>\n",
-                            "Dimensions:     (number: 1, time: 4384, step: 1, surface: 1, latitude: 201,\n",
-                            "                 longitude: 281)\n",
-                            "Coordinates:\n",
-                            "  * number      (number) int64 0\n",
-                            "  * time        (time) datetime64[ns] 2015-01-01 ... 2017-12-31T18:00:00\n",
-                            "  * step        (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface     (surface) float64 0.0\n",
-                            "  * latitude    (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude   (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "    valid_time  (time, step) datetime64[ns] ...\n",
-                            "Data variables:\n",
-                            "    t2m         (number, time, step, surface, latitude, longitude) float32 ...\n",
-                            "Attributes:\n",
-                            "    GRIB_edition:            1\n",
-                            "    GRIB_centre:             ecmf\n",
-                            "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
-                            "    GRIB_subCentre:          0\n",
-                            "    Conventions:             CF-1.7\n",
-                            "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1..."
-                        ]
-                    },
-                    "execution_count": 2,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Get some demonstration ERA5 data, this could be any url or path to an ERA5 grib or netCDF file.\n",
                 "remote_era5_file = earthkit_remote_test_data_file(\"test-data\", \"era5_temperature_europe_2015_2016_2017.grib\")\n",
                 "era5_data = ek_data.from_source(\"url\", remote_era5_file)\n",
-                "era5_data.to_xarray()"
+                "era5_xr = era5_data.to_xarray()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Calculate the monthly climatologies of the ERA5 data\n",
@@ -866,34 +422,34 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
+                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt; Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 25...\n",
+                            "    t2m_mean   (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-3f7fdf2e-86e4-45d5-bdfa-c6c1698dbbcc' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-3f7fdf2e-86e4-45d5-bdfa-c6c1698dbbcc' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-aa587096-e13d-481c-bbaa-24e81a5bd458' class='xr-section-summary-in' type='checkbox'  checked><label for='section-aa587096-e13d-481c-bbaa-24e81a5bd458' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-08ac6413-2500-4fd8-b886-8b2064795559' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-08ac6413-2500-4fd8-b886-8b2064795559' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0256a8d1-95b0-4f16-858b-d6b122415f58' class='xr-var-data-in' type='checkbox'><label for='data-0256a8d1-95b0-4f16-858b-d6b122415f58' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-eac238c5-5cfe-4f52-a182-4240a81dddd7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-eac238c5-5cfe-4f52-a182-4240a81dddd7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-66886a09-6eee-41d8-94c4-5c4708e67130' class='xr-var-data-in' type='checkbox'><label for='data-66886a09-6eee-41d8-94c4-5c4708e67130' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-39601108-4d57-4db1-9819-989baaf3bf63' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-39601108-4d57-4db1-9819-989baaf3bf63' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9e505f9a-5499-42a2-9dc2-a079c480d0de' class='xr-var-data-in' type='checkbox'><label for='data-9e505f9a-5499-42a2-9dc2-a079c480d0de' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-0decf6e2-cc84-4dca-be09-648f2eae68eb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0decf6e2-cc84-4dca-be09-648f2eae68eb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-826363cc-14d4-4b61-9b69-58f3519b44c0' class='xr-var-data-in' type='checkbox'><label for='data-826363cc-14d4-4b61-9b69-58f3519b44c0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-88b59754-1746-4780-b12b-9eeaf3e4f3fb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-88b59754-1746-4780-b12b-9eeaf3e4f3fb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-82240944-e99b-4927-b92e-66d1020b0d54' class='xr-var-data-in' type='checkbox'><label for='data-82240944-e99b-4927-b92e-66d1020b0d54' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-a94ebfca-2e35-4a0d-ace7-21e1c4d9186e' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-a94ebfca-2e35-4a0d-ace7-21e1c4d9186e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-db610c2b-8b52-472e-b33d-c4d5cbf243d6' class='xr-var-data-in' type='checkbox'><label for='data-db610c2b-8b52-472e-b33d-c4d5cbf243d6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-63f6ad18-a053-4fdf-873e-f9ca46199132' class='xr-section-summary-in' type='checkbox'  checked><label for='section-63f6ad18-a053-4fdf-873e-f9ca46199132' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>256.5 256.6 256.6 ... 286.5 284.3</div><input id='attrs-416b02d4-36de-45e5-bcbb-d86b920ecd33' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-416b02d4-36de-45e5-bcbb-d86b920ecd33' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2b65eb04-98f5-45e1-93e1-531148cf8d23' class='xr-var-data-in' type='checkbox'><label for='data-2b65eb04-98f5-45e1-93e1-531148cf8d23' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[256.51562, 256.5693 , 256.62274, ..., 259.1694 ,\n",
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-8f986c7b-e8b9-4e3e-b18b-01cda4dde70b' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-8f986c7b-e8b9-4e3e-b18b-01cda4dde70b' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-3c510943-0450-447b-af8b-c616ce400ea8' class='xr-section-summary-in' type='checkbox'  checked><label for='section-3c510943-0450-447b-af8b-c616ce400ea8' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-0c5c376e-c466-41d7-b823-4946ea30c5a4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0c5c376e-c466-41d7-b823-4946ea30c5a4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7929762d-3065-481a-b59e-a7983dbdc259' class='xr-var-data-in' type='checkbox'><label for='data-7929762d-3065-481a-b59e-a7983dbdc259' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-b3408654-0fb1-446b-8e5e-d986fc1ba458' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b3408654-0fb1-446b-8e5e-d986fc1ba458' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1c2e88d7-1006-4a8b-bed9-afab51451bd3' class='xr-var-data-in' type='checkbox'><label for='data-1c2e88d7-1006-4a8b-bed9-afab51451bd3' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-8e6e40a4-ad26-4ab0-a7e6-e8592dc3bf6d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-8e6e40a4-ad26-4ab0-a7e6-e8592dc3bf6d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3055b75a-ad31-41e7-9363-f68ec84bc3bc' class='xr-var-data-in' type='checkbox'><label for='data-3055b75a-ad31-41e7-9363-f68ec84bc3bc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-59e6a303-b4f6-4480-b1bf-9b4e19f653ef' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-59e6a303-b4f6-4480-b1bf-9b4e19f653ef' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1a542b04-836f-4eb9-9e66-1414539942de' class='xr-var-data-in' type='checkbox'><label for='data-1a542b04-836f-4eb9-9e66-1414539942de' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-ac0ca438-41e3-4d9a-930c-647dd62ffb16' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ac0ca438-41e3-4d9a-930c-647dd62ffb16' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d94a0a47-e37f-408e-a96a-101b99676a15' class='xr-var-data-in' type='checkbox'><label for='data-d94a0a47-e37f-408e-a96a-101b99676a15' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-7566af03-fb77-4fc5-b4b9-a7521b3a2d84' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-7566af03-fb77-4fc5-b4b9-a7521b3a2d84' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9d511be0-554f-462c-ba4b-549c814de563' class='xr-var-data-in' type='checkbox'><label for='data-9d511be0-554f-462c-ba4b-549c814de563' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-45ff5a51-c95e-44dc-afe6-329ea8c9d494' class='xr-section-summary-in' type='checkbox'  checked><label for='section-45ff5a51-c95e-44dc-afe6-329ea8c9d494' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m_mean</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>256.5 256.6 256.6 ... 286.5 284.3</div><input id='attrs-80afba72-bbac-4b2c-ba92-7f3373ea3735' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-80afba72-bbac-4b2c-ba92-7f3373ea3735' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4e5a339b-e46c-4421-8b97-16a1a1c4b52e' class='xr-var-data-in' type='checkbox'><label for='data-4e5a339b-e46c-4421-8b97-16a1a1c4b52e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[256.51562, 256.5693 , 256.62274, ..., 259.1694 ,\n",
                             "            259.19446, 259.29144],\n",
                             "           [256.7984 , 256.843  , 256.8873 , ..., 259.3892 ,\n",
                             "            259.3459 , 259.30286],\n",
                             "           [257.02753, 257.07336, 257.12482, ..., 259.51556,\n",
                             "            259.5228 , 259.52966],\n",
                             "           ...,\n",
                             "           [289.97018, 289.00494, 288.23837, ..., 286.95883,\n",
@@ -925,52 +481,52 @@
                             "            261.0329 , 260.9566 ],\n",
                             "           ...,\n",
                             "           [291.16565, 290.05692, 289.05536, ..., 286.98325,\n",
                             "            285.86285, 284.24298],\n",
                             "           [291.11502, 290.29156, 289.10825, ..., 287.19745,\n",
                             "            285.78732, 283.90726],\n",
                             "           [291.14703, 290.18015, 288.72662, ..., 287.72403,\n",
-                            "            286.5145 , 284.28705]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2d71478f-fb19-4416-a362-c3c09aa3626c' class='xr-section-summary-in' type='checkbox'  ><label for='section-2d71478f-fb19-4416-a362-c3c09aa3626c' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e5deb471-776e-4739-af96-065dae5a7cbf' class='xr-index-data-in' type='checkbox'/><label for='index-e5deb471-776e-4739-af96-065dae5a7cbf' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-86215264-f307-4494-901d-14e8b90fe16a' class='xr-index-data-in' type='checkbox'/><label for='index-86215264-f307-4494-901d-14e8b90fe16a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c66ac497-eff6-45b7-91f9-664589a4487e' class='xr-index-data-in' type='checkbox'/><label for='index-c66ac497-eff6-45b7-91f9-664589a4487e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-2942c874-1b73-4ec8-a370-5d2674a4c0ef' class='xr-index-data-in' type='checkbox'/><label for='index-2942c874-1b73-4ec8-a370-5d2674a4c0ef' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
+                            "            286.5145 , 284.28705]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-93d77b12-181e-484e-8b49-2dcba71d1cd6' class='xr-section-summary-in' type='checkbox'  ><label for='section-93d77b12-181e-484e-8b49-2dcba71d1cd6' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-5ccd1f89-5a2e-49c5-b2a4-c9152e5facc8' class='xr-index-data-in' type='checkbox'/><label for='index-5ccd1f89-5a2e-49c5-b2a4-c9152e5facc8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d2838203-35f8-4c58-8083-b13b50d43e18' class='xr-index-data-in' type='checkbox'/><label for='index-d2838203-35f8-4c58-8083-b13b50d43e18' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-1c13cec8-b5da-4aa9-9403-01206c5b1d99' class='xr-index-data-in' type='checkbox'/><label for='index-1c13cec8-b5da-4aa9-9403-01206c5b1d99' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-083040e1-6244-4b0e-a7a6-ff1c791851d9' class='xr-index-data-in' type='checkbox'/><label for='index-083040e1-6244-4b0e-a7a6-ff1c791851d9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
                             "       ...\n",
                             "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d70526ea-f664-4228-bcbb-091c9e93a8f9' class='xr-index-data-in' type='checkbox'/><label for='index-d70526ea-f664-4228-bcbb-091c9e93a8f9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-179792ac-6f7a-48c1-8459-e15977e01f51' class='xr-index-data-in' type='checkbox'/><label for='index-179792ac-6f7a-48c1-8459-e15977e01f51' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
                             "       ...\n",
                             "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-68ed4db5-6e0c-4346-bf94-7354e2c95060' class='xr-index-data-in' type='checkbox'/><label for='index-68ed4db5-6e0c-4346-bf94-7354e2c95060' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-fc55a7f6-eade-4f95-a8e0-a5109c4ce1fe' class='xr-section-summary-in' type='checkbox'  checked><label for='section-fc55a7f6-eade-4f95-a8e0-a5109c4ce1fe' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c2a1c8a9-2d92-4452-a8a6-abd035cffcde' class='xr-index-data-in' type='checkbox'/><label for='index-c2a1c8a9-2d92-4452-a8a6-abd035cffcde' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-6cbe7766-45ab-4ef0-af33-b7dd86de546f' class='xr-section-summary-in' type='checkbox'  checked><label for='section-6cbe7766-45ab-4ef0-af33-b7dd86de546f' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.34.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
-                            "<xarray.Dataset>\n",
+                            "<xarray.Dataset> Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 25...\n",
+                            "    t2m_mean   (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "climatology = ek_aggregate.climatology.mean(era5_data, frequency='month')\n",
+                "climatology = ek_aggregate.climatology.monthly_mean(era5_xr)\n",
                 "climatology"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1344,34 +900,34 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
+                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt; Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 27...\n",
+                            "    t2m_max    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-b2266ac2-8c9e-432a-8e22-fb7462fc4f7e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-b2266ac2-8c9e-432a-8e22-fb7462fc4f7e' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4f33299a-8cfb-4533-ae89-de7c69376ca3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4f33299a-8cfb-4533-ae89-de7c69376ca3' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-0a2254ae-a1c9-4e1e-922d-5e90b29e657d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0a2254ae-a1c9-4e1e-922d-5e90b29e657d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e7409067-045d-482f-92e4-56c7b35119f7' class='xr-var-data-in' type='checkbox'><label for='data-e7409067-045d-482f-92e4-56c7b35119f7' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-253fc88b-69d3-4597-8be2-3405067c3655' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-253fc88b-69d3-4597-8be2-3405067c3655' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2a230c85-cf17-49de-9e86-39a02ce28573' class='xr-var-data-in' type='checkbox'><label for='data-2a230c85-cf17-49de-9e86-39a02ce28573' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-e398f86a-e5ee-4765-9ccc-cf95dd0cccd5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e398f86a-e5ee-4765-9ccc-cf95dd0cccd5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7abe56f7-6801-4b5e-a2de-e3e56fe10caa' class='xr-var-data-in' type='checkbox'><label for='data-7abe56f7-6801-4b5e-a2de-e3e56fe10caa' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-9157f34a-cb97-400b-af6c-bf2e234bac34' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9157f34a-cb97-400b-af6c-bf2e234bac34' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3409b7a0-4606-4b9e-a27a-f49c8d4d7a3e' class='xr-var-data-in' type='checkbox'><label for='data-3409b7a0-4606-4b9e-a27a-f49c8d4d7a3e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-6e7482cd-5660-4827-919e-caaa0a1d313f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6e7482cd-5660-4827-919e-caaa0a1d313f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e4fc6e5f-4b14-4fdf-809b-24f52db71738' class='xr-var-data-in' type='checkbox'><label for='data-e4fc6e5f-4b14-4fdf-809b-24f52db71738' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-1d0a3ce2-fbc1-4da8-a770-afa3db4f0eec' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-1d0a3ce2-fbc1-4da8-a770-afa3db4f0eec' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6b582007-5a09-49ca-ac7e-1bf65ece0628' class='xr-var-data-in' type='checkbox'><label for='data-6b582007-5a09-49ca-ac7e-1bf65ece0628' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-6a9f95ad-b72b-4c0b-82f1-5827312211ac' class='xr-section-summary-in' type='checkbox'  checked><label for='section-6a9f95ad-b72b-4c0b-82f1-5827312211ac' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>272.4 272.4 272.5 ... 303.0 300.2</div><input id='attrs-fac9b878-59b1-4d7a-b6d1-0590a3a8c098' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-fac9b878-59b1-4d7a-b6d1-0590a3a8c098' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-becd069f-2486-4ddd-9ca4-3816f46a6434' class='xr-var-data-in' type='checkbox'><label for='data-becd069f-2486-4ddd-9ca4-3816f46a6434' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[272.3571 , 272.43326, 272.50943, ..., 273.53824,\n",
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5dc50606-e6ca-4a5c-887b-bda0930ebd13' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5dc50606-e6ca-4a5c-887b-bda0930ebd13' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-c4dca216-f4d8-454e-8b95-0ebc2aca8fc1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c4dca216-f4d8-454e-8b95-0ebc2aca8fc1' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-2f909aaa-c364-4f28-9fa7-56fd87d109fb' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2f909aaa-c364-4f28-9fa7-56fd87d109fb' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-280eb73b-0a9a-4a61-a213-3f5ead4dd504' class='xr-var-data-in' type='checkbox'><label for='data-280eb73b-0a9a-4a61-a213-3f5ead4dd504' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-e7d1f05b-28bb-4ed3-888d-c693c1f92d5d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e7d1f05b-28bb-4ed3-888d-c693c1f92d5d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-de1019d7-1106-442e-ad08-e8221bc84f92' class='xr-var-data-in' type='checkbox'><label for='data-de1019d7-1106-442e-ad08-e8221bc84f92' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-6fb32aec-a2ae-4b2a-9475-85dbcd74c1f9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6fb32aec-a2ae-4b2a-9475-85dbcd74c1f9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-42888d8e-b612-4844-88ee-5f939c82fb8f' class='xr-var-data-in' type='checkbox'><label for='data-42888d8e-b612-4844-88ee-5f939c82fb8f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-315c8aed-de42-4031-bdf7-cac1753135da' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-315c8aed-de42-4031-bdf7-cac1753135da' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-54ce1ce2-31da-4d45-a8cf-71ae1948cba7' class='xr-var-data-in' type='checkbox'><label for='data-54ce1ce2-31da-4d45-a8cf-71ae1948cba7' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-ba52107a-19b2-4c42-95e0-c9d6ceb3d49c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ba52107a-19b2-4c42-95e0-c9d6ceb3d49c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-2a244175-ae38-4a2d-b879-f93a65adcca6' class='xr-var-data-in' type='checkbox'><label for='data-2a244175-ae38-4a2d-b879-f93a65adcca6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-14985ef8-5bc6-439e-8db8-a0792b55a7b3' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-14985ef8-5bc6-439e-8db8-a0792b55a7b3' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6a65e284-ce3c-47f1-afce-915770f17e38' class='xr-var-data-in' type='checkbox'><label for='data-6a65e284-ce3c-47f1-afce-915770f17e38' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-733a15fc-1ff7-4890-8554-5789e074a827' class='xr-section-summary-in' type='checkbox'  checked><label for='section-733a15fc-1ff7-4890-8554-5789e074a827' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m_max</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>272.4 272.4 272.5 ... 303.0 300.2</div><input id='attrs-00edf600-ca5f-4e7d-8ea8-8313ec0729e8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-00edf600-ca5f-4e7d-8ea8-8313ec0729e8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-daaee8ec-8b15-4cee-b3e5-966ca7aabdcf' class='xr-var-data-in' type='checkbox'><label for='data-daaee8ec-8b15-4cee-b3e5-966ca7aabdcf' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[272.3571 , 272.43326, 272.50943, ..., 273.53824,\n",
                             "            273.55582, 273.56168],\n",
                             "           [273.11685, 273.12662, 273.13638, ..., 273.5496 ,\n",
                             "            273.5109 , 273.48746],\n",
                             "           [273.361  , 273.37076, 273.4059 , ..., 273.48514,\n",
                             "            273.4539 , 273.43472],\n",
                             "           ...,\n",
                             "           [294.4051 , 297.02032, 299.07697, ..., 301.70233,\n",
@@ -1403,52 +959,52 @@
                             "            272.27313, 272.27185],\n",
                             "           ...,\n",
                             "           [294.6776 , 295.74597, 298.63138, ..., 304.07922,\n",
                             "            302.39172, 300.77063],\n",
                             "           [294.0794 , 294.63074, 296.79544, ..., 304.16125,\n",
                             "            302.03235, 300.12415],\n",
                             "           [295.03217, 296.81628, 297.58777, ..., 305.17297,\n",
-                            "            302.95227, 300.19836]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-0cb54a4c-e136-4688-a312-5276cd8ca90d' class='xr-section-summary-in' type='checkbox'  ><label for='section-0cb54a4c-e136-4688-a312-5276cd8ca90d' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-5644a331-5e1b-4822-afc1-d64caccdb8e9' class='xr-index-data-in' type='checkbox'/><label for='index-5644a331-5e1b-4822-afc1-d64caccdb8e9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-6c7714ed-5367-4733-9cb3-ec473c3450fb' class='xr-index-data-in' type='checkbox'/><label for='index-6c7714ed-5367-4733-9cb3-ec473c3450fb' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-11b50826-6277-4483-b5fe-6c303416c303' class='xr-index-data-in' type='checkbox'/><label for='index-11b50826-6277-4483-b5fe-6c303416c303' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e8b8afab-361f-4c82-9f3d-842fae0a2403' class='xr-index-data-in' type='checkbox'/><label for='index-e8b8afab-361f-4c82-9f3d-842fae0a2403' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
+                            "            302.95227, 300.19836]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-5695a098-2226-43df-adb9-e820c2d21606' class='xr-section-summary-in' type='checkbox'  ><label for='section-5695a098-2226-43df-adb9-e820c2d21606' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c0b44c04-dc63-4d84-9d77-76e9d36b6318' class='xr-index-data-in' type='checkbox'/><label for='index-c0b44c04-dc63-4d84-9d77-76e9d36b6318' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-85f29a03-0671-477e-aba7-66d48f59551a' class='xr-index-data-in' type='checkbox'/><label for='index-85f29a03-0671-477e-aba7-66d48f59551a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-78b8fc15-bb39-41c3-ac60-e324732aeafe' class='xr-index-data-in' type='checkbox'/><label for='index-78b8fc15-bb39-41c3-ac60-e324732aeafe' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-b8dd4392-3a3c-46a6-9633-907966c25320' class='xr-index-data-in' type='checkbox'/><label for='index-b8dd4392-3a3c-46a6-9633-907966c25320' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
                             "       ...\n",
                             "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-99cfddc7-fb35-44e2-ac96-2498e37735fe' class='xr-index-data-in' type='checkbox'/><label for='index-99cfddc7-fb35-44e2-ac96-2498e37735fe' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-4a2f6d30-b7c0-4822-be77-d0dfb9e6efdc' class='xr-index-data-in' type='checkbox'/><label for='index-4a2f6d30-b7c0-4822-be77-d0dfb9e6efdc' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
                             "       ...\n",
                             "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e3db8aaf-15b4-4a1d-bf8d-6e288f913c45' class='xr-index-data-in' type='checkbox'/><label for='index-e3db8aaf-15b4-4a1d-bf8d-6e288f913c45' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-8da6e431-6528-4fec-b3d0-ef679206a86e' class='xr-section-summary-in' type='checkbox'  checked><label for='section-8da6e431-6528-4fec-b3d0-ef679206a86e' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-30c0387c-5716-4255-8e08-79e738bc4af3' class='xr-index-data-in' type='checkbox'/><label for='index-30c0387c-5716-4255-8e08-79e738bc4af3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-28482b83-15dc-4ff3-913f-1e84b138fb4e' class='xr-section-summary-in' type='checkbox'  checked><label for='section-28482b83-15dc-4ff3-913f-1e84b138fb4e' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.34.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
-                            "<xarray.Dataset>\n",
+                            "<xarray.Dataset> Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 27...\n",
+                            "    t2m_max    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:35 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "clim_max = ek_aggregate.climatology.max(era5_data, frequency='month')\n",
+                "clim_max = ek_aggregate.climatology.monthly_max(era5_data)\n",
                 "clim_max"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1822,111 +1378,111 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
+                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt; Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 24...\n",
+                            "    t2m_max    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-4119935f-fde4-498b-bc1a-b95b484b68b7' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4119935f-fde4-498b-bc1a-b95b484b68b7' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-f554d0b1-1a92-4af0-a653-2f5ee8c68003' class='xr-section-summary-in' type='checkbox'  checked><label for='section-f554d0b1-1a92-4af0-a653-2f5ee8c68003' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-a35dd590-0a48-4996-8b98-5fb3cd629af9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a35dd590-0a48-4996-8b98-5fb3cd629af9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-44ddbcc1-f95c-47af-9358-ec520648460a' class='xr-var-data-in' type='checkbox'><label for='data-44ddbcc1-f95c-47af-9358-ec520648460a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-d11b62d1-7bdb-498d-a514-c1bc8caa081a' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d11b62d1-7bdb-498d-a514-c1bc8caa081a' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6489a356-f767-44c4-aa55-322d03a4fc95' class='xr-var-data-in' type='checkbox'><label for='data-6489a356-f767-44c4-aa55-322d03a4fc95' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-145af078-a45f-4c8c-aefb-d08c5cabec90' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-145af078-a45f-4c8c-aefb-d08c5cabec90' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-615dfa51-f13b-425b-b406-9e1783110991' class='xr-var-data-in' type='checkbox'><label for='data-615dfa51-f13b-425b-b406-9e1783110991' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-912ee3a4-8f4c-4560-b76b-ee0ee0d4f5de' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-912ee3a4-8f4c-4560-b76b-ee0ee0d4f5de' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a0123871-898b-4d95-a0b5-f8cd922cbac2' class='xr-var-data-in' type='checkbox'><label for='data-a0123871-898b-4d95-a0b5-f8cd922cbac2' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-258bf679-299a-4694-a07c-ca55e428a074' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-258bf679-299a-4694-a07c-ca55e428a074' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-20404d74-8281-4bac-95a3-db97e179b7bd' class='xr-var-data-in' type='checkbox'><label for='data-20404d74-8281-4bac-95a3-db97e179b7bd' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-c315110d-4fc6-44e0-b622-75f1900e51e1' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-c315110d-4fc6-44e0-b622-75f1900e51e1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d4ace4c0-09ce-4254-b746-4f7b05f2a4b7' class='xr-var-data-in' type='checkbox'><label for='data-d4ace4c0-09ce-4254-b746-4f7b05f2a4b7' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-ec32b286-4071-440e-a7a2-106ecb89e40c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-ec32b286-4071-440e-a7a2-106ecb89e40c' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>247.2 247.3 247.3 ... 268.8 267.0</div><input id='attrs-68de6fd1-f64a-4b35-bcbd-b882123bba0d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-68de6fd1-f64a-4b35-bcbd-b882123bba0d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-65d8479b-2885-4aad-b2e6-8262137ac9cf' class='xr-var-data-in' type='checkbox'><label for='data-65d8479b-2885-4aad-b2e6-8262137ac9cf' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[247.17163, 247.25952, 247.29065, ..., 244.21461,\n",
-                            "            244.23189, 244.3608 ],\n",
-                            "           [247.2203 , 247.26328, 247.30624, ..., 244.35524,\n",
-                            "            244.30836, 244.26149],\n",
-                            "           [247.58945, 247.63242, 247.70663, ..., 244.22047,\n",
-                            "            244.34157, 244.46461],\n",
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-faa15f8b-d070-4065-84a3-bef044e5fb8f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-faa15f8b-d070-4065-84a3-bef044e5fb8f' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-f6a3b581-f7e8-4969-a86c-24b661614340' class='xr-section-summary-in' type='checkbox'  checked><label for='section-f6a3b581-f7e8-4969-a86c-24b661614340' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-eaca02b4-6e29-47bc-ba6b-1c9b45b756ed' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-eaca02b4-6e29-47bc-ba6b-1c9b45b756ed' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-55d83819-7088-4a58-a977-c49e82dba207' class='xr-var-data-in' type='checkbox'><label for='data-55d83819-7088-4a58-a977-c49e82dba207' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-978681c6-40eb-472d-97cb-309812f42de6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-978681c6-40eb-472d-97cb-309812f42de6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6f75e8d4-553a-4f46-9905-3b80aa3d28e3' class='xr-var-data-in' type='checkbox'><label for='data-6f75e8d4-553a-4f46-9905-3b80aa3d28e3' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-32aaabe1-e9cc-4c98-a778-34815714e9e9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-32aaabe1-e9cc-4c98-a778-34815714e9e9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-157c8d4d-92e2-4220-bc53-e31e4efa7f64' class='xr-var-data-in' type='checkbox'><label for='data-157c8d4d-92e2-4220-bc53-e31e4efa7f64' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-b1c37b08-450b-4a8a-b2fa-8d201f3181f9' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b1c37b08-450b-4a8a-b2fa-8d201f3181f9' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e0567c3c-6b90-4ccc-a050-1dba6146bfa6' class='xr-var-data-in' type='checkbox'><label for='data-e0567c3c-6b90-4ccc-a050-1dba6146bfa6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-3e265e93-4397-4cab-9824-cc30dba5ac38' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-3e265e93-4397-4cab-9824-cc30dba5ac38' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ca26f8df-6deb-461f-9da8-c4c342a5553c' class='xr-var-data-in' type='checkbox'><label for='data-ca26f8df-6deb-461f-9da8-c4c342a5553c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-1b25700e-3b3f-46df-942c-07df3fe11125' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-1b25700e-3b3f-46df-942c-07df3fe11125' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-031c9fd0-b2fb-4da7-a7d1-d2ef1f630949' class='xr-var-data-in' type='checkbox'><label for='data-031c9fd0-b2fb-4da7-a7d1-d2ef1f630949' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-69e3d03a-7734-41d9-a4a4-01d77175ab6e' class='xr-section-summary-in' type='checkbox'  checked><label for='section-69e3d03a-7734-41d9-a4a4-01d77175ab6e' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m_max</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>272.4 272.4 272.5 ... 303.0 300.2</div><input id='attrs-35ab4ab6-81ea-43c8-a92e-e53c989abbe4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-35ab4ab6-81ea-43c8-a92e-e53c989abbe4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-09de1502-94ed-4abc-8fdf-a3d90174540a' class='xr-var-data-in' type='checkbox'><label for='data-09de1502-94ed-4abc-8fdf-a3d90174540a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[272.3571 , 272.43326, 272.50943, ..., 273.53824,\n",
+                            "            273.55582, 273.56168],\n",
+                            "           [273.11685, 273.12662, 273.13638, ..., 273.5496 ,\n",
+                            "            273.5109 , 273.48746],\n",
+                            "           [273.361  , 273.37076, 273.4059 , ..., 273.48514,\n",
+                            "            273.4539 , 273.43472],\n",
                             "           ...,\n",
-                            "           [286.37683, 283.179  , 279.57352, ..., 269.89334,\n",
-                            "            269.84842, 269.1199 ],\n",
-                            "           [285.9156 , 284.51428, 279.86096, ..., 272.1238 ,\n",
-                            "            270.7742 , 269.15506],\n",
-                            "           [286.80286, 283.15002, 278.56604, ..., 272.9031 ,\n",
-                            "            271.8289 , 269.19608]]]]],\n",
+                            "           [294.4051 , 297.02032, 299.07697, ..., 301.70233,\n",
+                            "            299.79413, 298.1242 ],\n",
+                            "           [295.11224, 294.5008 , 298.4344 , ..., 301.841  ,\n",
+                            "            299.9074 , 297.8957 ],\n",
+                            "           [293.32513, 297.0086 , 297.9676 , ..., 303.03632,\n",
+                            "            300.97968, 298.38202]]]]],\n",
                             "\n",
                             "\n",
                             "\n",
                             "\n",
-                            "       [[[[[242.99715, 242.7784 , 242.5616 , ..., 245.64864,\n",
-                            "            245.56184, 245.68489],\n",
-                            "           [243.4405 , 243.19832, 242.95418, ..., 245.96461,\n",
+                            "       [[[[[272.80545, 272.8328 , 272.86014, ..., 271.3841 ,\n",
+                            "            271.39972, 271.39777],\n",
+                            "           [272.97537, 272.97147, 272.9695 , ..., 271.55402,\n",
                             "...\n",
-                            "            272.8979 , 271.79437],\n",
-                            "           [287.48035, 285.82483, 282.3092 , ..., 273.69086,\n",
-                            "            273.75336, 272.97797]]]]],\n",
+                            "            304.506  , 302.50992],\n",
+                            "           [298.04285, 301.73248, 304.03052, ..., 307.26968,\n",
+                            "            305.16812, 302.69742]]]]],\n",
                             "\n",
                             "\n",
                             "\n",
                             "\n",
-                            "       [[[[[246.4202 , 246.48074, 246.54129, ..., 250.52632,\n",
-                            "            250.46968, 250.52437],\n",
-                            "           [246.48074, 246.53152, 246.58035, ..., 250.91702,\n",
-                            "            250.7803 , 250.64163],\n",
-                            "           [246.73074, 246.78348, 246.84402, ..., 251.31474,\n",
-                            "            251.37529, 251.37405],\n",
+                            "       [[[[[272.84372, 272.90622, 272.96872, ..., 272.4333 ,\n",
+                            "            272.44305, 272.42938],\n",
+                            "           [273.10544, 273.1484 , 273.19138, ..., 272.4782 ,\n",
+                            "            272.4157 , 272.35516],\n",
+                            "           [273.30856, 273.35153, 273.4277 , ..., 272.34344,\n",
+                            "            272.27313, 272.27185],\n",
                             "           ...,\n",
-                            "           [287.29877, 284.61273, 281.28265, ..., 267.87012,\n",
-                            "            268.292  , 267.64355],\n",
-                            "           [287.54007, 286.13275, 281.43652, ..., 270.41553,\n",
-                            "            269.26318, 267.45996],\n",
-                            "           [286.82718, 284.19238, 279.9502 , ..., 270.33545,\n",
-                            "            268.7964 , 267.02832]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4ed50695-df13-4167-bf2c-ae72bed53127' class='xr-section-summary-in' type='checkbox'  ><label for='section-4ed50695-df13-4167-bf2c-ae72bed53127' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-94290f53-8377-49b5-9a55-d3da9bffa1a8' class='xr-index-data-in' type='checkbox'/><label for='index-94290f53-8377-49b5-9a55-d3da9bffa1a8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7557bcef-fda6-46ad-96a1-8c18df783f12' class='xr-index-data-in' type='checkbox'/><label for='index-7557bcef-fda6-46ad-96a1-8c18df783f12' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-59b554c6-ae14-44de-89b1-b79365be4a74' class='xr-index-data-in' type='checkbox'/><label for='index-59b554c6-ae14-44de-89b1-b79365be4a74' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d7bd156d-6b55-4585-b19d-9e5eed47b462' class='xr-index-data-in' type='checkbox'/><label for='index-d7bd156d-6b55-4585-b19d-9e5eed47b462' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
+                            "           [294.6776 , 295.74597, 298.63138, ..., 304.07922,\n",
+                            "            302.39172, 300.77063],\n",
+                            "           [294.0794 , 294.63074, 296.79544, ..., 304.16125,\n",
+                            "            302.03235, 300.12415],\n",
+                            "           [295.03217, 296.81628, 297.58777, ..., 305.17297,\n",
+                            "            302.95227, 300.19836]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-5e2d8dbc-d5f2-494f-b300-6b15a00d8786' class='xr-section-summary-in' type='checkbox'  ><label for='section-5e2d8dbc-d5f2-494f-b300-6b15a00d8786' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9f5314f2-073c-4c16-99aa-ac0a69922d49' class='xr-index-data-in' type='checkbox'/><label for='index-9f5314f2-073c-4c16-99aa-ac0a69922d49' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-68961c69-1f36-4fca-87fc-c1dbcd477d61' class='xr-index-data-in' type='checkbox'/><label for='index-68961c69-1f36-4fca-87fc-c1dbcd477d61' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-dc2d1f5b-7c71-49cb-922f-71c7e4b91cfb' class='xr-index-data-in' type='checkbox'/><label for='index-dc2d1f5b-7c71-49cb-922f-71c7e4b91cfb' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-45870723-0b3b-473c-9b04-a89ae9f12d30' class='xr-index-data-in' type='checkbox'/><label for='index-45870723-0b3b-473c-9b04-a89ae9f12d30' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
                             "       ...\n",
                             "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-924b44a8-c8df-4524-b65d-e1db9976aab6' class='xr-index-data-in' type='checkbox'/><label for='index-924b44a8-c8df-4524-b65d-e1db9976aab6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-d39c8836-878e-4986-bbe9-0d0d46b77e53' class='xr-index-data-in' type='checkbox'/><label for='index-d39c8836-878e-4986-bbe9-0d0d46b77e53' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
                             "       ...\n",
                             "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-c5ae409a-c21c-4ad2-9b66-dc08a01a7f99' class='xr-index-data-in' type='checkbox'/><label for='index-c5ae409a-c21c-4ad2-9b66-dc08a01a7f99' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7bfb47da-fc90-43ad-95ae-5cd7bf1c97db' class='xr-section-summary-in' type='checkbox'  checked><label for='section-7bfb47da-fc90-43ad-95ae-5cd7bf1c97db' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-75787cca-50a6-44e9-ab18-91e2ac398506' class='xr-index-data-in' type='checkbox'/><label for='index-75787cca-50a6-44e9-ab18-91e2ac398506' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d2058824-a536-4408-b8fe-eee1763d82c6' class='xr-section-summary-in' type='checkbox'  checked><label for='section-d2058824-a536-4408-b8fe-eee1763d82c6' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.34.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
-                            "<xarray.Dataset>\n",
+                            "<xarray.Dataset> Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 24...\n",
+                            "    t2m_max    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-03-27T17:11 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "clim_min = ek_aggregate.climatology.min(era5_data, frequency='month')\n",
+                "clim_min = ek_aggregate.climatology.monthly_min(era5_data, frequency='month')\n",
                 "clim_min"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2300,34 +1856,34 @@
                             "  vertical-align: middle;\n",
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
-                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
+                            "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt; Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 6....\n",
+                            "    t2m_std    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-d7ab710a-1cd5-47d1-8279-41e9138e928e' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-d7ab710a-1cd5-47d1-8279-41e9138e928e' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-c7ecdd3b-759f-413b-b354-ffb41afc8785' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c7ecdd3b-759f-413b-b354-ffb41afc8785' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-5a4893ca-547d-4698-9d5a-665dc4dd24df' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5a4893ca-547d-4698-9d5a-665dc4dd24df' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-24b75d22-19cc-45b1-850a-6dd7d8f7e599' class='xr-var-data-in' type='checkbox'><label for='data-24b75d22-19cc-45b1-850a-6dd7d8f7e599' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-cb1f8986-abf6-4ff9-9bbc-8c2467c992d8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-cb1f8986-abf6-4ff9-9bbc-8c2467c992d8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-744c2ab1-7cdb-4bad-b52c-d100cab08e09' class='xr-var-data-in' type='checkbox'><label for='data-744c2ab1-7cdb-4bad-b52c-d100cab08e09' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-48d3c0c7-58a8-4e83-9198-86c17e808c78' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-48d3c0c7-58a8-4e83-9198-86c17e808c78' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b43741fc-5a29-443c-816b-b7ed63368b45' class='xr-var-data-in' type='checkbox'><label for='data-b43741fc-5a29-443c-816b-b7ed63368b45' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-62a3a3d4-2be5-49a0-b01f-290f10be2a5e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-62a3a3d4-2be5-49a0-b01f-290f10be2a5e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c7cd2221-cb26-46e1-aeeb-9829c53b175f' class='xr-var-data-in' type='checkbox'><label for='data-c7cd2221-cb26-46e1-aeeb-9829c53b175f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-79bf1542-a95b-4985-8411-ab8d9619b62c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-79bf1542-a95b-4985-8411-ab8d9619b62c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-965194e2-8bbc-4841-a603-4921ea7b628a' class='xr-var-data-in' type='checkbox'><label for='data-965194e2-8bbc-4841-a603-4921ea7b628a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-311f922e-ec68-4b2d-8449-806792aa33e6' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-311f922e-ec68-4b2d-8449-806792aa33e6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ffe58e17-d000-49f9-bfb8-35403eadbcab' class='xr-var-data-in' type='checkbox'><label for='data-ffe58e17-d000-49f9-bfb8-35403eadbcab' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-bd77a02b-d5ad-468e-b497-5c9f89dff478' class='xr-section-summary-in' type='checkbox'  checked><label for='section-bd77a02b-d5ad-468e-b497-5c9f89dff478' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>6.064 6.071 6.08 ... 6.919 6.693</div><input id='attrs-769c1a43-1ac0-4d91-99a6-df16d01fe663' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-769c1a43-1ac0-4d91-99a6-df16d01fe663' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f95cc461-e89e-4097-9bcc-4aa77594fdb9' class='xr-var-data-in' type='checkbox'><label for='data-f95cc461-e89e-4097-9bcc-4aa77594fdb9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[6.0641294, 6.0714164, 6.0804405, ..., 6.7878475,\n",
+                            "    history:                 2024-03-27T17:12 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-3df872a6-e651-4f59-b66a-95a1fd8f7c6a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-3df872a6-e651-4f59-b66a-95a1fd8f7c6a' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li><li><span class='xr-has-index'>month</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-909ed637-378f-49ce-9483-41bd803d25d2' class='xr-section-summary-in' type='checkbox'  checked><label for='section-909ed637-378f-49ce-9483-41bd803d25d2' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-50ea48cc-e070-4208-b48f-af7e1f3bc56e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-50ea48cc-e070-4208-b48f-af7e1f3bc56e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-511cecd4-4655-4466-8189-d556ddb17335' class='xr-var-data-in' type='checkbox'><label for='data-511cecd4-4655-4466-8189-d556ddb17335' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-ebdb5aa7-d8a0-4ab7-8d3c-d26517d15d3d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ebdb5aa7-d8a0-4ab7-8d3c-d26517d15d3d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dc191a52-fc8f-4bd6-a123-02da8e4fdb73' class='xr-var-data-in' type='checkbox'><label for='data-dc191a52-fc8f-4bd6-a123-02da8e4fdb73' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-9b7f4a1d-4cdf-48e6-9340-6a051a99dcd1' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9b7f4a1d-4cdf-48e6-9340-6a051a99dcd1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bbcdb642-490c-44fb-9f21-5f0ff523534f' class='xr-var-data-in' type='checkbox'><label for='data-bbcdb642-490c-44fb-9f21-5f0ff523534f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-db4a9b7d-8992-4e4a-8d58-8fdbe964a986' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-db4a9b7d-8992-4e4a-8d58-8fdbe964a986' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9d8a8164-a9c3-412f-97fd-760e20f964ea' class='xr-var-data-in' type='checkbox'><label for='data-9d8a8164-a9c3-412f-97fd-760e20f964ea' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-6d57663e-4852-49d6-88ef-c6e82f662bda' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6d57663e-4852-49d6-88ef-c6e82f662bda' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a58e5242-41ef-4d85-a62d-84edab755b33' class='xr-var-data-in' type='checkbox'><label for='data-a58e5242-41ef-4d85-a62d-84edab755b33' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-c20a69ee-a23a-4935-b573-c6b6b8b5ea7c' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-c20a69ee-a23a-4935-b573-c6b6b8b5ea7c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-da6085b8-7984-4e61-b7ce-e68c534b9ce5' class='xr-var-data-in' type='checkbox'><label for='data-da6085b8-7984-4e61-b7ce-e68c534b9ce5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-7a46f61a-bafe-40c5-afab-f4dea152f525' class='xr-section-summary-in' type='checkbox'  checked><label for='section-7a46f61a-bafe-40c5-afab-f4dea152f525' class='xr-section-summary' >Data variables: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t2m_std</span></div><div class='xr-var-dims'>(month, number, step, surface, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>6.064 6.071 6.08 ... 6.919 6.693</div><input id='attrs-4a99d367-d742-48c5-9f4b-c2ceabb2d862' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4a99d367-d742-48c5-9f4b-c2ceabb2d862' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1ef9ca5d-1320-491b-ae44-498e85c99e49' class='xr-var-data-in' type='checkbox'><label for='data-1ef9ca5d-1320-491b-ae44-498e85c99e49' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>167</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>56481</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>surface</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>281</dd><dt><span>GRIB_Ny :</span></dt><dd>201</dd><dt><span>GRIB_cfName :</span></dt><dd>unknown</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t2m</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>0.25</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>80.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>-10.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>60.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>2 metre temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>2t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>2 metre temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>unknown</dd></dl></div><div class='xr-var-data'><pre>array([[[[[[6.0641294, 6.0714164, 6.0804405, ..., 6.7878475,\n",
                             "            6.7843814, 6.7464075],\n",
                             "           [6.129327 , 6.1344943, 6.141636 , ..., 6.80916  ,\n",
                             "            6.813963 , 6.819584 ],\n",
                             "           [6.1802926, 6.1890526, 6.1996555, ..., 6.9892044,\n",
                             "            6.9777513, 6.9670105],\n",
                             "           ...,\n",
                             "           [1.5109539, 2.5213206, 4.133559 , ..., 6.559523 ,\n",
@@ -2359,52 +1915,52 @@
                             "            5.2745705, 5.275142 ],\n",
                             "           ...,\n",
                             "           [1.3705329, 2.3231354, 3.8524024, ..., 7.3433356,\n",
                             "            7.034689 , 6.7784986],\n",
                             "           [1.3092585, 1.6695772, 3.689647 , ..., 7.047256 ,\n",
                             "            6.9631124, 6.7078376],\n",
                             "           [1.239815 , 2.5573583, 3.8950078, ..., 7.087673 ,\n",
-                            "            6.919222 , 6.692765 ]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-fd9ed5d2-e637-4fcf-8710-73c8fc1b41ff' class='xr-section-summary-in' type='checkbox'  ><label for='section-fd9ed5d2-e637-4fcf-8710-73c8fc1b41ff' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-49ad4409-7d48-468c-bda2-a10efab08c2c' class='xr-index-data-in' type='checkbox'/><label for='index-49ad4409-7d48-468c-bda2-a10efab08c2c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9d862ee1-0969-41f4-9ea1-042cdc96692e' class='xr-index-data-in' type='checkbox'/><label for='index-9d862ee1-0969-41f4-9ea1-042cdc96692e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-4dacdfb2-8409-455c-9977-b5f51562f593' class='xr-index-data-in' type='checkbox'/><label for='index-4dacdfb2-8409-455c-9977-b5f51562f593' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-de76a907-b0fa-4174-ba49-01b7a603aa71' class='xr-index-data-in' type='checkbox'/><label for='index-de76a907-b0fa-4174-ba49-01b7a603aa71' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
+                            "            6.919222 , 6.692765 ]]]]]], dtype=float32)</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-40ea5f00-9e20-4ba0-be50-c638346eaaef' class='xr-section-summary-in' type='checkbox'  ><label for='section-40ea5f00-9e20-4ba0-be50-c638346eaaef' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-3c9f8425-cac7-4f13-96b0-0543e348679b' class='xr-index-data-in' type='checkbox'/><label for='index-3c9f8425-cac7-4f13-96b0-0543e348679b' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-97f120e1-90a8-4a5e-bd3d-0c3c8d53bc14' class='xr-index-data-in' type='checkbox'/><label for='index-97f120e1-90a8-4a5e-bd3d-0c3c8d53bc14' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-3b717d64-33ee-4725-89e3-22fc4fcb16d6' class='xr-index-data-in' type='checkbox'/><label for='index-3b717d64-33ee-4725-89e3-22fc4fcb16d6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bc0c2e6b-7314-497e-918a-9bcd811a98a7' class='xr-index-data-in' type='checkbox'/><label for='index-bc0c2e6b-7314-497e-918a-9bcd811a98a7' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
                             "       ...\n",
                             "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-90979af0-9abb-44fc-aa83-9a68c40fed4c' class='xr-index-data-in' type='checkbox'/><label for='index-90979af0-9abb-44fc-aa83-9a68c40fed4c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-ba57eb64-9250-4872-9e9c-91a2cb21386a' class='xr-index-data-in' type='checkbox'/><label for='index-ba57eb64-9250-4872-9e9c-91a2cb21386a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
                             "       ...\n",
                             "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-a2d1b450-c646-44d3-b643-98ae384c77c4' class='xr-index-data-in' type='checkbox'/><label for='index-a2d1b450-c646-44d3-b643-98ae384c77c4' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-e0e42e64-96aa-4bfe-ae54-868b98ffd420' class='xr-section-summary-in' type='checkbox'  checked><label for='section-e0e42e64-96aa-4bfe-ae54-868b98ffd420' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.30.0 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-2bd9190f-83d8-45cb-b3a7-1ae0c5cea951' class='xr-index-data-in' type='checkbox'/><label for='index-2bd9190f-83d8-45cb-b3a7-1ae0c5cea951' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-5dad9de2-2ef0-4922-a084-411894273825' class='xr-section-summary-in' type='checkbox'  checked><label for='section-5dad9de2-2ef0-4922-a084-411894273825' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2024-03-27T17:12 GRIB to CDM+CF via cfgrib-0.9.10.4/ecCodes-2.34.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
-                            "<xarray.Dataset>\n",
+                            "<xarray.Dataset> Size: 3MB\n",
                             "Dimensions:    (number: 1, step: 1, surface: 1, latitude: 201, longitude: 281,\n",
                             "                month: 12)\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12\n",
                             "Data variables:\n",
-                            "    t2m        (month, number, step, surface, latitude, longitude) float32 6....\n",
+                            "    t2m_std    (month, number, step, surface, latitude, longitude) float32 3MB ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-09-08T14:36 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2024-03-27T17:12 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "clim_std = ek_aggregate.climatology.stdev(era5_data, frequency='month')\n",
+                "clim_std = ek_aggregate.climatology.monthly_std(era5_data, frequency='month')\n",
                 "clim_std"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
@@ -2772,24 +2328,24 @@
                             "  width: 1em;\n",
                             "  height: 1.5em !important;\n",
                             "  stroke-width: 0;\n",
                             "  stroke: currentColor;\n",
                             "  fill: currentColor;\n",
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.DataArray &#x27;t2m&#x27; (quantile: 3, number: 1, month: 12, step: 1,\n",
-                            "                         surface: 1, latitude: 201, longitude: 281)&gt;\n",
+                            "                         surface: 1, latitude: 201, longitude: 281)&gt; Size: 16MB\n",
                             "dask.array&lt;concatenate, shape=(3, 1, 12, 1, 1, 201, 281), dtype=float64, chunksize=(1, 1, 1, 1, 1, 201, 281), chunktype=numpy.ndarray&gt;\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * quantile   (quantile) float64 0.1 0.5 0.9\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'>'t2m'</div><ul class='xr-dim-list'><li><span class='xr-has-index'>quantile</span>: 3</li><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>month</span>: 12</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-b5263bbf-23e3-4af7-8e5a-1451f6e94687' class='xr-array-in' type='checkbox' checked><label for='section-b5263bbf-23e3-4af7-8e5a-1451f6e94687' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>dask.array&lt;chunksize=(1, 1, 1, 1, 1, 201, 281), meta=np.ndarray&gt;</span></div><div class='xr-array-data'><table>\n",
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * quantile   (quantile) float64 24B 0.1 0.5 0.9\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.DataArray</div><div class='xr-array-name'>'t2m'</div><ul class='xr-dim-list'><li><span class='xr-has-index'>quantile</span>: 3</li><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>month</span>: 12</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>surface</span>: 1</li><li><span class='xr-has-index'>latitude</span>: 201</li><li><span class='xr-has-index'>longitude</span>: 281</li></ul></div><ul class='xr-sections'><li class='xr-section-item'><div class='xr-array-wrap'><input id='section-878c17b1-cea0-41ac-8647-88547c4eebb9' class='xr-array-in' type='checkbox' checked><label for='section-878c17b1-cea0-41ac-8647-88547c4eebb9' title='Show/hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-array-preview xr-preview'><span>dask.array&lt;chunksize=(1, 1, 1, 1, 1, 201, 281), meta=np.ndarray&gt;</span></div><div class='xr-array-data'><table>\n",
                             "    <tr>\n",
                             "        <td>\n",
                             "            <table style=\"border-collapse: collapse;\">\n",
                             "                <thead>\n",
                             "                    <tr>\n",
                             "                        <td> </td>\n",
                             "                        <th> Array </th>\n",
@@ -2938,34 +2494,34 @@
                             "  <!-- Text -->\n",
                             "  <text x=\"364.948598\" y=\"120.784897\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" >281</text>\n",
                             "  <text x=\"444.948598\" y=\"57.866747\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" transform=\"rotate(-90,444.948598,57.866747)\">201</text>\n",
                             "  <text x=\"287.474299\" y=\"113.310598\" font-size=\"1.0rem\" font-weight=\"100\" text-anchor=\"middle\" transform=\"rotate(45,287.474299,113.310598)\">1</text>\n",
                             "</svg>\n",
                             "        </td>\n",
                             "    </tr>\n",
-                            "</table></div></div></li><li class='xr-section-item'><input id='section-4bf4a268-eeb2-4b71-ab95-9863d2b01b75' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4bf4a268-eeb2-4b71-ab95-9863d2b01b75' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-06860c51-1a31-4875-9499-6badb219c9b3' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-06860c51-1a31-4875-9499-6badb219c9b3' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-275e7acd-a861-41a4-b455-3cc799c5111a' class='xr-var-data-in' type='checkbox'><label for='data-275e7acd-a861-41a4-b455-3cc799c5111a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-c7cc68df-ae55-4598-9878-60df32187523' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c7cc68df-ae55-4598-9878-60df32187523' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-924e0c81-f5bb-419e-907a-30936a695262' class='xr-var-data-in' type='checkbox'><label for='data-924e0c81-f5bb-419e-907a-30936a695262' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-023dcd11-9eab-4c08-8508-37ca419f8281' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-023dcd11-9eab-4c08-8508-37ca419f8281' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0f323d6f-2c36-4372-8829-fd2b32f9aa57' class='xr-var-data-in' type='checkbox'><label for='data-0f323d6f-2c36-4372-8829-fd2b32f9aa57' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-21fc92b8-245d-40d1-84a2-52eaa4770f13' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-21fc92b8-245d-40d1-84a2-52eaa4770f13' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-72381553-b9b8-4b18-b33b-b74e39d432f1' class='xr-var-data-in' type='checkbox'><label for='data-72381553-b9b8-4b18-b33b-b74e39d432f1' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-e2d0970f-7b97-4370-ad1e-289ffd5d2363' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e2d0970f-7b97-4370-ad1e-289ffd5d2363' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-39f01b09-6df1-4cbb-bb25-7ed31b3bfe4c' class='xr-var-data-in' type='checkbox'><label for='data-39f01b09-6df1-4cbb-bb25-7ed31b3bfe4c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>quantile</span></div><div class='xr-var-dims'>(quantile)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.1 0.5 0.9</div><input id='attrs-3e7e4838-825e-4662-bc69-3eac09b4a8b6' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-3e7e4838-825e-4662-bc69-3eac09b4a8b6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-eb5d8138-1a10-4c62-9fe6-dbf514609e11' class='xr-var-data-in' type='checkbox'><label for='data-eb5d8138-1a10-4c62-9fe6-dbf514609e11' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([0.1, 0.5, 0.9])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-ed329ac8-b41f-43fe-82e2-7a9d881c7041' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-ed329ac8-b41f-43fe-82e2-7a9d881c7041' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-50c29b5d-b4ce-4a53-947e-798bca52b461' class='xr-var-data-in' type='checkbox'><label for='data-50c29b5d-b4ce-4a53-947e-798bca52b461' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-cc058c65-899d-4603-ac25-c0f3e6c14ed4' class='xr-section-summary-in' type='checkbox'  ><label for='section-cc058c65-899d-4603-ac25-c0f3e6c14ed4' class='xr-section-summary' >Indexes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e13981e9-0a9a-4439-a1bd-e29644205d79' class='xr-index-data-in' type='checkbox'/><label for='index-e13981e9-0a9a-4439-a1bd-e29644205d79' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7fba7d6d-468f-42a0-a6ca-c0f1a30998cd' class='xr-index-data-in' type='checkbox'/><label for='index-7fba7d6d-468f-42a0-a6ca-c0f1a30998cd' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-eb7fd5ad-4915-43dc-a7bd-b13a3acf86e0' class='xr-index-data-in' type='checkbox'/><label for='index-eb7fd5ad-4915-43dc-a7bd-b13a3acf86e0' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8ed7154f-d632-4de1-8ba0-557c64d1d394' class='xr-index-data-in' type='checkbox'/><label for='index-8ed7154f-d632-4de1-8ba0-557c64d1d394' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
+                            "</table></div></div></li><li class='xr-section-item'><input id='section-4686517c-6a8f-4e14-b161-a3b9e07cb827' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4686517c-6a8f-4e14-b161-a3b9e07cb827' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-276170f3-cb27-4afe-b07d-d7ad15cefc59' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-276170f3-cb27-4afe-b07d-d7ad15cefc59' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-6ed2e042-f87d-47b2-90f4-caeaa520e507' class='xr-var-data-in' type='checkbox'><label for='data-6ed2e042-f87d-47b2-90f4-caeaa520e507' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-a4b14a35-f5b4-49e2-b298-eeb194cf7ba8' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a4b14a35-f5b4-49e2-b298-eeb194cf7ba8' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e4bd542c-db9a-4023-a041-5a9fd5dd79b8' class='xr-var-data-in' type='checkbox'><label for='data-e4bd542c-db9a-4023-a041-5a9fd5dd79b8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>surface</span></div><div class='xr-var-dims'>(surface)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0</div><input id='attrs-6c6ff870-bef0-44bb-88b8-d14cd9ef19e1' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-6c6ff870-bef0-44bb-88b8-d14cd9ef19e1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4ac8a345-6c65-4feb-9921-f7c81b665626' class='xr-var-data-in' type='checkbox'><label for='data-4ac8a345-6c65-4feb-9921-f7c81b665626' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>original GRIB coordinate for key: level(surface)</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>array([0.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>80.0 79.75 79.5 ... 30.5 30.25 30.0</div><input id='attrs-b45ade30-2802-413d-873f-ebef1df43124' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b45ade30-2802-413d-873f-ebef1df43124' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dc5ee5ec-623e-4f21-bde8-ffe9944e4a61' class='xr-var-data-in' type='checkbox'><label for='data-dc5ee5ec-623e-4f21-bde8-ffe9944e4a61' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([80.  , 79.75, 79.5 , ..., 30.5 , 30.25, 30.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>-10.0 -9.75 -9.5 ... 59.75 60.0</div><input id='attrs-5dea8ab4-804b-453c-9645-b79e089107a6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5dea8ab4-804b-453c-9645-b79e089107a6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dd7e5c4e-40b0-46c6-9bd6-2001939a18d6' class='xr-var-data-in' type='checkbox'><label for='data-dd7e5c4e-40b0-46c6-9bd6-2001939a18d6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([-10.  ,  -9.75,  -9.5 , ...,  59.5 ,  59.75,  60.  ])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>quantile</span></div><div class='xr-var-dims'>(quantile)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.1 0.5 0.9</div><input id='attrs-6f118ae1-bd1b-4662-afa9-be968a5c15a4' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-6f118ae1-bd1b-4662-afa9-be968a5c15a4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-037bcfe6-1e77-4016-a6b1-f3e61724432e' class='xr-var-data-in' type='checkbox'><label for='data-037bcfe6-1e77-4016-a6b1-f3e61724432e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([0.1, 0.5, 0.9])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>month</span></div><div class='xr-var-dims'>(month)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1 2 3 4 5 6 7 8 9 10 11 12</div><input id='attrs-f3957264-c2b0-497a-a40c-a3965291c82c' class='xr-var-attrs-in' type='checkbox' disabled><label for='attrs-f3957264-c2b0-497a-a40c-a3965291c82c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-dbbc0602-0447-4399-a953-448cfbfdc761' class='xr-var-data-in' type='checkbox'><label for='data-dbbc0602-0447-4399-a953-448cfbfdc761' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'></dl></div><div class='xr-var-data'><pre>array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d3382e3d-5d5c-4276-b3e0-dc93ed0bce79' class='xr-section-summary-in' type='checkbox'  ><label for='section-d3382e3d-5d5c-4276-b3e0-dc93ed0bce79' class='xr-section-summary' >Indexes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-eb946fc2-3f43-4706-8dbb-6ad75f878a12' class='xr-index-data-in' type='checkbox'/><label for='index-eb946fc2-3f43-4706-8dbb-6ad75f878a12' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-74c58af1-690b-49f2-b73f-454f2b61d99d' class='xr-index-data-in' type='checkbox'/><label for='index-74c58af1-690b-49f2-b73f-454f2b61d99d' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>surface</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-728111ed-37c1-4644-9aa9-6372d44ab7ff' class='xr-index-data-in' type='checkbox'/><label for='index-728111ed-37c1-4644-9aa9-6372d44ab7ff' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.0], dtype=&#x27;float64&#x27;, name=&#x27;surface&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-0c44402c-0563-47cc-b393-a2231a8c9cc8' class='xr-index-data-in' type='checkbox'/><label for='index-0c44402c-0563-47cc-b393-a2231a8c9cc8' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([ 80.0, 79.75,  79.5, 79.25,  79.0, 78.75,  78.5, 78.25,  78.0, 77.75,\n",
                             "       ...\n",
                             "       32.25,  32.0, 31.75,  31.5, 31.25,  31.0, 30.75,  30.5, 30.25,  30.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-fa6db4ff-a53e-449a-a9cf-5cd31f9262bf' class='xr-index-data-in' type='checkbox'/><label for='index-fa6db4ff-a53e-449a-a9cf-5cd31f9262bf' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;, length=201))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-671d7cdb-f89f-44f7-8c05-bf438506332e' class='xr-index-data-in' type='checkbox'/><label for='index-671d7cdb-f89f-44f7-8c05-bf438506332e' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([-10.0, -9.75,  -9.5, -9.25,  -9.0, -8.75,  -8.5, -8.25,  -8.0, -7.75,\n",
                             "       ...\n",
                             "       57.75,  58.0, 58.25,  58.5, 58.75,  59.0, 59.25,  59.5, 59.75,  60.0],\n",
-                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>quantile</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-73f46153-3875-4332-97a9-46465948676c' class='xr-index-data-in' type='checkbox'/><label for='index-73f46153-3875-4332-97a9-46465948676c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.1, 0.5, 0.9], dtype=&#x27;float64&#x27;, name=&#x27;quantile&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-65fa04d2-3c3b-493d-8b9a-7229356486f6' class='xr-index-data-in' type='checkbox'/><label for='index-65fa04d2-3c3b-493d-8b9a-7229356486f6' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-ca56859a-d51e-4141-bd66-9435b3b88611' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ca56859a-d51e-4141-bd66-9435b3b88611' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
+                            "      dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;, length=281))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>quantile</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-e30da571-a669-4854-ad86-15b628a7ca44' class='xr-index-data-in' type='checkbox'/><label for='index-e30da571-a669-4854-ad86-15b628a7ca44' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([0.1, 0.5, 0.9], dtype=&#x27;float64&#x27;, name=&#x27;quantile&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>month</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-7f7e7381-c11d-4a66-896d-7643cecbf132' class='xr-index-data-in' type='checkbox'/><label for='index-7f7e7381-c11d-4a66-896d-7643cecbf132' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12], dtype=&#x27;int64&#x27;, name=&#x27;month&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-04207191-b71c-4f8c-8aba-861a22cbf15a' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-04207191-b71c-4f8c-8aba-861a22cbf15a' class='xr-section-summary'  title='Expand/collapse section'>Attributes: <span>(0)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.DataArray 't2m' (quantile: 3, number: 1, month: 12, step: 1,\n",
-                            "                         surface: 1, latitude: 201, longitude: 281)>\n",
+                            "                         surface: 1, latitude: 201, longitude: 281)> Size: 16MB\n",
                             "dask.array<concatenate, shape=(3, 1, 12, 1, 1, 201, 281), dtype=float64, chunksize=(1, 1, 1, 1, 1, 201, 281), chunktype=numpy.ndarray>\n",
                             "Coordinates:\n",
-                            "  * number     (number) int64 0\n",
-                            "  * step       (step) timedelta64[ns] 00:00:00\n",
-                            "  * surface    (surface) float64 0.0\n",
-                            "  * latitude   (latitude) float64 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
-                            "  * longitude  (longitude) float64 -10.0 -9.75 -9.5 -9.25 ... 59.5 59.75 60.0\n",
-                            "  * quantile   (quantile) float64 0.1 0.5 0.9\n",
-                            "  * month      (month) int64 1 2 3 4 5 6 7 8 9 10 11 12"
+                            "  * number     (number) int64 8B 0\n",
+                            "  * step       (step) timedelta64[ns] 8B 00:00:00\n",
+                            "  * surface    (surface) float64 8B 0.0\n",
+                            "  * latitude   (latitude) float64 2kB 80.0 79.75 79.5 79.25 ... 30.5 30.25 30.0\n",
+                            "  * longitude  (longitude) float64 2kB -10.0 -9.75 -9.5 ... 59.5 59.75 60.0\n",
+                            "  * quantile   (quantile) float64 24B 0.1 0.5 0.9\n",
+                            "  * month      (month) int64 96B 1 2 3 4 5 6 7 8 9 10 11 12"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2993,15 +2549,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.11.8"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "58c973d167e6390f895c0b1f5bfc390aa59fea9f5b6b442df4c096a67487aa21"
             }
         }
```

### Comparing `earthkit-aggregate-0.1.4/docs/notebooks/aggregate-spatial.ipynb` & `earthkit_aggregate-0.1.5/docs/notebooks/aggregate-spatial.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/earthkit/aggregate/__init__.py` & `earthkit_aggregate-0.1.5/earthkit/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/earthkit/aggregate/general.py` & `earthkit_aggregate-0.1.5/earthkit/aggregate/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 import numpy as np
 import xarray as xr
 
 from earthkit.aggregate import tools
 
 
+@tools.how_label_decorator()
 def _reduce_dataarray(
     dataarray: xr.DataArray,
-    how: T.Union[T.Callable, str] = "mean",
-    weights: T.Union[None, str, np.ndarray] = None,
-    how_label: str = "",
+    how: T.Callable | str = "mean",
+    weights: None | str | np.ndarray = None,
+    how_label: str | None = None,
     how_dropna=False,
     **kwargs,
 ):
     """
     Reduce an xarray.dataarray or xarray.dataset using a specified `how` method.
 
     With the option to apply weights either directly or using a specified
@@ -70,25 +71,30 @@
             if isinstance(how, str):
                 how_label = deepcopy(how)
                 how = tools.get_how(how)
             assert isinstance(how, T.Callable), f"how method not recognised: {how}"
 
             red_array = dataarray.reduce(how, **kwargs)
 
-    if how_label:
-        red_array = red_array.rename(f"{red_array.name}_{how_label}")
+    if how_label is not None:
+        # Update variable names, depends on dataset or dataarray format
+        if isinstance(red_array, xr.Dataset):
+            renames = {data_arr: f"{data_arr}_{how_label}" for data_arr in red_array}
+            red_array = red_array.rename(**renames)
+        else:
+            red_array = red_array.rename(f"{red_array.name}_{how_label}")
 
     if how_dropna:
         red_array = red_array.dropna(how_dropna)
 
     return red_array
 
 
 def reduce(
-    dataarray: T.Union[xr.DataArray, xr.Dataset],
+    dataarray: xr.Dataset | xr.DataArray,
     *args,
     **kwargs,
 ):
     """
     Reduce an xarray.dataarray or xarray.dataset using a specified `how` method.
 
     With the option to apply weights either directly or using a specified
@@ -115,25 +121,24 @@
         kwargs recognised by the how :func: `reduce`
 
     Returns
     -------
         A data array with reduce dimensions removed.
 
     """
-    if isinstance(dataarray, (xr.Dataset)):
-        out_ds = xr.Dataset().assign_attrs(dataarray.attrs)
-        for var in dataarray.data_vars:
-            out_da = _reduce_dataarray(dataarray[var], *args, **kwargs)
-            out_ds[out_da.name] = out_da
-        return out_ds
-    else:
-        return _reduce_dataarray(dataarray, *args, **kwargs)
+    # handle how as arg or kwarg
+    kwargs["how"] = args[0] if args else kwargs.get("how", "mean")
+    out = _reduce_dataarray(dataarray, **kwargs)
+    # Ensure any input attributes are preserved (maybe not necessary)
+    if isinstance(dataarray, xr.Dataset):
+        out.attrs.update(dataarray.attrs)
+    return out
 
 
-def rolling_reduce(dataarray: T.Union[xr.Dataset, xr.DataArray], *args, **kwargs) -> xr.DataArray:
+def rolling_reduce(dataarray: xr.Dataset | xr.DataArray, *args, **kwargs) -> xr.DataArray:
     """Return reduced data using a moving window over which to apply the reduction.
 
     Parameters
     ----------
     dataarray : xr.DataArray or xr.Dataset
         Data over which the moving window is applied according to the reduction method.
     windows :
@@ -211,15 +216,16 @@
     rolling_kwargs = {_kwarg: kwargs.pop(_kwarg) for _kwarg in rolling_kwargs_keys}
 
     # Any kwargs left after above reductions are kwargs for reduction method
     reduce_kwargs = kwargs
     # Create rolling groups:
     data_rolling = dataarray.rolling(**rolling_kwargs)
 
-    data_windowed = _reduce_dataarray(data_rolling, how=how_reduce, **reduce_kwargs)
+    reduce_kwargs.setdefault("how", how_reduce)
+    data_windowed = _reduce_dataarray(data_rolling, **reduce_kwargs)
 
     data_windowed = _dropna(data_windowed, window_dims, how_dropna)
 
     data_windowed.attrs.update(dataarray.attrs)
 
     return data_windowed
 
@@ -231,19 +237,21 @@
 
     for dim in dims:
         data = data.dropna(dim, how=how)
     return data
 
 
 def resample(
-    dataarray: T.Union[xr.Dataset, xr.DataArray],
-    frequency: str or int or float,
+    dataarray: xr.Dataset | xr.DataArray,
+    frequency: str | int | float,
     dim: str = "time",
     how: str = "mean",
     skipna: bool = True,
+    how_args: list[T.Any] = [],
+    how_kwargs: dict[str, T.Any] = {},
     **kwargs,
 ) -> xr.DataArray:
     """
     Resample dataarray to a user-defined frequency using a user-defined "how" method.
 
     Parameters
     ----------
@@ -260,12 +268,16 @@
         Keyword arguments to be passed to :func:`resample`. Defaults have been set as:
         `{"skipna": True}`
 
     Returns
     -------
     xr.DataArray
     """
+    # Get any how kwargs into appropriate dictionary:
+    for _k in ["q", "p"]:
+        if _k in kwargs:
+            how_kwargs[_k] = kwargs.pop(_k)
     # Translate and xarray frequencies to pandas language:
     frequency = tools._PANDAS_FREQUENCIES_R.get(frequency, frequency)
     resample = dataarray.resample(skipna=skipna, **{dim: frequency}, **kwargs)
-    result = resample.__getattribute__(how)(dim)
+    result = resample.__getattribute__(how)(*how_args, dim=dim, **how_kwargs)
     return result
```

### Comparing `earthkit-aggregate-0.1.4/earthkit/aggregate/spatial.py` & `earthkit_aggregate-0.1.5/earthkit/aggregate/spatial.py`

 * *Files 5% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     else:
         mask_function = mask_contains_points
 
     return mask_function(shapes, target.coords, **kwargs)
 
 
 def get_mask_dim_index(
-    mask_dim: T.Union[str, None, T.Dict[str, T.Any]],
+    mask_dim: str | None | T.Dict[str, T.Any],
     geodataframe: gpd.geodataframe.GeoDataFrame,
     default_index_name: str = "index",
 ):
     if isinstance(mask_dim, str):
         if mask_dim in geodataframe:
             mask_dim_index = pd.Index(geodataframe[mask_dim])
         else:
@@ -208,18 +208,18 @@
     else:
         raise ValueError("Unrecognised mask_dim format")
 
     return mask_dim_index
 
 
 def mask(
-    dataarray: T.Union[xr.Dataset, xr.DataArray],
+    dataarray: xr.Dataset | xr.DataArray,
     geodataframe: gpd.geodataframe.GeoDataFrame,
-    lat_key: T.Union[None, str] = None,
-    lon_key: T.Union[None, str] = None,
+    lat_key: str | None = None,
+    lon_key: str | None = None,
     **mask_kwargs,
 ):
     """
     Apply shape mask to some gridded data.
 
     The geodataframe object is treated as a single mask, any points that lie outside of any
     of the features are masked
@@ -244,19 +244,19 @@
     mask = shapes_to_mask(geodataframe, dataarray, **mask_kwargs)
     out = dataarray.where(mask)
     out.attrs.update(geodataframe.attrs)
     return out
 
 
 def masks(
-    dataarray: T.Union[xr.Dataset, xr.DataArray],
+    dataarray: xr.Dataset | xr.DataArray,
     geodataframe: gpd.geodataframe.GeoDataFrame,
-    mask_dim: T.Union[str, None] = None,
-    lat_key: T.Union[None, str] = None,
-    lon_key: T.Union[None, str] = None,
+    mask_dim: str | None = None,
+    lat_key: str | None = None,
+    lon_key: str | None = None,
     chunk: bool = True,
     **mask_kwargs,
 ):
     """
     Apply multiple shape masks to some gridded data.
 
     Each feauture in shape is treated as an individual mask to apply to
@@ -306,15 +306,15 @@
 
     out.attrs.update(geodataframe.attrs)
 
     return out
 
 
 def reduce(
-    dataarray: T.Union[xr.Dataset, xr.DataArray],
+    dataarray: xr.Dataset | xr.DataArray,
     geodataframe: gpd.GeoDataFrame | None = None,
     *args,
     **kwargs,
 ):
     """
     Apply a shape object to an xarray.DataArray object using the specified 'how' method.
 
@@ -383,22 +383,22 @@
         return _reduce_dataarray(dataarray, geodataframe=geodataframe, *args, **kwargs)
 
 
 def _reduce_dataarray(
     dataarray: xr.DataArray,
     geodataframe: gpd.GeoDataFrame | None = None,
     pd_dataframe: pd.DataFrame | None = None,
-    how: T.Union[T.Callable, str] = "mean",
-    weights: T.Union[None, str, np.ndarray] = None,
-    lat_key: T.Union[None, str] = None,
-    lon_key: T.Union[None, str] = None,
-    extra_reduce_dims: T.Union[list, str] = [],
-    mask_dim: T.Union[None, str] = None,
+    how: T.Callable | str = "mean",
+    weights: None | str | np.ndarray = None,
+    lat_key: str | None = None,
+    lon_key: str | None = None,
+    extra_reduce_dims: list | str = [],
+    mask_dim: str | None = None,
     return_as: str = "xarray",
-    how_label: T.Union[str, None] = None,
+    how_label: str | None = None,
     squeeze: bool = True,
     mask_kwargs: T.Dict[str, T.Any] = {},
     return_geometry_as_coord: bool = False,
     **reduce_kwargs,
 ):
     """
     Reduce an xarray.DataArray object over it's geospatial dimensions using the specified 'how' method.
```

### Comparing `earthkit-aggregate-0.1.4/earthkit/aggregate/tools.py` & `earthkit_aggregate-0.1.5/earthkit/aggregate/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import functools
 import typing as T
+from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 #: Mapping from pandas frequency strings to xarray time groups
 _PANDAS_FREQUENCIES = {
     "D": "dayofyear",
     "W": "weekofyear",
     "M": "month",
+    "ME": "month",
     "H": "hour",
 }
 _PANDAS_FREQUENCIES_R = {v: k for k, v in _PANDAS_FREQUENCIES.items()}
 
 #: The maximum limit of climatology time groups
 _BIN_MAXES = {
     "hour": 24,
@@ -32,18 +34,18 @@
     except AttributeError:
         return [thing]
 
 
 def time_dim_decorator(func):
     @functools.wraps(func)
     def wrapper(
-        dataarray: T.Union[xr.Dataset, xr.DataArray],
+        dataarray: xr.Dataset | xr.DataArray,
         *args,
-        time_dim: T.Union[str, None] = None,
-        time_shift: T.Union[None, dict, str, pd.Timedelta] = None,
+        time_dim: str | None = None,
+        time_shift: dict | str | pd.Timedelta | None = None,
         **kwargs,
     ):
         if time_dim is None:
             try:
                 time_dim = get_dim_key(dataarray, "t")
             except Exception:
                 # Not able to find time dimension in object so let fail its own way
@@ -92,14 +94,33 @@
         if kwargs.get("frequency", "NOTseason") in ["season"]:
             result.reindex(season=["DJF", "MAM", "JJA", "SON"])
         return result
 
     return wrapper
 
 
+def how_label_decorator(label_prefix: str = "", label_suffix: str = ""):
+    def actual_decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, how: str | T.Callable, how_label: str | None = None, **kwargs):
+            if not isinstance(how, str) and not callable(how):
+                raise ValueError("how must be a string or a callable")
+            if how_label is None:
+                if isinstance(how, str):
+                    how_label = deepcopy(how)
+                elif callable(how):
+                    how_label = how.__name__
+                how_label = f"{label_prefix}{how_label}{label_suffix}"
+            return func(*args, how=how, how_label=how_label, **kwargs)
+
+        return wrapper
+
+    return actual_decorator
+
+
 # TODO: Replace with method from meteokit
 def nanaverage(data, weights=None, **kwargs):
     """A merge of the functionality of np.nanmean and np.average.
 
     Parameters
     ----------
     data : numpy array
@@ -263,31 +284,36 @@
 
 def get_how(how: str, how_methods=HOW_METHODS):
     try:
         how = how_methods[how]
     except KeyError:
         try:
             module, function = how.split(".")
+        except Exception:
+            raise ValueError(f"how method not recognised or found: how={how}")
+
+        try:
             how = getattr(globals()[ALLOWED_LIBS[module]], function)
         except KeyError:
             raise ValueError(f"method must come from one of {ALLOWED_LIBS}")
         except AttributeError:
             raise AttributeError(f"module '{module}' has no attribute " f"'{function}'")
+
     return how
 
 
 STANDARD_AXIS_KEYS: dict[str, list[str]] = {
     "y": ["lat", "latitude"],
     "x": ["lon", "long", "longitude"],
     "t": ["time", "valid_time"],
 }
 
 
 def get_dim_key(
-    dataarray: T.Union[xr.DataArray, xr.Dataset],
+    dataarray: xr.Dataset | xr.DataArray,
     axis: str,
 ):
     """Return the key of the dimension."""
     # First check if the axis value is in any dim:
     for dim in dataarray.dims:
         if "axis" in dataarray[dim].attrs and dataarray[dim].attrs["axis"].lower() == axis.lower():
             return dim
@@ -331,7 +357,67 @@
     spatial_info = {
         "lat_key": lat_key,
         "lon_key": lon_key,
         "regular": regular,
         "spatial_dims": spatial_dims,
     }
     return spatial_info
+
+
+def _pandas_frequency_and_bins(
+    frequency: str,
+) -> tuple:
+    freq = frequency.lstrip("0123456789")
+    bins = int(frequency[: -len(freq)]) or None
+    freq = _PANDAS_FREQUENCIES.get(freq.lstrip(" "), frequency)
+    return freq, bins
+
+
+def groupby_time(
+    dataarray: xr.Dataset | xr.DataArray,
+    frequency: str | None = None,
+    bin_widths: int | None = None,
+    squeeze: bool = True,
+    time_dim: str = "time",
+):
+    if frequency is None:
+        try:
+            frequency = xr.infer_freq(dataarray.time)
+        except:  # noqa: E722
+            raise ValueError(
+                "Unable to infer time frequency from data; please pass the 'frequency' argument explicitly"
+            )
+        frequency, possible_bins = _pandas_frequency_and_bins(frequency)
+        bin_widths = bin_widths or possible_bins
+
+    if bin_widths is not None:
+        grouped_data = groupby_bins(dataarray, frequency, bin_widths, squeeze, time_dim=time_dim)
+    else:
+        try:
+            grouped_data = dataarray.groupby(f"{time_dim}.{frequency}", squeeze=squeeze)
+        except AttributeError:
+            raise ValueError(
+                f"Invalid frequency '{frequency}' - see xarray documentation for "
+                f"a full list of valid frequencies."
+            )
+
+    return grouped_data
+
+
+def groupby_bins(
+    dataarray: xr.Dataset | xr.DataArray,
+    frequency: str,
+    bin_widths: int = 1,
+    squeeze: bool = False,
+    time_dim: str = "time",
+):
+    if not isinstance(bin_widths, (list, tuple)):
+        max_value = _BIN_MAXES[frequency]
+        bin_widths = list(range(0, max_value + 1, bin_widths))
+    try:
+        grouped_data = dataarray.groupby_bins(f"{time_dim}.{frequency}", bin_widths, squeeze=squeeze)
+    except AttributeError:
+        raise ValueError(
+            f"Invalid frequency '{frequency}' - see xarray documentation for "
+            f"a full list of valid frequencies."
+        )
+    return grouped_data
```

### Comparing `earthkit-aggregate-0.1.4/earthkit_aggregate.egg-info/PKG-INFO` & `earthkit_aggregate-0.1.5/earthkit_aggregate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-aggregate
-Version: 0.1.4
+Version: 0.1.5
 Summary: Aggregation tools for meteorological and climate data.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `earthkit-aggregate-0.1.4/pyproject.toml` & `earthkit_aggregate-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/tests/test_10_tools.py` & `earthkit_aggregate-0.1.5/tests/test_10_tools.py`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/tests/test_20_general.py` & `earthkit_aggregate-0.1.5/tests/test_20_general.py`

 * *Files identical despite different names*

### Comparing `earthkit-aggregate-0.1.4/tests/test_30_spatial.py` & `earthkit_aggregate-0.1.5/tests/test_30_spatial.py`

 * *Files identical despite different names*

