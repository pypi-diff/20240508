# Comparing `tmp/spade_anomaly_detection-0.1.0.tar.gz` & `tmp/spade_anomaly_detection-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_anomaly_detection-0.1.0.tar", max compression
+gzip compressed data, was "spade_anomaly_detection-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spade_anomaly_detection-0.1.0.tar` & `spade_anomaly_detection-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,26 @@
--rw-r--r--   0        0        0        0 2024-05-04 00:46:42.868294 spade_anomaly_detection-0.1.0/README.md
--rw-r--r--   0        0        0      276 2024-05-04 00:46:42.872294 spade_anomaly_detection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 00:46:42.868294 spade_anomaly_detection-0.1.0/spade_anomaly_detection/__init__.py
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    30078 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14507 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/README.md
+-rw-r--r--   0        0        0     2743 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1808 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/Dockerfile
+-rw-r--r--   0        0        0     1384 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/__init__.py
+-rw-r--r--   0        0        0    26819 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_loader.py
+-rw-r--r--   0        0        0     1198 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/__init__.py
+-rw-r--r--   0        0        0    29960 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset.py
+-rw-r--r--   0        0        0     2055 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py
+-rw-r--r--   0        0        0     4475 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_utils.py
+-rw-r--r--   0        0        0    36573 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/feature_metadata.py
+-rw-r--r--   0        0        0     1570 2024-05-08 15:23:07.517925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/README.md
+-rw-r--r--   0        0        0  3671818 2024-05-08 15:23:07.529925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_10000.csv
+-rw-r--r--   0        0        0 36719403 2024-05-08 15:23:07.657925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_100000.csv
+-rw-r--r--   0        0        0  3689614 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pu_labeled.csv
+-rw-r--r--   0        0        0   582290 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv
+-rw-r--r--   0        0        0    42111 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/thyroid_labeled.csv
+-rw-r--r--   0        0        0    11656 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/occ_ensemble.py
+-rw-r--r--   0        0        0     9364 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/parameters.py
+-rw-r--r--   0        0        0      746 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/requirements.txt
+-rw-r--r--   0        0        0    23357 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/runner.py
+-rwxr-xr-x   0        0        0     1146 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/build_and_push_image.sh
+-rw-r--r--   0        0        0     3578 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh
+-rw-r--r--   0        0        0     6333 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/supervised_model.py
+-rw-r--r--   0        0        0    11178 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/task.py
+-rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.2.0/PKG-INFO
```

