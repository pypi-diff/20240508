# Comparing `tmp/femr-0.2.2.tar.gz` & `tmp/femr-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femr-0.2.2.tar", last modified: Thu Mar 21 17:52:32 2024, max compression
+gzip compressed data, was "femr-0.2.3.tar", last modified: Thu Mar 21 18:05:09 2024, max compression
```

## Comparing `femr-0.2.2.tar` & `femr-0.2.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.598189 femr-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 17:52:25.000000 femr-0.2.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-21 17:52:25.000000 femr-0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.578189 femr-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.582189 femr-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-21 17:52:25.000000 femr-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-21 17:52:25.000000 femr-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.586189 femr-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-21 17:52:25.000000 femr-0.2.2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 17:52:25.000000 femr-0.2.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 17:52:25.000000 femr-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-21 17:52:25.000000 femr-0.2.2/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-21 17:52:25.000000 femr-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-21 17:52:25.000000 femr-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-21 17:52:32.598189 femr-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-21 17:52:25.000000 femr-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 17:52:25.000000 femr-0.2.2/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-21 17:52:25.000000 femr-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 17:52:32.598189 femr-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.578189 femr-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.586189 femr-0.2.2/src/femr/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.586189 femr-0.2.2/src/femr/featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/featurizers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    21282 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/featurizers/featurizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/featurizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.586189 femr-0.2.2/src/femr/labelers/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/labelers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/labelers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/labelers/omop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/src/femr/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/rmsnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/models/xformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/pat_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/src/femr/post_etl_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/post_etl_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/post_etl_pipelines/stanford.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/splits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/stat_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/src/femr/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-03-21 17:52:25.000000 femr-0.2.2/src/femr/transforms/stanford.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/src/femr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-21 17:52:32.000000 femr-0.2.2/src/femr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:25.000000 femr-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/tests/featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-21 17:52:25.000000 femr-0.2.2/tests/featurizers/test_OnlineStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-03-21 17:52:25.000000 femr-0.2.2/tests/featurizers/test_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-21 17:52:25.000000 femr-0.2.2/tests/femr_test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/tests/labelers/
--rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-03-21 17:52:25.000000 femr-0.2.2/tests/labelers/test_CodeLabelers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-03-21 17:52:25.000000 femr-0.2.2/tests/labelers/test_TimeHorizonEventLabeler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-21 17:52:25.000000 femr-0.2.2/tests/models/test_batch_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-21 17:52:25.000000 femr-0.2.2/tests/models/test_survival_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-21 17:52:25.000000 femr-0.2.2/tests/test_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-03-21 17:52:25.000000 femr-0.2.2/tests/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.582189 femr-0.2.2/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.590189 femr-0.2.2/tools/stanford/
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-21 17:52:25.000000 femr-0.2.2/tools/stanford/download_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/1_Ontology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/2_Labeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/3_Count Featurization And Modeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/4_Train CLMBR.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/5_CLMBR Featurization And Modeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20018 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/6_Train MOTOR.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9580 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/7_MOTOR Featurization And Modeling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/input/clmbr_model/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/clmbr_model/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/clmbr_model/dictionary.msgpack
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/clmbr_model/main_split.csv
--rw-r--r--   0 runner    (1001) docker     (127)   317136 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/clmbr_model/model.safetensors
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/labels.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/input/meds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/input/meds/data/
--rw-r--r--   0 runner    (1001) docker     (127)    33814 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/meds/data/patients.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/meds/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)   208054 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/meds/ontology.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/input/motor_model/
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/motor_model/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/motor_model/dictionary.msgpack
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/motor_model/main_split.csv
--rw-r--r--   0 runner    (1001) docker     (127)   342424 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/input/motor_model/model.safetensors
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/synthetic_data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/synthetic_data_generation/generate_patients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:32.594189 femr-0.2.2/tutorials/trash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:52:25.000000 femr-0.2.2/tutorials/trash/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.409865 femr-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 18:05:04.000000 femr-0.2.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-21 18:05:04.000000 femr-0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.389862 femr-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.393862 femr-0.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-21 18:05:04.000000 femr-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-21 18:05:04.000000 femr-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.393862 femr-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-21 18:05:04.000000 femr-0.2.3/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 18:05:04.000000 femr-0.2.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 18:05:04.000000 femr-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-21 18:05:04.000000 femr-0.2.3/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-21 18:05:04.000000 femr-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-21 18:05:04.000000 femr-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-21 18:05:09.409865 femr-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-21 18:05:04.000000 femr-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 18:05:04.000000 femr-0.2.3/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-21 18:05:04.000000 femr-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 18:05:09.409865 femr-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.389862 femr-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.397863 femr-0.2.3/src/femr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.397863 femr-0.2.3/src/femr/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/featurizers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21282 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/featurizers/featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/featurizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.397863 femr-0.2.3/src/femr/labelers/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/labelers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/labelers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/labelers/omop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/src/femr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19602 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/rmsnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/models/xformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/pat_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/src/femr/post_etl_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/post_etl_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/post_etl_pipelines/stanford.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/splits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/stat_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/src/femr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-03-21 18:05:04.000000 femr-0.2.3/src/femr/transforms/stanford.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.409865 femr-0.2.3/src/femr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-21 18:05:09.000000 femr-0.2.3/src/femr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:04.000000 femr-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/tests/featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-21 18:05:04.000000 femr-0.2.3/tests/featurizers/test_OnlineStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-03-21 18:05:04.000000 femr-0.2.3/tests/featurizers/test_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-21 18:05:04.000000 femr-0.2.3/tests/femr_test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/tests/labelers/
+-rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-03-21 18:05:04.000000 femr-0.2.3/tests/labelers/test_CodeLabelers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-03-21 18:05:04.000000 femr-0.2.3/tests/labelers/test_TimeHorizonEventLabeler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-03-21 18:05:04.000000 femr-0.2.3/tests/models/test_batch_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-21 18:05:04.000000 femr-0.2.3/tests/models/test_survival_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-21 18:05:04.000000 femr-0.2.3/tests/test_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-03-21 18:05:04.000000 femr-0.2.3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.389862 femr-0.2.3/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.401863 femr-0.2.3/tools/stanford/
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-21 18:05:04.000000 femr-0.2.3/tools/stanford/download_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/1_Ontology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/2_Labeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/3_Count Featurization And Modeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/4_Train CLMBR.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/5_CLMBR Featurization And Modeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20018 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/6_Train MOTOR.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9580 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/7_MOTOR Featurization And Modeling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/input/clmbr_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/clmbr_model/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/clmbr_model/dictionary.msgpack
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/clmbr_model/main_split.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   317136 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/clmbr_model/model.safetensors
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/labels.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/input/meds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/input/meds/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    33814 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/meds/data/patients.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/meds/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)   208054 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/meds/ontology.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.405864 femr-0.2.3/tutorials/input/motor_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/motor_model/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/motor_model/dictionary.msgpack
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/motor_model/main_split.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   342424 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/input/motor_model/model.safetensors
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.409865 femr-0.2.3/tutorials/synthetic_data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/synthetic_data_generation/generate_patients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:09.409865 femr-0.2.3/tutorials/trash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:04.000000 femr-0.2.3/tutorials/trash/.gitkeep
```

### Comparing `femr-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `femr-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `femr-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/.github/workflows/build.yaml` & `femr-0.2.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/.github/workflows/tests.yaml` & `femr-0.2.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/.mypy.ini` & `femr-0.2.3/.mypy.ini`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/.pre-commit-config.yaml` & `femr-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/LICENSE` & `femr-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/PKG-INFO` & `femr-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22
 Requires-Dist: scipy>=1.6
 Requires-Dist: scikit-learn>=0.24
```

