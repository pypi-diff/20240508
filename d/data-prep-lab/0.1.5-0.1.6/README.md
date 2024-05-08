# Comparing `tmp/data_prep_lab-0.1.5.tar.gz` & `tmp/data_prep_lab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab-0.1.5.tar", last modified: Sat Apr 27 18:04:13 2024, max compression
+gzip compressed data, was "data_prep_lab-0.1.6.tar", last modified: Wed May  8 18:24:06 2024, max compression
```

## Comparing `data_prep_lab-0.1.5.tar` & `data_prep_lab-0.1.6.tar`

### file list

```diff
@@ -1,100 +1,115 @@
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.182617 data_prep_lab-0.1.5/
--rw-r--r--   0 boris      (501) staff       (20)      357 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/.gitignore
--rw-r--r--   0 boris      (501) staff       (20)     2287 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/Makefile
--rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-27 18:04:13.181410 data_prep_lab-0.1.5/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)      963 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.147023 data_prep_lab-0.1.5/doc/
--rw-r--r--   0 boris      (501) staff       (20)    12742 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/advanced-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)     7617 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/architecture.md
--rw-r--r--   0 boris      (501) staff       (20)     4940 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/launcher-options.md
--rw-r--r--   0 boris      (501) staff       (20)     1562 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/overview.md
--rw-r--r--   0 boris      (501) staff       (20)   137580 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/processing-architecture.jpg
--rw-r--r--   0 boris      (501) staff       (20)     8678 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/simplest-transform-tutorial.md
--rw-r--r--   0 boris      (501) staff       (20)      193 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/testing-e2e-transform.md
--rw-r--r--   0 boris      (501) staff       (20)     5888 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/testing-transforms.md
--rw-r--r--   0 boris      (501) staff       (20)    12175 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/transform-external-resources.md
--rw-r--r--   0 boris      (501) staff       (20)     3666 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/transform-porting.md
--rw-r--r--   0 boris      (501) staff       (20)    10818 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/transform-tutorials.md
--rw-r--r--   0 boris      (501) staff       (20)     1415 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/doc/transformer-utilities.md
--rw-r--r--   0 boris      (501) staff       (20)     3614 2024-04-26 07:07:23.000000 data_prep_lab-0.1.5/doc/using_s3_transformers.md
--rw-r--r--   0 boris      (501) staff       (20)      455 2024-04-27 17:55:40.000000 data_prep_lab-0.1.5/mkdocs.yml
--rw-r--r--   0 boris      (501) staff       (20)     1327 2024-04-27 18:02:55.000000 data_prep_lab-0.1.5/pyproject.toml
--rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-27 18:04:13.182822 data_prep_lab-0.1.5/setup.cfg
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.125020 data_prep_lab-0.1.5/src/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.177785 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/
--rw-r--r--   0 boris      (501) staff       (20)     1879 2024-04-27 18:04:12.000000 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     3020 2024-04-27 18:04:13.000000 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/SOURCES.txt
--rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-27 18:04:12.000000 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/dependency_links.txt
--rw-r--r--   0 boris      (501) staff       (20)      249 2024-04-27 18:04:12.000000 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/requires.txt
--rw-r--r--   0 boris      (501) staff       (20)       16 2024-04-27 18:04:12.000000 data_prep_lab-0.1.5/src/data_prep_lab.egg-info/top_level.txt
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.127817 data_prep_lab-0.1.5/src/data_processing/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.152716 data_prep_lab-0.1.5/src/data_processing/data_access/
--rw-r--r--   0 boris      (501) staff       (20)      427 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8830 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 boris      (501) staff       (20)     8484 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/data_access.py
--rw-r--r--   0 boris      (501) staff       (20)    11316 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 boris      (501) staff       (20)     5647 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 boris      (501) staff       (20)    15024 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 boris      (501) staff       (20)    13499 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.156360 data_prep_lab-0.1.5/src/data_processing/ray/
--rw-r--r--   0 boris      (501) staff       (20)      574 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     7404 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/ray_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     4760 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_launcher.py
--rw-r--r--   0 boris      (501) staff       (20)     6388 2024-04-27 17:55:40.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_orchestrator.py
--rw-r--r--   0 boris      (501) staff       (20)     5210 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_orchestrator_configuration.py
--rw-r--r--   0 boris      (501) staff       (20)     7261 2024-04-27 17:55:40.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_runtime.py
--rw-r--r--   0 boris      (501) staff       (20)     3073 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_statistics.py
--rw-r--r--   0 boris      (501) staff       (20)     9498 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/ray/transform_table_processor.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.157190 data_prep_lab-0.1.5/src/data_processing/test_support/
--rw-r--r--   0 boris      (501) staff       (20)       62 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     8234 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.157974 data_prep_lab-0.1.5/src/data_processing/test_support/ray/
--rw-r--r--   0 boris      (501) staff       (20)       58 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/ray/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4686 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/ray/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.159479 data_prep_lab-0.1.5/src/data_processing/test_support/transform/
--rw-r--r--   0 boris      (501) staff       (20)      120 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4050 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 boris      (501) staff       (20)     4476 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.160389 data_prep_lab-0.1.5/src/data_processing/transform/
--rw-r--r--   0 boris      (501) staff       (20)       77 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/transform/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     2298 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/transform/table_transform.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.163400 data_prep_lab-0.1.5/src/data_processing/utils/
--rw-r--r--   0 boris      (501) staff       (20)      354 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     3135 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     1695 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/config.py
--rw-r--r--   0 boris      (501) staff       (20)     2052 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/log.py
--rw-r--r--   0 boris      (501) staff       (20)     6029 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/params_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     6740 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.131861 data_prep_lab-0.1.5/test/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.132700 data_prep_lab-0.1.5/test/data_processing_tests/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.172396 data_prep_lab-0.1.5/test/data_processing_tests/data_access/
--rw-r--r--   0 boris      (501) staff       (20)    24548 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 boris      (501) staff       (20)     5734 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1545 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.174622 data_prep_lab-0.1.5/test/data_processing_tests/ray/
--rw-r--r--   0 boris      (501) staff       (20)     9851 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/ray/launcher_test.py
--rw-r--r--   0 boris      (501) staff       (20)     3282 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/ray/ray_util_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1685 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/ray/test_noop_launch.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.175400 data_prep_lab-0.1.5/test/data_processing_tests/transform/
--rw-r--r--   0 boris      (501) staff       (20)     1678 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.176116 data_prep_lab-0.1.5/test/data_processing_tests/util/
--rw-r--r--   0 boris      (501) staff       (20)     1386 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.128572 data_prep_lab-0.1.5/test-data/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.129692 data_prep_lab-0.1.5/test-data/data_processing/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.164196 data_prep_lab-0.1.5/test-data/data_processing/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.166039 data_prep_lab-0.1.5/test-data/data_processing/input_multiple/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.129980 data_prep_lab-0.1.5/test-data/data_processing/ray/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.131028 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.167758 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 boris      (501) staff       (20)     1128 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.168568 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.169218 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 boris      (501) staff       (20)    36132 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:04:13.170050 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 boris      (501) staff       (20)      753 2024-04-25 06:38:08.000000 data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.241081 data_prep_lab-0.1.6/
+-rw-r--r--   0 dawood     (501) staff       (20)      357 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/.gitignore
+-rw-r--r--   0 dawood     (501) staff       (20)     2287 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/Makefile
+-rw-r--r--   0 dawood     (501) staff       (20)     1879 2024-05-08 18:24:06.240804 data_prep_lab-0.1.6/PKG-INFO
+-rw-r--r--   0 dawood     (501) staff       (20)      963 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/README.md
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.215517 data_prep_lab-0.1.6/doc/
+-rw-r--r--   0 dawood     (501) staff       (20)    12805 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/advanced-transform-tutorial.md
+-rw-r--r--   0 dawood     (501) staff       (20)     7617 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/doc/architecture.md
+-rw-r--r--   0 dawood     (501) staff       (20)     5028 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/launcher-options.md
+-rw-r--r--   0 dawood     (501) staff       (20)    34920 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/logo-ibm-dark.png
+-rw-r--r--   0 dawood     (501) staff       (20)    35127 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/logo-ibm.png
+-rw-r--r--   0 dawood     (501) staff       (20)     1564 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/overview.md
+-rw-r--r--   0 dawood     (501) staff       (20)   137580 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/doc/processing-architecture.jpg
+-rw-r--r--   0 dawood     (501) staff       (20)     8860 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/simplest-transform-tutorial.md
+-rw-r--r--   0 dawood     (501) staff       (20)      193 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/doc/testing-e2e-transform.md
+-rw-r--r--   0 dawood     (501) staff       (20)     5888 2024-05-06 21:55:44.000000 data_prep_lab-0.1.6/doc/testing-transforms.md
+-rw-r--r--   0 dawood     (501) staff       (20)    12175 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/doc/transform-external-resources.md
+-rw-r--r--   0 dawood     (501) staff       (20)    10775 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/doc/transform-tutorials.md
+-rw-r--r--   0 dawood     (501) staff       (20)     1415 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/doc/transformer-utilities.md
+-rw-r--r--   0 dawood     (501) staff       (20)     3614 2024-04-26 14:56:16.000000 data_prep_lab-0.1.6/doc/using_s3_transformers.md
+-rw-r--r--   0 dawood     (501) staff       (20)     1327 2024-05-08 18:23:38.000000 data_prep_lab-0.1.6/pyproject.toml
+-rw-r--r--   0 dawood     (501) staff       (20)       38 2024-05-08 18:24:06.241137 data_prep_lab-0.1.6/setup.cfg
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.206938 data_prep_lab-0.1.6/src/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.239699 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/
+-rw-r--r--   0 dawood     (501) staff       (20)     1879 2024-05-08 18:24:06.000000 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/PKG-INFO
+-rw-r--r--   0 dawood     (501) staff       (20)     3467 2024-05-08 18:24:06.000000 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 dawood     (501) staff       (20)        1 2024-05-08 18:24:06.000000 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 dawood     (501) staff       (20)      249 2024-05-08 18:24:06.000000 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/requires.txt
+-rw-r--r--   0 dawood     (501) staff       (20)       16 2024-05-08 18:24:06.000000 data_prep_lab-0.1.6/src/data_prep_lab.egg-info/top_level.txt
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.216461 data_prep_lab-0.1.6/src/data_processing/
+-rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/src/data_processing/__init__.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.218295 data_prep_lab-0.1.6/src/data_processing/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)      427 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8830 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8484 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 dawood     (501) staff       (20)    11462 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 dawood     (501) staff       (20)     5647 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 dawood     (501) staff       (20)    15061 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 dawood     (501) staff       (20)    13499 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.220663 data_prep_lab-0.1.6/src/data_processing/ray/
+-rw-r--r--   0 dawood     (501) staff       (20)      574 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/ray/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     7404 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/ray/ray_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4760 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_launcher.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6388 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_orchestrator.py
+-rw-r--r--   0 dawood     (501) staff       (20)     5210 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_orchestrator_configuration.py
+-rw-r--r--   0 dawood     (501) staff       (20)     7261 2024-05-08 17:02:16.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_runtime.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3073 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_statistics.py
+-rw-r--r--   0 dawood     (501) staff       (20)     9498 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/ray/transform_table_processor.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.221207 data_prep_lab-0.1.6/src/data_processing/test_support/
+-rw-r--r--   0 dawood     (501) staff       (20)       62 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     8234 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.221721 data_prep_lab-0.1.6/src/data_processing/test_support/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)       69 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/src/data_processing/test_support/data_access/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2666 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/src/data_processing/test_support/data_access/data_access_factory_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.222297 data_prep_lab-0.1.6/src/data_processing/test_support/ray/
+-rw-r--r--   0 dawood     (501) staff       (20)       58 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/test_support/ray/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4686 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/test_support/ray/transform_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.223311 data_prep_lab-0.1.6/src/data_processing/test_support/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)      120 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4050 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 dawood     (501) staff       (20)     4476 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.224435 data_prep_lab-0.1.6/src/data_processing/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)       77 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/src/data_processing/transform/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2298 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/transform/table_transform.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.226482 data_prep_lab-0.1.6/src/data_processing/utils/
+-rw-r--r--   0 dawood     (501) staff       (20)      354 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/__init__.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3135 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1695 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/config.py
+-rw-r--r--   0 dawood     (501) staff       (20)     2052 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/log.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6029 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 dawood     (501) staff       (20)     6740 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.209140 data_prep_lab-0.1.6/test/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.209473 data_prep_lab-0.1.6/test/data_processing_tests/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.237240 data_prep_lab-0.1.6/test/data_processing_tests/data_access/
+-rw-r--r--   0 dawood     (501) staff       (20)     1256 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test/data_processing_tests/data_access/daf_local_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)    24597 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     5734 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1545 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.238199 data_prep_lab-0.1.6/test/data_processing_tests/ray/
+-rw-r--r--   0 dawood     (501) staff       (20)     9851 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/test/data_processing_tests/ray/launcher_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     3282 2024-05-08 13:58:20.000000 data_prep_lab-0.1.6/test/data_processing_tests/ray/ray_util_test.py
+-rw-r--r--   0 dawood     (501) staff       (20)     1685 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test/data_processing_tests/ray/test_noop_launch.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.238481 data_prep_lab-0.1.6/test/data_processing_tests/transform/
+-rw-r--r--   0 dawood     (501) staff       (20)     1678 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.238791 data_prep_lab-0.1.6/test/data_processing_tests/util/
+-rw-r--r--   0 dawood     (501) staff       (20)     1386 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.207834 data_prep_lab-0.1.6/test-data/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208570 data_prep_lab-0.1.6/test-data/data_processing/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208226 data_prep_lab-0.1.6/test-data/data_processing/daf/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208128 data_prep_lab-0.1.6/test-data/data_processing/daf/input/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.227469 data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds1/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds1/sample1.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds1/sample2.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.228376 data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds2/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds2/sample3.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208292 data_prep_lab-0.1.6/test-data/data_processing/daf/output/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.229241 data_prep_lab-0.1.6/test-data/data_processing/daf/output/ds1/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 18:16:43.000000 data_prep_lab-0.1.6/test-data/data_processing/daf/output/ds1/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.230551 data_prep_lab-0.1.6/test-data/data_processing/input/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.233075 data_prep_lab-0.1.6/test-data/data_processing/input_multiple/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208637 data_prep_lab-0.1.6/test-data/data_processing/ray/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.208888 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.234044 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 dawood     (501) staff       (20)     1128 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.234665 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 dawood     (501) staff       (20)      753 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.234958 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 18:24:06.235570 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 dawood     (501) staff       (20)      753 2024-04-24 18:22:56.000000 data_prep_lab-0.1.6/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_lab-0.1.5/Makefile` & `data_prep_lab-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/PKG-INFO` & `data_prep_lab-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_lab-0.1.5/README.md` & `data_prep_lab-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/advanced-transform-tutorial.md` & `data_prep_lab-0.1.6/doc/advanced-transform-tutorial.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Advanced Transform Tutorial
 
