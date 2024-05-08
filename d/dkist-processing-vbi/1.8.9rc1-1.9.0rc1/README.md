# Comparing `tmp/dkist_processing_vbi-1.8.9rc1.tar.gz` & `tmp/dkist_processing_vbi-1.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.8.9rc1.tar", last modified: Wed May  1 19:59:46 2024, max compression
+gzip compressed data, was "dkist_processing_vbi-1.9.0rc1.tar", last modified: Wed May  8 02:03:52 2024, max compression
```

## Comparing `dkist_processing_vbi-1.8.9rc1.tar` & `dkist_processing_vbi-1.9.0rc1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    17079 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5696 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     5465 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.464468 dkist_processing_vbi-1.8.9rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/changelog/73.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.464468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.464468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.464468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7036 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/mosaic_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6404 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    14101 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2301 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5873 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5477 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9879 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11437 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    13130 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6828 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     7374 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2698 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.464468 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-01 19:59:46.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-01 19:59:46.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 19:59:46.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-05-01 19:59:46.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-01 19:59:46.000000 dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 19:59:46.468468 dkist_processing_vbi-1.8.9rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1801 2024-05-01 19:59:46.472468 dkist_processing_vbi-1.8.9rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-01 19:59:40.000000 dkist_processing_vbi-1.8.9rc1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    17271 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5465 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/changelog/72.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7036 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/mosaic_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6404 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    14101 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5873 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5477 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9879 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9275 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     7374 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2024-05-08 02:03:52.232695 dkist_processing_vbi-1.9.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/towncrier_science.toml
```

### Comparing `dkist_processing_vbi-1.8.9rc1/.gitignore` & `dkist_processing_vbi-1.9.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/.pre-commit-config.yaml` & `dkist_processing_vbi-1.9.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/CHANGELOG.rst` & `dkist_processing_vbi-1.9.0rc1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.8.9 (2024-05-02)
+===================
+
+Misc
+----
+
+- Rename non-FITS L1 products to better manage namespace. (`#73 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/73>`__)
+
+
 v1.8.8 (2024-04-12)
 ===================
 
 Misc
 ----
 
 - Populate the value of MANPROCD in the L1 headers with a boolean indicating whether there were manual steps involved in the frames production. (`#71 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/71>`__)
```

### Comparing `dkist_processing_vbi-1.8.9rc1/PKG-INFO` & `dkist_processing_vbi-1.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.8.9rc1
+Version: 1.9.0rc1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: inventory
 Provides-Extra: asdf
+Provides-Extra: quality
 Provides-Extra: grogu
 Provides-Extra: docs
 
 dkist-processing-vbi
 ====================
 
 Overview
```

### Comparing `dkist_processing_vbi-1.8.9rc1/README.rst` & `dkist_processing_vbi-1.9.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.9.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/check_changelog_updated.sh` & `dkist_processing_vbi-1.9.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/filter.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/filter.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/mosaic_repeats.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/mosaic_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """VBI parse task."""
 from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 from dkist_processing_common.parsers.time import ExposureTimeFlower
+from dkist_processing_common.parsers.time import ObsIpStartTimeBud
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 from dkist_processing_common.tasks import ParseL0InputDataBase
 from dkist_processing_common.tasks.parse_l0_input_data import S
 
 from dkist_processing_vbi.models.constants import VbiBudName
 from dkist_processing_vbi.models.tags import VbiStemName
@@ -47,14 +48,15 @@
         """VBI specific constants to append to the common constants."""
         return super().constant_buds + [
             UniqueBud(
                 constant_name=VbiBudName.num_spatial_steps.value,
                 metadata_key="number_of_spatial_steps",
             ),
             SpatialStepPatternBud(),
+            ObsIpStartTimeBud(),
             TotalMosaicRepeatsBud(),
             TaskExposureTimesBud(
                 VbiBudName.gain_exposure_times.value, ip_task_type=TaskName.gain.value
             ),
             TaskExposureTimesBud(
                 VbiBudName.observe_exposure_times.value, ip_task_type=TaskName.observe.value
             ),
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/process_summit_processed.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/quality_metrics.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import chain
 
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.codecs.fits import fits_hdulist_encoder
+from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_vbi.models.constants import VbiBudName
 from dkist_processing_vbi.models.tags import VbiTag
 from dkist_processing_vbi.tasks.parse import ParseL0VbiInputData
 from dkist_processing_vbi.tests.conftest import generate_214_l0_fits_frame
 from dkist_processing_vbi.tests.conftest import Vbi122DarkFrames
@@ -221,14 +222,15 @@
         == parse_inputs_task.num_steps
     )
     assert (
         parse_inputs_task.constants._db_dict[VbiBudName.num_mosaics_repeats.value]
         == parse_inputs_task.test_num_mosaic_repeats
     )
     assert parse_inputs_task.constants._db_dict[VbiBudName.spatial_step_pattern.value] == "1,2,4,3"