### Comparing `femr-0.2.2/README.md` & `femr-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/pyproject.toml` & `femr-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/featurizers/core.py` & `femr-0.2.3/src/femr/featurizers/core.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/featurizers/featurizers.py` & `femr-0.2.3/src/femr/featurizers/featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/featurizers/utils.py` & `femr-0.2.3/src/femr/featurizers/utils.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/hf_utils.py` & `femr-0.2.3/src/femr/hf_utils.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/index.py` & `femr-0.2.3/src/femr/index.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/labelers/core.py` & `femr-0.2.3/src/femr/labelers/core.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/labelers/omop.py` & `femr-0.2.3/src/femr/labelers/omop.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/models/config.py` & `femr-0.2.3/src/femr/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         attention_width: int = 496,
         use_normed_ages: bool = False,
         use_bias: bool = True,
         hidden_act: str = "gelu",
         **kwargs,
     ) -> None:
         """Defined a configuration for a FEMR Transformer.
-        
+
         Arguments:
             vocab_size: The number of tokens in the vocabulary
-            is_hierarchical: Whether to use a hierarchical vocabulary. See FEMRTokenizer for more information.
+            is_hierarchical: Whether to use a hierarchical vocabulary. See FEMRTokenizer for more information
             hidden_size: The internal representation size
             intermediate_size: The size of the FFN in the transformer layers
             n_heads: The number of attention heads
             n_layers: The number of transformer encoder layers
-            attention_width: FEMR by default uses a local attention transformer. This defines the width of those attention windows.
+            attention_width: FEMR by default uses a local attention transformer with a width defined here
             use_normed_ages: Whether or not to provide normalized ages as a feature to the model
-            use_bias: Whether or not to use bias terms in the transformer layers. Current research indicates that this should be set to False.
-            hidden_act: The type of activation function to use in the transformer.
-            """
+            use_bias: Whether or not to use bias terms in the transformer layers
+            hidden_act: The type of activation function to use in the transformer
+        """
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.is_hierarchical = is_hierarchical
 
         self.hidden_size = hidden_size
         self.intermediate_size = intermediate_size
@@ -52,35 +52,37 @@
 
 
 class FEMRTaskConfig(transformers.PretrainedConfig):
     def __init__(self, task_type: str = "", task_kwargs: Mapping[str, Any] = {}, **kwargs):
         """A generic FEMR task definition. This holds state used for initalizing a tasks.py class.
 
         Task.get_task_config returns the task type and kwargs used to initialize this.
-        
+
         Arguments:
-            task_type: The name of the task. 
+            task_type: The name of the task.
             task_kwargs: Arbitrary arguments used to store state for that task.
         """
         super().__init__(**kwargs)
         self.task_type = task_type
         self.task_kwargs = task_kwargs
 
 
 class FEMRModelConfig(transformers.PretrainedConfig):
     """A model config is defined as the combination of a transformer config and a task config."""
+
     def __init__(
         self,
         transformer_config: Optional[Dict[str, Any]] = None,
         task_config: Optional[Dict[str, Any]] = None,
         **kwargs,
     ):
         """A combination of a transformer config and a task config.
-        
-        It is possible to initialize this with only a transformer config, in which case the model will be configured for inference only.
+
+        It is possible to initialize this with only a transformer config, in which
+        case the model will be configured for inference only.
         """
         super().__init__(**kwargs)
         if transformer_config is None:
             transformer_config = {}
         self.transformer_config = FEMRTransformerConfig(**transformer_config)
 
         self.task_config: Optional[FEMRTaskConfig]
```

### Comparing `femr-0.2.2/src/femr/models/processor.py` & `femr-0.2.3/src/femr/models/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
 import collections
 import datetime
 import functools
-from typing import Any, Dict, List, Mapping, Tuple, Optional
+from typing import Any, Dict, List, Mapping, Optional, Tuple
 
 import datasets
+import meds
 import numpy as np
 import torch.utils.data
 
-import meds
-
 import femr.hf_utils
 import femr.models.tokenizer
 import femr.pat_utils
 
 
 def map_preliminary_batch_stats(batch, indices, *, processor: FEMRBatchProcessor, max_length: int):
     """
     This function creates preliminary batch statistics, to be used for final batching.
 
