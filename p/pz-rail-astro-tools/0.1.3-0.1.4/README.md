# Comparing `tmp/pz_rail_astro_tools-0.1.3.tar.gz` & `tmp/pz_rail_astro_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_astro_tools-0.1.3.tar", last modified: Wed Apr 24 01:13:59 2024, max compression
+gzip compressed data, was "pz_rail_astro_tools-0.1.4.tar", last modified: Wed May  8 15:27:25 2024, max compression
```

## Comparing `pz_rail_astro_tools-0.1.3.tar` & `pz_rail_astro_tools-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.994484 pz_rail_astro_tools-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 01:13:58.000000 pz_rail_astro_tools-0.1.3/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.994484 pz_rail_astro_tools-0.1.3/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/photerr_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/photometric_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22176 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/creation/engines/gcr_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.002484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.026484 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/src/rail/tools/util_photometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:58.998484 pz_rail_astro_tools-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/tests/astro_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:13:59.030484 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 01:13:51.000000 pz_rail_astro_tools-0.1.3/tests/astro_tools/test_gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.355141 pz_rail_astro_tools-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:27:24.000000 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.355141 pz_rail_astro_tools-0.1.4/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/photometric_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/engines/gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.387141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/tools/photometry_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/tests/astro_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_gcr_engine.py
```

### Comparing `pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/pull_request_template.md` & `pz_rail_astro_tools-0.1.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/workflows/linting.yml` & `pz_rail_astro_tools-0.1.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_astro_tools-0.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/workflows/smoke-test.yml` & `pz_rail_astro_tools-0.1.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_astro_tools-0.1.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.gitignore` & `pz_rail_astro_tools-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/.pre-commit-config.yaml` & `pz_rail_astro_tools-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/LICENSE` & `pz_rail_astro_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/PKG-INFO` & `pz_rail_astro_tools-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.3
+Version: 0.1.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,15 +61,15 @@
 This package is part of the larger ecosystem of Photometric Redshifts
 in [RAIL](https://github.com/LSSTDESC/RAIL).
 
 ### Citing RAIL
 
 This code, while public on GitHub, has not yet been released by DESC and is
 still under active development. Our release of v1.0 will be accompanied by a
-journal paper describing the development and validation of RAIL.
+journal paper describing the development and validation of RAIL. 
 
 If you make use of the ideas or software in RAIL, please cite the repository 
 <https://github.com/LSSTDESC/RAIL>. You are welcome to re-use the code, which
 is open source and available under terms consistent with the MIT license.
 
 External contributors and DESC members wishing to use RAIL for non-DESC projects
 should consult with the Photometric Redshifts (PZ) Working Group conveners,
```

### Comparing `pz_rail_astro_tools-0.1.3/README.md` & `pz_rail_astro_tools-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 This package is part of the larger ecosystem of Photometric Redshifts
 in [RAIL](https://github.com/LSSTDESC/RAIL).
 
 ### Citing RAIL
 
 This code, while public on GitHub, has not yet been released by DESC and is
 still under active development. Our release of v1.0 will be accompanied by a
-journal paper describing the development and validation of RAIL.
+journal paper describing the development and validation of RAIL. 
 
 If you make use of the ideas or software in RAIL, please cite the repository 
 <https://github.com/LSSTDESC/RAIL>. You are welcome to re-use the code, which
 is open source and available under terms consistent with the MIT license.
 
 External contributors and DESC members wishing to use RAIL for non-DESC projects
 should consult with the Photometric Redshifts (PZ) Working Group conveners,
```

### Comparing `pz_rail_astro_tools-0.1.3/pyproject.toml` & `pz_rail_astro_tools-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.3
+Version: 0.1.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,15 +61,15 @@
 This package is part of the larger ecosystem of Photometric Redshifts
 in [RAIL](https://github.com/LSSTDESC/RAIL).
 
 ### Citing RAIL
 
 This code, while public on GitHub, has not yet been released by DESC and is
 still under active development. Our release of v1.0 will be accompanied by a
-journal paper describing the development and validation of RAIL.
+journal paper describing the development and validation of RAIL. 
 
 If you make use of the ideas or software in RAIL, please cite the repository 
 <https://github.com/LSSTDESC/RAIL>. You are welcome to re-use the code, which
 is open source and available under terms consistent with the MIT license.
 
 External contributors and DESC members wishing to use RAIL for non-DESC projects
 should consult with the Photometric Redshifts (PZ) Working Group conveners,
```

### Comparing `pz_rail_astro_tools-0.1.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,26 @@
 src/pz_rail_astro_tools.egg-info/PKG-INFO
 src/pz_rail_astro_tools.egg-info/SOURCES.txt
 src/pz_rail_astro_tools.egg-info/dependency_links.txt
 src/pz_rail_astro_tools.egg-info/requires.txt
 src/pz_rail_astro_tools.egg-info/top_level.txt
 src/rail/astro_tools/__init__.py
 src/rail/astro_tools/_version.py
-src/rail/creation/degradation/grid_selection.py
-src/rail/creation/degradation/lsst_error_model.py
-src/rail/creation/degradation/observing_condition_degrader.py
-src/rail/creation/degradation/photerr_demo.ipynb
-src/rail/creation/degradation/photometric_errors.py
-src/rail/creation/degradation/spectroscopic_degraders.py
-src/rail/creation/degradation/spectroscopic_selections.py
+src/rail/creation/degraders/grid_selection.py
+src/rail/creation/degraders/lsst_error_model.py
+src/rail/creation/degraders/observing_condition_degrader.py
+src/rail/creation/degraders/photometric_errors.py
+src/rail/creation/degraders/spectroscopic_degraders.py
+src/rail/creation/degraders/spectroscopic_selections.py
 src/rail/creation/engines/gcr_engine.py
 src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
 src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
 src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-src/rail/tools/util_photometry.py
+src/rail/tools/photometry_tools.py
 tests/astro_tools/test_core.py
 tests/astro_tools/test_degraders.py
 tests/astro_tools/test_gcr_engine.py
 tests/astro_tools/gcr_test_data/schema.yaml
 tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
```

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/grid_selection.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/grid_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import numpy as np
 import pandas as pd
 import pickle
 import tables_io
 from rail.creation.selector import Selector
-from rail.core.utils import find_rail_file
+from rail.utils.path_utils import find_rail_file
 from ceci.config import StageParameter as Param
 
 
 class GridSelection(Selector):
     """
     Uses the ratio of HSC spectroscpic galaxies to photometric galaxies to portion a sample
     into training and application samples. Option to implement a color-based redshift cut off in each pixel.
```

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/lsst_error_model.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/observing_condition_degrader.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/observing_condition_degrader.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/photometric_errors.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/photometric_errors.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_degraders.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/degradation/spectroscopic_selections.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_selections.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.creation.selector import Selector
 from scipy.interpolate import interp1d
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 
 
 class SpecSelection(Selector):
     """The super class of spectroscopic selections.
 
     Parameters
     ----------
```

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/creation/engines/gcr_engine.py` & `pz_rail_astro_tools-0.1.4/src/rail/creation/engines/gcr_engine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/src/rail/tools/util_photometry.py` & `pz_rail_astro_tools-0.1.4/src/rail/tools/photometry_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,23 +64,23 @@
     flux_error : array-like
         Flux error value(s).
     """
     flux_error = magnitude_error / hyperbolic.pogson * flux
     return flux_error
 
 
-class PhotormetryManipulator(RailStage, ABC):
+class PhotometryManipulator(RailStage, ABC):
     """
     Base class to perform opertations on magnitudes. A table with input magnitudes and errors is
     processed and transformed into an output table with new magnitudes and errors.
 
     Subclasses must implement the run() and compute() method.
     """
 
-    name = 'PhotormetryManipulator'
+    name = 'PhotometryManipulator'
     config_options = RailStage.config_options.copy()
     config_options.update(
         value_columns=Param(
             list, default=DEFAULT_MAG_COLS,
             msg="list of columns that prove photometric measurements (fluxes or magnitudes)"),
         error_columns=Param(
             list, default=DEFAULT_MAGERR_COLS,
@@ -167,23 +167,23 @@
         """
         self.set_data('input', data)
         self.run()
         self.finalize()
         return self.get_handle('output')
 
 
-class HyperbolicSmoothing(PhotormetryManipulator):
+class HyperbolicSmoothing(PhotometryManipulator):
     """
     Initial stage to compute hyperbolic magnitudes (Lupton et al. 1999). Estimates the smoothing
     parameter b that is used by the second stage (`HyperbolicMagnitudes`) to convert classical to
     hyperbolic magnitudes.
     """
 
     name = 'HyperbolicSmoothing'
-    config_options = PhotormetryManipulator.config_options.copy()
+    config_options = PhotometryManipulator.config_options.copy()
     inputs = [('input', PqHandle)]
     outputs = [('parameters', PqHandle)]
 
     def run(self):
         """
         Computes the smoothing parameter b (see Lupton et al. 1999) per photometric band.
         """
@@ -236,23 +236,23 @@
         """
         self.set_data('input', data)
         self.run()
         self.finalize()
         return self.get_handle('parameters')
 
 
-class HyperbolicMagnitudes(PhotormetryManipulator):
+class HyperbolicMagnitudes(PhotometryManipulator):
     """
     Convert a set of classical magnitudes to hyperbolic magnitudes  (Lupton et al. 1999). Requires
     input from the initial stage (`HyperbolicSmoothing`) to supply optimal values for the smoothing
     parameters (b).
     """
 
     name = 'HyperbolicMagnitudes'
-    config_options = PhotormetryManipulator.config_options.copy()
+    config_options = PhotometryManipulator.config_options.copy()
     inputs = [('input', PqHandle),
               ('parameters', PqHandle)]
     outputs = [('output', PqHandle)]
 
     def _check_filters(self, stats_table):
         """
         Check whether the column definition matches the loaded smoothing parameters.
```

### Comparing `pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/schema.yaml` & `pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/schema.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5` & `pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_core.py` & `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     Hdf5Handle,
     ModelHandle,
     PqHandle,
     QPHandle,
     TableHandle,
 )
 from rail.core.stage import RailStage
-from rail.tools.util_photometry import HyperbolicMagnitudes, HyperbolicSmoothing, PhotormetryManipulator, LSSTFluxToMagConverter, Dereddener
-from rail.core.utils import RAILDIR
+from rail.tools.photometry_tools import HyperbolicMagnitudes, HyperbolicSmoothing, PhotometryManipulator, LSSTFluxToMagConverter, Dereddener
+from rail.utils.path_utils import RAILDIR
 #from rail.tools.util_stages import (
 #    LSSTFluxToMagConverter,
 #    Dereddener,
 #)
 
 
 # def test_data_file():
@@ -94,46 +94,46 @@
     testFile = os.path.join(
         RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816_smoothing_params.pq"
     )
 
     return DS.read_file("test_data", TableHandle, testFile).data
 
 
-def test_PhotormetryManipulator(hyperbolic_configuration):
+def test_PhotometryManipulator(hyperbolic_configuration):
     DS = RailStage.data_store
     DS.clear()
     DS.__class__.allow_overwrite = False
 
-    # NOTE: the __init__ machinery of HyperbolicSmoothing is identical to PhotormetryManipulator
-    # and is used as substitute since PhotormetryManipulator cannot be instantiated.
+    # NOTE: the __init__ machinery of HyperbolicSmoothing is identical to PhotometryManipulator
+    # and is used as substitute since PhotometryManipulator cannot be instantiated.
     n_filters = len(hyperbolic_configuration["value_columns"])
 
     # wrong number of "error_columns"
     config = hyperbolic_configuration.copy()
     config["error_columns"] = hyperbolic_configuration["error_columns"][:-1]
     with pytest.raises(IndexError):
-        inst = HyperbolicSmoothing.make_stage(name="photormetry_manipulator", **config)
+        inst = HyperbolicSmoothing.make_stage(name="photometry_manipulator", **config)
 
     # wrong number of "zeropoints"
     config = hyperbolic_configuration.copy()
     config["zeropoints"] = np.arange(0, n_filters - 1)
     with pytest.raises(IndexError):
-        inst = HyperbolicSmoothing.make_stage(name="photormetry_manipulator", **config)
+        inst = HyperbolicSmoothing.make_stage(name="photometry_manipulator", **config)
 
     # default values for "zeropoints"
     config = hyperbolic_configuration.copy()
     config.pop("zeropoints")  # should resort to default of 0.0
-    inst = HyperbolicSmoothing.make_stage(name="photormetry_manipulator", **config)
+    inst = HyperbolicSmoothing.make_stage(name="photometry_manipulator", **config)
     assert len(inst.zeropoints) == n_filters
     assert all(zp == 0.0 for zp in inst.zeropoints)
 
     # if_flux preserves the values
     dummy_data = pd.DataFrame(dict(val=[1, 2, 3], err=[1, 2, 3]))
     config = dict(value_columns=["val"], error_columns=["err"], zeropoints=[0.0])
-    inst = HyperbolicSmoothing.make_stage(name="photormetry_manipulator", **config, is_flux=True)
+    inst = HyperbolicSmoothing.make_stage(name="photometry_manipulator", **config, is_flux=True)
     inst.set_data("input", dummy_data)
     data = inst.get_as_fluxes()
     assert np.allclose(data, dummy_data)
 
 
 def test_HyperbolicSmoothing(hyperbolic_configuration):
     DS = RailStage.data_store
```

### Comparing `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_degraders.py` & `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_degraders.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from photerr import LsstErrorModel as PhoterrErrorModel
 
 from rail.core.data import DATA_STORE, TableHandle
-from rail.core.utils import find_rail_file
-from rail.core.util_stages import ColumnMapper
-from rail.creation.degradation.spectroscopic_degraders import InvRedshiftIncompleteness, LineConfusion
-from rail.creation.degradation.spectroscopic_selections import *
-from rail.creation.degradation.observing_condition_degrader import ObsCondition
-from rail.creation.degradation.grid_selection import GridSelection
-from rail.creation.degradation.lsst_error_model import LSSTErrorModel
+from rail.utils.path_utils import find_rail_file
+from rail.tools.table_tools import ColumnMapper
+from rail.creation.degraders.spectroscopic_degraders import InvRedshiftIncompleteness, LineConfusion
+from rail.creation.degraders.spectroscopic_selections import *
+from rail.creation.degraders.observing_condition_degrader import ObsCondition
+from rail.creation.degraders.grid_selection import GridSelection
+from rail.creation.degraders.lsst_error_model import LSSTErrorModel
 
 
 @pytest.fixture
 def data():
     """Some dummy data to use below."""
 
     DS = DATA_STORE()
```

### Comparing `pz_rail_astro_tools-0.1.3/tests/astro_tools/test_gcr_engine.py` & `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_gcr_engine.py`

 * *Files identical despite different names*