-In this example, we implement an [ededup](../../transforms/universal/ededup) transform that 
-removes duplicate documents across all files. In this tutorial, we will show the following: 
+In this example, we implement an [ededup](../../transforms/universal/ededup) transform that
+removes duplicate documents across all files. In this tutorial, we will show the following:
 
 * How to write the `ededup` transform to generate the output table.
 * How to define transform-specific metadata that can be associated
   with each table transformation and aggregated across all transformations
   in a single run of the transform.
-* How to implement custom `TransformRuntime` to create supporting Ray objects and supplement 
+* How to implement custom `TransformRuntime` to create supporting Ray objects and supplement
   transform-specific metadata with the information about this statistics
 * How to define command line arguments that can be used to configure
   the operation of our _noop_ transform.
 
 The complete task involves the following:
 * EdedupTransform - class that implements the specific transformation
-* EdedupRuntime - class that implements custom TransformRuntime to create supporting Ray objects and enhance job output 
-  statistics 
+* EdedupRuntime - class that implements custom TransformRuntime to create supporting Ray objects and enhance job output
+  statistics
 * EdedupTableTransformConfiguration - class that provides configuration for the
-  EdedupTransform and EdedupRuntime, including transform runtime class and the command line arguments used to 
+  EdedupTransform and EdedupRuntime, including transform runtime class and the command line arguments used to
   configure them.
 * main() - simple creation and use of the TransformLauncher.
 
 (Currently, the complete code for the noop transform used for this
 tutorial can be found in the
 [ededup transform](../../transforms/universal/ededup) directory.
 
@@ -121,15 +121,15 @@
         out_table = table.filter(mask)
         # report statistics
         stats = {"source_documents": table.num_rows, "result_documents": out_table.num_rows}
         return [out_table], stats
 ```
 The single input to this method is the in-memory pyarrow table to be transformed.
 The return of this function is a list of tables and optional metadata.  In this
-case of simple 1:1 table conversion the list will contain a single table, result of removing 
+case of simple 1:1 table conversion the list will contain a single table, result of removing
 duplicates from input table.
 
 The metadata is a free-form dictionary of keys with numeric values that will be aggregated
 by the framework and reported as aggregated job statistics metadata.
 If there is no metadata then simply return an empty dictionary.
 
 ## EdedupRuntime
@@ -137,17 +137,17 @@
 First, let's define the transform runtime class.  To do this we extend
 the base abstract/interface class
 [DefaultTableTransformRuntime](../src/data_processing/ray/transform_runtime.py),
 which requires definition of the following:
 * an initializer (i.e. `init()`) that accepts a dictionary of configuration
   data.  For this example, the configuration data will only be defined by
   command line arguments (defined below).
-* the `get_transform_config()` method that takes `data_access_factory`, `statistics actor`, and 
+* the `get_transform_config()` method that takes `data_access_factory`, `statistics actor`, and
   `list of files to process` and produces a dictionary of parameters used by transform.
-* the `compute_execution_stats()` method that takes take a dictionary of metadata, enhances it and 
+* the `compute_execution_stats()` method that takes take a dictionary of metadata, enhances it and
   produces an enhanced metadata dictionary.
 
 We start with the simple definition of the class and its initializer
 
 ```python
 class EdedupRuntime(DefaultTableTransformRuntime):
 
@@ -166,23 +166,22 @@
             clazz=HashFilter,
             params={},
             actor_options={"num_cpus": self.params.get("hash_cpu", 0.5)},
             n_actors=self.params.get("num_hashes", 1),
         )
         return {"hashes": self.filters} | self.params
 ```
-Inputs to this method includes a set of parameters, that moght not be needed for this transformer, but 
+Inputs to this method includes a set of parameters, that moght not be needed for this transformer, but
 rather a superset of all parameters that can be used by different implementations of transform runtime (
-see for example [block listing](../../transforms/universal/blocklist), 
-[fuzzy dedup](../../transforms/universal/fdedup), etc).
+see for example [fuzzy dedup](../../transforms/universal/fdedup), etc).
 The return of this function is a dictionary information for transformer initialization. In this
 implementation we add additional parameters to the input dictionary, but in general, it can be a completely
 new dictionary build here
 
-Finally we define the `compute_execution_stats()` method, which which enhances metadata collected by statistics 
+Finally we define the `compute_execution_stats()` method, which which enhances metadata collected by statistics
 class
 
 ```python
     def compute_execution_stats(self, stats: dict[str, Any]) -> dict[str, Any]:
     # Get filters stats
     sum_hash = 0
     sum_hash_mem = 0