-    The overall problem this is trying to solve is that Patient records can be very long, so when we featurize patients we actually featurize subsequences of patients.
+    The overall problem this is trying to solve is that Patient records can be very long, so
+    when we featurize patients we actually featurize subsequences of patients.
 
-    AKA every patient in a batch is actually (patient_id, start_index, length), which specifies a subsequence of the patient.
+    AKA every patient in a batch is actually (patient_id, start_index, length), which
+    specifies a subsequence of the patient.
 
-    The trickiness becomes when a particular patient has multiple labels, some of which will require multiple subsequences.
+    The trickiness becomes when a particular patient has multiple labels, some
+    of which will require multiple subsequences.
 
-    The goal of this function is to compute the list [(patient_id, start_index, length)] such that every label is covered
-    by at least one batch. Note that some labels will be covered multiple times.
+    The goal of this function is to compute the list [(patient_id, start_index, length)] such
+    that every label is covered by at least one batch. Note that some labels will be covered multiple times.
+
+    Note that there is a special setting for tasks that don't need exact labeling
+    (needs_exact in tasks.py returns False).
 
-    Note that there is a special setting for tasks that don't need exact labeling (needs_exact in tasks.py returns False).
     For these patients we only generate one tuple for them, and drop some labels.
 
     Later code will then take [(patient_id, start_index, length)], and create actual batches.
     """
     lengths = []
 
     for patient_index, patient_id, events in zip(indices, batch["patient_id"], batch["events"]):
@@ -76,15 +80,16 @@
     lengths1.extend(lengths2)
 
     return lengths1
 
 
 class BatchCreator:
     """The BatchCreator is designed to generate batches from patient data."""
-    def __init__(self, tokenizer: femr.models.FEMRTokenizer, task: Optional[femr.tasks.Task] = None):
+
+    def __init__(self, tokenizer: femr.models.tokenizer.FEMRTokenizer, task: Optional[femr.models.tasks.Task] = None):
         """Initialize a BatchCreator, with a tokenizer, and optionally a task."""
         self.tokenizer = tokenizer
         self.task = task
 
     def start_batch(self):
         """Start a batch."""
         self.patient_ids = []
@@ -107,28 +112,29 @@
         self.label_indices = []
 
         if self.task is not None:
             self.task.start_batch()
 
     def add_patient(self, patient: meds.Patient, offset: int = 0, max_length: Optional[int] = None):
         """Add a patient to the current batch.
-        
+
         Note that the two optional parameters are used to add a subset of a patient to a batch.
-        It is generally recommended to never manually use offset or max_length as you should rely on FEMRBatchProcessor.convert_dataset.
+
+        It is generally recommended to never manually use offset or max_length as
+        you should rely on FEMRBatchProcessor.convert_dataset.
 
         Arguments:
             patient: The patient to add.
             offset: The offset into the patient to featurize.