+    assert BudName.obs_ip_start_time.value in parse_inputs_task.constants._db_dict
 
 
 def test_parse_l0_input_frames_found(parse_inputs_task, mocker):
     """
     Given: a set of raw inputs of multiple task types and a ParseL0VbiInputData task
     When: the task is run
     Then: the frames from each task type are correctly identified and tagged
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_parse_summit.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 DKIST: https://nso.edu/telescopes/dki-solar-telescope/
 
 VBI: https://nso.edu/telescopes/dkist/instruments/vbi/
 
 This workflow does *not* include the speckle reconstruction algorithms used in summit-calibrated data.
 Instead, darks and gains are generated by averaging the raw darks and gains, and are then subtracted from the science frames.
 """
-from dkist_processing_common.tasks import AddDatasetReceiptAccount
+from dkist_processing_common.tasks import AssembleQualityData
 from dkist_processing_common.tasks import PublishCatalogAndQualityMessages
 from dkist_processing_common.tasks import QualityL1Metrics
-from dkist_processing_common.tasks import SubmitQuality
+from dkist_processing_common.tasks import SubmitDatasetMetadata
 from dkist_processing_common.tasks import Teardown
 from dkist_processing_common.tasks import TransferL0Data
 from dkist_processing_common.tasks import TransferL1Data
 from dkist_processing_core import Workflow
 
 from dkist_processing_vbi.tasks import AssembleVbiMovie
 from dkist_processing_vbi.tasks import DarkCalibration
@@ -45,16 +45,16 @@
 l0_pipeline.add_node(task=ScienceCalibration, upstreams=GainCalibration)
 l0_pipeline.add_node(task=VbiWriteL1Frame, upstreams=ScienceCalibration)
 l0_pipeline.add_node(task=MakeVbiMovieFrames, upstreams=VbiWriteL1Frame)
 l0_pipeline.add_node(task=AssembleVbiMovie, upstreams=MakeVbiMovieFrames)
 l0_pipeline.add_node(task=QualityL1Metrics, upstreams=VbiWriteL1Frame)
 l0_pipeline.add_node(task=VbiQualityL1Metrics, upstreams=VbiWriteL1Frame)
 l0_pipeline.add_node(
-    task=SubmitQuality, upstreams=[VbiQualityL0Metrics, QualityL1Metrics, VbiQualityL1Metrics]
+    task=AssembleQualityData, upstreams=[VbiQualityL0Metrics, QualityL1Metrics, VbiQualityL1Metrics]
 )