@@ -194,33 +193,36 @@
             h_size, h_memory = ray.get(r)
             sum_hash = sum_hash + h_size
             sum_hash_mem = sum_hash_mem + h_memory
         remote_replies = not_ready
     dedup_prst = 100 * (1.0 - stats.get("result_documents", 1) / stats.get("source_documents", 1))
     return {"number of hashes": sum_hash, "hash memory, GB": sum_hash_mem, "de duplication %": dedup_prst} | stats
 ```
-Input to this method is a dictionary of metadata collected by statistics object. It then enhances it by information 
+Input to this method is a dictionary of metadata collected by statistics object. It then enhances it by information
 collected by hash actors and custom computations based on statistics data.
 
 ## EdedupTableTransformConfiguration
 
-The final class we need to implement is `EdedupTableTransformConfiguration` class and its initializer that 
+The final class we need to implement is `EdedupTableTransformConfiguration` class and its initializer that
 define the following:
 
 * The short name for the transform
 * The class implementing the transform - in our case EdedupTransform
 * The transform runtime class be used - in our case EdedupRuntime
 * Command line argument support.
 
 First we define the class and its initializer,
 
 ```python
+short_name = "ededup"
+cli_prefix = f"{short_name}_"
+
 class EdedupTableTransformConfiguration(DefaultTableTransformConfiguration):
     def __init__(self):