-            max_length: The maximum length of the batch sequence. There is no max when left at None. 
+            max_length: The maximum length of the batch sequence. There is no max when left at None.
 
         """
         current_date = None
         last_time = None
 
-
         # The overall algorithm here is a bit complex
         # First we featurize the entire patient
         # Then we slice the patient indices according to offset and max_length
 
         # These are the indices of the labels into the patient vectors
         per_patient_label_indices = []
 
@@ -143,17 +149,17 @@
 
         # For a regular tokenizer, we just have tokens
         per_patient_tokens = []
 
         # For a hierarchical tokenizer, we have a more complex setup
         # These are designed to match the inputs required for an EmbeddingBag.
         # See PyTorch's EmbeddingBag documentation to understand what these mean.
-        per_patient_hierarchical_tokens = []
-        per_patient_hierarchical_weights = []
-        per_patient_token_indices = [0]
+        per_patient_hierarchical_tokens: List[int] = []
+        per_patient_hierarchical_weights: List[float] = []
+        per_patient_token_indices: List[int] = [0]
 
         if self.task is not None:
             self.task.start_patient(patient, self.tokenizer.ontology)
 
         birth = femr.pat_utils.get_patient_birthdate(patient)
         self.tokenizer.start_patient()
 
@@ -184,25 +190,25 @@
                     for _ in range(num_added):
                         per_patient_label_indices.append(len(per_patient_ages) - 1)
 
                 if not self.tokenizer.is_hierarchical:
                     assert len(features) == 1
                     per_patient_tokens.append(features[0])
                 else:
+                    assert weights is not None
                     per_patient_hierarchical_tokens.extend(features)
                     per_patient_hierarchical_weights.extend(weights)
                     per_patient_token_indices.append(len(per_patient_hierarchical_tokens))
 
                 per_patient_ages.append((event["time"] - birth) / datetime.timedelta(days=1))
                 per_patient_normalized_ages.append(self.tokenizer.normalize_age(event["time"] - birth))
                 per_patient_timestamps.append(event["time"].replace(tzinfo=datetime.timezone.utc).timestamp())
 
                 last_time = event["time"]
 
-                
         if self.task is not None and last_time is not None:
             num_added = self.task.add_event(last_time, None, None)
             for _ in range(num_added):
                 per_patient_label_indices.append(len(per_patient_ages) - 1)
 
         # Now we want to actually add the patient data to the batch.
         # This will involve some clever slicing.
@@ -214,78 +220,76 @@
         else:
             length_to_add = length_found - offset
 
         start_index = len(self.ages)
 
         # Let's add the constants first
         self.valid_tokens.extend([True] * length_to_add)
-        self.patient_ids.extend([patient['patient_id']] * length_to_add)
+        self.patient_ids.extend([patient["patient_id"]] * length_to_add)
         self.offsets.append(offset)
         self.patient_lengths.append(length_to_add)
 
         # Ages, normalized ages and timestamps are also easy to add
-        self.ages.extend(per_patient_ages[offset: offset + length_to_add])
-        self.normalized_ages.extend(per_patient_normalized_ages[offset: offset + length_to_add])
-        self.timestamps.extend(per_patient_timestamps[offset: offset + length_to_add])
+        self.ages.extend(per_patient_ages[offset : offset + length_to_add])
+        self.normalized_ages.extend(per_patient_normalized_ages[offset : offset + length_to_add])
+        self.timestamps.extend(per_patient_timestamps[offset : offset + length_to_add])
 
         if not self.tokenizer.is_hierarchical:
             # Easy for simple tokenizer
-            self.tokens.extend(per_patient_tokens[offset: offset + length_to_add])
+            self.tokens.extend(per_patient_tokens[offset : offset + length_to_add])
         else:
             # Hierarchical tokenizer is more complex since we have to shift the indices as well
             # Remember, these arrays are all designed for PyTorch EmbeddingBag
 
             # We need to get the start and end at a particular offset
             internal_start = per_patient_token_indices[offset]
             internal_end = per_patient_token_indices[offset + length_to_add]
-            
-            # We need to offset the token indices to account for the existing tokens            
-            self.token_indices.extend([len(self.hierarchical_tokens) - internal_start + value for value in per_patient_token_indices[offset + 1:offset + length_to_add + 1]])
 
-            self.hierarchical_tokens.extend(per_patient_hierarchical_tokens[internal_start: internal_end])
-            self.hierarchical_weights.extend(per_patient_hierarchical_weights[internal_start: internal_end])
+            # We need to offset the token indices to account for the existing tokens
+            self.token_indices.extend(
+                [
+                    len(self.hierarchical_tokens) - internal_start + value
+                    for value in per_patient_token_indices[offset + 1 : offset + length_to_add + 1]
+                ]
+            )
 
+            self.hierarchical_tokens.extend(per_patient_hierarchical_tokens[internal_start:internal_end])
+            self.hierarchical_weights.extend(per_patient_hierarchical_weights[internal_start:internal_end])
 
         # The label indices are also a bit tricky as they have to be offset accordingly.
         # We also need to collect good labels that should be sent to the final numpy arrays.
         labels_to_add = []
         for i, label_index in enumerate(per_patient_label_indices):
             corrected_label = label_index - offset
 
             if 0 <= corrected_label < length_to_add:
                 labels_to_add.append(i)
                 self.label_indices.append(start_index + corrected_label)
 
         if self.task is not None:
             self.task.add_patient_labels(labels_to_add)
 
-
     def get_batch_data(self):
         """Convert the batch to numpy arrays. The data structure is defined inline in this function."""
         if self.tokenizer.vocab_size <= 2**15:
             token_dtype = np.int16
         else:
             token_dtype = np.int32
 
         transformer = {
             # Whether or not the token is valid at this index
             "valid_tokens": np.array(self.valid_tokens),
-
             # The age of the patient in days at this index
             "ages": np.array(self.ages, dtype=np.float32),
-
             # The normalized ages at this index
             "normalized_ages": np.array(self.normalized_ages, dtype=np.float16),
-
             # The timestamp (in seconds) at this index
             "timestamps": np.array(self.timestamps, dtype=np.int64),
-
             # The length of the patient
             "patient_lengths": np.array(self.patient_lengths, dtype=np.int32),
-
             # The indices of the labels
             "label_indices": np.array(self.label_indices, dtype=np.int32),
         }
 
         if not self.tokenizer.is_hierarchical:
             # For a single tokenizer, these are simple the token indices
             transformer["tokens"] = np.array(self.tokens, dtype=token_dtype)
@@ -349,32 +353,41 @@
         return data
     else:
         raise RuntimeError("Could not convert item of type " + str(type(data)))
 
 
 class FEMRBatchProcessor:
     """The FEMR Batch processor creates batches for processing by a transformer."""
+
     def __init__(self, tokenizer, task=None):
         self.creator = BatchCreator(tokenizer, task)
 
-    def convert_patient(self, patient: meds.Patient, offset: int =0, max_length: Optional[int]=None, tensor_type=None, **formatter_kwargs):
+    def convert_patient(
+        self,
+        patient: meds.Patient,
+        offset: int = 0,
+        max_length: Optional[int] = None,
+        tensor_type=None,
+        **formatter_kwargs,
+    ):
         """Convert a single patient to a batch.
-        
+
         Note that this can also convert parts of a patient to a batch using the offset and max_length parameters.
         This is useful for processing long patients.
 
-        NOTE: This function is primarily for debugging purposes. It is recommended to use convert_dataset for maximum correctness and efficiency.
+        NOTE: This function is primarily for debugging purposes. It is
+        recommended to use convert_dataset for maximum correctness and efficiency.
 
         Arguments:
             patient: The patient to convert
             offset: The integer offset into the patient to convert
             max_length: The maximum length to convert
             tensor_type: The dataset to return
             formatter_kwargs: Arguments for a datasets formatter when converting datatypes
-            
+
         Returns:
             A batch, ready to be fed into a FEMR transformer model
         """
         self.creator.start_batch()
         self.creator.add_patient(patient, offset=offset, max_length=max_length)
         batch_data = self.creator.get_batch_data()
         if tensor_type is not None:
@@ -385,21 +398,21 @@
     def collate(self, batches: List[Mapping[str, Any]]) -> Mapping[str, Any]:
         """A collate function that prepares batches for being fed into a dataloader."""
         assert len(batches) == 1, "Can only have one batch when collating"
         return {"batch": _add_dimension(self.creator.cleanup_batch(batches[0]))}
 
     def convert_dataset(self, dataset, tokens_per_batch: int, min_patients_per_batch: int = 4, num_proc: int = 1):
         """Convert an entire dataset to batches.