-l0_pipeline.add_node(task=AddDatasetReceiptAccount, upstreams=[AssembleVbiMovie, SubmitQuality])
-l0_pipeline.add_node(task=TransferL1Data, upstreams=AddDatasetReceiptAccount)
+l0_pipeline.add_node(task=SubmitDatasetMetadata, upstreams=[AssembleVbiMovie, AssembleQualityData])
+l0_pipeline.add_node(task=TransferL1Data, upstreams=SubmitDatasetMetadata)
 l0_pipeline.add_node(
     task=PublishCatalogAndQualityMessages,
     upstreams=TransferL1Data,
 )
 l0_pipeline.add_node(task=Teardown, upstreams=PublishCatalogAndQualityMessages)
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 This workflow is used when VBI data was processed on the DKIST summit.
 In this case it is then transferred to the DKIST Data Center for packaging, but no further calibrations are applied.
 
 To determine the type of calibrations applied, please inspect the `VBI__005` keyword in the FITS headers.
 It will indicate whether frame selection, speckle imaging, or other calibration algorithms were applied.
 """
-from dkist_processing_common.tasks import AddDatasetReceiptAccount
+from dkist_processing_common.tasks import AssembleQualityData
 from dkist_processing_common.tasks import PublishCatalogAndQualityMessages
 from dkist_processing_common.tasks import QualityL1Metrics
-from dkist_processing_common.tasks import SubmitQuality
+from dkist_processing_common.tasks import SubmitDatasetMetadata
 from dkist_processing_common.tasks import Teardown
 from dkist_processing_common.tasks import TransferL0Data
 from dkist_processing_common.tasks import TransferL1Data
 from dkist_processing_core import Workflow
 
 from dkist_processing_vbi.tasks import AssembleVbiMovie
 from dkist_processing_vbi.tasks import GenerateL1SummitData
@@ -38,18 +38,18 @@
 summit_processed_data.add_node(task=GenerateL1SummitData, upstreams=ParseL0VbiInputData)
 summit_processed_data.add_node(task=VbiWriteL1Frame, upstreams=GenerateL1SummitData)
 summit_processed_data.add_node(task=MakeVbiMovieFrames, upstreams=VbiWriteL1Frame)
 summit_processed_data.add_node(task=AssembleVbiMovie, upstreams=MakeVbiMovieFrames)
 summit_processed_data.add_node(task=VbiQualityL1Metrics, upstreams=VbiWriteL1Frame)
 summit_processed_data.add_node(task=QualityL1Metrics, upstreams=VbiWriteL1Frame)
 summit_processed_data.add_node(
-    task=SubmitQuality, upstreams=[VbiQualityL1Metrics, QualityL1Metrics]
+    task=AssembleQualityData, upstreams=[VbiQualityL1Metrics, QualityL1Metrics]
 )
 summit_processed_data.add_node(
-    task=AddDatasetReceiptAccount, upstreams=[AssembleVbiMovie, SubmitQuality]
+    task=SubmitDatasetMetadata, upstreams=[AssembleVbiMovie, AssembleQualityData]
 )
-summit_processed_data.add_node(task=TransferL1Data, upstreams=AddDatasetReceiptAccount)
+summit_processed_data.add_node(task=TransferL1Data, upstreams=SubmitDatasetMetadata)
 summit_processed_data.add_node(
     task=PublishCatalogAndQualityMessages,
     upstreams=TransferL1Data,
 )
 summit_processed_data.add_node(task=Teardown, upstreams=PublishCatalogAndQualityMessages)
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.8.9rc1
+Version: 1.9.0rc1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: inventory
 Provides-Extra: asdf
+Provides-Extra: quality
 Provides-Extra: grogu
 Provides-Extra: docs
 
 dkist-processing-vbi
 ====================
 
 Overview
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
-changelog/73.misc.rst
+changelog/72.feature.rst
 dkist_processing_vbi/__init__.py
 dkist_processing_vbi.egg-info/PKG-INFO
 dkist_processing_vbi.egg-info/SOURCES.txt
 dkist_processing_vbi.egg-info/dependency_links.txt
 dkist_processing_vbi.egg-info/requires.txt
 dkist_processing_vbi.egg-info/top_level.txt
 dkist_processing_vbi/models/__init__.py
```

### Comparing `dkist_processing_vbi-1.8.9rc1/dkist_processing_vbi.egg-info/requires.txt` & `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==6.2.1
+dkist-processing-common==6.2.2
 dkist-processing-math==2.1.0
 dkist-header-validator==5.1.0
 dkist-fits-specifications==4.1.1
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
 scipy==1.11.0
@@ -29,18 +29,22 @@
 pyparsing
 dkist-inventory>=1.3.1
 
 [inventory]
 dkist-processing-common[inventory]
 dkist-inventory==1.3.1
 
+[quality]
+dkist-quality==1.0.1
+
 [test]
 pytest
 pytest-cov
 pytest-mock
 pytest-xdist
 towncrier
 dkist-data-simulator>=5.1.1
 dkist-processing-common[inventory]
 dkist-inventory==1.3.1
 dkist-processing-common[asdf]
 dkist-inventory[asdf]==1.3.1
+dkist-quality==1.0.1
```

### Comparing `dkist_processing_vbi-1.8.9rc1/docs/Makefile` & `dkist_processing_vbi-1.9.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/docs/conf.py` & `dkist_processing_vbi-1.9.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/docs/make.bat` & `dkist_processing_vbi-1.9.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/licenses/LICENSE.rst` & `dkist_processing_vbi-1.9.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/pyproject.toml` & `dkist_processing_vbi-1.9.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.8.9rc1/setup.cfg` & `dkist_processing_vbi-1.9.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 6.2.1
+	dkist-processing-common == 6.2.2
 	dkist-processing-math == 2.1.0
 	dkist-header-validator == 5.1.0
 	dkist-fits-specifications == 4.1.1
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
 	scipy == 1.11.0
@@ -38,20 +38,23 @@
 	pytest-cov
 	pytest-mock
 	pytest-xdist
 	towncrier
 	dkist-data-simulator >= 5.1.1
 	%(inventory)s  # identify pip conflicts in test
 	%(asdf)s  # identify pip conflicts in test
+	%(quality)s  # identify pip conflicts in test
 inventory = 
 	dkist-processing-common[inventory]
 	dkist-inventory==1.3.1
 asdf = 
 	dkist-processing-common[asdf]
 	dkist-inventory[asdf]==1.3.1
+quality = 
+	dkist-quality==1.0.1
 grogu = 
 	dkist
 	pyparsing
 	dkist-inventory >= 1.3.1
 docs = 
 	sphinx
 	sphinx-astropy
```