-        super().__init__(name="ededup", runtime_class=EdedupRuntime, transform_class=EdedupTransform)
+        super().__init__(name=short_name, runtime_class=EdedupRuntime, transform_class=EdedupTransform)
         self.params = {}
 ```
 
 The initializer extends the DefaultTableTransformConfiguration which provides simple
 capture of our configuration data and enables picklability through the network.
 It also adds a `params` field that will be used below to hold the transform's
 configuration data (used in `EdedupRuntime.init()` above).
@@ -230,31 +232,30 @@
 First we define the method establishes the command line arguments.
 This method is given a global argument parser to which the `EdedupTransform` arguments are added.
 It is good practice to include a common prefix to all transform-specific options (i.e. pii, lang, etc).
 In our case we will use `noop_`.
 
 ```python
     def add_input_params(self, parser: ArgumentParser) -> None:
-        parser.add_argument("--hash_cpu", type=float, default=0.5, help="number of CPUs per hash")
-        parser.add_argument("--num_hashes", type=int, default=0, help="number of hash actors to use")
-        parser.add_argument("--doc_column", type=str, default="contents", help="key for accessing data")
+      parser.add_argument(f"--{cli_prefix}hash_cpu", type=float, default=0.5, help="number of CPUs per hash")
+      parser.add_argument(f"--{cli_prefix}num_hashes", type=int, default=0, help="number of hash actors to use")
+      parser.add_argument(f"--{cli_prefix}doc_column", type=str, default="contents", help="key for accessing data")
 ```
 Next we implement a method that is called after the framework has parsed the CLI args
 and which allows us to capture the `EdedupTransform`-specific arguments and optionally validate them.
 
 ```python
     def apply_input_params(self, args: Namespace) -> bool:
-        if args.num_hashes <= 0:
-            print(f"Number of hashes should be greater then zero, provided {args.num_hashes}")
-            return False
-        self.params["doc_column"] = args.doc_column
-        self.params["hash_cpu"] = args.hash_cpu
-        self.params["num_hashes"] = args.num_hashes
-        print(f"exact dedup params are {self.params}")
-        return True
+      captured = CLIArgumentProvider.capture_parameters(args, cli_prefix, False)
+      self.params = self.params | captured
+      if self.params["num_hashes"] <= 0:
+        logger.info(f"Number of hashes should be greater then zero, provided {args.num_hashes}")
+        return False
+      logger.info(f"exact dedup params are {self.params}")
+      return True
 ```
 
 ## main()
 
 Next, we show how to launch the framework with the `EdedupTransform` using the
 framework's `TransformLauncher` class.
 
@@ -265,18 +266,19 @@
 ```
 The launcher requires only an instance of DefaultTableTransformConfiguration
 (our `EdedupTransformConfiguration` class).
 A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
-Assuming the above `main()` is placed in `ededup_transform.py` we can run the transform on local data as follows:
+Assuming the above `main()` is placed in `ededup_transform.py` we can run the transform on data
+in COS as follows:
 
 ```shell
-python ededup_transform.py --ededup_hash_cpu 0.5 --ededup_num_hashes 2  --ededup_doc_column "contents" \
+python ededup_transform.py --hash_cpu 0.5 --num_hashes 2 --doc_column "contents" \
   --run_locally True  \
-  --data_local_config="{'input_folder': '<project location>/transforms/universal/ededup/test-data/input', 'output_folder': '<project location>/transforms/universal/ededup/output'}"
+  --s3_cred "{'access_key': 'KEY', 'secret_key': 'SECRET', 'cos_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
+  --s3_config "{'input_folder': 'cos-optimal-llm-pile/test/david/input/', 'output_folder': 'cos-optimal-llm-pile/test/david/output/'}"
 ```
 This is a minimal set of options to run locally.
 See the [launcher options](launcher-options.md) for a complete list of
 transform-independent command line options.
-
```

### Comparing `data_prep_lab-0.1.5/doc/architecture.md` & `data_prep_lab-0.1.6/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/launcher-options.md` & `data_prep_lab-0.1.6/doc/launcher-options.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,19 +13,19 @@
                          [--data_local_config DATA_LOCAL_CONFIG]
                          [--data_max_files DATA_MAX_FILES]
                          [--data_checkpointing DATA_CHECKPOINTING]
                          [--data_data_sets DATA_DATA_SETS]
                          [--data_max_files MAX_FILES]
                          [--data_files_to_use DATA_FILES_TO_USE]
                          [--data_num_samples DATA_NUM_SAMPLES]
-                         [--num_workers NUM_WORKERS] 
-                         [--worker_options WORKER_OPTIONS]
-                         [--pipeline_id PIPELINE_ID] [--job_id JOB_ID]
-                         [--creation_delay CREATION_DELAY]
-                         [--code_location CODE_LOCATION]
+                         [--runtime_num_workers NUM_WORKERS] 
+                         [--runtime_worker_options WORKER_OPTIONS]
+                         [--runtime_pipeline_id PIPELINE_ID] [--job_id JOB_ID]
+                         [--runtime_creation_delay CREATION_DELAY]
+                         [--runtime_code_location CODE_LOCATION]
 
 Driver for NOOP processing
 
 options:
   -h, --help            show this help message and exit
   --run_locally RUN_LOCALLY
                         running ray local flag
@@ -53,32 +53,32 @@
                         checkpointing flag
   --data_data_sets DATA_SETS
                         List of data sets
   --data_files_to_use DATA_FILES_TO_USE
                         files extensions to use, default .parquet
   --data_num_samples DATA_NUM_SAMPLES
                         number of randomply picked files to use
-  --num_workers NUM_WORKERS
+  --runtime_num_workers NUM_WORKERS
                         number of workers
-  --worker_options WORKER_OPTIONS
+  --runtime_worker_options WORKER_OPTIONS
                         AST string defining worker resource requirements.
                         num_cpus: Required number of CPUs.
                         num_gpus: Required number of GPUs
                         resources: The complete list can be found at
                                    https://docs.ray.io/en/latest/ray-core/api/doc/ray.remote_function.RemoteFunction.options.html#ray.remote_function.RemoteFunction.options
                                    and contains accelerator_type, memory, name, num_cpus, num_gpus, object_store_memory, placement_group,
                                    placement_group_bundle_index, placement_group_capture_child_tasks, resources, runtime_env,
                                    scheduling_strategy, _metadata, concurrency_groups, lifetime, max_concurrency, max_restarts,
                                    max_task_retries, max_pending_calls, namespace, get_if_exists
                         Example: { 'num_cpus': '8', 'num_gpus': '1', 'resources': '{"special_hardware": 1, "custom_label": 1}' }
-  --pipeline_id PIPELINE_ID
+  --runtime_pipeline_id PIPELINE_ID
                         pipeline id
-  --job_id JOB_ID       job id
-  --creation_delay CREATION_DELAY
+  --runtime_job_id JOB_ID       job id
+  --runtime_creation_delay CREATION_DELAY
                         delay between actor' creation