-        
+
         Arguments:
             dataset: A huggingface dataset containing MEDS patients
             tokens_per_batch: The number of tokens allowed per batch
             min_patients_per_batch: The minimum number of patients per batch
             num_proc: The number of processers to use when converting
-        
+
         Returns:
             A huggingface dataset object containing batches
         """
         if isinstance(dataset, datasets.DatasetDict):
             return datasets.DatasetDict(
                 {
                     k: self.convert_dataset(v, tokens_per_batch, min_patients_per_batch, num_proc)
```

### Comparing `femr-0.2.2/src/femr/models/rmsnorm.py` & `femr-0.2.3/src/femr/models/rmsnorm.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/models/tasks.py` & `femr-0.2.3/src/femr/models/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,27 @@
         ...
 
     @abc.abstractmethod
     def start_patient(self, patient: meds.Patient, ontology: Optional[femr.ontology.Ontology]) -> None:
         ...
 
     @abc.abstractmethod
+    def add_patient_labels(self, patient_label_offsets: List[int]) -> None:
+        ...
+
+    @abc.abstractmethod
     def needs_exact(self) -> bool:
         ...
 
     @abc.abstractmethod
     def add_event(
-        self, current_date: datetime.datetime, next_date: datetime.datetime, next_features: Sequence[int]
+        self,
+        current_date: datetime.datetime,
+        next_date: Optional[datetime.datetime],
+        next_features: Optional[Sequence[int]],
     ) -> int:
         ...
 
     @abc.abstractmethod
     def get_batch_data(self) -> Mapping[str, np.ndarray]:
         ...
 
@@ -84,15 +91,18 @@
         pass
 
     def add_patient_labels(self, _patient_label_offsets: List[int]) -> None:
         """As there is no per label state, this is ignored"""
         pass
 
     def add_event(
-        self, current_date: datetime.datetime, next_date: datetime.datetime, next_features: Optional[Sequence[int]] = None
+        self,
+        current_date: datetime.datetime,
+        next_date: Optional[datetime.datetime],
+        next_features: Optional[Sequence[int]] = None,
     ) -> int:
         has_label = False
 
         while True:
             if self.current_label_index == len(self.current_labels):
                 break
 
@@ -107,15 +117,15 @@
 
             if is_valid:
                 has_label = True
                 self.current_label_index += 1
             else:
                 # The next label isn't valid, so we have to break here
                 break
-        
+
         if has_label:
             return 1
         else:
             return 0
 
     def get_batch_data(self) -> Mapping[str, np.ndarray]:
         return {}
@@ -139,15 +149,18 @@
     def start_batch(self) -> None:
         self.batch_labels: List[int] = []
 
     def add_patient_labels(self, patient_label_offsets: List[int]) -> None:
         self.batch_labels.extend([self.per_patient_batch_labels[i] for i in patient_label_offsets])
 
     def add_event(
-        self, current_date: datetime.datetime, next_date: datetime.datetime, next_features: Optional[Sequence[int]] = None
+        self,
+        current_date: datetime.datetime,
+        next_date: Optional[datetime.datetime],
+        next_features: Optional[Sequence[int]] = None,
     ) -> int:
         if next_features is None:
             return 0
 
         if len(next_features) != 1:
             raise RuntimeError("Only supports one for right now")
 
@@ -322,16 +335,16 @@
             ),
         )
 
     def start_patient(self, patient: meds.Patient, ontology: Optional[femr.ontology.Ontology]) -> None:
         assert ontology
         self.calculator = SurvivalCalculator(ontology, patient, self.pretraining_task_codes)
 
-        self.per_patient_censor_time = []
-        self.per_patient_time_sparse = {
+        self.per_patient_censor_time: List[float] = []
+        self.per_patient_time_sparse: Dict[str, List[float]] = {
             "data": [],
             "indices": [],
             "indptr": [0],
         }
 
     def needs_exact(self) -> bool:
         return False
@@ -346,23 +359,26 @@
         }
 
     def add_patient_labels(self, patient_label_offsets: List[int]) -> None:
         """Add per-patient labels to the global task labels."""
         self.censor_time.extend([self.per_patient_censor_time[i] for i in patient_label_offsets])
 
         for index in patient_label_offsets:
-            start = self.per_patient_time_sparse['indptr'][index]
-            end = self.per_patient_time_sparse['indptr'][index + 1]
+            start = int(self.per_patient_time_sparse["indptr"][index])
+            end = int(self.per_patient_time_sparse["indptr"][index + 1])
 
-            self.time_sparse['data'].extend(self.per_patient_time_sparse['data'][start:end])
-            self.time_sparse['indices'].extend(self.per_patient_time_sparse['indices'][start:end])
-            self.time_sparse['indptr'].append(len(self.time_sparse['indices']))
+            self.time_sparse["data"].extend(self.per_patient_time_sparse["data"][start:end])
+            self.time_sparse["indices"].extend(self.per_patient_time_sparse["indices"][start:end])
+            self.time_sparse["indptr"].append(len(self.time_sparse["indices"]))
 
     def add_event(
-        self, current_date: datetime.datetime, next_date: datetime.datetime, next_features: Sequence[int]
+        self,
+        current_date: datetime.datetime,
+        next_date: Optional[datetime.datetime],
+        next_features: Optional[Sequence[int]] = None,
     ) -> int:
         if not should_make_survival_prediction(current_date, next_date):
             return 0
 
         censor_time, tte = self.calculator.get_future_events_for_time(current_date)
 
         if len(tte) == 0:
```

### Comparing `femr-0.2.2/src/femr/models/tokenizer.py` & `femr-0.2.3/src/femr/models/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import bisect
 import collections
 import datetime
 import functools
 import math
 import os
-from typing import Any, Dict, Mapping, Optional, Set, Union, Tuple, List
+from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 import meds
 import msgpack
 import numpy as np
 import transformers
 
 import femr.hf_utils
@@ -386,15 +386,17 @@
 
     def start_patient(self):
         """Compute per-patient statistics that are required to generate features."""
 
         # This is currently a null-op, but is required for cost featurization
         pass
 
-    def get_feature_codes(self, _time: datetime.datetime, measurement: meds.Measurement) -> Tuple[List[int], Optional[List[float]]]:
+    def get_feature_codes(
+        self, _time: datetime.datetime, measurement: meds.Measurement
+    ) -> Tuple[List[int], Optional[List[float]]]:
         """Get codes for the provided measurement and time"""
 
         # Note that time is currently not used in this code, but it is required for cost featurization
         if self.is_hierarchical:
             assert self.ontology is not None
             codes = [
                 self.code_lookup[parent]
```

### Comparing `femr-0.2.2/src/femr/models/transformer.py` & `femr-0.2.3/src/femr/models/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import collections
-import datetime
 import math
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
 import datasets
 import meds
 import numpy as np
 import torch
@@ -192,15 +191,15 @@
         logits = self.final_layer(features)
         labels = batch["labels"]
         loss = F.cross_entropy(logits, labels)
 
         if not return_logits:
             logits = None
 
-        return loss, {'logits': logits}
+        return loss, {"logits": logits}
 
 
 class MOTORTaskHead(nn.Module):
     def __init__(
         self,
         hidden_size: int,
         pretraining_task_info: List[Tuple[str, float]],
@@ -237,15 +236,15 @@
         event_loss = -math.log(2) * torch.where(batch["is_event"], time_dependent_logits, 0).mean()
 
         loss = survival_loss + event_loss
 
         if not return_logits:
             time_dependent_logits = None
 
-        return loss, {'time_dependent_logits': time_dependent_logits}
+        return loss, {"time_dependent_logits": time_dependent_logits}
 
 
 def remove_first_dimension(data: Any) -> Any:
     if isinstance(data, collections.abc.Mapping):
         return {k: remove_first_dimension(v) for k, v in data.items()}
     elif isinstance(data, torch.Tensor):
         assert data.shape[0] == 1
@@ -300,15 +299,15 @@
             if return_logits or return_reprs:
                 result["timestamps"] = batch["transformer"]["timestamps"][batch["transformer"]["label_indices"]]
                 result["patient_ids"] = batch["patient_ids"][batch["transformer"]["label_indices"]]
             return loss, result
         else:
             loss = 0
             features = features.reshape(-1, features.shape[-1])
-            if 'task' in batch:
+            if "task" in batch:
                 features = features[batch["transformer"]["label_indices"], :]
                 result = {
                     "timestamps": batch["transformer"]["timestamps"][batch["transformer"]["label_indices"]],
                     "patient_ids": batch["patient_ids"][batch["transformer"]["label_indices"]],
                     "representations": features,
                 }
             else:
@@ -317,15 +316,14 @@
                     "patient_ids": batch["patient_ids"],
                     "representations": features,
                 }
 
             return loss, result
 
 
-
 def compute_features(
     dataset: datasets.Dataset,
     model_path: str,
     labels: List[meds.Label],
     num_proc: int = 1,
     tokens_per_batch: int = 1024,
     device: Optional[torch.device] = None,
@@ -360,10 +358,10 @@
             _, result = model(batch, return_reprs=True)
             all_patient_ids.append(result["patient_ids"].cpu().numpy())
             all_feature_times.append(result["timestamps"].cpu().numpy())
             all_representations.append(result["representations"].cpu().numpy())
 
     return {
         "patient_ids": np.concatenate(all_patient_ids),
-        "feature_times": np.concatenate(all_feature_times).astype('datetime64[s]'),
+        "feature_times": np.concatenate(all_feature_times).astype("datetime64[s]"),
         "features": np.concatenate(all_representations),
     }
```

### Comparing `femr-0.2.2/src/femr/models/xformers.py` & `femr-0.2.3/src/femr/models/xformers.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/ontology.py` & `femr-0.2.3/src/femr/ontology.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/post_etl_pipelines/stanford.py` & `femr-0.2.3/src/femr/post_etl_pipelines/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/splits.py` & `femr-0.2.3/src/femr/splits.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/stat_utils.py` & `femr-0.2.3/src/femr/stat_utils.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/transforms/__init__.py` & `femr-0.2.3/src/femr/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr/transforms/stanford.py` & `femr-0.2.3/src/femr/transforms/stanford.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/src/femr.egg-info/PKG-INFO` & `femr-0.2.3/src/femr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Framework for Electronic Medical Records. A python package for building models using EHR data.
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22
 Requires-Dist: scipy>=1.6
 Requires-Dist: scikit-learn>=0.24
```

### Comparing `femr-0.2.2/src/femr.egg-info/SOURCES.txt` & `femr-0.2.3/src/femr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/featurizers/test_OnlineStatistics.py` & `femr-0.2.3/tests/featurizers/test_OnlineStatistics.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/featurizers/test_featurizers.py` & `femr-0.2.3/tests/featurizers/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/femr_test_tools.py` & `femr-0.2.3/tests/femr_test_tools.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/labelers/test_CodeLabelers.py` & `femr-0.2.3/tests/labelers/test_CodeLabelers.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/labelers/test_TimeHorizonEventLabeler.py` & `femr-0.2.3/tests/labelers/test_TimeHorizonEventLabeler.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/models/test_batch_creator.py` & `femr-0.2.3/tests/models/test_batch_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,75 @@
-import femr.models.processor
-import femr.models.tasks
 import datetime
 
 from femr_test_tools import create_patients_dataset
 
+import femr.models.processor
+import femr.models.tasks
+
+
 class DummyTokenizer:
     def __init__(self, is_hierarchical: bool = False):
         self.is_hierarchical = is_hierarchical
         self.ontology = None
         self.vocab_size = 100
 
     def start_patient(self):
         pass
 
     def get_feature_codes(self, time, measurement):
-        if measurement['code'] == 'SNOMED/184099003':
+        if measurement["code"] == "SNOMED/184099003":
             return [1], None
         else:
-            return [int(measurement['code'])], None
+            return [int(measurement["code"])], None
 
     def normalize_age(self, age):
         return 0.5
 
+
 def assert_two_batches_equal_third(batch1, batch2, batch3):
     """This asserts that batch1 + batch2 = batchs3"""
-    assert batch3['patient_ids'].tolist() == batch1['patient_ids'].tolist() + batch2['patient_ids'].tolist()
-
-    assert batch3['transformer']['ages'].tolist() == batch1['transformer']['ages'].tolist() + batch2['transformer']['ages'].tolist()
-    assert batch3['transformer']['timestamps'].tolist() == batch1['transformer']['timestamps'].tolist() + batch2['transformer']['timestamps'].tolist()
+    assert batch3["patient_ids"].tolist() == batch1["patient_ids"].tolist() + batch2["patient_ids"].tolist()
 
+    assert (
+        batch3["transformer"]["ages"].tolist()
+        == batch1["transformer"]["ages"].tolist() + batch2["transformer"]["ages"].tolist()
+    )
+    assert (
+        batch3["transformer"]["timestamps"].tolist()
+        == batch1["transformer"]["timestamps"].tolist() + batch2["transformer"]["timestamps"].tolist()
+    )
 
     # Checking the label indices is a bit more involved as we have to map to age/patient id and then check that
     target_label_ages = []
     target_label_patient_ids = []
 
-    for label_index in batch1['transformer']['label_indices'].tolist():
-        target_label_ages.append(batch1['transformer']['ages'][label_index])
-        target_label_patient_ids.append(batch1['patient_ids'][label_index])
-
-    for label_index in batch2['transformer']['label_indices'].tolist():
-        target_label_ages.append(batch2['transformer']['ages'][label_index])
-        target_label_patient_ids.append(batch2['patient_ids'][label_index])
+    for label_index in batch1["transformer"]["label_indices"].tolist():
+        target_label_ages.append(batch1["transformer"]["ages"][label_index])
+        target_label_patient_ids.append(batch1["patient_ids"][label_index])
+
+    for label_index in batch2["transformer"]["label_indices"].tolist():
+        target_label_ages.append(batch2["transformer"]["ages"][label_index])
+        target_label_patient_ids.append(batch2["patient_ids"][label_index])
 
     actual_label_ages = []
     actual_label_patient_ids = []
 
-    for label_index in batch3['transformer']['label_indices'].tolist():
-        actual_label_ages.append(batch3['transformer']['ages'][label_index])
-        actual_label_patient_ids.append(batch3['patient_ids'][label_index])
+    for label_index in batch3["transformer"]["label_indices"].tolist():
+        actual_label_ages.append(batch3["transformer"]["ages"][label_index])
+        actual_label_patient_ids.append(batch3["patient_ids"][label_index])
 
     assert target_label_ages == actual_label_ages
     assert target_label_patient_ids == actual_label_patient_ids
 
-    if 'tokens' in batch3['transformer']:
-        assert batch3['transformer']['tokens'].tolist() == batch1['transformer']['tokens'].tolist() + batch2['transformer']['tokens'].tolist()
+    if "tokens" in batch3["transformer"]:
+        assert (
+            batch3["transformer"]["tokens"].tolist()
+            == batch1["transformer"]["tokens"].tolist() + batch2["transformer"]["tokens"].tolist()
+        )
+
 
 def test_two_patients_concat_no_task():
     tokenizer = DummyTokenizer()
 
     fake_patients = create_patients_dataset(10)
 
     fake_patient1 = fake_patients[1]
@@ -71,63 +83,65 @@
     data_for_patient1 = creator.get_batch_data()
 
     creator.start_batch()
     creator.add_patient(fake_patient2)
 
     data_for_patient2 = creator.get_batch_data()
 
-    
     creator.start_batch()
     creator.add_patient(fake_patient1)
     creator.add_patient(fake_patient2)
 
     data_for_patients = creator.get_batch_data()
 
     assert_two_batches_equal_third(data_for_patient1, data_for_patient2, data_for_patients)
 
+
 def test_split_patients_concat_no_task():
     tokenizer = DummyTokenizer()
 
     fake_patients = create_patients_dataset(10)
 
     fake_patient = fake_patients[1]
 
     creator = femr.models.processor.BatchCreator(tokenizer)
 
     creator.start_batch()
     creator.add_patient(fake_patient)
 
     data_for_patient = creator.get_batch_data()
 
-    length = len(data_for_patient['transformer']['timestamps'])
-    
+    length = len(data_for_patient["transformer"]["timestamps"])
+
     creator.start_batch()
-    creator.add_patient(fake_patient, offset=0, max_length = length // 2)
+    creator.add_patient(fake_patient, offset=0, max_length=length // 2)
 
     data_for_part1 = creator.get_batch_data()
 
     creator.start_batch()
-    creator.add_patient(fake_patient, offset=length // 2, max_length = None)
+    creator.add_patient(fake_patient, offset=length // 2, max_length=None)
 
     data_for_part2 = creator.get_batch_data()
 
     assert_two_batches_equal_third(data_for_part1, data_for_part2, data_for_patient)
 
+
 def test_two_patients_concat_task():
     tokenizer = DummyTokenizer()
 
     fake_patients = create_patients_dataset(10)
-    
-    task = femr.models.tasks.LabeledPatientTask([
-        {'patient_id': 1, 'prediction_time': datetime.datetime(2011, 7, 6)},
-        {'patient_id': 1, 'prediction_time': datetime.datetime(2017, 1, 1)},
-        
-        {'patient_id': 5, 'prediction_time': datetime.datetime(2011, 11, 6)},
-        {'patient_id': 5, 'prediction_time': datetime.datetime(2017, 2, 1)}
-    ])
+
+    task = femr.models.tasks.LabeledPatientTask(
+        [
+            {"patient_id": 1, "prediction_time": datetime.datetime(2011, 7, 6)},
+            {"patient_id": 1, "prediction_time": datetime.datetime(2017, 1, 1)},
+            {"patient_id": 5, "prediction_time": datetime.datetime(2011, 11, 6)},
+            {"patient_id": 5, "prediction_time": datetime.datetime(2017, 2, 1)},
+        ]
+    )
 
     fake_patient1 = fake_patients[1]
     fake_patient2 = fake_patients[5]
 
     creator = femr.models.processor.BatchCreator(tokenizer, task=task)
 
     creator.start_batch()
@@ -136,48 +150,50 @@
     data_for_patient1 = creator.get_batch_data()
 
     creator.start_batch()
     creator.add_patient(fake_patient2)
 
     data_for_patient2 = creator.get_batch_data()
 
-    
     creator.start_batch()
     creator.add_patient(fake_patient1)
     creator.add_patient(fake_patient2)
 
     data_for_patients = creator.get_batch_data()
 
     assert_two_batches_equal_third(data_for_patient1, data_for_patient2, data_for_patients)
 
+
 def test_split_patients_concat_task():
     tokenizer = DummyTokenizer()
 
     fake_patients = create_patients_dataset(10)
 
     fake_patient = fake_patients[1]
 
-    task = femr.models.tasks.LabeledPatientTask([
-        {'patient_id': 1, 'prediction_time': datetime.datetime(2011, 7, 6)},
-        {'patient_id': 1, 'prediction_time': datetime.datetime(2017, 1, 1)},
-    ])
+    task = femr.models.tasks.LabeledPatientTask(
+        [
+            {"patient_id": 1, "prediction_time": datetime.datetime(2011, 7, 6)},
+            {"patient_id": 1, "prediction_time": datetime.datetime(2017, 1, 1)},
+        ]
+    )
 
     creator = femr.models.processor.BatchCreator(tokenizer, task=task)
 
     creator.start_batch()
     creator.add_patient(fake_patient)
 
     data_for_patient = creator.get_batch_data()
 
-    length = len(data_for_patient['transformer']['timestamps'])
-    
+    length = len(data_for_patient["transformer"]["timestamps"])
+
     creator.start_batch()
-    creator.add_patient(fake_patient, offset=0, max_length = length // 2)
+    creator.add_patient(fake_patient, offset=0, max_length=length // 2)
 
     data_for_part1 = creator.get_batch_data()
 
     creator.start_batch()
-    creator.add_patient(fake_patient, offset=length // 2, max_length = None)
+    creator.add_patient(fake_patient, offset=length // 2, max_length=None)
 
     data_for_part2 = creator.get_batch_data()
 
-    assert_two_batches_equal_third(data_for_part1, data_for_part2, data_for_patient)
+    assert_two_batches_equal_third(data_for_part1, data_for_part2, data_for_patient)
```

### Comparing `femr-0.2.2/tests/models/test_survival_calculator.py` & `femr-0.2.3/tests/models/test_survival_calculator.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/test_ontology.py` & `femr-0.2.3/tests/test_ontology.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tests/test_transforms.py` & `femr-0.2.3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tools/stanford/download_bigquery.py` & `femr-0.2.3/tools/stanford/download_bigquery.py`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/1_Ontology.ipynb` & `femr-0.2.3/tutorials/1_Ontology.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/2_Labeling.ipynb` & `femr-0.2.3/tutorials/2_Labeling.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/3_Count Featurization And Modeling.ipynb` & `femr-0.2.3/tutorials/3_Count Featurization And Modeling.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/4_Train CLMBR.ipynb` & `femr-0.2.3/tutorials/4_Train CLMBR.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/5_CLMBR Featurization And Modeling.ipynb` & `femr-0.2.3/tutorials/5_CLMBR Featurization And Modeling.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/6_Train MOTOR.ipynb` & `femr-0.2.3/tutorials/6_Train MOTOR.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/7_MOTOR Featurization And Modeling.ipynb` & `femr-0.2.3/tutorials/7_MOTOR Featurization And Modeling.ipynb`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/clmbr_model/config.json` & `femr-0.2.3/tutorials/input/clmbr_model/config.json`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/clmbr_model/dictionary.msgpack` & `femr-0.2.3/tutorials/input/clmbr_model/dictionary.msgpack`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/clmbr_model/main_split.csv` & `femr-0.2.3/tutorials/input/clmbr_model/main_split.csv`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/clmbr_model/model.safetensors` & `femr-0.2.3/tutorials/input/clmbr_model/model.safetensors`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/labels.csv` & `femr-0.2.3/tutorials/input/labels.csv`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/meds/data/patients.parquet` & `femr-0.2.3/tutorials/input/meds/data/patients.parquet`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/meds/ontology.pkl` & `femr-0.2.3/tutorials/input/meds/ontology.pkl`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/motor_model/config.json` & `femr-0.2.3/tutorials/input/motor_model/config.json`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/motor_model/dictionary.msgpack` & `femr-0.2.3/tutorials/input/motor_model/dictionary.msgpack`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/motor_model/main_split.csv` & `femr-0.2.3/tutorials/input/motor_model/main_split.csv`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/input/motor_model/model.safetensors` & `femr-0.2.3/tutorials/input/motor_model/model.safetensors`

 * *Files identical despite different names*

### Comparing `femr-0.2.2/tutorials/synthetic_data_generation/generate_patients.py` & `femr-0.2.3/tutorials/synthetic_data_generation/generate_patients.py`

 * *Files identical despite different names*

