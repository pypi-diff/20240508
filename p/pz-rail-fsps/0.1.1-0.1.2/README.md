# Comparing `tmp/pz-rail-fsps-0.1.1.tar.gz` & `tmp/pz_rail_fsps-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-fsps-0.1.1.tar", last modified: Wed Nov  1 18:53:44 2023, max compression
+gzip compressed data, was "pz_rail_fsps-0.1.2.tar", last modified: Wed May  8 17:47:10 2024, max compression
```

## Comparing `pz-rail-fsps-0.1.1.tar` & `pz_rail_fsps-0.1.2.tar`

### file list

```diff
@@ -1,73 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.063518 pz-rail-fsps-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-11-01 18:53:44.063518 pz-rail-fsps-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    21010 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/examples/creation_examples/fsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 18:53:44.063518 pz-rail-fsps-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-11-01 18:53:44.000000 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-11-01 18:53:44.000000 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 18:53:44.000000 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-01 18:53:44.000000 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-01 18:53:44.000000 pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.055518 pz-rail-fsps-0.1.1/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/creation/engines/fsps_photometry_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    39884 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/creation/engines/fsps_sed_modeler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.059518 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.059518 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)    14608 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)    15568 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_u_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)    17296 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_y_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/mzls_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_b_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_v_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (127)   353648 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/input_galaxy_properties_fsps.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/lsf_bad_wave_array.dat
--rw-r--r--   0 runner    (1001) docker     (127)   703248 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/model_FSPSSedModeler.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/rail_fsps_test_sfh.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/sfh_bad_age_array.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/test_fsps_sed.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.059518 pz-rail-fsps-0.1.1/src/rail/fsps/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/src/rail/fsps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-01 18:53:43.000000 pz-rail-fsps-0.1.1/src/rail/fsps/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.051518 pz-rail-fsps-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 18:53:44.063518 pz-rail-fsps-0.1.1/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2023-11-01 18:53:29.000000 pz-rail-fsps-0.1.1/tests/creation/test_fsps_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.703823 pz_rail_fsps-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.703823 pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.703823 pz_rail_fsps-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.707823 pz_rail_fsps-0.1.2/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/creation/engines/fsps_photometry_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39884 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/creation/engines/fsps_sed_modeler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.707823 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_u_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    17296 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_y_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/mzls_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_b_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_v_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (127)   353648 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/input_galaxy_properties_fsps.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/lsf_bad_wave_array.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   703248 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/model_FSPSSedModeler.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/rail_fsps_test_sfh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/sfh_bad_age_array.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/test_fsps_sed.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/src/rail/fsps/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/src/rail/fsps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 17:47:10.000000 pz_rail_fsps-0.1.2/src/rail/fsps/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.699823 pz_rail_fsps-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:47:10.711823 pz_rail_fsps-0.1.2/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-05-08 17:47:03.000000 pz_rail_fsps-0.1.2/tests/creation/test_fsps_interface.py
```

### Comparing `pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_fsps-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/pull_request_template.md` & `pz_rail_fsps-0.1.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/workflows/build_documentation.yml` & `pz_rail_fsps-0.1.2/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/workflows/linting.yml` & `pz_rail_fsps-0.1.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_fsps-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/workflows/smoke-test.yml` & `pz_rail_fsps-0.1.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_fsps-0.1.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.gitignore` & `pz_rail_fsps-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.pre-commit-config.yaml` & `pz_rail_fsps-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/.prepare_project.sh` & `pz_rail_fsps-0.1.2/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/LICENSE` & `pz_rail_fsps-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/PKG-INFO` & `pz_rail_fsps-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-fsps
-Version: 0.1.1
+Version: 0.1.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-fsps-0.1.1/README.md` & `pz_rail_fsps-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/pyproject.toml` & `pz_rail_fsps-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/PKG-INFO` & `pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-fsps
-Version: 0.1.1
+Version: 0.1.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-fsps-0.1.1/src/pz_rail_fsps.egg-info/SOURCES.txt` & `pz_rail_fsps-0.1.2/src/pz_rail_fsps.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 .github/ISSUE_TEMPLATE/2-feature_request.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/build_documentation.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
-examples/creation_examples/fsps_sed_demo.ipynb
 src/pz_rail_fsps.egg-info/PKG-INFO
 src/pz_rail_fsps.egg-info/SOURCES.txt
 src/pz_rail_fsps.egg-info/dependency_links.txt
 src/pz_rail_fsps.egg-info/requires.txt
 src/pz_rail_fsps.egg-info/top_level.txt
 src/rail/creation/engines/fsps_photometry_creator.py
 src/rail/creation/engines/fsps_sed_modeler.py
```

### Comparing `pz-rail-fsps-0.1.1/src/rail/creation/engines/fsps_photometry_creator.py` & `pz_rail_fsps-0.1.2/src/rail/creation/engines/fsps_photometry_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rail.creation.engine import Creator
 from rail.core.stage import RailStage
 from rail.core.data import Hdf5Handle
 from ceci.config import StageParameter as Param
 import numpy as np
-from rail.core.utils import find_rail_file
+from rail.utils.path_utils import find_rail_file
 from astropy.cosmology import Planck15, w0waCDM
 from scipy import interpolate
 import os
 import h5py
 
 
 class FSPSPhotometryCreator(Creator):
```

### Comparing `pz-rail-fsps-0.1.1/src/rail/creation/engines/fsps_sed_modeler.py` & `pz_rail_fsps-0.1.2/src/rail/creation/engines/fsps_sed_modeler.py`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_g_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_r_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/bass_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_g_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_i_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_r_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_u_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_u_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_y_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_y_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_z_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/lsst_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/mzls_z_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/mzls_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_b_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_b_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_g_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_i_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_r_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_v_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_v_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_z_transmission.h5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/filters/suprimecam_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/input_galaxy_properties_fsps.hdf5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/input_galaxy_properties_fsps.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/model_FSPSSedModeler.hdf5` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/model_FSPSSedModeler.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/rail_fsps_test_sfh.txt` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/rail_fsps_test_sfh.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/src/rail/examples_data/creation_data/data/fsps_default_data/test_fsps_sed.fits` & `pz_rail_fsps-0.1.2/src/rail/examples_data/creation_data/data/fsps_default_data/test_fsps_sed.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-fsps-0.1.1/tests/creation/test_fsps_interface.py` & `pz_rail_fsps-0.1.2/tests/creation/test_fsps_interface.py`

 * *Files identical despite different names*