-  --code_location CODE_LOCATION
+  --runtime_code_location CODE_LOCATION
                         AST string containing code location
                         github: Github repository URL.
                         commit_hash: github commit hash
                         path: Path within the repository
                         Example: { 'github': 'https://github.com/somerepo', 'commit_hash': '13241231asdfaed', 'path': 'transforms/universal/ededup' }
 ```
```

### Comparing `data_prep_lab-0.1.5/doc/overview.md` & `data_prep_lab-0.1.6/doc/overview.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 scalable processing/transformation of virtually unlimited amounts of data. 
 
 The framework allows simple 1:1 transformation of parquet files, but also enables
 more complex transformations requiring coordination among transforming nodes.
 This might include operations such as de-duplication, merging, and splitting.
 The framework uses a plugin-model for the primary functions.  The key ones for
 developers of data transformation are:
+
 * [Transformation](../src/data_processing/transform/table_transform.py) - a simple, easily-implemented interface defines
 the specifics of a given data transformation.
 * [Transform Configuration](../src/data_processing/ray/transform_runtime.py) - defines
 the transform implementation and runtime classes, the 
 command line arguments specific to transform, and the short name for the transform.
 * [Transformation Runtime](../src/data_processing/ray/transform_runtime.py) - allows for customization of the Ray environment for the transformer.
 This might include provisioning of shared memory objects or creation of additional actors.
 
 To learn more consider the following:
+
 * [Transform Tutorials](transform-tutorials.md)
 * [Testing transformers with S3](using_s3_transformers.md)
 * [Architecture Deep Dive](architecture.md)
 * [Transform project root readme](../../transforms/README.md)
```

### Comparing `data_prep_lab-0.1.5/doc/processing-architecture.jpg` & `data_prep_lab-0.1.6/doc/processing-architecture.jpg`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/simplest-transform-tutorial.md` & `data_prep_lab-0.1.6/doc/simplest-transform-tutorial.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # Simplest Transform Tutorial
 In this example, we implement a [noop](../../transforms/universal/noop) transform that takes no action
 on the input table and returns it unmodified - a _no operation_ (noop).
-This effectively enables a copy of a directory tree of 
+This effectively enables a copy of a directory tree of
 parquet files to an output directory.
 This is functionally not too powerful, but allows us to focus
 on the minimum requirements for a simple transform that converts
 one table to another.  That said, we will show the following:
 
 * How to write the _noop_ transform to generate the output table.
 * How to define transform-specific metadata that can be associated
-with each table transformation and aggregated across all transformations
-in a single run of the transform.
+  with each table transformation and aggregated across all transformations
+  in a single run of the transform.
 * How to define command line arguments that can be used to configure
   the operation of our _noop_ transform.
 
 We will **not** be showing the following:
 * The creation of a custom TransformRuntime that would enable more global
-state and/or coordination among the transforms running in other ray actors.
-This will be covered in an advanced tutorial.
+  state and/or coordination among the transforms running in other ray actors.
+  This will be covered in an advanced tutorial.
 
 The complete task involves the following:
 * NOOPTransform - class that implements the specific transformation
-* NOOPTableTransformConfiguration - class that provides configuration for the 
-NOOPTransform, specifically the command line arguments used to configure it.
+* NOOPTableTransformConfiguration - class that provides configuration for the
+  NOOPTransform, specifically the command line arguments used to configure it.
 * main() - simple creation and use of the TransformLauncher.
 
 (Currently, the complete code for the noop transform used for this
 tutorial can be found in the
 [noop transform](../../transforms/universal/noop) directory.
 
 Finally, we show to use the command line to run the transform in a local ray cluster
 
 ## NOOPTransform
 
 First, let's define the transform class.  To do this we extend
-the base abstract/interface class 
-[AbstractTableTransform](../src/data_processing/transform/table_transform.py),
+the base abstract/interface class
+[AbstractTableTransform](../src/data_processing_ibm/transform/table_transform.py),
 which requires definition of the following:
 * an initializer (i.e. `init()`) that accepts a dictionary of configuration
-data.  For this example, the configuration data will only be defined by
-command line arguments (defined below).
+  data.  For this example, the configuration data will only be defined by
+  command line arguments (defined below).
 * the `transform()` method itself that takes an input table produces an output
-table and any associated metadata for that table transformation.
+  table and any associated metadata for that table transformation.
 
 Other methods such as `flush()` need not be overridden/redefined for this simple example.
 
 We start with the simple definition of the class, its initializer and the imports required
 by subsequent code:
 
 ```python
@@ -88,107 +88,110 @@
         metadata = {"nfiles": 1, "nrows": len(table)}
         return [table], metadata
 ```
 The single input to this method is the in-memory pyarrow table to be transformed.
 The return of this function is a list of tables and optional metadata.  In this
 case of simple 1:1 table conversion the list will contain a single table, the input.
 The metadata is a free-form dictionary of keys with numeric values that will be aggregated
-by the framework and reported as aggregated job statistics metadata. 
+by the framework and reported as aggregated job statistics metadata.
 If there is no metadata then simply return an empty dictionary.
 
 ## NOOPTransformConfiguration
 
 Next we define the `NOOPTransformConfiguration` class and its initializer that define the following:
 
 * The short name for the transform
 * The class implementing the transform - in our case NOOPTransform
 * Command line argument support.
 * The transform runtime class be used.  We will use the `DefaultTableTransformRuntime`
-which is sufficient for most 1:1 table transforms.  Extensions to this class can be
-used when more complex interactions among transform is required.*
+  which is sufficient for most 1:1 table transforms.  Extensions to this class can be
+  used when more complex interactions among transform is required.*
 
 First we define the class and its initializer,
 
 ```python
+short_name = "NOOP"
+cli_prefix = f"{short_name}_"
+
 class NOOPTransformConfiguration(DefaultTableTransformConfiguration):
     
     def __init__(self):
-        super().__init__(name="NOOP", 
-                         runtime_class=DefaultTableTransformRuntime, 
-                         transform_class=NOOPTransform)
+        super().__init__(name=short_name, transform_class=NOOPTransform)
         self.params = {}
 ```
 The initializer extends the DefaultTableTransformConfiguration which provides simple
 capture of our configuration data and enables picklability through the network.
-It also adds a `params` field that will be used below to hold the transform's 
+It also adds a `params` field that will be used below to hold the transform's
 configuration data (used in `NOOPTransform.init()` above).
 
-Next, we provide two methods that define and capture the command line configuration that 
+Next, we provide two methods that define and capture the command line configuration that
 is specific to the `NOOPTransform`, in this case the number of seconds to sleep during transformation
 and an example command line, `pwd`, option holding sensitive data that we don't want reported
 in the job metadata produced by the ray orchestrator.
 First we define the method establishes the command line arguments.
 This method is given a global argument parser to which the `NOOPTransform` arguments are added.
 It is good practice to include a common prefix to all transform-specific options (i.e. pii, lang, etc).
 In our case we will use `noop_`.
 
 ```python
     def add_input_params(self, parser: ArgumentParser) -> None:
         parser.add_argument(
-            "--noop_sleep_sec",
+            f"--{cli_prefix}noop_sleep_sec",
             type=int,
             default=1,
             help="Sleep actor for a number of seconds while processing the data frame",
         )
         # An example of a command line option that we don't want included in the metadata collected by the Ray orchestrator
         # See below for remove_from_metadata addition so that it is not reported.
         parser.add_argument(
-            "--noop_pwd",
+            f"--{cli_prefix}noop_pwd",
             type=str,
             default="nothing",
             help="A dummy password which should be filtered out of the metadata",
         )
 ```
 Next we implement a method that is called after the framework has parsed the CLI args
 and which allows us to capture the `NOOPTransform`-specific arguments, optionally validate them
 and flag that the `pwd` parameter should not be reported in the metadata.
 
 ```python
     def apply_input_params(self, args: Namespace) -> bool:
-        if args.noop_sleep_sec <= 0:
-            print(f"Parameter noop_sleep_sec should be greater then 0, you specified {args.noop_sleep_sec}")
-            return False
-        self.params["sleep"] = args.noop_sleep_sec
-        self.params["pwd"] = args.noop_pwd
+        captured = CLIArgumentProvider.capture_parameters(args, cli_prefix, False)
+        if captured.get(sleep_key) < 0:
+          print(f"Parameter noop_sleep_sec should be non-negative. you specified {args.noop_sleep_sec}")
+          return False
+      
+        self.params = self.params | captured
+        logger.info(f"noop parameters are : {self.params}")
         # Don't publish this in the metadata produced by the ray orchestrator.
-        self.remove_from_metadata.append["pwd"]
+        self.remove_from_metadata.append(pwd_key)
         return True
 ```
 
 ## main()
 
-Next, we show how to launch the framework with the `NOOPTransform` using the 
+Next, we show how to launch the framework with the `NOOPTransform` using the
 framework's `TransformLauncher` class.
 
 ```python
 if __name__ == "__main__":
     launcher = TransformLauncher(transform_runtime_config=NOOPTransformConfiguration())
     launcher.launch()
 ```
-The launcher requires only an instance of DefaultTableTransformConfiguration 
+The launcher requires only an instance of DefaultTableTransformConfiguration
 (our `NOOPTransformConfiguration` class).
 A single method `launch()` is then invoked to run the transform in a Ray cluster.
 
 ## Running
 
-Assuming the above `main()` is placed in `noop_main.py` we can run the transform on local data as follows:
+Assuming the above `main()` is placed in `noop_main.py` we can run the transform on data
+in COS as follows:
 
 ```shell
-python noop_transform.py \
-  --noop_sleep_sec 2  \
-  --run_locally=True  \
-  --data_local_config="{'input_folder': '<project location>/transforms/universal/noop/test-data/input', 'output_folder': '<project location>/transforms/universal/noop/output'}"
+python noop_main.py --noop_sleep_msec 2 \
+  --run_locally True  \
+  --s3_cred "{'access_key': 'KEY', 'secret_key': 'SECRET', 'cos_url': 'https://s3.us-east.cloud-object-storage.appdomain.cloud'}" \
+  --s3_config "{'input_folder': 'cos-optimal-llm-pile/test/david/input/', 'output_folder': 'cos-optimal-llm-pile/test/david/output/'}"
 ```
 This is a minimal set of options to run locally.
 See the [launcher options](launcher-options.md) for a complete list of
 transform-independent command line options.
-
```

### Comparing `data_prep_lab-0.1.5/doc/testing-transforms.md` & `data_prep_lab-0.1.6/doc/testing-transforms.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/transform-external-resources.md` & `data_prep_lab-0.1.6/doc/transform-external-resources.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/transform-tutorials.md` & `data_prep_lab-0.1.6/doc/transform-tutorials.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Metadata accumulated across calls to all transforms is stored in the destination.
 
 ### Transform Basics
 In support of this model the class 
 [AbstractTableTransform](../src/data_processing/transform/table_transform.py) 
 is expected to be extended when implementing a transform.
 The following methods are defined:
+
 * ```__init__(self, config:dict)``` - an initializer through which the transform can be created 
 with implementation-specific configuration.  For example, the location of a model, maximum number of
 rows in a table, column(s) to use, etc. 
 * ```transform(self, table:pyarrow.Table) -> tuple(list[pyarrow.Table], dict)``` - this method is responsible
 for the actual transformation of a given table to zero or more output tables, and optional 
 metadata regarding the transformation applied.  Zero tables might be returned when
 merging tables across calls to `transform()` and more than 1 table might be returned
@@ -33,14 +34,15 @@
 make use of buffering (e.g. [coalesce](../../transforms/universal/coalesce/src/coalesce_transform.py)) across calls 
 to `transform()` and need to be flushed of all buffered data at the end of processing of input tables.  
 The return values are handled the same waa as the return values for `transform()`.  Since most transforms will likely
 not need this feature, a default implementation is provided to return an empty list and empty dictionary.
 
 ### Running in Ray
 When a transform is run using the Ray-based framework a number of other capabilities are involved:
+
 * [Transform Runtime](../src/data_processing/ray/transform_runtime.py) - this provides the ability for the
 transform implementor to create additional Ray resources 
 and include them in the configuration used to create a transform
 (see, for example, [exact dedup](../../transforms/universal/ededup/src/ededup_transform.py) 
 or [blocklist](../../transforms/universal/blocklisting/src/blocklist_transform.py)).
 This also provide the ability to supplement the statics collected by
 [Statistics](../src/data_processing/ray/transform_statistics.py) (see below).
@@ -49,14 +51,15 @@
   * command line arguments used to initialize the Transform Runtime and generally, the Transform.
   * Transform Runtime class to use
   * transform short name 
 * [Transform Launcher](../src/data_processing/ray/transform_launcher.py) - this is a class generally used to 
 implement `main()` that makes use of a Transform Configuration to start the Ray runtime and execute the transforms.
 
 Roughly speaking the following steps are completed to establish transforms in the RayWorkers
+
 1. Launcher parses the CLI parameters using an ArgumentParser configured with its own CLI parameters 
 along with those of the Transform Configuration, 
 2. Launcher passes the Transform Configuration and CLI parameters to the [RayOrchestrator](../src/data_processing/ray/transform_orchestrator.py)
 3. RayOrchestrator creates the Transform Runtime using the Transform Configuration and its CLI parameter values
 4. Transform Runtime creates transform initialization/configuration including the CLI parameters,  
 and any Ray components need by the transform.
 5. [RayWorker](../src/data_processing/ray/transform_table_processor.py) is started with configuration from the Transform Runtime.
@@ -167,24 +170,25 @@
 
 
 ### Tutorial Examples
 With these basic concepts in mind, we start with a simple example and 
 progress to more complex transforms. 
 Before getting started  you may want to consult the 
 [transform project root readme](../../transforms/README.md) documentation.
+
 * [Simplest transform](simplest-transform-tutorial.md) - 
 Here we will take a simple example to show the basics of creating a simple transform
 that takes a single input Table, and produces a single Table.
 * [External resources transform](transform-external-resources.md) - shows how to load additional
 resources (models, configuration, etc) for a transform.
 * [Advanced transform](advanced-transform-tutorial.md)
-* [Porting from GUF 0.1.6](transform-porting.md)
 
 Once a transform has been built, testing can be enabled with the testing framework:
+
 * [Transform Testing](testing-transforms.md) - shows how to test a transform
 independent of the Ray framework.
 * [End-to-End Testing](testing-e2e-transform.md) - shows how to test the
 transform running in the Ray environment.
 
 ### Additional transform support
 
-We also strted a library of [transform utilities](transformer-utilities.md)
+We also strted a library of [transform utilities](transformer-utilities.md)
```

### Comparing `data_prep_lab-0.1.5/doc/transformer-utilities.md` & `data_prep_lab-0.1.6/doc/transformer-utilities.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/doc/using_s3_transformers.md` & `data_prep_lab-0.1.6/doc/using_s3_transformers.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/pyproject.toml` & `data_prep_lab-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data_prep_lab"
-version = "0.1.5"
+version = "0.1.6"
 requires-python = ">=3.10"
 description = "Data Preparation Laboratory Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
```

### Comparing `data_prep_lab-0.1.5/src/data_prep_lab.egg-info/PKG-INFO` & `data_prep_lab-0.1.6/src/data_prep_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_prep_lab
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Preparation Laboratory Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
```

### Comparing `data_prep_lab-0.1.5/src/data_prep_lab.egg-info/SOURCES.txt` & `data_prep_lab-0.1.6/src/data_prep_lab.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 .gitignore
 Makefile
 README.md
-mkdocs.yml
 pyproject.toml
 doc/advanced-transform-tutorial.md
 doc/architecture.md
 doc/launcher-options.md
+doc/logo-ibm-dark.png
+doc/logo-ibm.png
 doc/overview.md
 doc/processing-architecture.jpg
 doc/simplest-transform-tutorial.md
 doc/testing-e2e-transform.md
 doc/testing-transforms.md
 doc/transform-external-resources.md
-doc/transform-porting.md
 doc/transform-tutorials.md
 doc/transformer-utilities.md
 doc/using_s3_transformers.md
 src/data_prep_lab.egg-info/PKG-INFO
 src/data_prep_lab.egg-info/SOURCES.txt
 src/data_prep_lab.egg-info/dependency_links.txt
 src/data_prep_lab.egg-info/requires.txt
 src/data_prep_lab.egg-info/top_level.txt
+src/data_processing/__init__.py
 src/data_processing/data_access/__init__.py
 src/data_processing/data_access/arrow_s3.py
 src/data_processing/data_access/data_access.py
 src/data_processing/data_access/data_access_factory.py
 src/data_processing/data_access/data_access_factory_base.py
 src/data_processing/data_access/data_access_local.py
 src/data_processing/data_access/data_access_s3.py
@@ -34,36 +35,43 @@
 src/data_processing/ray/transform_orchestrator.py
 src/data_processing/ray/transform_orchestrator_configuration.py
 src/data_processing/ray/transform_runtime.py
 src/data_processing/ray/transform_statistics.py
 src/data_processing/ray/transform_table_processor.py
 src/data_processing/test_support/__init__.py
 src/data_processing/test_support/abstract_test.py
+src/data_processing/test_support/data_access/__init__.py
+src/data_processing/test_support/data_access/data_access_factory_test.py
 src/data_processing/test_support/ray/__init__.py
 src/data_processing/test_support/ray/transform_test.py
 src/data_processing/test_support/transform/__init__.py
 src/data_processing/test_support/transform/noop_transform.py
 src/data_processing/test_support/transform/transform_test.py
 src/data_processing/transform/__init__.py
 src/data_processing/transform/table_transform.py
 src/data_processing/utils/__init__.py
 src/data_processing/utils/cli_utils.py
 src/data_processing/utils/config.py
 src/data_processing/utils/log.py
 src/data_processing/utils/params_utils.py
 src/data_processing/utils/transform_utils.py
+test-data/data_processing/daf/input/ds1/sample1.parquet
+test-data/data_processing/daf/input/ds1/sample2.parquet
+test-data/data_processing/daf/input/ds2/sample3.parquet
+test-data/data_processing/daf/output/ds1/sample1.parquet
 test-data/data_processing/input/sample1.parquet
 test-data/data_processing/input_multiple/sample1.parquet
 test-data/data_processing/input_multiple/sample2.parquet
 test-data/data_processing/input_multiple/sample3.parquet
 test-data/data_processing/ray/noop/expected/metadata.json
 test-data/data_processing/ray/noop/expected/sample1.parquet
 test-data/data_processing/ray/noop/expected/subdir/test1.parquet
 test-data/data_processing/ray/noop/input/sample1.parquet
 test-data/data_processing/ray/noop/input/subdir/test1.parquet
+test/data_processing_tests/data_access/daf_local_test.py
 test/data_processing_tests/data_access/data_access_local_test.py
 test/data_processing_tests/data_access/data_access_s3_test.py
 test/data_processing_tests/data_access/sample_input_data_test.py
 test/data_processing_tests/ray/launcher_test.py
 test/data_processing_tests/ray/ray_util_test.py
 test/data_processing_tests/ray/test_noop_launch.py
 test/data_processing_tests/transform/test_noop.py
```

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/arrow_s3.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/arrow_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/data_access.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/data_access_factory.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/data_access_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,23 +109,28 @@
         )
         parser.add_argument(
             f"--{self.cli_arg_prefix}checkpointing",
             type=lambda x: bool(str2bool(x)),
             default=False,
             help="checkpointing flag",
         )
-        parser.add_argument(f"--{self.cli_arg_prefix}data_sets", type=str, default=None, help="List of data sets")
+        parser.add_argument(
+            f"--{self.cli_arg_prefix}data_sets",
+            type=ast.literal_eval,
+            default=None,
+            help="List of sub-directories of input directory to use for input. For example, ['dir1', 'dir2']",
+        )
         parser.add_argument(
             f"--{self.cli_arg_prefix}files_to_use",
             type=ast.literal_eval,
             default=ast.literal_eval("['.parquet']"),
-            help="list of files extensions to choose",
+            help="list of file extensions to choose for input.",
         )
         parser.add_argument(
-            f"--{self.cli_arg_prefix}num_samples", type=int, default=-1, help="number of random files to process"
+            f"--{self.cli_arg_prefix}num_samples", type=int, default=-1, help="number of random input files to process"
         )
 
     def apply_input_params(self, args: Union[dict, argparse.Namespace]) -> bool:
         """
         Validate data access specific parameters
         This might need to be extended if new data access implementation is added
         :param args: user defined arguments
@@ -200,22 +205,22 @@
                 f"Both max files {max_files} and random samples {n_samples} are defined. Only one allowed at a time"
             )
             return False
         self.checkpointing = checkpointing
         self.max_files = max_files
         self.n_samples = n_samples
         self.files_to_use = files_to_use
+        self.dsets = data_sets
         if data_sets is None or len(data_sets) < 1:
             self.logger.info(
                 f"data factory {self.cli_arg_prefix} "
                 f"Not using data sets, checkpointing {self.checkpointing}, max files {self.max_files}, "
                 f"random samples {self.n_samples}, files to use {self.files_to_use}"
             )
         else:
-            self.dsets = data_sets.split(",")
             self.logger.info(
                 f"data factory {self.cli_arg_prefix} "
                 f"Using data sets {self.dsets}, checkpointing {self.checkpointing}, max files {self.max_files}, "
                 f"random samples {self.n_samples}, files to use {self.files_to_use}"
             )
         return True
```

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/data_access_local.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/data_access_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,19 +76,18 @@
         :param path: starting path
         :param extensions: List of extensions, None - all
         :return: List of files
         """
         files = []
         for c_path in sorted(Path(path).rglob("*")):
             # for every file
+            if c_path.is_dir():
+                continue
             s_path = str(c_path.absolute())
-            if extensions is None:
-                if c_path.is_dir():
-                    continue
-            else:
+            if extensions is not None:
                 _, extension = os.path.splitext(s_path)
                 if extension not in extensions:
                     continue
             files.append(s_path)
         return files
 
     def _get_files_folder(
@@ -141,34 +140,36 @@
         :return: tuple of file list and profile
         """
         if not self.checkpoint:
             return self._get_files_folder(
                 path=input_path, cm_files=cm_files, min_file_size=min_file_size, max_file_size=max_file_size
             )
 
-        input_files = set(self._get_all_files_ext(path=input_path, extensions=self.files_to_use))
-        output_files = set(self._get_all_files_ext(path=output_path, extensions=self.files_to_use))
-        input_only_files = input_files - output_files
+        input_files = self._get_all_files_ext(path=input_path, extensions=self.files_to_use)
+        output_files = self._get_all_files_ext(path=output_path, extensions=self.files_to_use)
 
         total_input_file_size = 0
         i = 0
-        output_files = []
-        for filename in sorted(input_only_files):
+        result_files = []
+        for filename in sorted(input_files):
+            out_f_name = self.get_output_location(filename)
+            if out_f_name in output_files:
+                continue
             if i >= cm_files > 0:
                 break
-            output_files.append(filename)
+            result_files.append(filename)
             size = os.path.getsize(os.path.join(input_path, filename))
             total_input_file_size += size
             if min_file_size > size:
                 min_file_size = size
             if max_file_size < size:
                 max_file_size = size
             i += 1
         return (
-            output_files,
+            result_files,
             {
                 "max_file_size": max_file_size / MB,
                 "min_file_size": min_file_size / MB,
                 "total_file_size": total_input_file_size / MB,
             },
         )
```

### Comparing `data_prep_lab-0.1.5/src/data_processing/data_access/data_access_s3.py` & `data_prep_lab-0.1.6/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/__init__.py` & `data_prep_lab-0.1.6/src/data_processing/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/ray_utils.py` & `data_prep_lab-0.1.6/src/data_processing/ray/ray_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_launcher.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_orchestrator.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_orchestrator.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_orchestrator_configuration.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_orchestrator_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_runtime.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_runtime.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_statistics.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/ray/transform_table_processor.py` & `data_prep_lab-0.1.6/src/data_processing/ray/transform_table_processor.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/test_support/abstract_test.py` & `data_prep_lab-0.1.6/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/test_support/ray/transform_test.py` & `data_prep_lab-0.1.6/src/data_processing/test_support/ray/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_lab-0.1.6/src/data_processing/test_support/transform/noop_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/test_support/transform/transform_test.py` & `data_prep_lab-0.1.6/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/transform/table_transform.py` & `data_prep_lab-0.1.6/src/data_processing/transform/table_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/utils/cli_utils.py` & `data_prep_lab-0.1.6/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/utils/config.py` & `data_prep_lab-0.1.6/src/data_processing/utils/config.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/utils/log.py` & `data_prep_lab-0.1.6/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/utils/params_utils.py` & `data_prep_lab-0.1.6/src/data_processing/utils/params_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/src/data_processing/utils/transform_utils.py` & `data_prep_lab-0.1.6/src/data_processing/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,16 +106,18 @@
 
 
 class TestGetInputFiles(TestInit):
     def setup_directories(self, prefix=""):
         """
         Utility function that sets up input and output directories
         """
-        input_path = Path(os.path.join(self.dal.input_folder, f"{prefix}input_dir"))
-        output_path = Path(os.path.join(self.dal.output_folder, f"{prefix}output_dir"))
+        #        input_path = Path(os.path.join(self.dal.input_folder, f"{prefix}input_dir"))
+        #        output_path = Path(os.path.join(self.dal.output_folder, f"{prefix}output_dir"))
+        input_path = Path(self.dal.input_folder)
+        output_path = Path(self.dal.output_folder)
         os.makedirs(input_path, exist_ok=True)
         os.makedirs(output_path, exist_ok=True)
         return input_path, output_path
 
     @staticmethod
     def cleanup(directories_to_remove=[], files_to_remove=[]):
         """
@@ -167,17 +169,16 @@
         output_file = output_path / "file2.parquet"
         for file in input_files:
             file.touch()
         output_file.touch()
 
         file_list, size_dict = self.dal._get_input_files(str(input_path), str(output_path), cm_files=0)
         result = (file_list, size_dict)
-
         expected_result = (
-            [str(file.absolute()) for file in input_files if str(file.absolute()) != str(output_file.absolute())],
+            [str(file.absolute()) for file in input_files if str(file.name) != str(output_file.name)],
             self.size_stat_dict,
         )
 
         input_files.append(output_file)
         self.cleanup(
             directories_to_remove=[input_path, output_path],
             files_to_remove=input_files,
@@ -308,16 +309,16 @@
             in_path_1,
             out_path_1,
             in_path_2,
             out_path_2,
         ) = self.multiple_missing_files_setup()
 
         expected_result = (
-            [str(file.absolute()) for file in in_files_1 if file.absolute() != out_file_2.absolute()]
-            + [str(file.absolute()) for file in in_files_2 if str(file.absolute()) != str(out_file_2.absolute())],
+            [str(file.absolute()) for file in in_files_1]
+            + [str(file.absolute()) for file in in_files_2 if str(file.name) != str(out_file_2.name)],
             self.size_stat_dict_1,
         )
         self.multiple_missing_files_cleanup(
             in_files_1, in_files_2, out_file_2, in_path_1, out_path_1, in_path_2, out_path_2
         )
 
         assert result == expected_result
```

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/ray/launcher_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/ray/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/ray/ray_util_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/ray/ray_util_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/ray/test_noop_launch.py` & `data_prep_lab-0.1.6/test/data_processing_tests/ray/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/transform/test_noop.py` & `data_prep_lab-0.1.6/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_lab-0.1.6/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/input/sample1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds1/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/daf/input/ds2/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/daf/output/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_lab-0.1.5/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_lab-0.1.6/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

