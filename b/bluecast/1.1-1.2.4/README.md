# Comparing `tmp/bluecast-1.1.tar.gz` & `tmp/bluecast-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-1.1.tar", max compression
+gzip compressed data, was "bluecast-1.2.4.tar", max compression
```

## Comparing `bluecast-1.1.tar` & `bluecast-1.2.4.tar`

### file list

```diff
@@ -1,191 +1,191 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-1.1/LICENSE
--rw-r--r--   0        0        0     9144 2024-04-30 07:17:24.287488 bluecast-1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-1.1/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.1/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-1.1/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-1.1/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    21664 2024-04-28 05:02:43.280924 bluecast-1.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0    15528 2023-11-09 06:04:30.460510 bluecast-1.1/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0    11974 2024-04-27 16:21:53.610446 bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc
--rw-r--r--   0        0        0     5752 2023-11-08 09:05:35.035550 bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc
--rw-r--r--   0        0        0     8688 2024-04-27 16:21:53.626446 bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-310.pyc
--rw-r--r--   0        0        0     5079 2023-12-03 17:36:58.336581 bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-38.pyc
--rw-r--r--   0        0        0    18494 2024-04-27 16:21:53.618446 bluecast-1.1/bluecast/blueprints/__pycache__/cast_regression.cpython-310.pyc
--rw-r--r--   0        0        0    15267 2023-12-03 17:34:01.804139 bluecast-1.1/bluecast/blueprints/__pycache__/cast_regression.cpython-38.pyc
--rw-r--r--   0        0        0    32945 2024-04-27 16:21:58.518511 bluecast-1.1/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0    18120 2024-04-26 07:23:40.665222 bluecast-1.1/bluecast/blueprints/cast_cv.py
--rw-r--r--   0        0        0    11668 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/blueprints/cast_cv_regression.py
--rw-r--r--   0        0        0    27093 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/blueprints/cast_regression.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.1/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-1.1/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-1.1/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1535 2023-12-03 17:43:20.708381 bluecast-1.1/bluecast/config/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1514 2023-12-03 17:36:58.256581 bluecast-1.1/bluecast/config/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     8971 2024-04-28 05:02:43.500927 bluecast-1.1/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     8123 2023-12-03 17:34:01.804139 bluecast-1.1/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-11-20 13:28:18.349644 bluecast-1.1/bluecast/config/base_classes.py
--rw-r--r--   0        0        0     8271 2024-04-30 06:29:43.413117 bluecast-1.1/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/__init__.py
--rw-r--r--   0        0        0      169 2024-04-27 16:21:52.806435 bluecast-1.1/bluecast/conformal_prediction/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1156 2024-04-27 16:21:52.806435 bluecast-1.1/bluecast/conformal_prediction/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     3034 2024-04-27 16:21:52.806435 bluecast-1.1/bluecast/conformal_prediction/__pycache__/conformal_prediction.cpython-310.pyc
--rw-r--r--   0        0        0     3362 2024-04-27 16:21:53.622446 bluecast-1.1/bluecast/conformal_prediction/__pycache__/conformal_prediction_regression.cpython-310.pyc
--rw-r--r--   0        0        0     2759 2024-04-27 16:21:52.806435 bluecast-1.1/bluecast/conformal_prediction/__pycache__/nonconformity_measures.cpython-310.pyc
--rw-r--r--   0        0        0     1552 2024-04-27 16:21:53.622446 bluecast-1.1/bluecast/conformal_prediction/__pycache__/nonconformity_measures_regression.cpython-310.pyc
--rw-r--r--   0        0        0      703 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/base_classes.py
--rw-r--r--   0        0        0     3228 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/conformal_prediction.py
--rw-r--r--   0        0        0     2905 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/conformal_prediction_regression.py
--rw-r--r--   0        0        0     2112 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/effectiveness_nonconformity_measures.py
--rw-r--r--   0        0        0     2055 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/evaluation.py
--rw-r--r--   0        0        0     3227 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/nonconformity_measures.py
--rw-r--r--   0        0        0     1339 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/conformal_prediction/nonconformity_measures_regression.py
--rw-r--r--   0        0        0        0 2023-06-30 06:22:16.681826 bluecast-1.1/bluecast/eda/__init__.py
--rw-r--r--   0        0        0      152 2023-07-04 05:47:32.270463 bluecast-1.1/bluecast/eda/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      150 2023-12-03 17:32:26.107900 bluecast-1.1/bluecast/eda/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    16574 2024-03-15 07:41:22.312232 bluecast-1.1/bluecast/eda/__pycache__/analyse.cpython-310.pyc
--rw-r--r--   0        0        0     9305 2023-12-03 17:32:26.127900 bluecast-1.1/bluecast/eda/__pycache__/analyse.cpython-38.pyc
--rw-r--r--   0        0        0     2777 2023-11-08 12:54:43.294360 bluecast-1.1/bluecast/eda/__pycache__/data_leakage_checks.cpython-310.pyc
--rw-r--r--   0        0        0     2748 2023-12-03 17:32:26.395901 bluecast-1.1/bluecast/eda/__pycache__/data_leakage_checks.cpython-38.pyc
--rw-r--r--   0        0        0    21726 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/eda/analyse.py
--rw-r--r--   0        0        0     3064 2023-10-30 08:48:38.178728 bluecast-1.1/bluecast/eda/data_leakage_checks.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-1.1/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-1.1/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-1.1/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6309 2024-04-27 16:21:52.806435 bluecast-1.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     6209 2023-12-03 17:34:01.880140 bluecast-1.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     4768 2024-03-21 14:26:37.635823 bluecast-1.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1177 2023-11-08 09:05:35.019550 bluecast-1.1/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     7837 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     6887 2024-03-18 06:17:55.960882 bluecast-1.1/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-10-17 11:59:56.817023 bluecast-1.1/bluecast/experimentation/__init__.py
--rw-r--r--   0        0        0      164 2023-11-08 12:54:42.730351 bluecast-1.1/bluecast/experimentation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      162 2023-10-17 12:03:57.356075 bluecast-1.1/bluecast/experimentation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4073 2024-03-15 06:56:20.852200 bluecast-1.1/bluecast/experimentation/__pycache__/tracking.cpython-310.pyc
--rw-r--r--   0        0        0     4062 2023-12-03 17:36:58.256581 bluecast-1.1/bluecast/experimentation/__pycache__/tracking.cpython-38.pyc
--rw-r--r--   0        0        0     5008 2023-12-07 12:56:56.993837 bluecast-1.1/bluecast/experimentation/tracking.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-1.1/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-1.1/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-1.1/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3165 2024-04-27 16:21:53.250441 bluecast-1.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2776 2023-11-08 09:05:35.019550 bluecast-1.1/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     3185 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.1/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-1.1/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-1.1/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2082 2024-03-15 06:56:21.392218 bluecast-1.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     2037 2023-12-03 17:36:58.260581 bluecast-1.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0    19009 2024-04-27 16:21:53.522445 bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0    18168 2023-12-03 17:36:58.340581 bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0    16965 2024-04-27 16:21:53.626446 bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-310.pyc
--rw-r--r--   0        0        0    16725 2023-12-03 17:36:58.260581 bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-38.pyc
--rw-r--r--   0        0        0     1615 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    35613 2024-04-30 07:17:23.351472 bluecast-1.1/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0    31766 2024-04-30 07:17:23.299471 bluecast-1.1/bluecast/ml_modelling/xgboost_regression.py
--rw-r--r--   0        0        0        0 2024-01-25 07:16:38.510980 bluecast-1.1/bluecast/monitoring/__init__.py
--rw-r--r--   0        0        0      159 2024-03-15 07:41:23.524254 bluecast-1.1/bluecast/monitoring/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7853 2024-03-15 07:41:23.524254 bluecast-1.1/bluecast/monitoring/__pycache__/data_monitoring.cpython-310.pyc
--rw-r--r--   0        0        0     9111 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/monitoring/data_monitoring.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.1/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-1.1/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-1.1/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1618 2024-03-15 06:56:21.392218 bluecast-1.1/bluecast/preprocessing/__pycache__/category_encoder_orchestration.cpython-310.pyc
--rw-r--r--   0        0        0     1924 2024-03-15 06:56:21.392218 bluecast-1.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-1.1/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2024-03-15 06:56:21.392218 bluecast-1.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1493 2023-12-03 17:36:58.264581 bluecast-1.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3975 2024-04-27 16:21:53.542445 bluecast-1.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3930 2023-10-17 12:03:57.360075 bluecast-1.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     2506 2024-03-15 06:56:21.396218 bluecast-1.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     2495 2023-12-03 17:36:58.264581 bluecast-1.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2024-04-27 16:21:53.546445 bluecast-1.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4893 2023-12-03 17:32:26.247901 bluecast-1.1/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2024-03-15 06:56:21.408219 bluecast-1.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-1.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     2442 2024-03-15 06:56:21.408219 bluecast-1.1/bluecast/preprocessing/__pycache__/onehot_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     2242 2024-03-15 06:56:21.592225 bluecast-1.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     2276 2023-11-08 09:05:35.031550 bluecast-1.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     5230 2024-03-15 06:56:21.592225 bluecast-1.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5245 2023-10-17 12:03:57.368075 bluecast-1.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2024-03-15 06:56:21.592225 bluecast-1.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     2332 2023-11-08 09:05:35.035550 bluecast-1.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1325 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/category_encoder_orchestration.py
--rw-r--r--   0        0        0     1403 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1418 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3698 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     2332 2023-12-07 12:56:56.993837 bluecast-1.1/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6463 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      863 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     2326 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/onehot_encoding.py
--rw-r--r--   0        0        0     1755 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4911 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2873 2024-02-27 13:10:51.070694 bluecast-1.1/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-1.1/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-1.1/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7898 2024-03-15 07:41:22.140229 bluecast-1.1/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    18758 2024-03-15 07:41:22.900242 bluecast-1.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    10802 2024-03-15 07:41:23.436252 bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4601 2024-03-15 07:41:23.440252 bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    18082 2024-03-15 07:41:23.504253 bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv_regression.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    16323 2024-03-15 07:41:23.512253 bluecast-1.1/bluecast/tests/__pycache__/test_cast_regression.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2177 2024-03-15 07:41:23.516254 bluecast-1.1/bluecast/tests/__pycache__/test_category_encoder_orchestrator.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3142 2023-09-11 13:19:23.630591 bluecast-1.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5803 2024-04-12 13:43:14.526075 bluecast-1.1/bluecast/tests/__pycache__/test_conformal_prediction.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5919 2024-04-19 13:03:27.424659 bluecast-1.1/bluecast/tests/__pycache__/test_conformal_prediction_regression.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-1.1/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3029 2024-03-15 07:41:23.520254 bluecast-1.1/bluecast/tests/__pycache__/test_data_leakage_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2140 2024-03-15 07:41:23.520254 bluecast-1.1/bluecast/tests/__pycache__/test_data_monitoring.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1198 2024-03-15 07:41:23.524254 bluecast-1.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-1.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5126 2023-11-08 12:54:43.298360 bluecast-1.1/bluecast/tests/__pycache__/test_experiment_tracker.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4822 2024-03-15 07:41:23.532254 bluecast-1.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2985 2024-03-15 07:41:23.532254 bluecast-1.1/bluecast/tests/__pycache__/test_fine_tune.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1325 2024-03-15 07:41:23.536254 bluecast-1.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4379 2024-04-12 12:05:44.044458 bluecast-1.1/bluecast/tests/__pycache__/test_nonconformity_measures.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-1.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2212 2024-03-15 07:41:23.536254 bluecast-1.1/bluecast/tests/__pycache__/test_onehot_encoding.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-1.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-1.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4314 2024-03-15 13:42:57.632562 bluecast-1.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-1.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1471 2023-11-08 12:54:43.314360 bluecast-1.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-1.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-1.1/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-1.1/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2102 2024-03-15 06:56:21.596225 bluecast-1.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     3692 2023-12-07 12:56:56.993837 bluecast-1.1/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     7343 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_analyse.py
--rw-r--r--   0        0        0    17880 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     4146 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_binary_conformal_prediction.py
--rw-r--r--   0        0        0     6888 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_cv.py
--rw-r--r--   0        0        0     4166 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_cv_binary_conformal_prediction.py
--rw-r--r--   0        0        0     3065 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_cv_multiclass.py
--rw-r--r--   0        0        0     4166 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_cv_multiclass_conformal_prediction.py
--rw-r--r--   0        0        0    13375 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_cv_regression.py
--rw-r--r--   0        0        0    15892 2024-04-26 07:23:40.669222 bluecast-1.1/bluecast/tests/test_cast_regression.py
--rw-r--r--   0        0        0     1123 2024-02-27 13:10:51.074694 bluecast-1.1/bluecast/tests/test_category_encoder_orchestrator.py
--rw-r--r--   0        0        0     1321 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     5164 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_conformal_prediction.py
--rw-r--r--   0        0        0     3693 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_conformal_prediction_evaluation.py
--rw-r--r--   0        0        0     4574 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_conformal_prediction_regression.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-1.1/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     2789 2024-02-27 13:10:51.074694 bluecast-1.1/bluecast/tests/test_data_leakage_checks.py
--rw-r--r--   0        0        0     1591 2024-01-25 07:16:38.510980 bluecast-1.1/bluecast/tests/test_data_monitoring.py
--rw-r--r--   0        0        0     1178 2023-11-15 06:29:25.379715 bluecast-1.1/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0      938 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_effectiveness_nonconformity_measures.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-1.1/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     4335 2023-10-20 06:58:59.816708 bluecast-1.1/bluecast/tests/test_experiment_tracker.py
--rw-r--r--   0        0        0     2624 2023-11-15 06:29:25.379715 bluecast-1.1/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     3570 2023-12-07 12:56:56.997838 bluecast-1.1/bluecast/tests/test_fine_tune.py
--rw-r--r--   0        0        0     1386 2023-12-07 12:56:56.997838 bluecast-1.1/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     2193 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_nonconformity_measures.py
--rw-r--r--   0        0        0      972 2024-04-26 07:23:40.673222 bluecast-1.1/bluecast/tests/test_nonconformity_measures_regression.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-1.1/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1676 2024-02-27 13:10:51.074694 bluecast-1.1/bluecast/tests/test_onehot_encoding.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-1.1/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-1.1/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     3400 2024-03-18 06:17:55.964882 bluecast-1.1/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-1.1/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      756 2023-09-13 05:44:23.720213 bluecast-1.1/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-1.1/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1670 2024-04-28 07:51:02.473835 bluecast-1.1/pyproject.toml
--rw-r--r--   0        0        0    10365 1970-01-01 00:00:00.000000 bluecast-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-1.2.4/LICENSE
+-rw-r--r--   0        0        0     9172 2024-05-08 18:16:54.751684 bluecast-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-1.2.4/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.2.4/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-1.2.4/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-1.2.4/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    21664 2024-04-28 05:02:43.280924 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0    15528 2023-11-09 06:04:30.460510 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0    11974 2024-04-27 16:21:53.610446 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc
+-rw-r--r--   0        0        0     5752 2023-11-08 09:05:35.035550 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc
+-rw-r--r--   0        0        0     9189 2024-05-07 13:38:01.217726 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-310.pyc
+-rw-r--r--   0        0        0     5079 2023-12-03 17:36:58.336581 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-38.pyc
+-rw-r--r--   0        0        0    18494 2024-04-27 16:21:53.618446 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_regression.cpython-310.pyc
+-rw-r--r--   0        0        0    15267 2023-12-03 17:34:01.804139 bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_regression.cpython-38.pyc
+-rw-r--r--   0        0        0    32945 2024-04-27 16:21:58.518511 bluecast-1.2.4/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0    18120 2024-04-26 07:23:40.665222 bluecast-1.2.4/bluecast/blueprints/cast_cv.py
+-rw-r--r--   0        0        0    12437 2024-05-06 04:06:23.692640 bluecast-1.2.4/bluecast/blueprints/cast_cv_regression.py
+-rw-r--r--   0        0        0    27093 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/blueprints/cast_regression.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.2.4/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-1.2.4/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-1.2.4/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1535 2023-12-03 17:43:20.708381 bluecast-1.2.4/bluecast/config/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1514 2023-12-03 17:36:58.256581 bluecast-1.2.4/bluecast/config/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     9419 2024-05-08 16:29:20.221238 bluecast-1.2.4/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     8123 2023-12-03 17:34:01.804139 bluecast-1.2.4/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-11-20 13:28:18.349644 bluecast-1.2.4/bluecast/config/base_classes.py
+-rw-r--r--   0        0        0     8702 2024-05-08 18:16:48.343603 bluecast-1.2.4/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-27 16:21:52.806435 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1156 2024-04-27 16:21:52.806435 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     3034 2024-04-27 16:21:52.806435 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/conformal_prediction.cpython-310.pyc
+-rw-r--r--   0        0        0     3362 2024-04-27 16:21:53.622446 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/conformal_prediction_regression.cpython-310.pyc
+-rw-r--r--   0        0        0     2759 2024-04-27 16:21:52.806435 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/nonconformity_measures.cpython-310.pyc
+-rw-r--r--   0        0        0     1552 2024-04-27 16:21:53.622446 bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/nonconformity_measures_regression.cpython-310.pyc
+-rw-r--r--   0        0        0      703 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/base_classes.py
+-rw-r--r--   0        0        0     3228 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/conformal_prediction.py
+-rw-r--r--   0        0        0     2905 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/conformal_prediction_regression.py
+-rw-r--r--   0        0        0     2112 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/effectiveness_nonconformity_measures.py
+-rw-r--r--   0        0        0     2055 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/evaluation.py
+-rw-r--r--   0        0        0     3227 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/nonconformity_measures.py
+-rw-r--r--   0        0        0     1339 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/conformal_prediction/nonconformity_measures_regression.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:22:16.681826 bluecast-1.2.4/bluecast/eda/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-04 05:47:32.270463 bluecast-1.2.4/bluecast/eda/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      150 2023-12-03 17:32:26.107900 bluecast-1.2.4/bluecast/eda/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    16574 2024-03-15 07:41:22.312232 bluecast-1.2.4/bluecast/eda/__pycache__/analyse.cpython-310.pyc
+-rw-r--r--   0        0        0     9305 2023-12-03 17:32:26.127900 bluecast-1.2.4/bluecast/eda/__pycache__/analyse.cpython-38.pyc
+-rw-r--r--   0        0        0     2777 2023-11-08 12:54:43.294360 bluecast-1.2.4/bluecast/eda/__pycache__/data_leakage_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     2748 2023-12-03 17:32:26.395901 bluecast-1.2.4/bluecast/eda/__pycache__/data_leakage_checks.cpython-38.pyc
+-rw-r--r--   0        0        0    21726 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/eda/analyse.py
+-rw-r--r--   0        0        0     3064 2023-10-30 08:48:38.178728 bluecast-1.2.4/bluecast/eda/data_leakage_checks.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-1.2.4/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-1.2.4/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-1.2.4/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6309 2024-04-27 16:21:52.806435 bluecast-1.2.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     6209 2023-12-03 17:34:01.880140 bluecast-1.2.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     4768 2024-03-21 14:26:37.635823 bluecast-1.2.4/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1177 2023-11-08 09:05:35.019550 bluecast-1.2.4/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     7837 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     6887 2024-03-18 06:17:55.960882 bluecast-1.2.4/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-10-17 11:59:56.817023 bluecast-1.2.4/bluecast/experimentation/__init__.py
+-rw-r--r--   0        0        0      164 2023-11-08 12:54:42.730351 bluecast-1.2.4/bluecast/experimentation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      162 2023-10-17 12:03:57.356075 bluecast-1.2.4/bluecast/experimentation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4073 2024-03-15 06:56:20.852200 bluecast-1.2.4/bluecast/experimentation/__pycache__/tracking.cpython-310.pyc
+-rw-r--r--   0        0        0     4062 2023-12-03 17:36:58.256581 bluecast-1.2.4/bluecast/experimentation/__pycache__/tracking.cpython-38.pyc
+-rw-r--r--   0        0        0     5008 2023-12-07 12:56:56.993837 bluecast-1.2.4/bluecast/experimentation/tracking.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-1.2.4/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-1.2.4/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-1.2.4/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3940 2024-05-07 13:38:00.617716 bluecast-1.2.4/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2776 2023-11-08 09:05:35.019550 bluecast-1.2.4/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3899 2024-05-06 04:04:32.318845 bluecast-1.2.4/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.2.4/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2082 2024-03-15 06:56:21.392218 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     2037 2023-12-03 17:36:58.260581 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0    18860 2024-05-07 13:38:01.105724 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0    18168 2023-12-03 17:36:58.340581 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0    16775 2024-05-07 13:38:01.213726 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-310.pyc
+-rw-r--r--   0        0        0    16725 2023-12-03 17:36:58.260581 bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-38.pyc
+-rw-r--r--   0        0        0     1615 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    36259 2024-05-06 04:52:12.935306 bluecast-1.2.4/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0    32419 2024-05-06 04:52:12.883305 bluecast-1.2.4/bluecast/ml_modelling/xgboost_regression.py
+-rw-r--r--   0        0        0        0 2024-01-25 07:16:38.510980 bluecast-1.2.4/bluecast/monitoring/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-15 07:41:23.524254 bluecast-1.2.4/bluecast/monitoring/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7853 2024-03-15 07:41:23.524254 bluecast-1.2.4/bluecast/monitoring/__pycache__/data_monitoring.cpython-310.pyc
+-rw-r--r--   0        0        0     9111 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/monitoring/data_monitoring.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-1.2.4/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-1.2.4/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-1.2.4/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1618 2024-03-15 06:56:21.392218 bluecast-1.2.4/bluecast/preprocessing/__pycache__/category_encoder_orchestration.cpython-310.pyc
+-rw-r--r--   0        0        0     1924 2024-03-15 06:56:21.392218 bluecast-1.2.4/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-1.2.4/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2024-03-15 06:56:21.392218 bluecast-1.2.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1493 2023-12-03 17:36:58.264581 bluecast-1.2.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3975 2024-04-27 16:21:53.542445 bluecast-1.2.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3930 2023-10-17 12:03:57.360075 bluecast-1.2.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     2506 2024-03-15 06:56:21.396218 bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     2495 2023-12-03 17:36:58.264581 bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2024-04-27 16:21:53.546445 bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4893 2023-12-03 17:32:26.247901 bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2024-03-15 06:56:21.408219 bluecast-1.2.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-1.2.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     2442 2024-03-15 06:56:21.408219 bluecast-1.2.4/bluecast/preprocessing/__pycache__/onehot_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     2242 2024-03-15 06:56:21.592225 bluecast-1.2.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     2276 2023-11-08 09:05:35.031550 bluecast-1.2.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     5230 2024-03-15 06:56:21.592225 bluecast-1.2.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5245 2023-10-17 12:03:57.368075 bluecast-1.2.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2024-03-15 06:56:21.592225 bluecast-1.2.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     2332 2023-11-08 09:05:35.035550 bluecast-1.2.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1325 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/category_encoder_orchestration.py
+-rw-r--r--   0        0        0     1403 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1418 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3698 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     2332 2023-12-07 12:56:56.993837 bluecast-1.2.4/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6463 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      863 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     2326 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/onehot_encoding.py
+-rw-r--r--   0        0        0     1755 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4911 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2873 2024-02-27 13:10:51.070694 bluecast-1.2.4/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-1.2.4/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-1.2.4/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7898 2024-03-15 07:41:22.140229 bluecast-1.2.4/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    18758 2024-03-15 07:41:22.900242 bluecast-1.2.4/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    10802 2024-03-15 07:41:23.436252 bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4601 2024-03-15 07:41:23.440252 bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    18082 2024-03-15 07:41:23.504253 bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv_regression.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    16323 2024-03-15 07:41:23.512253 bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_regression.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2177 2024-03-15 07:41:23.516254 bluecast-1.2.4/bluecast/tests/__pycache__/test_category_encoder_orchestrator.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3142 2023-09-11 13:19:23.630591 bluecast-1.2.4/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5803 2024-04-12 13:43:14.526075 bluecast-1.2.4/bluecast/tests/__pycache__/test_conformal_prediction.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5919 2024-04-19 13:03:27.424659 bluecast-1.2.4/bluecast/tests/__pycache__/test_conformal_prediction_regression.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-1.2.4/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3029 2024-03-15 07:41:23.520254 bluecast-1.2.4/bluecast/tests/__pycache__/test_data_leakage_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2140 2024-03-15 07:41:23.520254 bluecast-1.2.4/bluecast/tests/__pycache__/test_data_monitoring.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1198 2024-03-15 07:41:23.524254 bluecast-1.2.4/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-1.2.4/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5126 2023-11-08 12:54:43.298360 bluecast-1.2.4/bluecast/tests/__pycache__/test_experiment_tracker.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4822 2024-03-15 07:41:23.532254 bluecast-1.2.4/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2985 2024-03-15 07:41:23.532254 bluecast-1.2.4/bluecast/tests/__pycache__/test_fine_tune.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1325 2024-03-15 07:41:23.536254 bluecast-1.2.4/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4379 2024-04-12 12:05:44.044458 bluecast-1.2.4/bluecast/tests/__pycache__/test_nonconformity_measures.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-1.2.4/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2212 2024-03-15 07:41:23.536254 bluecast-1.2.4/bluecast/tests/__pycache__/test_onehot_encoding.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-1.2.4/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-1.2.4/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4314 2024-03-15 13:42:57.632562 bluecast-1.2.4/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-1.2.4/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1471 2023-11-08 12:54:43.314360 bluecast-1.2.4/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-1.2.4/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-1.2.4/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-1.2.4/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2102 2024-03-15 06:56:21.596225 bluecast-1.2.4/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     3692 2023-12-07 12:56:56.993837 bluecast-1.2.4/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     7343 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_analyse.py
+-rw-r--r--   0        0        0    17880 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     4146 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast_binary_conformal_prediction.py
+-rw-r--r--   0        0        0     6938 2024-05-06 04:57:34.640317 bluecast-1.2.4/bluecast/tests/test_cast_cv.py
+-rw-r--r--   0        0        0     4166 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast_cv_binary_conformal_prediction.py
+-rw-r--r--   0        0        0     3065 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast_cv_multiclass.py
+-rw-r--r--   0        0        0     4166 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast_cv_multiclass_conformal_prediction.py
+-rw-r--r--   0        0        0    14016 2024-05-06 06:51:28.604538 bluecast-1.2.4/bluecast/tests/test_cast_cv_regression.py
+-rw-r--r--   0        0        0    15892 2024-04-26 07:23:40.669222 bluecast-1.2.4/bluecast/tests/test_cast_regression.py
+-rw-r--r--   0        0        0     1123 2024-02-27 13:10:51.074694 bluecast-1.2.4/bluecast/tests/test_category_encoder_orchestrator.py
+-rw-r--r--   0        0        0     1321 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     5164 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_conformal_prediction.py
+-rw-r--r--   0        0        0     3693 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_conformal_prediction_evaluation.py
+-rw-r--r--   0        0        0     4574 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_conformal_prediction_regression.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-1.2.4/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     2789 2024-02-27 13:10:51.074694 bluecast-1.2.4/bluecast/tests/test_data_leakage_checks.py
+-rw-r--r--   0        0        0     1591 2024-01-25 07:16:38.510980 bluecast-1.2.4/bluecast/tests/test_data_monitoring.py
+-rw-r--r--   0        0        0     1178 2023-11-15 06:29:25.379715 bluecast-1.2.4/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0      938 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_effectiveness_nonconformity_measures.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-1.2.4/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     4335 2023-10-20 06:58:59.816708 bluecast-1.2.4/bluecast/tests/test_experiment_tracker.py
+-rw-r--r--   0        0        0     2624 2023-11-15 06:29:25.379715 bluecast-1.2.4/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     3570 2023-12-07 12:56:56.997838 bluecast-1.2.4/bluecast/tests/test_fine_tune.py
+-rw-r--r--   0        0        0     1386 2023-12-07 12:56:56.997838 bluecast-1.2.4/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     2193 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_nonconformity_measures.py
+-rw-r--r--   0        0        0      972 2024-04-26 07:23:40.673222 bluecast-1.2.4/bluecast/tests/test_nonconformity_measures_regression.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-1.2.4/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1676 2024-02-27 13:10:51.074694 bluecast-1.2.4/bluecast/tests/test_onehot_encoding.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-1.2.4/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-1.2.4/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     3400 2024-03-18 06:17:55.964882 bluecast-1.2.4/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-1.2.4/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      756 2023-09-13 05:44:23.720213 bluecast-1.2.4/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-1.2.4/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1672 2024-05-05 13:32:13.042911 bluecast-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    10395 1970-01-01 00:00:00.000000 bluecast-1.2.4/PKG-INFO
```

### Comparing `bluecast-1.1/LICENSE` & `bluecast-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/README.md` & `bluecast-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 Documentation is provided via [Read the Docs](https://bluecast.readthedocs.io/en/latest/)
 On GitHub we offer multiple ReadMes to cover all aspects of working
 with BlueCast, covering:
 
 * [Installation](docs/source/Installation.md)
 * [EDA](docs/source/EDA.md)
 * [Basic usage](docs/source/Basic%20usage.md)
-* [Advanced usage](docs/source/Advanced%20usage.md)
+* [Customize training settings](docs/source/Customize%20training%20settings.md)
 * [Customizing configurations and objects](docs/source/Customizing%20configurations%20and%20objects.md)
 * [Model evaluation](docs/source/Model%20evaluation.md)
 * [Model explainability (XAI)](docs/source/Model%20explainability%20(XAI).md)
 * [Uncertainty quantification](docs/source/Uncertainty%20quantification.md)
 * [Monitoring](docs/source/Monitoring.md)
 
 ### How to contribute
```

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast.cpython-38.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-310.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 26 07:23:40 2024 UTC, .py size: 11668 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7c56 2b66 942d 0000  o.......|V+f.-..
+00000000: 6f0d 0d0a 0000 0000 3f57 3866 9530 0000  o.......?W8f.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 5a08 6400 6402 6c09 5a0a 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c0b 6d0c 5a0c 0100 6400 6404 6c0d  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0e 0100 6400 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
@@ -28,516 +28,548 @@
 000001b0: 6f6e 5772 6170 7065 7229 01da 1145 7870  onWrapper)...Exp
 000001c0: 6572 696d 656e 7454 7261 636b 6572 2901  erimentTracker).
 000001d0: da06 6c6f 6767 6572 2901 da0c 5867 626f  ..logger)...Xgbo
 000001e0: 6f73 744d 6f64 656c 2901 da13 4375 7374  ostModel)...Cust
 000001f0: 6f6d 5072 6570 726f 6365 7373 696e 6729  omPreprocessing)
 00000200: 01da 0d52 4645 4356 5365 6c65 6374 6f72  ...RFECVSelector
 00000210: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000220: 001a 0000 0040 0000 0073 7801 0000 6500  .....@...sx...e.
+00000220: 001a 0000 0040 0000 0073 8201 0000 6500  .....@...s....e.
 00000230: 5a01 6400 5a02 6401 5a03 0902 0903 0903  Z.d.Z.d.Z.......
 00000240: 0903 0903 0903 0903 0903 0903 0903 0903  ................
-00000250: 642b 6404 6504 6402 1900 6405 6505 6506  d+d.e.d...d.e.e.
+00000250: 642e 6404 6504 6402 1900 6405 6505 6506  d.d.e.d...d.e.e.
 00000260: 1900 6406 6505 6507 1900 6407 6505 6508  ..d.e.e...d.e.e.
 00000270: 1900 6408 6505 6509 1900 6409 6505 650a  ..d.e.e...d.e.e.
 00000280: 1900 640a 6505 650b 1900 640b 6505 650b  ..d.e.e...d.e.e.
 00000290: 1900 640c 6505 650b 1900 640d 6505 650c  ..d.e.e...d.e.e.
 000002a0: 650d 650b 6602 1900 1900 640e 6505 650c  e.e.f.....d.e.e.
 000002b0: 650e 6506 6602 1900 1900 6616 640f 6410  e.e.f.....f.d.d.
 000002c0: 8405 5a0f 6411 6510 6a11 6412 6512 6413  ..Z.d.e.j.d.e.d.
 000002d0: 6513 6510 6a11 6510 6a14 6602 1900 6606  e.e.j.e.j.f...f.
-000002e0: 6414 6415 8404 5a15 642c 6417 6512 6413  d.d...Z.d,d.e.d.
+000002e0: 6414 6415 8404 5a15 642f 6417 6512 6413  d.d...Z.d/d.e.d.
 000002f0: 6513 6516 6516 6602 1900 6604 6418 6419  e.e.e.f...f.d.d.
 00000300: 8405 5a17 6411 6510 6a11 641a 6512 6413  ..Z.d.e.j.d.e.d.
 00000310: 6403 6606 641b 641c 8404 5a18 6411 6510  d.f.d.d...Z.d.e.
 00000320: 6a11 641a 6512 6413 6513 6516 6516 6602  j.d.e.d.e.e.e.f.
 00000330: 1900 6606 641d 641e 8404 5a19 091f 091f  ..f.d.d...Z.....
-00000340: 642d 6411 6510 6a11 6420 651a 6421 651a  d-d.e.j.d e.d!e.
-00000350: 6413 650c 6510 6a11 6510 6a14 6602 1900  d.e.e.j.e.j.f...
-00000360: 6608 6422 6423 8405 5a1b 6424 6510 6a11  f.d"d#..Z.d$e.j.
-00000370: 6425 6510 6a14 6413 6403 6606 6426 6427  d%e.j.d.d.f.d&d'
-00000380: 8404 5a1c 6411 6510 6a11 6428 651d 6516  ..Z.d.e.j.d(e.e.
-00000390: 1900 6413 6510 6a11 6606 6429 642a 8404  ..d.e.j.f.d)d*..
-000003a0: 5a1e 6403 5300 292e da14 426c 7565 4361  Z.d.S.)...BlueCa
-000003b0: 7374 4356 5265 6772 6573 7369 6f6e 7ab4  stCVRegressionz.
-000003c0: 5772 6170 7065 7220 746f 2074 7261 696e  Wrapper to train
-000003d0: 2061 6e64 2070 7265 6469 6374 206d 756c   and predict mul
-000003e0: 7469 706c 6520 626c 7565 4361 7374 2069  tiple blueCast i
-000003f0: 6e74 7374 616e 6365 732e 0a0a 2020 2020  ntstances...    
-00000400: 4368 6563 6b20 7468 6520 426c 7565 4361  Check the BlueCa
-00000410: 7374 2063 6c61 7373 2064 6f63 756d 656e  st class documen
-00000420: 7461 7469 6f6e 2066 6f72 2061 6464 6974  tation for addit
-00000430: 696f 6e61 6c20 7061 7261 6d65 7465 7220  ional parameter 
-00000440: 6465 7461 696c 732e 0a20 2020 2041 2063  details..    A c
-00000450: 7573 746f 6d20 7370 6c69 7474 6572 2063  ustom splitter c
-00000460: 616e 2062 6520 7072 6f76 6964 6564 2e0a  an be provided..
-00000470: 2020 2020 da0a 7265 6772 6573 7369 6f6e      ..regression
-00000480: 4eda 0d63 6c61 7373 5f70 726f 626c 656d  N..class_problem
-00000490: da0a 7374 7261 7469 6669 6572 da0d 636f  ..stratifier..co
-000004a0: 6e66 5f74 7261 696e 696e 67da 0c63 6f6e  nf_training..con
-000004b0: 665f 7867 626f 6f73 74da 1363 6f6e 665f  f_xgboost..conf_
-000004c0: 7061 7261 6d73 5f78 6762 6f6f 7374 da12  params_xgboost..
-000004d0: 6578 7065 7269 6d65 6e74 5f74 7261 636b  experiment_track
-000004e0: 6572 da1b 6375 7374 6f6d 5f69 6e5f 666f  er..custom_in_fo
-000004f0: 6c64 5f70 7265 7072 6f63 6573 736f 72da  ld_preprocessor.
-00000500: 1c63 7573 746f 6d5f 6c61 7374 5f6d 696c  .custom_last_mil
-00000510: 655f 636f 6d70 7574 6174 696f 6eda 1363  e_computation..c
-00000520: 7573 746f 6d5f 7072 6570 726f 6365 7373  ustom_preprocess
-00000530: 6f72 da17 6375 7374 6f6d 5f66 6561 7475  or..custom_featu
-00000540: 7265 5f73 656c 6563 746f 72da 086d 6c5f  re_selector..ml_
-00000550: 6d6f 6465 6c63 0c00 0000 0000 0000 0000  modelc..........
-00000560: 0000 0c00 0000 0200 0000 4300 0000 7362  ..........C...sb
-00000570: 0000 007c 017c 005f 007c 047c 005f 017c  ...|.|._.|.|._.|
-00000580: 037c 005f 027c 057c 005f 037c 077c 005f  .|._.|.|._.|.|._
-00000590: 047c 097c 005f 057c 0a7c 005f 067c 087c  .|.|._.|.|._.|.|
-000005a0: 005f 0767 007c 005f 087c 027c 005f 097c  ._.g.|._.|.|._.|
-000005b0: 0b7c 005f 0a64 007c 005f 0b7c 0672 2b7c  .|._.d.|._.|.r+|
-000005c0: 067c 005f 0c64 0053 0074 0d83 007c 005f  .|._.d.S.t...|._
-000005d0: 0c64 0053 0029 014e 290e 7215 0000 0072  .d.S.).N).r....r
-000005e0: 1800 0000 7217 0000 0072 1900 0000 721b  ....r....r....r.
-000005f0: 0000 0072 1d00 0000 721e 0000 0072 1c00  ...r....r....r..
-00000600: 0000 da0f 626c 7565 6361 7374 5f6d 6f64  ....bluecast_mod
-00000610: 656c 7372 1600 0000 721f 0000 00da 1c63  elsr....r......c
-00000620: 6f6e 666f 726d 616c 5f70 7265 6469 6374  onformal_predict
-00000630: 696f 6e5f 7772 6170 7065 7272 1a00 0000  ion_wrapperr....
-00000640: 720e 0000 0029 0cda 0473 656c 6672 1500  r....)...selfr..
-00000650: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000660: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000670: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000680: 1f00 0000 a900 7223 0000 00fa 4c2f 686f  ......r#....L/ho
-00000690: 6d65 2f74 686f 6d61 732f 4964 6561 5072  me/thomas/IdeaPr
-000006a0: 6f6a 6563 7473 2f42 6c75 6543 6173 742f  ojects/BlueCast/
-000006b0: 626c 7565 6361 7374 2f62 6c75 6570 7269  bluecast/bluepri
-000006c0: 6e74 732f 6361 7374 5f63 765f 7265 6772  nts/cast_cv_regr
-000006d0: 6573 7369 6f6e 2e70 79da 085f 5f69 6e69  ession.py..__ini
-000006e0: 745f 5f1d 0000 0073 2000 0000 0610 0601  t__....s .......
-000006f0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00000700: 0601 0203 04fe 0404 0a01 0c02 7a1d 426c  ............z.Bl
-00000710: 7565 4361 7374 4356 5265 6772 6573 7369  ueCastCVRegressi
-00000720: 6f6e 2e5f 5f69 6e69 745f 5fda 0264 66da  on.__init__..df.
-00000730: 0674 6172 6765 74da 0672 6574 7572 6e63  .target..returnc
-00000740: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-00000750: 0400 0000 4300 0000 732a 0000 007c 016a  ....C...s*...|.j
-00000760: 0064 0164 028d 017d 017c 017c 0219 007d  .d.d...}.|.|...}
-00000770: 037c 016a 017c 0264 0364 048d 027d 047c  .|.j.|.d.d...}.|
-00000780: 047c 0366 0253 0029 054e 54a9 01da 0464  .|.f.S.).NT....d
-00000790: 726f 70e9 0100 0000 a901 da04 6178 6973  rop.........axis
-000007a0: 2902 da0b 7265 7365 745f 696e 6465 7872  )...reset_indexr
-000007b0: 2a00 0000 2905 7222 0000 0072 2600 0000  *...).r"...r&...
-000007c0: 7227 0000 00da 0179 da01 5872 2300 0000  r'.....y..Xr#...
-000007d0: 7223 0000 0072 2400 0000 da0c 7072 6570  r#...r$.....prep
-000007e0: 6172 655f 6461 7461 4100 0000 7308 0000  are_dataA...s...
-000007f0: 000c 0308 010e 0108 017a 2142 6c75 6543  .........z!BlueC
-00000800: 6173 7443 5652 6567 7265 7373 696f 6e2e  astCVRegression.
-00000810: 7072 6570 6172 655f 6461 7461 da04 524d  prepare_data..RM
-00000820: 5345 da06 6d65 7472 6963 6302 0000 0000  SE..metricc.....
-00000830: 0000 0000 0000 0008 0000 0006 0000 0043  ...............C
-00000840: 0000 0073 6e00 0000 6700 7d02 7c00 6a00  ...sn...g.}.|.j.
-00000850: 4400 5d10 7d03 7c03 6a01 7215 7c03 6a01  D.].}.|.j.r.|.j.
-00000860: a002 7c01 a101 7d04 7c02 a003 7c04 a101  ..|...}.|...|...
-00000870: 0100 7105 7404 a005 7c02 a101 a006 a100  ..q.t...|.......
-00000880: 7d05 7404 a005 7c02 a101 a007 a100 7d06  }.t...|.......}.
-00000890: 6401 7c01 9b00 6402 7c05 9b00 6403 7c06  d.|...d.|...d.|.
-000008a0: 9b00 9d06 7d07 7408 7c07 8301 0100 7c05  ....}.t.|.....|.
-000008b0: 7c06 6602 5300 2904 61a2 0100 000a 2020  |.f.S.).a.....  
-000008c0: 2020 2020 2020 5368 6f77 206f 7574 206f        Show out o
-000008d0: 6620 666f 6c64 2073 636f 7265 732e 0a0a  f fold scores...
-000008e0: 2020 2020 2020 2020 5768 656e 2063 616c          When cal
-000008f0: 6c69 6e67 2042 6c75 6543 6173 7443 5652  ling BlueCastCVR
-00000900: 6567 7265 7373 696f 6e27 7320 6669 745f  egression's fit_
-00000910: 6576 616c 2066 756e 6374 696f 6e20 6d75  eval function mu
-00000920: 6c74 6970 6c65 2042 6c75 6543 6173 7452  ltiple BlueCastR
-00000930: 6567 7265 7373 696f 6e0a 2020 2020 2020  egression.      
-00000940: 2020 696e 7374 616e 6365 7320 6172 6520    instances are 
-00000950: 6361 6c6c 6564 2061 6e64 2065 6163 6820  called and each 
-00000960: 6f66 2074 6865 6d20 7072 6564 6963 7473  of them predicts
-00000970: 206f 6e20 756e 7365 656e 2f6f 6f66 2064   on unseen/oof d
-00000980: 6174 612e 0a0a 2020 2020 2020 2020 5468  ata...        Th
-00000990: 6973 2066 756e 6374 696f 6e20 636f 6c6c  is function coll
-000009a0: 6563 7473 2074 6865 7365 2073 636f 7265  ects these score
-000009b0: 7320 616e 6420 7265 7475 726e 206d 6561  s and return mea
-000009c0: 6e20 616e 6420 6176 6572 6167 6520 6f66  n and average of
-000009d0: 2074 6865 6d2e 0a0a 2020 2020 2020 2020   them...        
-000009e0: 3a70 6172 616d 206d 6574 7269 633a 2053  :param metric: S
-000009f0: 7472 696e 6720 696e 6469 6361 7469 6e67  tring indicating
-00000a00: 2077 6869 6368 206d 6574 7269 6320 7368   which metric sh
-00000a10: 616c 6c20 6265 2072 6574 7572 6e65 642e  all be returned.
-00000a20: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00000a30: 3a20 5475 706c 6520 7769 7468 2028 6d65  : Tuple with (me
-00000a40: 616e 2c20 7374 6429 206f 6620 6f6f 6620  an, std) of oof 
-00000a50: 7363 6f72 6573 0a20 2020 2020 2020 207a  scores.        z
-00000a60: 1554 6865 206d 6561 6e20 6f75 7420 6f66  .The mean out of
-00000a70: 2066 6f6c 6420 7a0a 2073 636f 7265 2069   fold z. score i
-00000a80: 7320 7a10 2077 6974 6820 616e 2073 7464  s z. with an std
-00000a90: 206f 6620 2909 7220 0000 00da 0c65 7661   of ).r .....eva
-00000aa0: 6c5f 6d65 7472 6963 73da 0367 6574 da06  l_metrics..get..
-00000ab0: 6170 7065 6e64 da02 6e70 da07 6173 6172  append..np..asar
-00000ac0: 7261 79da 046d 6561 6eda 0373 7464 720f  ray..mean..stdr.
-00000ad0: 0000 0029 0872 2200 0000 7233 0000 00da  ...).r"...r3....
-00000ae0: 0b61 6c6c 5f6d 6574 7269 6373 da11 626c  .all_metrics..bl
-00000af0: 7565 6361 7374 5f69 6e73 7461 6e63 65da  uecast_instance.
-00000b00: 0573 636f 7265 da0a 7363 6f72 655f 6d65  .score..score_me
-00000b10: 616e da09 7363 6f72 655f 7374 64da 076d  an..score_std..m
-00000b20: 6573 7361 6765 7223 0000 0072 2300 0000  essager#...r#...
-00000b30: 7224 0000 00da 0f73 686f 775f 6f6f 665f  r$.....show_oof_
-00000b40: 7363 6f72 6573 4900 0000 7316 0000 0004  scoresI...s.....
-00000b50: 0c0a 0106 010c 010a 0102 800e 020e 0116  ................
-00000b60: 0108 0108 027a 2442 6c75 6543 6173 7443  .....z$BlueCastC
-00000b70: 5652 6567 7265 7373 696f 6e2e 7368 6f77  VRegression.show
-00000b80: 5f6f 6f66 5f73 636f 7265 73da 0a74 6172  _oof_scores..tar
-00000b90: 6765 745f 636f 6c63 0300 0000 0000 0000  get_colc........
-00000ba0: 0000 0000 0e00 0000 0d00 0000 4300 0000  ............C...
-00000bb0: 734c 0100 007c 00a0 007c 017c 02a1 025c  sL...|...|.|...\
-00000bc0: 027d 037d 047c 006a 0173 0f74 0283 007c  .}.}.|.j.s.t...|
-00000bd0: 005f 017c 006a 0373 1c74 0464 0164 027c  ._.|.j.s.t.d.d.|
-00000be0: 006a 016a 0564 038d 037c 005f 0374 067c  .j.j.d...|._.t.|
-00000bf0: 006a 03a0 077c 037c 04a1 0283 0144 005d  .j...|.|.....D.]
-00000c00: 7e5c 027d 055c 027d 067d 077c 036a 087c  ~\.}.\.}.}.|.j.|
-00000c10: 0619 007c 036a 087c 0719 0002 027d 087d  ...|.j.|.....}.}
-00000c20: 097c 046a 087c 0619 007c 046a 087c 0719  .|.j.|...|.j.|..
-00000c30: 0002 027d 0a7d 0b74 096a 0a7c 087c 0967  ...}.}.t.j.|.|.g
-00000c40: 0264 0264 048d 027d 0c74 096a 0a7c 0a7c  .d.d...}.t.j.|.|
-00000c50: 0b67 0264 0264 048d 027d 0a7c 0c6a 0b64  .g.d.d...}.|.j.d
-00000c60: 0264 058d 017d 087c 0a6a 0b64 0264 058d  .d...}.|.j.d.d..
-00000c70: 017d 0a7c 0a6a 0c7c 087c 023c 007c 006a  .}.|.j.|.|.<.|.j
-00000c80: 0104 006a 057c 006a 016a 0d37 0002 005f  ...j.|.j.j.7..._
-00000c90: 0574 0e64 067c 059b 0064 077c 006a 016a  .t.d.|...d.|.j.j
-00000ca0: 059b 009d 0483 0101 0074 0f7c 006a 107c  .........t.|.j.|
-00000cb0: 006a 017c 006a 117c 006a 127c 006a 137c  .j.|.j.|.j.|.j.|
-00000cc0: 006a 147c 006a 157c 006a 167c 006a 177c  .j.|.j.|.j.|.j.|
-00000cd0: 006a 1864 088d 0a7d 0d7c 0d6a 197c 087c  .j.d...}.|.j.|.|
-00000ce0: 0264 098d 0201 007c 006a 1aa0 1b7c 0da1  .d.....|.j...|..
-00000cf0: 0101 007c 0d6a 137c 005f 1371 2564 0a53  ...|.j.|._.q%d.S
-00000d00: 0029 0b7a 7446 6974 206d 756c 7469 706c  .).ztFit multipl
-00000d10: 6520 426c 7565 4361 7374 5265 6772 6573  e BlueCastRegres
-00000d20: 7369 6f6e 2069 6e73 7461 6e63 6573 206f  sion instances o
-00000d30: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
-00000d40: 2073 706c 6974 732e 0a0a 2020 2020 2020   splits...      
-00000d50: 2020 496e 7075 7420 6466 2069 7320 6578    Input df is ex
-00000d60: 7065 6374 6564 2074 6865 2074 6172 6765  pected the targe
-00000d70: 7420 636f 6c75 6d6e 2ee9 0500 0000 54a9  t column......T.
-00000d80: 03da 086e 5f73 706c 6974 73da 0773 6875  ...n_splits..shu
-00000d90: 6666 6c65 da0c 7261 6e64 6f6d 5f73 7461  ffle..random_sta
-00000da0: 7465 2901 da0c 6967 6e6f 7265 5f69 6e64  te)...ignore_ind
-00000db0: 6578 7229 0000 00fa 1b53 7461 7274 2066  exr).....Start f
-00000dc0: 6974 7469 6e67 206d 6f64 656c 206e 756d  itting model num
-00000dd0: 6265 7220 fa12 2077 6974 6820 7261 6e64  ber .. with rand
-00000de0: 6f6d 2073 6565 6420 a90a 7215 0000 0072  om seed ..r....r
-00000df0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000e00: 0000 0072 1b00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000e10: 0000 721c 0000 0072 1f00 0000 a901 7242  ..r....r......rB
-00000e20: 0000 004e 291c 7231 0000 0072 1700 0000  ...N).r1...r....
-00000e30: 720a 0000 0072 1600 0000 7208 0000 00da  r....r....r.....
-00000e40: 1367 6c6f 6261 6c5f 7261 6e64 6f6d 5f73  .global_random_s
-00000e50: 7461 7465 da09 656e 756d 6572 6174 65da  tate..enumerate.
-00000e60: 0573 706c 6974 da04 696c 6f63 da02 7064  .split..iloc..pd
-00000e70: da06 636f 6e63 6174 722e 0000 00da 0676  ..concatr......v
-00000e80: 616c 7565 73da 2769 6e63 7265 6173 655f  alues.'increase_
-00000e90: 7261 6e64 6f6d 5f73 7461 7465 5f69 6e5f  random_state_in_
-00000ea0: 626c 7565 6361 7374 5f63 765f 6279 720f  bluecast_cv_byr.
-00000eb0: 0000 0072 0900 0000 7215 0000 0072 1800  ...r....r....r..
-00000ec0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000ed0: 0072 1d00 0000 721e 0000 0072 1c00 0000  .r....r....r....
-00000ee0: 721f 0000 00da 0366 6974 7220 0000 0072  r......fitr ...r
-00000ef0: 3600 0000 290e 7222 0000 0072 2600 0000  6...).r"...r&...
-00000f00: 7242 0000 0072 3000 0000 722f 0000 00da  rB...r0...r/....
-00000f10: 0266 6eda 0774 726e 5f69 6478 da07 7661  .fn..trn_idx..va
-00000f20: 6c5f 6964 78da 0758 5f74 7261 696e da05  l_idx..X_train..
-00000f30: 585f 7661 6cda 0779 5f74 7261 696e da05  X_val..y_train..
-00000f40: 795f 7661 6cda 0778 5f74 7261 696e da06  y_val..x_train..
-00000f50: 6175 746f 6d6c 7223 0000 0072 2300 0000  automlr#...r#...
-00000f60: 7224 0000 0072 5500 0000 6200 0000 734e  r$...rU...b...sN
-00000f70: 0000 0010 0406 0208 0106 0202 0102 0102  ................
-00000f80: 0106 0108 fd1e 0616 0116 0112 0112 010c  ................
-00000f90: 020c 010a 0108 0206 0106 ff02 0312 0104  ................
-00000fa0: ff02 0404 0104 0104 0104 0104 0104 0104  ................
-00000fb0: 0104 0104 0104 0106 f60e 0c0c 010a 0304  ................
-00000fc0: df7a 1842 6c75 6543 6173 7443 5652 6567  .z.BlueCastCVReg
-00000fd0: 7265 7373 696f 6e2e 6669 7463 0300 0000  ression.fitc....
-00000fe0: 0000 0000 0000 0000 0f00 0000 0d00 0000  ................
-00000ff0: 4300 0000 732c 0100 007c 00a0 007c 017c  C...s,...|...|.|
-00001000: 02a1 025c 027d 037d 047c 006a 0173 0f74  ...\.}.}.|.j.s.t
-00001010: 0283 007c 005f 017c 006a 0373 1c74 0464  ...|._.|.j.s.t.d
-00001020: 0164 027c 006a 016a 0564 038d 037c 005f  .d.|.j.j.d...|._
-00001030: 0374 067c 006a 03a0 077c 037c 04a1 0283  .t.|.j...|.|....
-00001040: 0144 005d 665c 027d 055c 027d 067d 077c  .D.]f\.}.\.}.}.|
-00001050: 036a 087c 0619 007c 036a 087c 0719 0002  .j.|...|.j.|....
-00001060: 027d 087d 097c 046a 087c 0619 007c 046a  .}.}.|.j.|...|.j
-00001070: 087c 0719 0002 027d 0a7d 0b7c 0a7c 086a  .|.....}.}.|.|.j
-00001080: 0964 0464 0485 027c 0266 023c 007c 006a  .d.d...|.f.<.|.j
-00001090: 0104 006a 057c 006a 016a 0a37 0002 005f  ...j.|.j.j.7..._
-000010a0: 0574 0b64 057c 059b 0064 067c 006a 016a  .t.d.|...d.|.j.j
-000010b0: 059b 009d 0483 0101 0074 0c7c 006a 0d7c  .........t.|.j.|
-000010c0: 006a 017c 006a 0e7c 006a 0f7c 006a 107c  .j.|.j.|.j.|.j.|
-000010d0: 006a 117c 006a 127c 006a 137c 006a 147c  .j.|.j.|.j.|.j.|
-000010e0: 006a 1564 078d 0a7d 0c7c 0c6a 167c 087c  .j.d...}.|.j.|.|
-000010f0: 097c 0b7c 0264 088d 0401 007c 006a 17a0  .|.|.d.....|.j..
-00001100: 187c 0ca1 0101 007c 0c6a 107c 005f 1071  .|.....|.j.|._.q
-00001110: 257c 00a0 19a1 005c 027d 0d7d 0e7c 0d7c  %|.....\.}.}.|.|
-00001120: 0e66 0253 0029 0961 a601 0000 4669 7420  .f.S.).a....Fit 
-00001130: 6d75 6c74 6970 6c65 2042 6c75 6543 6173  multiple BlueCas
-00001140: 7452 6567 7265 7373 696f 6e20 696e 7374  tRegression inst
-00001150: 616e 6365 7320 6f6e 2064 6966 6665 7265  ances on differe
-00001160: 6e74 2064 6174 6120 7370 6c69 7473 2e0a  nt data splits..
-00001170: 0a20 2020 2020 2020 2049 6e70 7574 2064  .        Input d
-00001180: 6620 6973 2065 7870 6563 7465 6420 7468  f is expected th
-00001190: 6520 7461 7267 6574 2063 6f6c 756d 6e2e  e target column.
-000011a0: 2045 7661 6c75 6174 696f 6e20 6973 2065   Evaluation is e
-000011b0: 7865 6375 7465 6420 6f6e 206f 7574 2d6f  xecuted on out-o
-000011c0: 662d 666f 6c64 2064 6174 6173 6574 0a20  f-fold dataset. 
-000011d0: 2020 2020 2020 2069 6e20 6561 6368 2073         in each s
-000011e0: 706c 6974 2e0a 2020 2020 2020 2020 3a70  plit..        :p
-000011f0: 6172 616d 2064 663a 2050 616e 6461 7320  aram df: Pandas 
-00001200: 4461 7461 4672 616d 6520 7468 6174 2069  DataFrame that i
-00001210: 6e63 6c75 6465 7320 7468 6520 7461 7267  ncludes the targ
-00001220: 6574 2063 6f6c 756d 6e0a 2020 2020 2020  et column.      
-00001230: 2020 3a70 6172 616d 2074 6172 6765 745f    :param target_
-00001240: 636f 6c3a 2053 7472 696e 6720 696e 6469  col: String indi
-00001250: 6361 7469 6e67 2074 6865 206e 616d 6520  cating the name 
-00001260: 6f66 2074 6865 2074 6172 6765 7420 636f  of the target co
-00001270: 6c75 6d6e 0a20 2020 2020 2020 203a 7265  lumn.        :re
-00001280: 7475 726e 7320 5475 706c 6520 6f66 2028  turns Tuple of (
-00001290: 6f6f 665f 6d65 616e 2c20 6f6f 665f 7374  oof_mean, oof_st
-000012a0: 6429 2077 6974 6820 7363 6f72 6573 206f  d) with scores o
-000012b0: 6e20 756e 7365 656e 2064 6174 6120 6475  n unseen data du
-000012c0: 7269 6e67 2065 7661 6c0a 2020 2020 2020  ring eval.      
-000012d0: 2020 7243 0000 0054 7244 0000 004e 7249    rC...TrD...NrI
-000012e0: 0000 0072 4a00 0000 724b 0000 0072 4c00  ...rJ...rK...rL.
-000012f0: 0000 291a 7231 0000 0072 1700 0000 720a  ..).r1...r....r.
-00001300: 0000 0072 1600 0000 7208 0000 0072 4d00  ...r....r....rM.
-00001310: 0000 724e 0000 0072 4f00 0000 7250 0000  ..rN...rO...rP..
-00001320: 00da 036c 6f63 7254 0000 0072 0f00 0000  ...locrT...r....
-00001330: 7209 0000 0072 1500 0000 7218 0000 0072  r....r....r....r
-00001340: 1900 0000 721a 0000 0072 1b00 0000 721d  ....r....r....r.
-00001350: 0000 0072 1e00 0000 721c 0000 0072 1f00  ...r....r....r..
-00001360: 0000 da08 6669 745f 6576 616c 7220 0000  ....fit_evalr ..
-00001370: 0072 3600 0000 7241 0000 0029 0f72 2200  .r6...rA...).r".
-00001380: 0000 7226 0000 0072 4200 0000 7230 0000  ..r&...rB...r0..
-00001390: 0072 2f00 0000 7256 0000 0072 5700 0000  .r/...rV...rW...
-000013a0: 7258 0000 0072 5900 0000 725a 0000 0072  rX...rY...rZ...r
-000013b0: 5b00 0000 725c 0000 0072 5e00 0000 da08  [...r\...r^.....
-000013c0: 6f6f 665f 6d65 616e da07 6f6f 665f 7374  oof_mean..oof_st
-000013d0: 6472 2300 0000 7223 0000 0072 2400 0000  dr#...r#...r$...
-000013e0: 7260 0000 0095 0000 0073 4800 0000 1009  r`.......sH.....
-000013f0: 0602 0801 0602 0201 0201 0201 0601 08fd  ................
-00001400: 1e06 1601 1601 1202 0802 0601 06ff 0203  ................
-00001410: 1201 04ff 0204 0401 0401 0401 0401 0401  ................
-00001420: 0401 0401 0401 0401 0401 06f6 120c 0c01  ................
-00001430: 0a03 0c02 0801 7a1d 426c 7565 4361 7374  ......z.BlueCast
-00001440: 4356 5265 6772 6573 7369 6f6e 2e66 6974  CVRegression.fit
-00001450: 5f65 7661 6c46 da17 7265 7475 726e 5f73  _evalF..return_s
-00001460: 7562 5f6d 6f64 656c 735f 7072 6564 73da  ub_models_preds.
-00001470: 1073 6176 655f 7368 6170 5f76 616c 7565  .save_shap_value
-00001480: 7363 0400 0000 0000 0000 0000 0000 0a00  sc..............
-00001490: 0000 0500 0000 4300 0000 7374 0000 007c  ......C...st...|
-000014a0: 016a 007d 0467 007d 0574 01a0 02a1 007d  .j.}.g.}.t.....}
-000014b0: 0674 037c 006a 0483 0144 005d 215c 027d  .t.|.j...D.]!\.}
-000014c0: 077d 087c 086a 057c 016a 0664 0164 0185  .}.|.j.|.j.d.d..
-000014d0: 027c 0466 0219 007c 0364 028d 027d 097c  .|.f...|.d...}.|
-000014e0: 097c 0664 037c 079b 009d 023c 007c 05a0  .|.d.|.....<.|..
-000014f0: 0764 037c 079b 009d 02a1 0101 0071 0e7c  .d.|.........q.|
-00001500: 0272 347c 0653 007c 066a 0864 0464 058d  .r4|.S.|.j.d.d..
-00001510: 0153 0029 0661 bd01 0000 5072 6564 6963  .S.).a....Predic
-00001520: 7420 6f6e 2075 6e73 6565 6e20 6461 7461  t on unseen data
-00001530: 2075 7369 6e67 206d 756c 7469 706c 6520   using multiple 
-00001540: 7472 6169 6e65 6420 426c 7565 4361 7374  trained BlueCast
-00001550: 5265 6772 6573 7369 6f6e 2069 6e73 7461  Regression insta
-00001560: 6e63 6573 2e0a 0a20 2020 2020 2020 203a  nces...        :
-00001570: 7061 7261 6d20 6466 3a20 5061 6e64 6173  param df: Pandas
-00001580: 2044 6174 6146 7261 6d65 2077 6974 6820   DataFrame with 
-00001590: 756e 7365 656e 2064 6174 610a 2020 2020  unseen data.    
-000015a0: 2020 2020 3a70 6172 616d 2072 6574 7572      :param retur
-000015b0: 6e5f 7375 625f 6d6f 6465 6c73 5f70 7265  n_sub_models_pre
-000015c0: 6473 3a20 4966 2074 7275 6520 7769 6c6c  ds: If true will
-000015d0: 2072 6574 7572 6e20 6120 4461 7461 4672   return a DataFr
-000015e0: 616d 6520 7769 7468 2074 6865 2070 7265  ame with the pre
-000015f0: 6469 6374 696f 6e73 206f 6620 6561 6368  dictions of each
-00001600: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-00001610: 2020 2073 746f 7265 6420 696e 2073 6570     stored in sep
-00001620: 6172 6174 6520 636f 6c75 6d6e 732e 0a20  arate columns.. 
-00001630: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-00001640: 7665 5f73 6861 705f 7661 6c75 6573 3a20  ve_shap_values: 
-00001650: 4966 2054 7275 652c 2063 616c 6375 6c61  If True, calcula
-00001660: 7465 7320 616e 6420 7361 7665 7320 7368  tes and saves sh
-00001670: 6170 2076 616c 7565 732c 2073 6f20 7468  ap values, so th
-00001680: 6579 2063 616e 2062 6520 7573 6564 2074  ey can be used t
-00001690: 6f20 706c 6f74 0a20 2020 2020 2020 2020  o plot.         
-000016a0: 2020 2077 6174 6572 6661 6c6c 2070 6c6f     waterfall plo
-000016b0: 7473 2066 6f72 2073 656c 6563 7465 6420  ts for selected 
-000016c0: 726f 7773 206f 2064 656d 616e 642e 0a20  rows o demand.. 
-000016d0: 2020 2020 2020 204e 2901 7264 0000 005a         N).rd...Z
-000016e0: 0670 7265 6473 5f72 2b00 0000 722c 0000  .preds_r+...r,..
-000016f0: 0029 09da 0763 6f6c 756d 6e73 7251 0000  .)...columnsrQ..
-00001700: 00da 0944 6174 6146 7261 6d65 724e 0000  ...DataFramerN..
-00001710: 0072 2000 0000 da07 7072 6564 6963 7472  .r .....predictr
-00001720: 5f00 0000 7236 0000 0072 3900 0000 290a  _...r6...r9...).
-00001730: 7222 0000 0072 2600 0000 7263 0000 0072  r"...r&...rc...r
-00001740: 6400 0000 da07 6f72 5f63 6f6c 735a 0970  d.....or_colsZ.p
-00001750: 7265 645f 636f 6c73 da09 7265 7375 6c74  red_cols..result
-00001760: 5f64 6672 5600 0000 da08 7069 7065 6c69  _dfrV.....pipeli
-00001770: 6e65 da07 795f 7072 6564 7372 2300 0000  ne..y_predsr#...
-00001780: 7223 0000 0072 2400 0000 7267 0000 00cc  r#...r$...rg....
-00001790: 0000 0073 1800 0000 060e 0401 0801 1202  ...s............
-000017a0: 0401 1201 06ff 0e03 1201 0402 0401 0c02  ................
-000017b0: 7a1c 426c 7565 4361 7374 4356 5265 6772  z.BlueCastCVRegr
-000017c0: 6573 7369 6f6e 2e70 7265 6469 6374 da0d  ession.predict..
-000017d0: 785f 6361 6c69 6272 6174 696f 6eda 0d79  x_calibration..y
-000017e0: 5f63 616c 6962 7261 7469 6f6e 6303 0000  _calibrationc...
-000017f0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001800: 004b 0000 0073 2400 0000 7400 7c00 6601  .K...s$...t.|.f.
-00001810: 6900 7c03 a401 8e01 7c00 5f01 7c00 6a01  i.|.....|._.|.j.
-00001820: a002 7c01 7c02 a102 0100 6401 5300 2902  ..|.|.....d.S.).
-00001830: 61ee 0100 0043 616c 6962 7261 7465 2074  a....Calibrate t
-00001840: 6865 206d 6f64 656c 2e0a 0a20 2020 2020  he model...     
-00001850: 2020 2056 6961 2074 6869 7320 6675 6e63     Via this func
-00001860: 7469 6f6e 2074 6865 206e 6f6e 636f 6e66  tion the nonconf
-00001870: 6f72 6d69 7479 206d 6561 7375 7265 7320  ormity measures 
-00001880: 6172 6520 7461 6b65 6e20 616e 6420 7573  are taken and us
-00001890: 6564 2074 6f20 7072 6564 6963 7420 7072  ed to predict pr
-000018a0: 6564 6963 7469 6f6e 2069 6e74 6572 7661  ediction interva
-000018b0: 6c73 2076 6973 2074 6865 0a20 2020 2020  ls vis the.     
-000018c0: 2020 2070 7265 6469 6374 5f69 6e74 6572     predict_inter
-000018d0: 7661 6c20 6675 6e63 7469 6f6e 2e20 5573  val function. Us
-000018e0: 6564 2069 7320 7468 6520 6d65 616e 2070  ed is the mean p
-000018f0: 7265 6469 6374 696f 6e20 6f66 2061 6c6c  rediction of all
-00001900: 2073 7562 206d 6f64 656c 732e 0a20 2020   sub models..   
-00001910: 2020 2020 203a 7061 7261 6d3a 2078 5f63       :param: x_c
-00001920: 616c 6962 7261 7469 6f6e 3a20 5061 6e64  alibration: Pand
-00001930: 6173 2044 6174 6146 7261 6d65 2077 6974  as DataFrame wit
-00001940: 686f 7574 2074 6172 6765 7420 636f 6c75  hout target colu
-00001950: 6d6e 2c20 7468 6174 2068 6173 206e 6f74  mn, that has not
-00001960: 2062 6565 6e20 7365 656e 2062 7920 7468   been seen by th
-00001970: 6520 6d6f 6465 6c20 6475 7269 6e67 0a20  e model during. 
-00001980: 2020 2020 2020 2020 2020 2074 7261 696e             train
-00001990: 696e 672e 0a20 2020 2020 2020 203a 7061  ing..        :pa
-000019a0: 7261 6d20 795f 6361 6c69 6272 6174 696f  ram y_calibratio
-000019b0: 6e3a 2050 616e 6461 7320 5365 7269 6573  n: Pandas Series
-000019c0: 2068 6f6c 6469 6e67 2074 6865 2074 6172   holding the tar
-000019d0: 6765 7420 7661 6c75 652c 2068 6174 2068  get value, hat h
-000019e0: 6173 206e 6f74 2062 6565 6e20 7365 656e  as not been seen
-000019f0: 2062 7920 7468 6520 6d6f 6465 6c20 6475   by the model du
-00001a00: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
-00001a10: 2074 7261 696e 696e 672e 0a20 2020 2020   training..     
-00001a20: 2020 204e 2903 720d 0000 0072 2100 0000     N).r....r!...
-00001a30: da09 6361 6c69 6272 6174 6529 0472 2200  ..calibrate).r".
-00001a40: 0000 726c 0000 0072 6d00 0000 da06 6b77  ..rl...rm.....kw
-00001a50: 6172 6773 7223 0000 0072 2300 0000 7224  argsr#...r#...r$
-00001a60: 0000 0072 6e00 0000 ea00 0000 730c 0000  ...rn.......s...
-00001a70: 0002 0c02 0104 ff02 0108 ff12 037a 1e42  .............z.B
-00001a80: 6c75 6543 6173 7443 5652 6567 7265 7373  lueCastCVRegress
-00001a90: 696f 6e2e 6361 6c69 6272 6174 65da 0661  ion.calibrate..a
-00001aa0: 6c70 6861 7363 0300 0000 0000 0000 0000  lphasc..........
-00001ab0: 0000 0400 0000 0400 0000 4300 0000 7322  ..........C...s"
-00001ac0: 0000 007c 006a 0072 0d7c 006a 006a 017c  ...|.j.r.|.j.j.|
-00001ad0: 017c 0264 018d 027d 037c 0353 0074 0264  .|.d...}.|.S.t.d
-00001ae0: 0283 0182 0129 0361 4202 0000 4372 6561  .....).aB...Crea
-00001af0: 7465 2070 7265 6469 6374 696f 6e20 696e  te prediction in
-00001b00: 7465 7276 616c 7320 6261 7365 6420 6f6e  tervals based on
-00001b10: 2061 2063 6572 7461 696e 2063 6f6e 6669   a certain confi
-00001b20: 6465 6e63 6520 6c65 7665 6c73 2e0a 0a20  dence levels... 
-00001b30: 2020 2020 2020 2043 6f6e 666f 726d 616c         Conformal
-00001b40: 2070 7265 6469 6374 696f 6e20 6775 6172   prediction guar
-00001b50: 616e 7465 6573 2c20 7468 6174 2074 6865  antees, that the
-00001b60: 2063 6f72 7265 6374 2076 616c 7565 2069   correct value i
-00001b70: 7320 7072 6573 656e 7420 696e 2074 6865  s present in the
-00001b80: 2070 7265 6469 6374 696f 6e20 6261 6e64   prediction band
-00001b90: 2077 6974 6820 6120 7072 6f62 6162 696c   with a probabil
-00001ba0: 6974 7920 6f66 0a20 2020 2020 2020 2031  ity of.        1
-00001bb0: 202d 2061 6c70 6861 2e0a 2020 2020 2020   - alpha..      
-00001bc0: 2020 3a70 6172 616d 2064 663a 2050 616e    :param df: Pan
-00001bd0: 6461 7320 4461 7461 4672 616d 6520 686f  das DataFrame ho
-00001be0: 6c64 696e 6720 756e 7365 656e 2064 6174  lding unseen dat
-00001bf0: 610a 2020 2020 2020 2020 3a70 6172 616d  a.        :param
-00001c00: 2061 6c70 6861 733a 204c 6973 7420 6f66   alphas: List of
-00001c10: 2066 6c6f 6174 7320 696e 6469 6361 7469   floats indicati
-00001c20: 6e67 2074 6865 2064 6573 6972 6564 2063  ng the desired c
-00001c30: 6f6e 6669 6465 6e63 6520 6c65 7665 6c73  onfidence levels
-00001c40: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001c50: 6e73 2041 2050 616e 6461 7320 4461 7461  ns A Pandas Data
-00001c60: 4672 616d 6520 7769 7468 2020 736f 7274  Frame with  sort
-00001c70: 6564 2063 6f6c 756d 6e73 2027 616c 7068  ed columns 'alph
-00001c80: 615f 5858 5f6c 6f77 2720 2861 6c70 6861  a_XX_low' (alpha
-00001c90: 2920 616e 6420 2761 6c70 6861 5f58 585f  ) and 'alpha_XX_
-00001ca0: 6869 6768 2720 2831 202d 2061 6c70 6861  high' (1 - alpha
-00001cb0: 2920 666f 7220 6561 6368 0a20 2020 2020  ) for each.     
-00001cc0: 2020 2020 2020 2061 6c70 6861 2069 6e20         alpha in 
-00001cd0: 7468 6520 7072 6f76 6964 6564 206c 6973  the provided lis
-00001ce0: 7420 6f66 2061 6c70 6861 732e 2054 6f20  t of alphas. To 
-00001cf0: 6f62 7461 696e 2074 6865 206d 6561 6e20  obtain the mean 
-00001d00: 7072 6564 6963 7469 6f6e 2063 616c 6c20  prediction call 
-00001d10: 7468 6520 2770 7265 6469 6374 2720 6d65  the 'predict' me
-00001d20: 7468 6f64 2e0a 2020 2020 2020 2020 2901  thod..        ).
-00001d30: 7270 0000 007a 7354 6869 7320 696e 7374  rp...zsThis inst
-00001d40: 616e 6365 2068 6173 206e 6f74 2062 6565  ance has not bee
-00001d50: 6e20 6361 6c69 6272 6174 6564 2079 6574  n calibrated yet
-00001d60: 2e20 4d61 6b65 2075 7365 206f 6620 6361  . Make use of ca
-00001d70: 6c69 6272 6174 6520 746f 2066 6974 2074  librate to fit t
-00001d80: 6865 0a20 2020 2020 2020 2020 2020 2043  he.            C
-00001d90: 6f6e 666f 726d 616c 5072 6564 6963 7469  onformalPredicti
-00001da0: 6f6e 5772 6170 7065 722e 2903 7221 0000  onWrapper.).r!..
-00001db0: 00da 1070 7265 6469 6374 5f69 6e74 6572  ...predict_inter
-00001dc0: 7661 6cda 0a56 616c 7565 4572 726f 7229  val..ValueError)
-00001dd0: 0472 2200 0000 7226 0000 0072 7000 0000  .r"...r&...rp...
-00001de0: da0d 7072 6564 5f69 6e74 6572 7661 6c72  ..pred_intervalr
-00001df0: 2300 0000 7223 0000 0072 2400 0000 7271  #...r#...r$...rq
-00001e00: 0000 00fb 0000 0073 1000 0000 060a 0601  .......s........
-00001e10: 0401 06ff 0403 0202 0201 04ff 7a25 426c  ............z%Bl
-00001e20: 7565 4361 7374 4356 5265 6772 6573 7369  ueCastCVRegressi
-00001e30: 6f6e 2e70 7265 6469 6374 5f69 6e74 6572  on.predict_inter
-00001e40: 7661 6c29 0b72 1400 0000 4e4e 4e4e 4e4e  val).r....NNNNNN
-00001e50: 4e4e 4e4e 2901 7232 0000 0029 0246 4629  NNNN).r2...).FF)
-00001e60: 1fda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001e70: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001e80: 616d 655f 5fda 075f 5f64 6f63 5f5f 7204  ame__..__doc__r.
-00001e90: 0000 0072 0500 0000 7202 0000 0072 0a00  ...r....r....r..
-00001ea0: 0000 da17 5867 626f 6f73 7454 756e 6550  ....XgboostTuneP
-00001eb0: 6172 616d 7343 6f6e 6669 6772 0b00 0000  aramsConfigr....
-00001ec0: 720e 0000 0072 1100 0000 7207 0000 0072  r....r....r....r
-00001ed0: 1200 0000 7210 0000 0072 2500 0000 7251  ....r....r%...rQ
-00001ee0: 0000 0072 6600 0000 da03 7374 7272 0600  ...rf.....strr..
-00001ef0: 0000 da06 5365 7269 6573 7231 0000 00da  ....Seriesr1....
-00001f00: 0566 6c6f 6174 7241 0000 0072 5500 0000  .floatrA...rU...
-00001f10: 7260 0000 00da 0462 6f6f 6c72 6700 0000  r`.....boolrg...
-00001f20: 726e 0000 0072 0300 0000 7271 0000 0072  rn...r....rq...r
-00001f30: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
-00001f40: 0000 0072 1300 0000 1600 0000 7386 0000  ...r........s...
-00001f50: 0008 0004 0102 0802 0102 0102 0102 0102  ................
-00001f60: 0102 0102 0102 0102 0302 0104 f206 0202  ................
-00001f70: fe06 0302 fd06 0402 fc06 0502 fb06 0602  ................
-00001f80: fa06 0702 f906 0802 f806 0902 f706 0a02  ................
-00001f90: f602 0b0a 0102 ff02 f50e 0e0a f202 2404  ..............$.
-00001fa0: 0102 ff02 0102 ff0e 020a fe1c 0818 1920  ............... 
-00001fb0: 3302 3a02 0104 fc04 0202 fe02 0302 fd02  3.:.............
-00001fc0: 0402 fc0e 050a fb02 1e04 0102 ff04 0102  ................
-00001fd0: ff02 020a fe22 1172 1300 0000 2921 da06  .....".r....)!..
-00001fe0: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00001ff0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00002000: 0700 0000 da05 6e75 6d70 7972 3700 0000  ......numpyr7...
-00002010: da06 7061 6e64 6173 7251 0000 00da 1773  ..pandasrQ.....s
-00002020: 6b6c 6561 726e 2e6d 6f64 656c 5f73 656c  klearn.model_sel
-00002030: 6563 7469 6f6e 7208 0000 00da 2362 6c75  ectionr.....#blu
-00002040: 6563 6173 742e 626c 7565 7072 696e 7473  ecast.blueprints
-00002050: 2e63 6173 745f 7265 6772 6573 7369 6f6e  .cast_regression
-00002060: 7209 0000 00da 1f62 6c75 6563 6173 742e  r......bluecast.
-00002070: 636f 6e66 6967 2e74 7261 696e 696e 675f  config.training_
-00002080: 636f 6e66 6967 720a 0000 0072 0b00 0000  configr....r....
-00002090: 720c 0000 0072 7800 0000 da3d 626c 7565  r....rx....=blue
-000020a0: 6361 7374 2e63 6f6e 666f 726d 616c 5f70  cast.conformal_p
-000020b0: 7265 6469 6374 696f 6e2e 636f 6e66 6f72  rediction.confor
-000020c0: 6d61 6c5f 7072 6564 6963 7469 6f6e 5f72  mal_prediction_r
-000020d0: 6567 7265 7373 696f 6e72 0d00 0000 da21  egressionr.....!
-000020e0: 626c 7565 6361 7374 2e65 7870 6572 696d  bluecast.experim
-000020f0: 656e 7461 7469 6f6e 2e74 7261 636b 696e  entation.trackin
-00002100: 6772 0e00 0000 da24 626c 7565 6361 7374  gr.....$bluecast
-00002110: 2e67 656e 6572 616c 5f75 7469 6c73 2e67  .general_utils.g
-00002120: 656e 6572 616c 5f75 7469 6c73 720f 0000  eneral_utilsr...
-00002130: 00da 1d62 6c75 6563 6173 742e 6d6c 5f6d  ...bluecast.ml_m
-00002140: 6f64 656c 6c69 6e67 2e78 6762 6f6f 7374  odelling.xgboost
-00002150: 7210 0000 00da 1d62 6c75 6563 6173 742e  r......bluecast.
-00002160: 7072 6570 726f 6365 7373 696e 672e 6375  preprocessing.cu
-00002170: 7374 6f6d 7211 0000 00da 2862 6c75 6563  stomr.....(bluec
-00002180: 6173 742e 7072 6570 726f 6365 7373 696e  ast.preprocessin
-00002190: 672e 6665 6174 7572 655f 7365 6c65 6374  g.feature_select
-000021a0: 696f 6e72 1200 0000 7213 0000 0072 2300  ionr....r....r#.
-000021b0: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-000021c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000021d0: 1c00 0000 2000 0802 0801 0c01 0c02 1001  .... ...........
-000021e0: 0c01 0c03 0c03 0c01 0c01 0c01 0c01 1203  ................
+00000340: 0920 6430 6411 6510 6a11 6421 651a 6422  . d0d.e.j.d!e.d"
+00000350: 651a 6423 6504 6424 1900 6413 650c 6510  e.d#e.d$..d.e.e.
+00000360: 6a11 6510 6a14 6602 1900 660a 6425 6426  j.e.j.f...f.d%d&
+00000370: 8405 5a1b 6427 6510 6a11 6428 6510 6a14  ..Z.d'e.j.d(e.j.
+00000380: 6413 6403 6606 6429 642a 8404 5a1c 6411  d.d.f.d)d*..Z.d.
+00000390: 6510 6a11 642b 651d 6516 1900 6413 6510  e.j.d+e.e...d.e.
+000003a0: 6a11 6606 642c 642d 8404 5a1e 6403 5300  j.f.d,d-..Z.d.S.
+000003b0: 2931 da14 426c 7565 4361 7374 4356 5265  )1..BlueCastCVRe
+000003c0: 6772 6573 7369 6f6e 7ab4 5772 6170 7065  gressionz.Wrappe
+000003d0: 7220 746f 2074 7261 696e 2061 6e64 2070  r to train and p
+000003e0: 7265 6469 6374 206d 756c 7469 706c 6520  redict multiple 
+000003f0: 626c 7565 4361 7374 2069 6e74 7374 616e  blueCast intstan
+00000400: 6365 732e 0a0a 2020 2020 4368 6563 6b20  ces...    Check 
+00000410: 7468 6520 426c 7565 4361 7374 2063 6c61  the BlueCast cla
+00000420: 7373 2064 6f63 756d 656e 7461 7469 6f6e  ss documentation
+00000430: 2066 6f72 2061 6464 6974 696f 6e61 6c20   for additional 
+00000440: 7061 7261 6d65 7465 7220 6465 7461 696c  parameter detail
+00000450: 732e 0a20 2020 2041 2063 7573 746f 6d20  s..    A custom 
+00000460: 7370 6c69 7474 6572 2063 616e 2062 6520  splitter can be 
+00000470: 7072 6f76 6964 6564 2e0a 2020 2020 da0a  provided..    ..
+00000480: 7265 6772 6573 7369 6f6e 4eda 0d63 6c61  regressionN..cla
+00000490: 7373 5f70 726f 626c 656d da0a 7374 7261  ss_problem..stra
+000004a0: 7469 6669 6572 da0d 636f 6e66 5f74 7261  tifier..conf_tra
+000004b0: 696e 696e 67da 0c63 6f6e 665f 7867 626f  ining..conf_xgbo
+000004c0: 6f73 74da 1363 6f6e 665f 7061 7261 6d73  ost..conf_params
+000004d0: 5f78 6762 6f6f 7374 da12 6578 7065 7269  _xgboost..experi
+000004e0: 6d65 6e74 5f74 7261 636b 6572 da1b 6375  ment_tracker..cu
+000004f0: 7374 6f6d 5f69 6e5f 666f 6c64 5f70 7265  stom_in_fold_pre
+00000500: 7072 6f63 6573 736f 72da 1c63 7573 746f  processor..custo
+00000510: 6d5f 6c61 7374 5f6d 696c 655f 636f 6d70  m_last_mile_comp
+00000520: 7574 6174 696f 6eda 1363 7573 746f 6d5f  utation..custom_
+00000530: 7072 6570 726f 6365 7373 6f72 da17 6375  preprocessor..cu
+00000540: 7374 6f6d 5f66 6561 7475 7265 5f73 656c  stom_feature_sel
+00000550: 6563 746f 72da 086d 6c5f 6d6f 6465 6c63  ector..ml_modelc
+00000560: 0c00 0000 0000 0000 0000 0000 0c00 0000  ................
+00000570: 0200 0000 4300 0000 7362 0000 007c 017c  ....C...sb...|.|
+00000580: 005f 007c 047c 005f 017c 037c 005f 027c  ._.|.|._.|.|._.|
+00000590: 057c 005f 037c 077c 005f 047c 097c 005f  .|._.|.|._.|.|._
+000005a0: 057c 0a7c 005f 067c 087c 005f 0767 007c  .|.|._.|.|._.g.|
+000005b0: 005f 087c 027c 005f 097c 0b7c 005f 0a64  ._.|.|._.|.|._.d
+000005c0: 007c 005f 0b7c 0672 2b7c 067c 005f 0c64  .|._.|.r+|.|._.d
+000005d0: 0053 0074 0d83 007c 005f 0c64 0053 0029  .S.t...|._.d.S.)
+000005e0: 014e 290e 7215 0000 0072 1800 0000 7217  .N).r....r....r.
+000005f0: 0000 0072 1900 0000 721b 0000 0072 1d00  ...r....r....r..
+00000600: 0000 721e 0000 0072 1c00 0000 da0f 626c  ..r....r......bl
+00000610: 7565 6361 7374 5f6d 6f64 656c 7372 1600  uecast_modelsr..
+00000620: 0000 721f 0000 00da 1c63 6f6e 666f 726d  ..r......conform
+00000630: 616c 5f70 7265 6469 6374 696f 6e5f 7772  al_prediction_wr
+00000640: 6170 7065 7272 1a00 0000 720e 0000 0029  apperr....r....)
+00000650: 0cda 0473 656c 6672 1500 0000 7216 0000  ...selfr....r...
+00000660: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000670: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000680: 1d00 0000 721e 0000 0072 1f00 0000 a900  ....r....r......
+00000690: 7223 0000 00fa 4c2f 686f 6d65 2f74 686f  r#....L/home/tho
+000006a0: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
+000006b0: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
+000006c0: 7374 2f62 6c75 6570 7269 6e74 732f 6361  st/blueprints/ca
+000006d0: 7374 5f63 765f 7265 6772 6573 7369 6f6e  st_cv_regression
+000006e0: 2e70 79da 085f 5f69 6e69 745f 5f1d 0000  .py..__init__...
+000006f0: 0073 2000 0000 0610 0601 0601 0601 0601  .s .............
+00000700: 0601 0601 0601 0601 0601 0601 0203 04fe  ................
+00000710: 0404 0a01 0c02 7a1d 426c 7565 4361 7374  ......z.BlueCast
+00000720: 4356 5265 6772 6573 7369 6f6e 2e5f 5f69  CVRegression.__i
+00000730: 6e69 745f 5fda 0264 66da 0674 6172 6765  nit__..df..targe
+00000740: 74da 0672 6574 7572 6e63 0300 0000 0000  t..returnc......
+00000750: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00000760: 0000 732a 0000 007c 016a 0064 0164 028d  ..s*...|.j.d.d..
+00000770: 017d 017c 017c 0219 007d 037c 016a 017c  .}.|.|...}.|.j.|
+00000780: 0264 0364 048d 027d 047c 047c 0366 0253  .d.d...}.|.|.f.S
+00000790: 0029 054e 54a9 01da 0464 726f 70e9 0100  .).NT....drop...
+000007a0: 0000 a901 da04 6178 6973 2902 da0b 7265  ......axis)...re
+000007b0: 7365 745f 696e 6465 7872 2a00 0000 2905  set_indexr*...).
+000007c0: 7222 0000 0072 2600 0000 7227 0000 00da  r"...r&...r'....
+000007d0: 0179 da01 5872 2300 0000 7223 0000 0072  .y..Xr#...r#...r
+000007e0: 2400 0000 da0c 7072 6570 6172 655f 6461  $.....prepare_da
+000007f0: 7461 4100 0000 7308 0000 000c 0308 010e  taA...s.........
+00000800: 0108 017a 2142 6c75 6543 6173 7443 5652  ...z!BlueCastCVR
+00000810: 6567 7265 7373 696f 6e2e 7072 6570 6172  egression.prepar
+00000820: 655f 6461 7461 da04 524d 5345 da06 6d65  e_data..RMSE..me
+00000830: 7472 6963 6302 0000 0000 0000 0000 0000  tricc...........
+00000840: 0008 0000 0006 0000 0043 0000 0073 6e00  .........C...sn.
+00000850: 0000 6700 7d02 7c00 6a00 4400 5d10 7d03  ..g.}.|.j.D.].}.
+00000860: 7c03 6a01 7215 7c03 6a01 a002 7c01 a101  |.j.r.|.j...|...
+00000870: 7d04 7c02 a003 7c04 a101 0100 7105 7404  }.|...|.....q.t.
+00000880: a005 7c02 a101 a006 a100 7d05 7404 a005  ..|.......}.t...
+00000890: 7c02 a101 a007 a100 7d06 6401 7c01 9b00  |.......}.d.|...
+000008a0: 6402 7c05 9b00 6403 7c06 9b00 9d06 7d07  d.|...d.|.....}.
+000008b0: 7408 7c07 8301 0100 7c05 7c06 6602 5300  t.|.....|.|.f.S.
+000008c0: 2904 61a2 0100 000a 2020 2020 2020 2020  ).a.....        
+000008d0: 5368 6f77 206f 7574 206f 6620 666f 6c64  Show out of fold
+000008e0: 2073 636f 7265 732e 0a0a 2020 2020 2020   scores...      
+000008f0: 2020 5768 656e 2063 616c 6c69 6e67 2042    When calling B
+00000900: 6c75 6543 6173 7443 5652 6567 7265 7373  lueCastCVRegress
+00000910: 696f 6e27 7320 6669 745f 6576 616c 2066  ion's fit_eval f
+00000920: 756e 6374 696f 6e20 6d75 6c74 6970 6c65  unction multiple
+00000930: 2042 6c75 6543 6173 7452 6567 7265 7373   BlueCastRegress
+00000940: 696f 6e0a 2020 2020 2020 2020 696e 7374  ion.        inst
+00000950: 616e 6365 7320 6172 6520 6361 6c6c 6564  ances are called
+00000960: 2061 6e64 2065 6163 6820 6f66 2074 6865   and each of the
+00000970: 6d20 7072 6564 6963 7473 206f 6e20 756e  m predicts on un
+00000980: 7365 656e 2f6f 6f66 2064 6174 612e 0a0a  seen/oof data...
+00000990: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+000009a0: 6374 696f 6e20 636f 6c6c 6563 7473 2074  ction collects t
+000009b0: 6865 7365 2073 636f 7265 7320 616e 6420  hese scores and 
+000009c0: 7265 7475 726e 206d 6561 6e20 616e 6420  return mean and 
+000009d0: 6176 6572 6167 6520 6f66 2074 6865 6d2e  average of them.
+000009e0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000009f0: 206d 6574 7269 633a 2053 7472 696e 6720   metric: String 
+00000a00: 696e 6469 6361 7469 6e67 2077 6869 6368  indicating which
+00000a10: 206d 6574 7269 6320 7368 616c 6c20 6265   metric shall be
+00000a20: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
+00000a30: 2020 203a 7265 7475 726e 3a20 5475 706c     :return: Tupl
+00000a40: 6520 7769 7468 2028 6d65 616e 2c20 7374  e with (mean, st
+00000a50: 6429 206f 6620 6f6f 6620 7363 6f72 6573  d) of oof scores
+00000a60: 0a20 2020 2020 2020 207a 1554 6865 206d  .        z.The m
+00000a70: 6561 6e20 6f75 7420 6f66 2066 6f6c 6420  ean out of fold 
+00000a80: 7a0a 2073 636f 7265 2069 7320 7a10 2077  z. score is z. w
+00000a90: 6974 6820 616e 2073 7464 206f 6620 2909  ith an std of ).
+00000aa0: 7220 0000 00da 0c65 7661 6c5f 6d65 7472  r .....eval_metr
+00000ab0: 6963 73da 0367 6574 da06 6170 7065 6e64  ics..get..append
+00000ac0: da02 6e70 da07 6173 6172 7261 79da 046d  ..np..asarray..m
+00000ad0: 6561 6eda 0373 7464 720f 0000 0029 0872  ean..stdr....).r
+00000ae0: 2200 0000 7233 0000 00da 0b61 6c6c 5f6d  "...r3.....all_m
+00000af0: 6574 7269 6373 da11 626c 7565 6361 7374  etrics..bluecast
+00000b00: 5f69 6e73 7461 6e63 65da 0573 636f 7265  _instance..score
+00000b10: da0a 7363 6f72 655f 6d65 616e da09 7363  ..score_mean..sc
+00000b20: 6f72 655f 7374 64da 076d 6573 7361 6765  ore_std..message
+00000b30: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+00000b40: 0f73 686f 775f 6f6f 665f 7363 6f72 6573  .show_oof_scores
+00000b50: 4900 0000 7316 0000 0004 0c0a 0106 010c  I...s...........
+00000b60: 010a 0102 800e 020e 0116 0108 0108 027a  ...............z
+00000b70: 2442 6c75 6543 6173 7443 5652 6567 7265  $BlueCastCVRegre
+00000b80: 7373 696f 6e2e 7368 6f77 5f6f 6f66 5f73  ssion.show_oof_s
+00000b90: 636f 7265 73da 0a74 6172 6765 745f 636f  cores..target_co
+00000ba0: 6c63 0300 0000 0000 0000 0000 0000 0e00  lc..............
+00000bb0: 0000 0d00 0000 4300 0000 734c 0100 007c  ......C...sL...|
+00000bc0: 00a0 007c 017c 02a1 025c 027d 037d 047c  ...|.|...\.}.}.|
+00000bd0: 006a 0173 0f74 0283 007c 005f 017c 006a  .j.s.t...|._.|.j
+00000be0: 0373 1c74 0464 0164 027c 006a 016a 0564  .s.t.d.d.|.j.j.d
+00000bf0: 038d 037c 005f 0374 067c 006a 03a0 077c  ...|._.t.|.j...|
+00000c00: 037c 04a1 0283 0144 005d 7e5c 027d 055c  .|.....D.]~\.}.\
+00000c10: 027d 067d 077c 036a 087c 0619 007c 036a  .}.}.|.j.|...|.j
+00000c20: 087c 0719 0002 027d 087d 097c 046a 087c  .|.....}.}.|.j.|
+00000c30: 0619 007c 046a 087c 0719 0002 027d 0a7d  ...|.j.|.....}.}
+00000c40: 0b74 096a 0a7c 087c 0967 0264 0264 048d  .t.j.|.|.g.d.d..
+00000c50: 027d 0c74 096a 0a7c 0a7c 0b67 0264 0264  .}.t.j.|.|.g.d.d
+00000c60: 048d 027d 0a7c 0c6a 0b64 0264 058d 017d  ...}.|.j.d.d...}
+00000c70: 087c 0a6a 0b64 0264 058d 017d 0a7c 0a6a  .|.j.d.d...}.|.j
+00000c80: 0c7c 087c 023c 007c 006a 0104 006a 057c  .|.|.<.|.j...j.|
+00000c90: 006a 016a 0d37 0002 005f 0574 0e64 067c  .j.j.7..._.t.d.|
+00000ca0: 059b 0064 077c 006a 016a 059b 009d 0483  ...d.|.j.j......
+00000cb0: 0101 0074 0f7c 006a 107c 006a 017c 006a  ...t.|.j.|.j.|.j
+00000cc0: 117c 006a 127c 006a 137c 006a 147c 006a  .|.j.|.j.|.j.|.j
+00000cd0: 157c 006a 167c 006a 177c 006a 1864 088d  .|.j.|.j.|.j.d..
+00000ce0: 0a7d 0d7c 0d6a 197c 087c 0264 098d 0201  .}.|.j.|.|.d....
+00000cf0: 007c 006a 1aa0 1b7c 0da1 0101 007c 0d6a  .|.j...|.....|.j
+00000d00: 137c 005f 1371 2564 0a53 0029 0b7a 7446  .|._.q%d.S.).ztF
+00000d10: 6974 206d 756c 7469 706c 6520 426c 7565  it multiple Blue
+00000d20: 4361 7374 5265 6772 6573 7369 6f6e 2069  CastRegression i
+00000d30: 6e73 7461 6e63 6573 206f 6e20 6469 6666  nstances on diff
+00000d40: 6572 656e 7420 6461 7461 2073 706c 6974  erent data split
+00000d50: 732e 0a0a 2020 2020 2020 2020 496e 7075  s...        Inpu
+00000d60: 7420 6466 2069 7320 6578 7065 6374 6564  t df is expected
+00000d70: 2074 6865 2074 6172 6765 7420 636f 6c75   the target colu
+00000d80: 6d6e 2ee9 0500 0000 54a9 03da 086e 5f73  mn......T....n_s
+00000d90: 706c 6974 73da 0773 6875 6666 6c65 da0c  plits..shuffle..
+00000da0: 7261 6e64 6f6d 5f73 7461 7465 2901 da0c  random_state)...
+00000db0: 6967 6e6f 7265 5f69 6e64 6578 7229 0000  ignore_indexr)..
+00000dc0: 00fa 1b53 7461 7274 2066 6974 7469 6e67  ...Start fitting
+00000dd0: 206d 6f64 656c 206e 756d 6265 7220 fa12   model number ..
+00000de0: 2077 6974 6820 7261 6e64 6f6d 2073 6565   with random see
+00000df0: 6420 a90a 7215 0000 0072 1700 0000 7218  d ..r....r....r.
+00000e00: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000e10: 0000 721d 0000 0072 1e00 0000 721c 0000  ..r....r....r...
+00000e20: 0072 1f00 0000 a901 7242 0000 004e 291c  .r......rB...N).
+00000e30: 7231 0000 0072 1700 0000 720a 0000 0072  r1...r....r....r
+00000e40: 1600 0000 7208 0000 00da 1367 6c6f 6261  ....r......globa
+00000e50: 6c5f 7261 6e64 6f6d 5f73 7461 7465 da09  l_random_state..
+00000e60: 656e 756d 6572 6174 65da 0573 706c 6974  enumerate..split
+00000e70: da04 696c 6f63 da02 7064 da06 636f 6e63  ..iloc..pd..conc
+00000e80: 6174 722e 0000 00da 0676 616c 7565 73da  atr......values.
+00000e90: 2769 6e63 7265 6173 655f 7261 6e64 6f6d  'increase_random
+00000ea0: 5f73 7461 7465 5f69 6e5f 626c 7565 6361  _state_in_blueca
+00000eb0: 7374 5f63 765f 6279 720f 0000 0072 0900  st_cv_byr....r..
+00000ec0: 0000 7215 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000ed0: 0072 1a00 0000 721b 0000 0072 1d00 0000  .r....r....r....
+00000ee0: 721e 0000 0072 1c00 0000 721f 0000 00da  r....r....r.....
+00000ef0: 0366 6974 7220 0000 0072 3600 0000 290e  .fitr ...r6...).
+00000f00: 7222 0000 0072 2600 0000 7242 0000 0072  r"...r&...rB...r
+00000f10: 3000 0000 722f 0000 00da 0266 6eda 0774  0...r/.....fn..t
+00000f20: 726e 5f69 6478 da07 7661 6c5f 6964 78da  rn_idx..val_idx.
+00000f30: 0758 5f74 7261 696e da05 585f 7661 6cda  .X_train..X_val.
+00000f40: 0779 5f74 7261 696e da05 795f 7661 6cda  .y_train..y_val.
+00000f50: 0778 5f74 7261 696e da06 6175 746f 6d6c  .x_train..automl
+00000f60: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+00000f70: 5500 0000 6200 0000 734e 0000 0010 0406  U...b...sN......
+00000f80: 0208 0106 0202 0102 0102 0106 0108 fd1e  ................
+00000f90: 0616 0116 0112 0112 010c 020c 010a 0108  ................
+00000fa0: 0206 0106 ff02 0312 0104 ff02 0404 0104  ................
+00000fb0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+00000fc0: 0106 f60e 0c0c 010a 0304 df7a 1842 6c75  ...........z.Blu
+00000fd0: 6543 6173 7443 5652 6567 7265 7373 696f  eCastCVRegressio
+00000fe0: 6e2e 6669 7463 0300 0000 0000 0000 0000  n.fitc..........
+00000ff0: 0000 0f00 0000 0d00 0000 4300 0000 732c  ..........C...s,
+00001000: 0100 007c 00a0 007c 017c 02a1 025c 027d  ...|...|.|...\.}
+00001010: 037d 047c 006a 0173 0f74 0283 007c 005f  .}.|.j.s.t...|._
+00001020: 017c 006a 0373 1c74 0464 0164 027c 006a  .|.j.s.t.d.d.|.j
+00001030: 016a 0564 038d 037c 005f 0374 067c 006a  .j.d...|._.t.|.j
+00001040: 03a0 077c 037c 04a1 0283 0144 005d 665c  ...|.|.....D.]f\
+00001050: 027d 055c 027d 067d 077c 036a 087c 0619  .}.\.}.}.|.j.|..
+00001060: 007c 036a 087c 0719 0002 027d 087d 097c  .|.j.|.....}.}.|
+00001070: 046a 087c 0619 007c 046a 087c 0719 0002  .j.|...|.j.|....
+00001080: 027d 0a7d 0b7c 0a7c 086a 0964 0464 0485  .}.}.|.|.j.d.d..
+00001090: 027c 0266 023c 007c 006a 0104 006a 057c  .|.f.<.|.j...j.|
+000010a0: 006a 016a 0a37 0002 005f 0574 0b64 057c  .j.j.7..._.t.d.|
+000010b0: 059b 0064 067c 006a 016a 059b 009d 0483  ...d.|.j.j......
+000010c0: 0101 0074 0c7c 006a 0d7c 006a 017c 006a  ...t.|.j.|.j.|.j
+000010d0: 0e7c 006a 0f7c 006a 107c 006a 117c 006a  .|.j.|.j.|.j.|.j
+000010e0: 127c 006a 137c 006a 147c 006a 1564 078d  .|.j.|.j.|.j.d..
+000010f0: 0a7d 0c7c 0c6a 167c 087c 097c 0b7c 0264  .}.|.j.|.|.|.|.d
+00001100: 088d 0401 007c 006a 17a0 187c 0ca1 0101  .....|.j...|....
+00001110: 007c 0c6a 107c 005f 1071 257c 00a0 19a1  .|.j.|._.q%|....
+00001120: 005c 027d 0d7d 0e7c 0d7c 0e66 0253 0029  .\.}.}.|.|.f.S.)
+00001130: 0961 a601 0000 4669 7420 6d75 6c74 6970  .a....Fit multip
+00001140: 6c65 2042 6c75 6543 6173 7452 6567 7265  le BlueCastRegre
+00001150: 7373 696f 6e20 696e 7374 616e 6365 7320  ssion instances 
+00001160: 6f6e 2064 6966 6665 7265 6e74 2064 6174  on different dat
+00001170: 6120 7370 6c69 7473 2e0a 0a20 2020 2020  a splits...     
+00001180: 2020 2049 6e70 7574 2064 6620 6973 2065     Input df is e
+00001190: 7870 6563 7465 6420 7468 6520 7461 7267  xpected the targ
+000011a0: 6574 2063 6f6c 756d 6e2e 2045 7661 6c75  et column. Evalu
+000011b0: 6174 696f 6e20 6973 2065 7865 6375 7465  ation is execute
+000011c0: 6420 6f6e 206f 7574 2d6f 662d 666f 6c64  d on out-of-fold
+000011d0: 2064 6174 6173 6574 0a20 2020 2020 2020   dataset.       
+000011e0: 2069 6e20 6561 6368 2073 706c 6974 2e0a   in each split..
+000011f0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00001200: 663a 2050 616e 6461 7320 4461 7461 4672  f: Pandas DataFr
+00001210: 616d 6520 7468 6174 2069 6e63 6c75 6465  ame that include
+00001220: 7320 7468 6520 7461 7267 6574 2063 6f6c  s the target col
+00001230: 756d 6e0a 2020 2020 2020 2020 3a70 6172  umn.        :par
+00001240: 616d 2074 6172 6765 745f 636f 6c3a 2053  am target_col: S
+00001250: 7472 696e 6720 696e 6469 6361 7469 6e67  tring indicating
+00001260: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+00001270: 2074 6172 6765 7420 636f 6c75 6d6e 0a20   target column. 
+00001280: 2020 2020 2020 203a 7265 7475 726e 7320         :returns 
+00001290: 5475 706c 6520 6f66 2028 6f6f 665f 6d65  Tuple of (oof_me
+000012a0: 616e 2c20 6f6f 665f 7374 6429 2077 6974  an, oof_std) wit
+000012b0: 6820 7363 6f72 6573 206f 6e20 756e 7365  h scores on unse
+000012c0: 656e 2064 6174 6120 6475 7269 6e67 2065  en data during e
+000012d0: 7661 6c0a 2020 2020 2020 2020 7243 0000  val.        rC..
+000012e0: 0054 7244 0000 004e 7249 0000 0072 4a00  .TrD...NrI...rJ.
+000012f0: 0000 724b 0000 0072 4c00 0000 291a 7231  ..rK...rL...).r1
+00001300: 0000 0072 1700 0000 720a 0000 0072 1600  ...r....r....r..
+00001310: 0000 7208 0000 0072 4d00 0000 724e 0000  ..r....rM...rN..
+00001320: 0072 4f00 0000 7250 0000 00da 036c 6f63  .rO...rP.....loc
+00001330: 7254 0000 0072 0f00 0000 7209 0000 0072  rT...r....r....r
+00001340: 1500 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+00001350: 0000 0072 1b00 0000 721d 0000 0072 1e00  ...r....r....r..
+00001360: 0000 721c 0000 0072 1f00 0000 da08 6669  ..r....r......fi
+00001370: 745f 6576 616c 7220 0000 0072 3600 0000  t_evalr ...r6...
+00001380: 7241 0000 0029 0f72 2200 0000 7226 0000  rA...).r"...r&..
+00001390: 0072 4200 0000 7230 0000 0072 2f00 0000  .rB...r0...r/...
+000013a0: 7256 0000 0072 5700 0000 7258 0000 0072  rV...rW...rX...r
+000013b0: 5900 0000 725a 0000 0072 5b00 0000 725c  Y...rZ...r[...r\
+000013c0: 0000 0072 5e00 0000 da08 6f6f 665f 6d65  ...r^.....oof_me
+000013d0: 616e da07 6f6f 665f 7374 6472 2300 0000  an..oof_stdr#...
+000013e0: 7223 0000 0072 2400 0000 7260 0000 0095  r#...r$...r`....
+000013f0: 0000 0073 4800 0000 1009 0602 0801 0602  ...sH...........
+00001400: 0201 0201 0201 0601 08fd 1e06 1601 1601  ................
+00001410: 1202 0802 0601 06ff 0203 1201 04ff 0204  ................
+00001420: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001430: 0401 0401 06f6 120c 0c01 0a03 0c02 0801  ................
+00001440: 7a1d 426c 7565 4361 7374 4356 5265 6772  z.BlueCastCVRegr
+00001450: 6573 7369 6f6e 2e66 6974 5f65 7661 6c46  ession.fit_evalF
+00001460: da0a 6172 6974 686d 6574 6963 da17 7265  ..arithmetic..re
+00001470: 7475 726e 5f73 7562 5f6d 6f64 656c 735f  turn_sub_models_
+00001480: 7072 6564 73da 1073 6176 655f 7368 6170  preds..save_shap
+00001490: 5f76 616c 7565 73da 096d 6561 6e5f 7479  _values..mean_ty
+000014a0: 7065 2904 7263 0000 00da 066d 6564 6961  pe).rc.....media
+000014b0: 6eda 0967 656f 6d65 7472 6963 da08 6861  n..geometric..ha
+000014c0: 726d 6f6e 6963 6305 0000 0000 0000 0000  rmonicc.........
+000014d0: 0000 000b 0000 0007 0000 0043 0000 0073  ...........C...s
+000014e0: ec00 0000 7c01 6a00 7d05 6700 7d06 7401  ....|.j.}.g.}.t.
+000014f0: a002 a100 7d07 7403 7c00 6a04 8301 4400  ....}.t.|.j...D.
+00001500: 5d21 5c02 7d08 7d09 7c09 6a05 7c01 6a06  ]!\.}.}.|.j.|.j.
+00001510: 6401 6401 8502 7c05 6602 1900 7c03 6402  d.d...|.f...|.d.
+00001520: 8d02 7d0a 7c0a 7c07 6403 7c08 9b00 9d02  ..}.|.|.d.|.....
+00001530: 3c00 7c06 a007 6403 7c08 9b00 9d02 a101  <.|...d.|.......
+00001540: 0100 710e 7c02 7234 7c07 5300 7c04 6404  ..q.|.r4|.S.|.d.
+00001550: 6b02 723e 7c07 6a08 6405 6406 8d01 5300  k.r>|.j.d.d...S.
+00001560: 7c04 6407 6b02 7255 7409 a00a 7409 a00b  |.d.k.rUt...t...
+00001570: 7c07 6a0c 6405 6406 8d01 a101 7c07 a00d  |.j.d.d.....|...
+00001580: a100 a00e 6405 a101 1b00 a101 5300 7c04  ....d.......S.|.
+00001590: 6408 6b02 7266 740f 7c06 8301 7409 6a0e  d.k.rft.|...t.j.
+000015a0: 6405 7c07 1b00 6405 6406 8d02 1b00 5300  d.|...d.d.....S.
+000015b0: 7c04 6409 6b02 7270 7c07 6a10 6405 6406  |.d.k.rp|.j.d.d.
+000015c0: 8d01 5300 7c07 6a08 6405 6406 8d01 5300  ..S.|.j.d.d...S.
+000015d0: 290a 6192 0200 0050 7265 6469 6374 206f  ).a....Predict o
+000015e0: 6e20 756e 7365 656e 2064 6174 6120 7573  n unseen data us
+000015f0: 696e 6720 6d75 6c74 6970 6c65 2074 7261  ing multiple tra
+00001600: 696e 6564 2042 6c75 6543 6173 7452 6567  ined BlueCastReg
+00001610: 7265 7373 696f 6e20 696e 7374 616e 6365  ression instance
+00001620: 732e 0a0a 2020 2020 2020 2020 3a70 6172  s...        :par
+00001630: 616d 2064 663a 2050 616e 6461 7320 4461  am df: Pandas Da
+00001640: 7461 4672 616d 6520 7769 7468 2075 6e73  taFrame with uns
+00001650: 6565 6e20 6461 7461 0a20 2020 2020 2020  een data.       
+00001660: 203a 7061 7261 6d20 7265 7475 726e 5f73   :param return_s
+00001670: 7562 5f6d 6f64 656c 735f 7072 6564 733a  ub_models_preds:
+00001680: 2049 6620 7472 7565 2077 696c 6c20 7265   If true will re
+00001690: 7475 726e 2061 2044 6174 6146 7261 6d65  turn a DataFrame
+000016a0: 2077 6974 6820 7468 6520 7072 6564 6963   with the predic
+000016b0: 7469 6f6e 7320 6f66 2065 6163 6820 6d6f  tions of each mo
+000016c0: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+000016d0: 7374 6f72 6564 2069 6e20 7365 7061 7261  stored in separa
+000016e0: 7465 2063 6f6c 756d 6e73 2e0a 2020 2020  te columns..    
+000016f0: 2020 2020 3a70 6172 616d 2073 6176 655f      :param save_
+00001700: 7368 6170 5f76 616c 7565 733a 2049 6620  shap_values: If 
+00001710: 5472 7565 2c20 6361 6c63 756c 6174 6573  True, calculates
+00001720: 2061 6e64 2073 6176 6573 2073 6861 7020   and saves shap 
+00001730: 7661 6c75 6573 2c20 736f 2074 6865 7920  values, so they 
+00001740: 6361 6e20 6265 2075 7365 6420 746f 2070  can be used to p
+00001750: 6c6f 740a 2020 2020 2020 2020 2020 2020  lot.            
+00001760: 7761 7465 7266 616c 6c20 706c 6f74 7320  waterfall plots 
+00001770: 666f 7220 7365 6c65 6374 6564 2072 6f77  for selected row
+00001780: 7320 6f20 6465 6d61 6e64 2e0a 2020 2020  s o demand..    
+00001790: 2020 2020 3a70 6172 616d 206d 6561 6e5f      :param mean_
+000017a0: 7479 7065 3a20 5374 7269 6e67 2069 6e64  type: String ind
+000017b0: 6963 6174 696e 6720 7468 6520 7479 7065  icating the type
+000017c0: 206f 6620 6d65 616e 2074 6f20 6265 2075   of mean to be u
+000017d0: 7365 6420 746f 2062 6c65 6e64 2074 6865  sed to blend the
+000017e0: 2070 7265 6469 6374 696f 6e73 206f 6620   predictions of 
+000017f0: 7468 6520 7375 6220 6d6f 6465 6c73 2e0a  the sub models..
+00001800: 2020 2020 2020 2020 2020 2020 506f 7373              Poss
+00001810: 6962 6c65 2076 616c 7565 7320 6172 6520  ible values are 
+00001820: 2761 7269 7468 6d65 7469 6327 2c20 2767  'arithmetic', 'g
+00001830: 656f 6d65 7472 6963 2720 616e 6420 2768  eometric' and 'h
+00001840: 6172 6d6f 6e69 6327 2028 6465 6661 756c  armonic' (defaul
+00001850: 743d 2761 7269 7468 6d65 7469 6327 292e  t='arithmetic').
+00001860: 0a20 2020 2020 2020 204e 2901 7265 0000  .        N).re..
+00001870: 005a 0670 7265 6473 5f72 6300 0000 722b  .Z.preds_rc...r+
+00001880: 0000 0072 2c00 0000 7268 0000 0072 6900  ...r,...rh...ri.
+00001890: 0000 7267 0000 0029 11da 0763 6f6c 756d  ..rg...)...colum
+000018a0: 6e73 7251 0000 00da 0944 6174 6146 7261  nsrQ.....DataFra
+000018b0: 6d65 724e 0000 0072 2000 0000 da07 7072  merN...r .....pr
+000018c0: 6564 6963 7472 5f00 0000 7236 0000 0072  edictr_...r6...r
+000018d0: 3900 0000 7237 0000 00da 0365 7870 da03  9...r7.....exp..
+000018e0: 6c6f 67da 0470 726f 64da 056e 6f74 6e61  log..prod..notna
+000018f0: da03 7375 6dda 036c 656e 7267 0000 0029  ..sum..lenrg...)
+00001900: 0b72 2200 0000 7226 0000 0072 6400 0000  .r"...r&...rd...
+00001910: 7265 0000 0072 6600 0000 da07 6f72 5f63  re...rf.....or_c
+00001920: 6f6c 735a 0970 7265 645f 636f 6c73 da09  olsZ.pred_cols..
+00001930: 7265 7375 6c74 5f64 6672 5600 0000 da08  result_dfrV.....
+00001940: 7069 7065 6c69 6e65 da07 795f 7072 6564  pipeline..y_pred
+00001950: 7372 2300 0000 7223 0000 0072 2400 0000  sr#...r#...r$...
+00001960: 726c 0000 00cc 0000 0073 2800 0000 0613  rl.......s(.....
+00001970: 0401 0801 1202 0401 1201 06ff 0e03 1201  ................
+00001980: 0402 0401 0802 0c01 0801 2601 0801 1a01  ..........&.....
+00001990: 0801 0c01 0c02 7a1c 426c 7565 4361 7374  ......z.BlueCast
+000019a0: 4356 5265 6772 6573 7369 6f6e 2e70 7265  CVRegression.pre
+000019b0: 6469 6374 da0d 785f 6361 6c69 6272 6174  dict..x_calibrat
+000019c0: 696f 6eda 0d79 5f63 616c 6962 7261 7469  ion..y_calibrati
+000019d0: 6f6e 6303 0000 0000 0000 0000 0000 0004  onc.............
+000019e0: 0000 0004 0000 004b 0000 0073 2400 0000  .......K...s$...
+000019f0: 7400 7c00 6601 6900 7c03 a401 8e01 7c00  t.|.f.i.|.....|.
+00001a00: 5f01 7c00 6a01 a002 7c01 7c02 a102 0100  _.|.j...|.|.....
+00001a10: 6401 5300 2902 61ee 0100 0043 616c 6962  d.S.).a....Calib
+00001a20: 7261 7465 2074 6865 206d 6f64 656c 2e0a  rate the model..
+00001a30: 0a20 2020 2020 2020 2056 6961 2074 6869  .        Via thi
+00001a40: 7320 6675 6e63 7469 6f6e 2074 6865 206e  s function the n
+00001a50: 6f6e 636f 6e66 6f72 6d69 7479 206d 6561  onconformity mea
+00001a60: 7375 7265 7320 6172 6520 7461 6b65 6e20  sures are taken 
+00001a70: 616e 6420 7573 6564 2074 6f20 7072 6564  and used to pred
+00001a80: 6963 7420 7072 6564 6963 7469 6f6e 2069  ict prediction i
+00001a90: 6e74 6572 7661 6c73 2076 6973 2074 6865  ntervals vis the
+00001aa0: 0a20 2020 2020 2020 2070 7265 6469 6374  .        predict
+00001ab0: 5f69 6e74 6572 7661 6c20 6675 6e63 7469  _interval functi
+00001ac0: 6f6e 2e20 5573 6564 2069 7320 7468 6520  on. Used is the 
+00001ad0: 6d65 616e 2070 7265 6469 6374 696f 6e20  mean prediction 
+00001ae0: 6f66 2061 6c6c 2073 7562 206d 6f64 656c  of all sub model
+00001af0: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+00001b00: 6d3a 2078 5f63 616c 6962 7261 7469 6f6e  m: x_calibration
+00001b10: 3a20 5061 6e64 6173 2044 6174 6146 7261  : Pandas DataFra
+00001b20: 6d65 2077 6974 686f 7574 2074 6172 6765  me without targe
+00001b30: 7420 636f 6c75 6d6e 2c20 7468 6174 2068  t column, that h
+00001b40: 6173 206e 6f74 2062 6565 6e20 7365 656e  as not been seen
+00001b50: 2062 7920 7468 6520 6d6f 6465 6c20 6475   by the model du
+00001b60: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00001b70: 2074 7261 696e 696e 672e 0a20 2020 2020   training..     
+00001b80: 2020 203a 7061 7261 6d20 795f 6361 6c69     :param y_cali
+00001b90: 6272 6174 696f 6e3a 2050 616e 6461 7320  bration: Pandas 
+00001ba0: 5365 7269 6573 2068 6f6c 6469 6e67 2074  Series holding t
+00001bb0: 6865 2074 6172 6765 7420 7661 6c75 652c  he target value,
+00001bc0: 2068 6174 2068 6173 206e 6f74 2062 6565   hat has not bee
+00001bd0: 6e20 7365 656e 2062 7920 7468 6520 6d6f  n seen by the mo
+00001be0: 6465 6c20 6475 7269 6e67 0a20 2020 2020  del during.     
+00001bf0: 2020 2020 2020 2074 7261 696e 696e 672e         training.
+00001c00: 0a20 2020 2020 2020 204e 2903 720d 0000  .        N).r...
+00001c10: 0072 2100 0000 da09 6361 6c69 6272 6174  .r!.....calibrat
+00001c20: 6529 0472 2200 0000 7277 0000 0072 7800  e).r"...rw...rx.
+00001c30: 0000 da06 6b77 6172 6773 7223 0000 0072  ....kwargsr#...r
+00001c40: 2300 0000 7224 0000 0072 7900 0000 f800  #...r$...ry.....
+00001c50: 0000 730c 0000 0002 0c02 0104 ff02 0108  ..s.............
+00001c60: ff12 037a 1e42 6c75 6543 6173 7443 5652  ...z.BlueCastCVR
+00001c70: 6567 7265 7373 696f 6e2e 6361 6c69 6272  egression.calibr
+00001c80: 6174 65da 0661 6c70 6861 7363 0300 0000  ate..alphasc....
+00001c90: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00001ca0: 4300 0000 7322 0000 007c 006a 0072 0d7c  C...s"...|.j.r.|
+00001cb0: 006a 006a 017c 017c 0264 018d 027d 037c  .j.j.|.|.d...}.|
+00001cc0: 0353 0074 0264 0283 0182 0129 0361 4202  .S.t.d.....).aB.
+00001cd0: 0000 4372 6561 7465 2070 7265 6469 6374  ..Create predict
+00001ce0: 696f 6e20 696e 7465 7276 616c 7320 6261  ion intervals ba
+00001cf0: 7365 6420 6f6e 2061 2063 6572 7461 696e  sed on a certain
+00001d00: 2063 6f6e 6669 6465 6e63 6520 6c65 7665   confidence leve
+00001d10: 6c73 2e0a 0a20 2020 2020 2020 2043 6f6e  ls...        Con
+00001d20: 666f 726d 616c 2070 7265 6469 6374 696f  formal predictio
+00001d30: 6e20 6775 6172 616e 7465 6573 2c20 7468  n guarantees, th
+00001d40: 6174 2074 6865 2063 6f72 7265 6374 2076  at the correct v
+00001d50: 616c 7565 2069 7320 7072 6573 656e 7420  alue is present 
+00001d60: 696e 2074 6865 2070 7265 6469 6374 696f  in the predictio
+00001d70: 6e20 6261 6e64 2077 6974 6820 6120 7072  n band with a pr
+00001d80: 6f62 6162 696c 6974 7920 6f66 0a20 2020  obability of.   
+00001d90: 2020 2020 2031 202d 2061 6c70 6861 2e0a       1 - alpha..
+00001da0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00001db0: 663a 2050 616e 6461 7320 4461 7461 4672  f: Pandas DataFr
+00001dc0: 616d 6520 686f 6c64 696e 6720 756e 7365  ame holding unse
+00001dd0: 656e 2064 6174 610a 2020 2020 2020 2020  en data.        
+00001de0: 3a70 6172 616d 2061 6c70 6861 733a 204c  :param alphas: L
+00001df0: 6973 7420 6f66 2066 6c6f 6174 7320 696e  ist of floats in
+00001e00: 6469 6361 7469 6e67 2074 6865 2064 6573  dicating the des
+00001e10: 6972 6564 2063 6f6e 6669 6465 6e63 6520  ired confidence 
+00001e20: 6c65 7665 6c73 2e0a 2020 2020 2020 2020  levels..        
+00001e30: 3a72 6574 7572 6e73 2041 2050 616e 6461  :returns A Panda
+00001e40: 7320 4461 7461 4672 616d 6520 7769 7468  s DataFrame with
+00001e50: 2020 736f 7274 6564 2063 6f6c 756d 6e73    sorted columns
+00001e60: 2027 616c 7068 615f 5858 5f6c 6f77 2720   'alpha_XX_low' 
+00001e70: 2861 6c70 6861 2920 616e 6420 2761 6c70  (alpha) and 'alp
+00001e80: 6861 5f58 585f 6869 6768 2720 2831 202d  ha_XX_high' (1 -
+00001e90: 2061 6c70 6861 2920 666f 7220 6561 6368   alpha) for each
+00001ea0: 0a20 2020 2020 2020 2020 2020 2061 6c70  .            alp
+00001eb0: 6861 2069 6e20 7468 6520 7072 6f76 6964  ha in the provid
+00001ec0: 6564 206c 6973 7420 6f66 2061 6c70 6861  ed list of alpha
+00001ed0: 732e 2054 6f20 6f62 7461 696e 2074 6865  s. To obtain the
+00001ee0: 206d 6561 6e20 7072 6564 6963 7469 6f6e   mean prediction
+00001ef0: 2063 616c 6c20 7468 6520 2770 7265 6469   call the 'predi
+00001f00: 6374 2720 6d65 7468 6f64 2e0a 2020 2020  ct' method..    
+00001f10: 2020 2020 2901 727b 0000 007a 7354 6869      ).r{...zsThi
+00001f20: 7320 696e 7374 616e 6365 2068 6173 206e  s instance has n
+00001f30: 6f74 2062 6565 6e20 6361 6c69 6272 6174  ot been calibrat
+00001f40: 6564 2079 6574 2e20 4d61 6b65 2075 7365  ed yet. Make use
+00001f50: 206f 6620 6361 6c69 6272 6174 6520 746f   of calibrate to
+00001f60: 2066 6974 2074 6865 0a20 2020 2020 2020   fit the.       
+00001f70: 2020 2020 2043 6f6e 666f 726d 616c 5072       ConformalPr
+00001f80: 6564 6963 7469 6f6e 5772 6170 7065 722e  edictionWrapper.
+00001f90: 2903 7221 0000 00da 1070 7265 6469 6374  ).r!.....predict
+00001fa0: 5f69 6e74 6572 7661 6cda 0a56 616c 7565  _interval..Value
+00001fb0: 4572 726f 7229 0472 2200 0000 7226 0000  Error).r"...r&..
+00001fc0: 0072 7b00 0000 da0d 7072 6564 5f69 6e74  .r{.....pred_int
+00001fd0: 6572 7661 6c72 2300 0000 7223 0000 0072  ervalr#...r#...r
+00001fe0: 2400 0000 727c 0000 0009 0100 0073 1000  $...r|.......s..
+00001ff0: 0000 060a 0601 0401 06ff 0403 0202 0201  ................
+00002000: 04ff 7a25 426c 7565 4361 7374 4356 5265  ..z%BlueCastCVRe
+00002010: 6772 6573 7369 6f6e 2e70 7265 6469 6374  gression.predict
+00002020: 5f69 6e74 6572 7661 6c29 0b72 1400 0000  _interval).r....
+00002030: 4e4e 4e4e 4e4e 4e4e 4e4e 2901 7232 0000  NNNNNNNNNN).r2..
+00002040: 0029 0346 4672 6300 0000 291f da08 5f5f  .).FFrc...)...__
+00002050: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00002060: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00002070: da07 5f5f 646f 635f 5f72 0400 0000 7205  ..__doc__r....r.
+00002080: 0000 0072 0200 0000 720a 0000 00da 1758  ...r....r......X
+00002090: 6762 6f6f 7374 5475 6e65 5061 7261 6d73  gboostTuneParams
+000020a0: 436f 6e66 6967 720b 0000 0072 0e00 0000  Configr....r....
+000020b0: 7211 0000 0072 0700 0000 7212 0000 0072  r....r....r....r
+000020c0: 1000 0000 7225 0000 0072 5100 0000 726b  ....r%...rQ...rk
+000020d0: 0000 00da 0373 7472 7206 0000 00da 0653  .....strr......S
+000020e0: 6572 6965 7372 3100 0000 da05 666c 6f61  eriesr1.....floa
+000020f0: 7472 4100 0000 7255 0000 0072 6000 0000  trA...rU...r`...
+00002100: da04 626f 6f6c 726c 0000 0072 7900 0000  ..boolrl...ry...
+00002110: 7203 0000 0072 7c00 0000 7223 0000 0072  r....r|...r#...r
+00002120: 2300 0000 7223 0000 0072 2400 0000 7213  #...r#...r$...r.
+00002130: 0000 0016 0000 0073 9000 0000 0800 0401  .......s........
+00002140: 0208 0201 0201 0201 0201 0201 0201 0201  ................
+00002150: 0201 0203 0201 04f2 0602 02fe 0603 02fd  ................
+00002160: 0604 02fc 0605 02fb 0606 02fa 0607 02f9  ................
+00002170: 0608 02f8 0609 02f7 060a 02f6 020b 0a01  ................
+00002180: 02ff 02f5 0e0e 0af2 0224 0401 02ff 0201  .........$......
+00002190: 02ff 0e02 0afe 1c08 1819 2033 023a 0201  .......... 3.:..
+000021a0: 0203 04f9 0402 02fe 0203 02fd 0204 02fc  ................
+000021b0: 0205 0201 02ff 02fb 0e08 0af8 022c 0401  .............,..
+000021c0: 02ff 0401 02ff 0202 0afe 2211 7213 0000  ..........".r...
+000021d0: 0029 21da 0674 7970 696e 6772 0200 0000  .)!..typingr....
+000021e0: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+000021f0: 0600 0000 7207 0000 00da 056e 756d 7079  ....r......numpy
+00002200: 7237 0000 00da 0670 616e 6461 7372 5100  r7.....pandasrQ.
+00002210: 0000 da17 736b 6c65 6172 6e2e 6d6f 6465  ....sklearn.mode
+00002220: 6c5f 7365 6c65 6374 696f 6e72 0800 0000  l_selectionr....
+00002230: da23 626c 7565 6361 7374 2e62 6c75 6570  .#bluecast.bluep
+00002240: 7269 6e74 732e 6361 7374 5f72 6567 7265  rints.cast_regre
+00002250: 7373 696f 6e72 0900 0000 da1f 626c 7565  ssionr......blue
+00002260: 6361 7374 2e63 6f6e 6669 672e 7472 6169  cast.config.trai
+00002270: 6e69 6e67 5f63 6f6e 6669 6772 0a00 0000  ning_configr....
+00002280: 720b 0000 0072 0c00 0000 7283 0000 00da  r....r....r.....
+00002290: 3d62 6c75 6563 6173 742e 636f 6e66 6f72  =bluecast.confor
+000022a0: 6d61 6c5f 7072 6564 6963 7469 6f6e 2e63  mal_prediction.c
+000022b0: 6f6e 666f 726d 616c 5f70 7265 6469 6374  onformal_predict
+000022c0: 696f 6e5f 7265 6772 6573 7369 6f6e 720d  ion_regressionr.
+000022d0: 0000 00da 2162 6c75 6563 6173 742e 6578  ....!bluecast.ex
+000022e0: 7065 7269 6d65 6e74 6174 696f 6e2e 7472  perimentation.tr
+000022f0: 6163 6b69 6e67 720e 0000 00da 2462 6c75  ackingr.....$blu
+00002300: 6563 6173 742e 6765 6e65 7261 6c5f 7574  ecast.general_ut
+00002310: 696c 732e 6765 6e65 7261 6c5f 7574 696c  ils.general_util
+00002320: 7372 0f00 0000 da1d 626c 7565 6361 7374  sr......bluecast
+00002330: 2e6d 6c5f 6d6f 6465 6c6c 696e 672e 7867  .ml_modelling.xg
+00002340: 626f 6f73 7472 1000 0000 da1d 626c 7565  boostr......blue
+00002350: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
+00002360: 6e67 2e63 7573 746f 6d72 1100 0000 da28  ng.customr.....(
+00002370: 626c 7565 6361 7374 2e70 7265 7072 6f63  bluecast.preproc
+00002380: 6573 7369 6e67 2e66 6561 7475 7265 5f73  essing.feature_s
+00002390: 656c 6563 7469 6f6e 7212 0000 0072 1300  electionr....r..
+000023a0: 0000 7223 0000 0072 2300 0000 7223 0000  ..r#...r#...r#..
+000023b0: 0072 2400 0000 da08 3c6d 6f64 756c 653e  .r$.....<module>
+000023c0: 0100 0000 731c 0000 0020 0008 0208 010c  ....s.... ......
+000023d0: 010c 0210 010c 010c 030c 030c 010c 010c  ................
+000023e0: 010c 0112 03                             .....
```

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-38.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_cv_regression.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_regression.cpython-310.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_regression.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/__pycache__/cast_regression.cpython-38.pyc` & `bluecast-1.2.4/bluecast/blueprints/__pycache__/cast_regression.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/cast.py` & `bluecast-1.2.4/bluecast/blueprints/cast.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/cast_cv.py` & `bluecast-1.2.4/bluecast/blueprints/cast_cv.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/blueprints/cast_cv_regression.py` & `bluecast-1.2.4/bluecast/blueprints/cast_cv_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -202,22 +202,27 @@
         return oof_mean, oof_std
 
     def predict(
         self,
         df: pd.DataFrame,
         return_sub_models_preds: bool = False,
         save_shap_values: bool = False,
+        mean_type: Literal[
+            "arithmetic", "median", "geometric", "harmonic"
+        ] = "arithmetic",
     ) -> Union[pd.DataFrame, pd.Series]:
         """Predict on unseen data using multiple trained BlueCastRegression instances.
 
         :param df: Pandas DataFrame with unseen data
         :param return_sub_models_preds: If true will return a DataFrame with the predictions of each model
             stored in separate columns.
         :param save_shap_values: If True, calculates and saves shap values, so they can be used to plot
             waterfall plots for selected rows o demand.
+        :param mean_type: String indicating the type of mean to be used to blend the predictions of the sub models.
+            Possible values are 'arithmetic', 'geometric' and 'harmonic' (default='arithmetic').
         """
         or_cols = df.columns
         pred_cols: list[str] = []
         result_df = pd.DataFrame()  # Create an empty DataFrame to store results
 
         for fn, pipeline in enumerate(self.bluecast_models):
             y_preds = pipeline.predict(
@@ -225,15 +230,24 @@
             )
             result_df[f"preds_{fn}"] = y_preds
             pred_cols.append(f"preds_{fn}")
 
         if return_sub_models_preds:
             return result_df
         else:
-            return result_df.mean(axis=1)
+            if mean_type == "arithmetic":
+                return result_df.mean(axis=1)
+            elif mean_type == "geometric":
+                return np.exp(np.log(result_df.prod(axis=1)) / result_df.notna().sum(1))
+            elif mean_type == "harmonic":
+                return len(pred_cols) / np.sum(1 / result_df, axis=1)
+            elif mean_type == "median":
+                return result_df.median(axis=1)
+            else:
+                return result_df.mean(axis=1)
 
     def calibrate(
         self, x_calibration: pd.DataFrame, y_calibration: pd.Series, **kwargs
     ) -> None:
         """Calibrate the model.
 
         Via this function the nonconformity measures are taken and used to predict prediction intervals vis the
```

### Comparing `bluecast-1.1/bluecast/blueprints/cast_regression.py` & `bluecast-1.2.4/bluecast/blueprints/cast_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/config/__pycache__/base_classes.cpython-310.pyc` & `bluecast-1.2.4/bluecast/config/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/config/__pycache__/base_classes.cpython-38.pyc` & `bluecast-1.2.4/bluecast/config/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-1.2.4/bluecast/config/__pycache__/training_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 28 05:01:13 2024 UTC, .py size: 8270 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 19d8 2d66 4e20 0000  o.........-fN ..
+00000000: 6f0d 0d0a 0000 0000 4ea8 3b66 ff21 0000  o.......N.;f.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a09 4700 6407  d.d...d...Z.G.d.
 00000070: 6408 8400 6408 6506 8303 5a0a 4700 6409  d...d.e...Z.G.d.
@@ -54,508 +54,536 @@
 00000350: 00fa 452f 686f 6d65 2f74 686f 6d61 732f  ..E/home/thomas/
 00000360: 4964 6561 5072 6f6a 6563 7473 2f42 6c75  IdeaProjects/Blu
 00000370: 6543 6173 742f 626c 7565 6361 7374 2f63  eCast/bluecast/c
 00000380: 6f6e 6669 672f 7472 6169 6e69 6e67 5f63  onfig/training_c
 00000390: 6f6e 6669 672e 7079 7207 0000 000f 0000  onfig.pyr.......
 000003a0: 0073 0400 0000 0800 0801 7207 0000 0063  .s........r....c
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003c0: 0300 0000 4000 0000 7354 0100 0065 005a  ....@...sT...e.Z
+000003c0: 0300 0000 4000 0000 736c 0100 0065 005a  ....@...sl...e.Z
 000003d0: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
 000003e0: 0565 0664 033c 0064 045a 0765 0565 0664  .e.d.<.d.Z.e.e.d
 000003f0: 053c 0064 065a 0865 0965 0664 073c 0064  .<.d.Z.e.e.d.<.d
 00000400: 085a 0a65 0565 0664 093c 0064 0a5a 0b65  .Z.e.e.d.<.d.Z.e
 00000410: 0565 0664 0b3c 0064 0c5a 0c65 0565 0664  .e.d.<.d.Z.e.e.d
 00000420: 0d3c 0064 0e5a 0d65 0965 0664 0f3c 0064  .<.d.Z.e.e.d.<.d
-00000430: 105a 0e65 0f65 0519 0065 0664 113c 0064  .Z.e.e...e.d.<.d
-00000440: 065a 1065 0965 0664 123c 0064 0e5a 1165  .Z.e.e.d.<.d.Z.e
-00000450: 0965 0664 133c 0064 065a 1265 0965 0664  .e.d.<.d.Z.e.e.d
-00000460: 143c 0064 1567 015a 1365 1465 0519 0065  .<.d.g.Z.e.e...e
-00000470: 0664 163c 0064 0c5a 1565 0565 0664 173c  .d.<.d.Z.e.e.d.<
-00000480: 0064 0e5a 1665 0965 0664 183c 0064 195a  .d.Z.e.e.d.<.d.Z
-00000490: 1765 1865 0664 1a3c 0064 065a 1965 0965  .e.e.d.<.d.Z.e.e
-000004a0: 0664 1b3c 0064 0e5a 1a65 0965 0664 1c3c  .d.<.d.Z.e.e.d.<
-000004b0: 0064 1d5a 1b65 0565 0664 1e3c 0064 1d5a  .d.Z.e.e.d.<.d.Z
-000004c0: 1c65 0565 0664 1f3c 0064 0e5a 1d65 0965  .e.e.d.<.d.Z.e.e
-000004d0: 0664 203c 0064 0e5a 1e65 0965 0664 213c  .d <.d.Z.e.e.d!<
-000004e0: 0064 025a 1f65 0565 0664 223c 0064 0e5a  .d.Z.e.e.d"<.d.Z
-000004f0: 2065 0965 0664 233c 0064 0a5a 2165 0565   e.e.d#<.d.Z!e.e
-00000500: 0664 243c 0064 1d5a 2265 0565 0664 253c  .d$<.d.Z"e.e.d%<
-00000510: 0064 265a 2365 2465 0664 273c 0064 1053  .d&Z#e$e.d'<.d.S
-00000520: 0029 28da 0e54 7261 696e 696e 6743 6f6e  .)(..TrainingCon
-00000530: 6669 6761 490f 0000 4465 6669 6e65 2067  figaI...Define g
-00000540: 656e 6572 616c 2074 7261 696e 696e 6720  eneral training 
-00000550: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
-00000560: 203a 7061 7261 6d20 676c 6f62 616c 5f72   :param global_r
-00000570: 616e 646f 6d5f 7374 6174 653a 2047 6c6f  andom_state: Glo
-00000580: 6261 6c20 7261 6e64 6f6d 2073 7461 7465  bal random state
-00000590: 2074 6f20 7573 6520 666f 7220 7265 7072   to use for repr
-000005a0: 6f64 7563 6962 696c 6974 792e 0a20 2020  oducibility..   
-000005b0: 203a 7061 7261 6d20 696e 6372 6561 7365   :param increase
-000005c0: 5f72 616e 646f 6d5f 7374 6174 655f 696e  _random_state_in
-000005d0: 5f62 6c75 6563 6173 745f 6376 5f62 793a  _bluecast_cv_by:
-000005e0: 2049 6e20 426c 7565 4361 7374 4356 206d   In BlueCastCV m
-000005f0: 756c 7469 706c 6520 6d6f 6465 6c73 2061  ultiple models a
-00000600: 7265 2074 7261 696e 6564 2e20 4465 6669  re trained. Defi
-00000610: 6e65 2062 7920 686f 7720 6d75 6368 2074  ne by how much t
-00000620: 6865 0a20 2020 2020 2020 2072 616e 646f  he.        rando
-00000630: 6d20 7374 6174 6520 6368 616e 6765 7320  m state changes 
-00000640: 7769 7468 2065 6163 6820 6164 6469 7469  with each additi
-00000650: 6f6e 616c 206d 6f64 656c 2e0a 2020 2020  onal model..    
-00000660: 3a70 6172 616d 2073 6875 6666 6c65 5f64  :param shuffle_d
-00000670: 7572 696e 675f 7472 6169 6e69 6e67 3a20  uring_training: 
-00000680: 5768 6574 6865 7220 746f 2073 6875 6666  Whether to shuff
-00000690: 6c65 2074 6865 2064 6174 6120 6475 7269  le the data duri
-000006a0: 6e67 2074 7261 696e 696e 6720 7768 656e  ng training when
-000006b0: 2068 7970 6572 7475 6e69 6e67 5f63 765f   hypertuning_cv_
-000006c0: 666f 6c64 7320 3e20 312e 0a20 2020 203a  folds > 1..    :
-000006d0: 7061 7261 6d20 6879 7065 7270 6172 616d  param hyperparam
-000006e0: 6574 6572 5f74 756e 696e 675f 726f 756e  eter_tuning_roun
-000006f0: 6473 3a20 4e75 6d62 6572 206f 6620 6879  ds: Number of hy
-00000700: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
-00000710: 696e 6720 726f 756e 6473 2e20 4e6f 7420  ing rounds. Not 
-00000720: 7573 6564 2077 6865 6e20 6375 7374 6f6d  used when custom
-00000730: 204d 4c20 6d6f 6465 6c20 6973 2070 6173   ML model is pas
-00000740: 7365 642e 0a20 2020 203a 7061 7261 6d20  sed..    :param 
-00000750: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
-00000760: 756e 696e 675f 6d61 785f 7275 6e74 696d  uning_max_runtim
-00000770: 655f 7365 6373 3a20 4d61 7869 6d75 6d20  e_secs: Maximum 
-00000780: 7275 6e74 696d 6520 696e 2073 6563 6f6e  runtime in secon
-00000790: 6473 2066 6f72 2068 7970 6572 7061 7261  ds for hyperpara
-000007a0: 6d65 7465 7220 7475 6e69 6e67 2e20 4e6f  meter tuning. No
-000007b0: 7420 7573 6564 2077 6865 6e0a 2020 2020  t used when.    
-000007c0: 2020 2020 6375 7374 6f6d 204d 4c20 6d6f      custom ML mo
-000007d0: 6465 6c20 6973 2070 6173 7365 642e 0a20  del is passed.. 
-000007e0: 2020 203a 7061 7261 6d20 6879 7065 7274     :param hypert
-000007f0: 756e 696e 675f 6376 5f66 6f6c 6473 3a20  uning_cv_folds: 
-00000800: 4e75 6d62 6572 206f 6620 6372 6f73 732d  Number of cross-
-00000810: 7661 6c69 6461 7469 6f6e 2066 6f6c 6473  validation folds
-00000820: 2074 6f20 7573 6520 666f 7220 6879 7065   to use for hype
-00000830: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
-00000840: 672e 204e 6f74 2075 7365 6420 7768 656e  g. Not used when
-00000850: 0a20 2020 2020 2020 2063 7573 746f 6d20  .        custom 
-00000860: 4d4c 206d 6f64 656c 2069 7320 7061 7373  ML model is pass
-00000870: 6564 2e0a 2020 2020 3a70 6172 616d 2070  ed..    :param p
-00000880: 7265 6369 7365 5f63 765f 7475 6e69 6e67  recise_cv_tuning
-00000890: 3a20 4966 2065 6e61 626c 6564 2077 696c  : If enabled wil
-000008a0: 6c20 7377 6974 6368 2066 726f 6d20 7573  l switch from us
-000008b0: 696e 6720 5867 626f 6f73 7427 7320 6f77  ing Xgboost's ow
-000008c0: 6e20 6376 206d 6574 686f 6420 746f 2061  n cv method to a
-000008d0: 2063 7573 746f 6d20 6372 6f73 7320 7661   custom cross va
-000008e0: 6c69 6461 7469 6f6e 0a20 2020 2020 2020  lidation.       
-000008f0: 2072 6f75 7469 6e65 2e20 5468 6973 2069   routine. This i
-00000900: 7320 6e65 6564 6564 2077 6865 6e20 7468  s needed when th
-00000910: 6520 696e 2d66 6f6c 6420 7072 6570 726f  e in-fold prepro
-00000920: 6365 7373 696e 6720 6973 206e 6563 6573  cessing is neces
-00000930: 7361 7279 2074 6861 7420 776f 756c 6420  sary that would 
-00000940: 6361 7573 6520 6f76 6572 6669 7474 696e  cause overfittin
-00000950: 6720 7769 7468 2075 7375 616c 2063 762e  g with usual cv.
-00000960: 0a20 2020 2020 2020 2054 6869 7320 6861  .        This ha
-00000970: 7320 6120 6d75 6368 206c 6f6e 6765 7220  s a much longer 
-00000980: 7275 6e74 696d 6520 6173 204f 7074 756e  runtime as Optun
-00000990: 6127 7320 7072 756e 696e 6720 6361 6c6c  a's pruning call
-000009a0: 2069 7320 6d69 7373 696e 6720 616e 6420   is missing and 
-000009b0: 616c 6c20 7472 6961 6c73 2077 696c 6c20  all trials will 
-000009c0: 7275 6e20 756e 7469 6c20 7468 6520 656e  run until the en
-000009d0: 642e 0a20 2020 203a 7061 7261 6d20 6561  d..    :param ea
-000009e0: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
-000009f0: 6e64 733a 204e 756d 6265 7220 6f66 2065  nds: Number of e
-00000a00: 6172 6c79 2073 746f 7070 696e 6720 726f  arly stopping ro
-00000a10: 756e 6473 2e20 4e6f 7420 7573 6564 2077  unds. Not used w
-00000a20: 6865 6e20 6375 7374 6f6d 204d 4c20 6d6f  hen custom ML mo
-00000a30: 6465 6c20 6973 2070 6173 7365 642e 2041  del is passed. A
-00000a40: 6c73 6f0a 2020 2020 2020 2020 6e6f 7420  lso.        not 
-00000a50: 7573 6564 2077 6865 6e20 6879 7065 7274  used when hypert
-00000a60: 756e 696e 675f 6376 5f66 6f6c 6473 2069  uning_cv_folds i
-00000a70: 7320 6772 6561 7465 7220 7468 616e 2031  s greater than 1
-00000a80: 2e0a 2020 2020 3a70 6172 616d 2061 7574  ..    :param aut
-00000a90: 6f74 756e 655f 6d6f 6465 6c3a 2057 6865  otune_model: Whe
-00000aa0: 7468 6572 2074 6f20 6175 746f 7475 6e65  ther to autotune
-00000ab0: 2074 6865 206d 6f64 656c 2e20 4e6f 7420   the model. Not 
-00000ac0: 7573 6564 2077 6865 6e20 6375 7374 6f6d  used when custom
-00000ad0: 204d 4c20 6d6f 6465 6c20 6973 2070 6173   ML model is pas
-00000ae0: 7365 642e 0a20 2020 203a 7061 7261 6d20  sed..    :param 
-00000af0: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
-00000b00: 656c 6563 7469 6f6e 3a20 5768 6574 6865  election: Whethe
-00000b10: 7220 746f 2065 6e61 626c 6520 7265 6375  r to enable recu
-00000b20: 7273 6976 6520 6665 6174 7572 6520 7365  rsive feature se
-00000b30: 6c65 6374 696f 6e2e 0a20 2020 203a 7061  lection..    :pa
-00000b40: 7261 6d20 6361 6c63 756c 6174 655f 7368  ram calculate_sh
-00000b50: 6170 5f76 616c 7565 733a 2057 6865 7468  ap_values: Wheth
-00000b60: 6572 2074 6f20 6361 6c63 756c 6174 6520  er to calculate 
-00000b70: 7368 6170 2076 616c 7565 732e 2041 6c73  shap values. Als
-00000b80: 6f20 7573 6564 2077 6865 6e20 6375 7374  o used when cust
-00000b90: 6f6d 204d 4c20 6d6f 6465 6c20 6973 2070  om ML model is p
-00000ba0: 6173 7365 642e 204e 6f74 0a20 2020 2020  assed. Not.     
-00000bb0: 2020 2063 6f6d 7061 7469 626c 6520 7769     compatible wi
-00000bc0: 7468 2061 6c6c 204d 4c20 6d6f 6465 6c73  th all ML models
-00000bd0: 2e20 5365 6520 7468 6520 5348 4150 2064  . See the SHAP d
-00000be0: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
-00000bf0: 206d 6f72 6520 6465 7461 696c 732e 0a20   more details.. 
-00000c00: 2020 203a 7061 7261 6d20 7368 6170 5f77     :param shap_w
-00000c10: 6174 6572 6661 6c6c 5f69 6e64 6963 6573  aterfall_indices
-00000c20: 3a20 4c69 7374 206f 6620 7361 6d70 6c65  : List of sample
-00000c30: 2069 6e64 6963 6573 2074 6f20 706c 6f74   indices to plot
-00000c40: 2e20 4561 6368 2069 6e64 6578 2072 6570  . Each index rep
-00000c50: 7265 7365 6e74 7320 6120 7361 6d70 6c65  resents a sample
-00000c60: 2028 692e 652e 3a20 5b30 2c20 312c 2034   (i.e.: [0, 1, 4
-00000c70: 3939 5d29 2e0a 2020 2020 3a70 6172 616d  99])..    :param
-00000c80: 2073 686f 775f 6465 7065 6e64 656e 6365   show_dependence
-00000c90: 5f70 6c6f 7473 5f6f 665f 746f 705f 6e5f  _plots_of_top_n_
-00000ca0: 6665 6174 7572 6573 3a20 4d61 7869 6d75  features: Maximu
-00000cb0: 6d20 6e75 6d62 6572 206f 6620 6465 7065  m number of depe
-00000cc0: 6e64 656e 6365 2070 6c6f 7473 2074 6f20  ndence plots to 
-00000cd0: 7368 6f77 2e20 4e6f 7420 7573 6564 2077  show. Not used w
-00000ce0: 6865 6e20 6375 7374 6f6d 204d 4c0a 2020  hen custom ML.  
-00000cf0: 2020 2020 2020 6d6f 6465 6c20 6973 2070        model is p
-00000d00: 6173 7365 642e 0a20 2020 203a 7061 7261  assed..    :para
-00000d10: 6d20 7374 6f72 655f 7368 6170 5f76 616c  m store_shap_val
-00000d20: 7565 735f 696e 5f69 6e73 7461 6e63 653a  ues_in_instance:
-00000d30: 2057 6865 7468 6572 2074 6f20 7374 6f72   Whether to stor
-00000d40: 6520 7468 6520 5348 4150 2076 616c 7565  e the SHAP value
-00000d50: 7320 696e 2074 6865 2042 6c75 6543 6173  s in the BlueCas
-00000d60: 7420 696e 7374 616e 6365 2e20 4e6f 7420  t instance. Not 
-00000d70: 6170 706c 6963 6162 6c65 2077 6865 6e0a  applicable when.
-00000d80: 2020 2020 2020 2020 6375 7374 6f6d 204d          custom M
-00000d90: 4c20 6d6f 6465 6c20 6973 2075 7365 642e  L model is used.
-00000da0: 0a20 2020 203a 7061 7261 6d20 7472 6169  .    :param trai
-00000db0: 6e5f 7369 7a65 3a20 5472 6169 6e20 7369  n_size: Train si
-00000dc0: 7a65 2074 6f20 7573 6520 666f 7220 7472  ze to use for tr
-00000dd0: 6169 6e2d 7465 7374 2073 706c 6974 2e0a  ain-test split..
-00000de0: 2020 2020 3a70 6172 616d 2074 7261 696e      :param train
-00000df0: 5f73 706c 6974 5f73 7472 6174 6966 793a  _split_stratify:
-00000e00: 2057 6865 7468 6572 2074 6f20 7374 7261   Whether to stra
-00000e10: 7469 6679 2074 6865 2074 7261 696e 2d74  tify the train-t
-00000e20: 6573 7420 7370 6c69 742e 204e 6f74 2075  est split. Not u
-00000e30: 7365 6420 7768 656e 2063 7573 746f 6d20  sed when custom 
-00000e40: 4d4c 206d 6f64 656c 2069 7320 7061 7373  ML model is pass
-00000e50: 6564 2e0a 2020 2020 3a70 6172 616d 2075  ed..    :param u
-00000e60: 7365 5f66 756c 6c5f 6461 7461 5f66 6f72  se_full_data_for
-00000e70: 5f66 696e 616c 5f6d 6f64 656c 3a20 5768  _final_model: Wh
-00000e80: 6574 6865 7220 746f 2075 7365 2074 6865  ether to use the
-00000e90: 2066 756c 6c20 6461 7461 2066 6f72 2074   full data for t
-00000ea0: 6865 2066 696e 616c 206d 6f64 656c 2e20  he final model. 
-00000eb0: 5468 6973 206d 6967 6874 2063 6175 7365  This might cause
-00000ec0: 206f 7665 7266 6974 7469 6e67 2e0a 2020   overfitting..  
-00000ed0: 2020 2020 2020 4e6f 7420 7573 6564 2077        Not used w
-00000ee0: 6865 6e20 6375 7374 6f6d 204d 4c20 6d6f  hen custom ML mo
-00000ef0: 6465 6c20 6973 2070 6173 7365 642e 0a20  del is passed.. 
-00000f00: 2020 203a 7061 7261 6d20 6d69 6e5f 6665     :param min_fe
-00000f10: 6174 7572 6573 5f74 6f5f 7365 6c65 6374  atures_to_select
-00000f20: 3a20 4d69 6e69 6d75 6d20 6e75 6d62 6572  : Minimum number
-00000f30: 206f 6620 6665 6174 7572 6573 2074 6f20   of features to 
-00000f40: 7365 6c65 6374 2e20 4f6e 6c79 2075 7365  select. Only use
-00000f50: 6420 7768 656e 2065 6e61 626c 655f 6665  d when enable_fe
-00000f60: 6174 7572 655f 7365 6c65 6374 696f 6e20  ature_selection 
-00000f70: 6973 0a20 2020 2020 2020 2054 7275 652e  is.        True.
-00000f80: 0a20 2020 203a 7061 7261 6d20 6361 7264  .    :param card
-00000f90: 696e 616c 6974 795f 7468 7265 7368 6f6c  inality_threshol
-00000fa0: 645f 666f 725f 6f6e 6568 6f74 5f65 6e63  d_for_onehot_enc
-00000fb0: 6f64 696e 673a 2043 6174 6567 6f72 6963  oding: Categoric
-00000fc0: 616c 2066 6561 7475 7265 7320 7769 7468  al features with
-00000fd0: 2061 2063 6172 6469 6e61 6c69 7479 206f   a cardinality o
-00000fe0: 6620 6c65 7373 206f 7220 6571 7561 6c0a  f less or equal.
-00000ff0: 2020 2020 2020 2020 7468 6973 2074 6872          this thr
-00001000: 6573 686f 6c64 2077 696c 6c20 6265 206f  eshold will be o
-00001010: 6e65 686f 7420 656e 636f 6465 642e 2054  nehot encoded. T
-00001020: 6865 2072 6573 7420 7769 6c6c 2062 6520  he rest will be 
-00001030: 7461 7267 6574 2065 6e63 6f64 6564 2e20  target encoded. 
-00001040: 5769 6c6c 2062 6520 6967 6e6f 7265 6420  Will be ignored 
-00001050: 6966 0a20 2020 2020 2020 2063 6174 5f65  if.        cat_e
-00001060: 6e63 6f64 696e 675f 7669 615f 6d6c 5f61  ncoding_via_ml_a
-00001070: 6c67 6f72 6974 686d 2069 7320 7365 7420  lgorithm is set 
-00001080: 746f 2074 7275 652e 0a20 2020 203a 7061  to true..    :pa
-00001090: 7261 6d20 6361 745f 656e 636f 6469 6e67  ram cat_encoding
-000010a0: 5f76 6961 5f6d 6c5f 616c 676f 7269 7468  _via_ml_algorith
-000010b0: 6d3a 2057 6865 7468 6572 2074 6f20 7573  m: Whether to us
-000010c0: 6520 616e 204d 4c20 616c 676f 7269 7468  e an ML algorith
-000010d0: 6d20 666f 7220 6361 7465 676f 7269 6361  m for categorica
-000010e0: 6c20 656e 636f 6469 6e67 2e20 4966 2054  l encoding. If T
-000010f0: 7275 652c 2074 6865 0a20 2020 2020 2020  rue, the.       
-00001100: 2063 6174 6567 6f72 6963 616c 2065 6e63   categorical enc
-00001110: 6f64 696e 6720 6973 2064 6f6e 6520 7669  oding is done vi
-00001120: 6120 6120 4d4c 2061 6c67 6f72 6974 686d  a a ML algorithm
-00001130: 2e20 4966 2046 616c 7365 2c20 7468 6520  . If False, the 
-00001140: 6361 7465 676f 7269 6361 6c20 656e 636f  categorical enco
-00001150: 6469 6e67 2069 7320 646f 6e65 2076 6961  ding is done via
-00001160: 2061 2020 7461 7267 6574 0a20 2020 2020   a  target.     
-00001170: 2020 2065 6e63 6f64 696e 6720 696e 2074     encoding in t
-00001180: 6865 2070 7265 7072 6f63 6573 7369 6e67  he preprocessing
-00001190: 2073 7465 7073 2e20 5365 6520 7468 6520   steps. See the 
-000011a0: 5265 6164 4d65 2066 6f72 206d 6f72 6520  ReadMe for more 
-000011b0: 6465 7461 696c 732e 0a20 2020 203a 7061  details..    :pa
-000011c0: 7261 6d20 7368 6f77 5f64 6574 6169 6c65  ram show_detaile
-000011d0: 645f 7475 6e69 6e67 5f6c 6f67 733a 2057  d_tuning_logs: W
-000011e0: 6865 7468 6572 2074 6f20 7368 6f77 2064  hether to show d
-000011f0: 6574 6169 6c65 6420 7475 6e69 6e67 206c  etailed tuning l
-00001200: 6f67 732e 204e 6f74 2075 7365 6420 7768  ogs. Not used wh
-00001210: 656e 2063 7573 746f 6d20 4d4c 206d 6f64  en custom ML mod
-00001220: 656c 2069 7320 7061 7373 6564 2e0a 2020  el is passed..  
-00001230: 2020 3a70 6172 616d 2065 6e61 626c 655f    :param enable_
-00001240: 6772 6964 5f73 6561 7263 685f 6669 6e65  grid_search_fine
-00001250: 5f74 756e 696e 673a 2041 6674 6572 2068  _tuning: After h
-00001260: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
-00001270: 6e69 6e67 2072 756e 2047 7269 6473 6561  ning run Gridsea
-00001280: 7263 6820 7475 6e69 6e67 206f 6e20 6120  rch tuning on a 
-00001290: 6669 6e65 2d67 7261 696e 6564 2067 7269  fine-grained gri
-000012a0: 640a 2020 2020 2020 2020 6261 7365 6420  d.        based 
-000012b0: 6f6e 2074 6865 2070 7265 7669 6f75 7320  on the previous 
-000012c0: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
-000012d0: 756e 696e 672e 204f 6e6c 7920 706f 7373  uning. Only poss
-000012e0: 6962 6c65 2077 6865 6e20 6175 746f 7475  ible when autotu
-000012f0: 6e65 5f6d 6f64 656c 2069 7320 5472 7565  ne_model is True
-00001300: 2e0a 2020 2020 3a70 6172 616d 2067 7269  ..    :param gri
-00001310: 6473 6561 7263 685f 6e62 5f70 6172 616d  dsearch_nb_param
-00001320: 6574 6572 735f 7065 725f 6772 6964 3a20  eters_per_grid: 
-00001330: 4465 6369 6465 7320 686f 7720 6d61 6e79  Decides how many
-00001340: 2073 7465 7073 2074 6865 2067 7269 6420   steps the grid 
-00001350: 7368 616c 6c20 6861 7665 2070 6572 2070  shall have per p
-00001360: 6172 616d 6574 6572 2e0a 2020 2020 3a70  arameter..    :p
-00001370: 6172 616d 2067 7269 6473 6561 7263 685f  aram gridsearch_
-00001380: 7475 6e69 6e67 5f6d 6178 5f72 756e 7469  tuning_max_runti
-00001390: 6d65 5f73 6563 733a 2053 6574 7320 7468  me_secs: Sets th
-000013a0: 6520 6d61 7869 6d75 6d20 7469 6d65 2069  e maximum time i
-000013b0: 6e20 7365 636f 6e64 7320 7468 6520 7475  n seconds the tu
-000013c0: 6e69 6e67 2073 6861 6c6c 2072 756e 2e20  ning shall run. 
-000013d0: 5468 6973 2077 696c 6c20 6669 6e69 7368  This will finish
-000013e0: 0a20 2020 2020 2020 2074 6865 206c 6174  .        the lat
-000013f0: 6573 7420 7472 6961 6c20 6e64 2077 696c  est trial nd wil
-00001400: 6c20 6578 6365 6564 2074 6869 7320 6c69  l exceed this li
-00001410: 6d69 7420 7468 6f75 6768 2e0a 2020 2020  mit though..    
-00001420: 3a70 6172 616d 2065 7870 6572 696d 656e  :param experimen
-00001430: 745f 6e61 6d65 3a20 4e61 6d65 206f 6620  t_name: Name of 
-00001440: 7468 6520 6578 7065 7269 6d65 6e74 2e20  the experiment. 
-00001450: 5769 6c6c 2062 6520 6c6f 6767 6564 2069  Will be logged i
-00001460: 6e73 6964 6520 7468 6520 4578 7065 7269  nside the Experi
-00001470: 6d65 6e74 5472 6163 6b65 722e 0a20 2020  mentTracker..   
-00001480: 20e9 0a00 0000 da13 676c 6f62 616c 5f72   .......global_r
-00001490: 616e 646f 6d5f 7374 6174 65e9 2100 0000  andom_state.!...
-000014a0: da27 696e 6372 6561 7365 5f72 616e 646f  .'increase_rando
-000014b0: 6d5f 7374 6174 655f 696e 5f62 6c75 6563  m_state_in_bluec
-000014c0: 6173 745f 6376 5f62 7954 da17 7368 7566  ast_cv_byT..shuf
-000014d0: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
-000014e0: 696e 67e9 c800 0000 da1c 6879 7065 7270  ing.......hyperp
-000014f0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
-00001500: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
-00001510: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
-00001520: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
-00001530: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
-00001540: 756e 696e 675f 6376 5f66 6f6c 6473 46da  uning_cv_foldsF.
-00001550: 1170 7265 6369 7365 5f63 765f 7475 6e69  .precise_cv_tuni
-00001560: 6e67 4eda 1565 6172 6c79 5f73 746f 7070  ngN..early_stopp
-00001570: 696e 675f 726f 756e 6473 da0e 6175 746f  ing_rounds..auto
-00001580: 7475 6e65 5f6d 6f64 656c da18 656e 6162  tune_model..enab
-00001590: 6c65 5f66 6561 7475 7265 5f73 656c 6563  le_feature_selec
-000015a0: 7469 6f6e da15 6361 6c63 756c 6174 655f  tion..calculate_
-000015b0: 7368 6170 5f76 616c 7565 7372 0100 0000  shap_valuesr....
-000015c0: da16 7368 6170 5f77 6174 6572 6661 6c6c  ..shap_waterfall
-000015d0: 5f69 6e64 6963 6573 da27 7368 6f77 5f64  _indices.'show_d
-000015e0: 6570 656e 6465 6e63 655f 706c 6f74 735f  ependence_plots_
-000015f0: 6f66 5f74 6f70 5f6e 5f66 6561 7475 7265  of_top_n_feature
-00001600: 73da 1d73 746f 7265 5f73 6861 705f 7661  s..store_shap_va
-00001610: 6c75 6573 5f69 6e5f 696e 7374 616e 6365  lues_in_instance
-00001620: e79a 9999 9999 99e9 3fda 0a74 7261 696e  ........?..train
-00001630: 5f73 697a 65da 1474 7261 696e 5f73 706c  _size..train_spl
-00001640: 6974 5f73 7472 6174 6966 79da 1d75 7365  it_stratify..use
-00001650: 5f66 756c 6c5f 6461 7461 5f66 6f72 5f66  _full_data_for_f
-00001660: 696e 616c 5f6d 6f64 656c e905 0000 00da  inal_model......
-00001670: 166d 696e 5f66 6561 7475 7265 735f 746f  .min_features_to
-00001680: 5f73 656c 6563 74da 2963 6172 6469 6e61  _select.)cardina
-00001690: 6c69 7479 5f74 6872 6573 686f 6c64 5f66  lity_threshold_f
-000016a0: 6f72 5f6f 6e65 686f 745f 656e 636f 6469  or_onehot_encodi
-000016b0: 6e67 da1d 6361 745f 656e 636f 6469 6e67  ng..cat_encoding
-000016c0: 5f76 6961 5f6d 6c5f 616c 676f 7269 7468  _via_ml_algorith
-000016d0: 6dda 1973 686f 775f 6465 7461 696c 6564  m..show_detailed
-000016e0: 5f74 756e 696e 675f 6c6f 6773 da1f 6f70  _tuning_logs..op
-000016f0: 7475 6e61 5f73 616d 706c 6572 5f6e 5f73  tuna_sampler_n_s
-00001700: 7461 7274 7570 5f74 7269 616c 73da 1e65  tartup_trials..e
-00001710: 6e61 626c 655f 6772 6964 5f73 6561 7263  nable_grid_searc
-00001720: 685f 6669 6e65 5f74 756e 696e 67da 2267  h_fine_tuning."g
-00001730: 7269 6473 6561 7263 685f 7475 6e69 6e67  ridsearch_tuning
-00001740: 5f6d 6178 5f72 756e 7469 6d65 5f73 6563  _max_runtime_sec
-00001750: 73da 2167 7269 6473 6561 7263 685f 6e62  s.!gridsearch_nb
-00001760: 5f70 6172 616d 6574 6572 735f 7065 725f  _parameters_per_
-00001770: 6772 6964 7a0e 6e65 7720 6578 7065 7269  gridz.new experi
-00001780: 6d65 6e74 da0f 6578 7065 7269 6d65 6e74  ment..experiment
-00001790: 5f6e 616d 6529 2572 0800 0000 7209 0000  _name)%r....r...
-000017a0: 0072 0a00 0000 da07 5f5f 646f 635f 5f72  .r......__doc__r
-000017b0: 0f00 0000 da03 696e 74da 0f5f 5f61 6e6e  ......int..__ann
-000017c0: 6f74 6174 696f 6e73 5f5f 7211 0000 0072  otations__r....r
-000017d0: 1200 0000 da04 626f 6f6c 7214 0000 0072  ......boolr....r
-000017e0: 1500 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-000017f0: 0000 0072 0400 0000 721a 0000 0072 1b00  ...r....r....r..
-00001800: 0000 721c 0000 0072 1d00 0000 7203 0000  ..r....r....r...
-00001810: 0072 1e00 0000 721f 0000 0072 2100 0000  .r....r....r!...
-00001820: da05 666c 6f61 7472 2200 0000 7223 0000  ..floatr"...r#..
-00001830: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00001840: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-00001850: 2b00 0000 722c 0000 0072 2d00 0000 da03  +...r,...r-.....
-00001860: 7374 7272 0b00 0000 720b 0000 0072 0b00  strr....r....r..
-00001870: 0000 720c 0000 0072 0d00 0000 1300 0000  ..r....r........
-00001880: 7338 0000 000a 0004 010c 2e0c 010c 010c  s8..............
-00001890: 010c 010c 010c 0110 010c 010c 010c 0112  ................
-000018a0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-000018b0: 010c 010c 010c 010c 010c 0110 0172 0d00  .............r..
-000018c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000018d0: 0000 0003 0000 0040 0000 0073 5601 0000  .......@...sV...
-000018e0: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-000018f0: 5a04 6505 6506 6403 3c00 6404 5a07 6505  Z.e.e.d.<.d.Z.e.
-00001900: 6506 6405 3c00 6406 5a08 6509 6506 6407  e.d.<.d.Z.e.e.d.
-00001910: 3c00 6408 5a0a 6509 6506 6409 3c00 6406  <.d.Z.e.e.d.<.d.
-00001920: 5a0b 6509 6506 640a 3c00 6408 5a0c 6509  Z.e.e.d.<.d.Z.e.
-00001930: 6506 640b 3c00 6406 5a0d 6509 6506 640c  e.d.<.d.Z.e.e.d.
-00001940: 3c00 6408 5a0e 6509 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
-00001950: 5a0f 6509 6506 640f 3c00 6408 5a10 6509  Z.e.e.d.<.d.Z.e.
-00001960: 6506 6410 3c00 6411 5a11 6505 6506 6412  e.d.<.d.Z.e.e.d.
-00001970: 3c00 6411 5a12 6505 6506 6413 3c00 6414  <.d.Z.e.e.d.<.d.
-00001980: 5a13 6509 6506 6415 3c00 6416 5a14 6509  Z.e.e.d.<.d.Z.e.
-00001990: 6506 6417 3c00 6414 5a15 6509 6506 6418  e.d.<.d.Z.e.e.d.
-000019a0: 3c00 6416 5a16 6509 6506 6419 3c00 6414  <.d.Z.e.e.d.<.d.
-000019b0: 5a17 6509 6506 641a 3c00 6416 5a18 6509  Z.e.e.d.<.d.Z.e.
-000019c0: 6506 641b 3c00 641c 5a19 6509 6506 641d  e.d.<.d.Z.e.e.d.
-000019d0: 3c00 6414 5a1a 6509 6506 641e 3c00 641f  <.d.Z.e.e.d.<.d.
-000019e0: 5a1b 6505 6506 6420 3c00 6421 5a1c 6505  Z.e.e.d <.d!Z.e.
-000019f0: 6506 6422 3c00 6411 5a1d 6505 6506 6423  e.d"<.d.Z.e.e.d#
-00001a00: 3c00 6411 5a1e 6505 6506 6424 3c00 6425  <.d.Z.e.e.d$<.d%
-00001a10: 5a1f 6520 6506 6426 3c00 6427 5a21 6520  Z.e e.d&<.d'Z!e 
-00001a20: 6506 6428 3c00 6429 5a22 6520 6506 642a  e.d(<.d)Z"e e.d*
-00001a30: 3c00 642b 5300 292c da17 5867 626f 6f73  <.d+S.),..Xgboos
-00001a40: 7454 756e 6550 6172 616d 7343 6f6e 6669  tTuneParamsConfi
-00001a50: 67fa 2a44 6566 696e 6520 6879 7065 7270  g.*Define hyperp
-00001a60: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
-00001a70: 7365 6172 6368 2073 7061 6365 2ee9 0200  search space....
-00001a80: 0000 da0d 6d61 785f 6465 7074 685f 6d69  ....max_depth_mi
-00001a90: 6ee9 0c00 0000 da0d 6d61 785f 6465 7074  n.......max_dept
-00001aa0: 685f 6d61 78e7 3a8c 30e2 8e79 453e da09  h_max.:.0..yE>..
-00001ab0: 616c 7068 615f 6d69 6ee7 0000 0000 0000  alpha_min.......
-00001ac0: 2440 da09 616c 7068 615f 6d61 78da 0a6c  $@..alpha_max..l
-00001ad0: 616d 6264 615f 6d69 6eda 0a6c 616d 6264  ambda_min..lambd
-00001ae0: 615f 6d61 78da 0967 616d 6d61 5f6d 696e  a_max..gamma_min
-00001af0: da09 6761 6d6d 615f 6d61 78e7 0000 0000  ..gamma_max.....
-00001b00: 0000 0000 da0d 7375 6273 616d 706c 655f  ......subsample_
-00001b10: 6d69 6eda 0d73 7562 7361 6d70 6c65 5f6d  min..subsample_m
-00001b20: 6178 7201 0000 00da 0e6d 6178 5f6c 6561  axr......max_lea
-00001b30: 7665 735f 6d69 6eda 0e6d 6178 5f6c 6561  ves_min..max_lea
-00001b40: 7665 735f 6d61 78e7 3333 3333 3333 d33f  ves_max.333333.?
-00001b50: da0e 7375 625f 7361 6d70 6c65 5f6d 696e  ..sub_sample_min
-00001b60: e700 0000 0000 00f0 3fda 0e73 7562 5f73  ........?..sub_s
-00001b70: 616d 706c 655f 6d61 78da 1663 6f6c 5f73  ample_max..col_s
-00001b80: 616d 706c 655f 6279 5f74 7265 655f 6d69  ample_by_tree_mi
-00001b90: 6eda 1663 6f6c 5f73 616d 706c 655f 6279  n..col_sample_by
-00001ba0: 5f74 7265 655f 6d61 78da 1763 6f6c 5f73  _tree_max..col_s
-00001bb0: 616d 706c 655f 6279 5f6c 6576 656c 5f6d  ample_by_level_m
-00001bc0: 696e da17 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
-00001bd0: 795f 6c65 7665 6c5f 6d61 78e7 fca9 f1d2  y_level_max.....
-00001be0: 4d62 503f da07 6574 615f 6d69 6eda 0765  MbP?..eta_min..e
-00001bf0: 7461 5f6d 6178 e932 0000 00da 0973 7465  ta_max.2.....ste
-00001c00: 7073 5f6d 696e e9e8 0300 00da 0973 7465  ps_min.......ste
-00001c10: 7073 5f6d 6178 da26 7665 7262 6f73 6974  ps_max.&verbosit
-00001c20: 795f 6475 7269 6e67 5f68 7970 6572 7061  y_during_hyperpa
-00001c30: 7261 6d65 7465 725f 7475 6e69 6e67 da25  rameter_tuning.%
-00001c40: 7665 7262 6f73 6974 795f 6475 7269 6e67  verbosity_during
-00001c50: 5f66 696e 616c 5f6d 6f64 656c 5f74 7261  _final_model_tra
-00001c60: 696e 696e 677a 0e6d 756c 7469 3a73 6f66  iningz.multi:sof
-00001c70: 7470 726f 62da 1178 6762 6f6f 7374 5f6f  tprob..xgboost_o
-00001c80: 626a 6563 7469 7665 da08 6d6c 6f67 6c6f  bjective..mloglo
-00001c90: 7373 da13 7867 626f 6f73 745f 6576 616c  ss..xgboost_eval
-00001ca0: 5f6d 6574 7269 63da 0667 6274 7265 65da  _metric..gbtree.
-00001cb0: 0762 6f6f 7374 6572 4ea9 2372 0800 0000  .boosterN.#r....
-00001cc0: 7209 0000 0072 0a00 0000 722e 0000 0072  r....r....r....r
-00001cd0: 3700 0000 722f 0000 0072 3000 0000 7239  7...r/...r0...r9
-00001ce0: 0000 0072 3b00 0000 7232 0000 0072 3d00  ...r;...r2...r=.
-00001cf0: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
-00001d00: 0072 4100 0000 7243 0000 0072 4400 0000  .rA...rC...rD...
-00001d10: 7245 0000 0072 4600 0000 7248 0000 0072  rE...rF...rH...r
-00001d20: 4a00 0000 724b 0000 0072 4c00 0000 724d  J...rK...rL...rM
-00001d30: 0000 0072 4e00 0000 7250 0000 0072 5100  ...rN...rP...rQ.
-00001d40: 0000 7253 0000 0072 5500 0000 7256 0000  ..rS...rU...rV..
-00001d50: 0072 5700 0000 7258 0000 0072 3300 0000  .rW...rX...r3...
-00001d60: 725a 0000 0072 5c00 0000 720b 0000 0072  rZ...r\...r....r
-00001d70: 0b00 0000 720b 0000 0072 0c00 0000 7234  ....r....r....r4
-00001d80: 0000 005e 0000 00f3 3a00 0000 0a00 0401  ...^....:.......
-00001d90: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001da0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001db0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001dc0: 0c01 0c01 1001 7234 0000 0063 0000 0000  ......r4...c....
-00001dd0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00001de0: 4000 0000 7356 0100 0065 005a 0164 005a  @...sV...e.Z.d.Z
-00001df0: 0255 0064 015a 0364 025a 0465 0565 0664  .U.d.Z.d.Z.e.e.d
-00001e00: 033c 0064 045a 0765 0565 0664 053c 0064  .<.d.Z.e.e.d.<.d
-00001e10: 065a 0865 0965 0664 073c 0064 085a 0a65  .Z.e.e.d.<.d.Z.e
-00001e20: 0965 0664 093c 0064 065a 0b65 0965 0664  .e.d.<.d.Z.e.e.d
-00001e30: 0a3c 0064 085a 0c65 0965 0664 0b3c 0064  .<.d.Z.e.e.d.<.d
-00001e40: 065a 0d65 0965 0664 0c3c 0064 085a 0e65  .Z.e.e.d.<.d.Z.e
-00001e50: 0965 0664 0d3c 0064 0e5a 0f65 0965 0664  .e.d.<.d.Z.e.e.d
-00001e60: 0f3c 0064 085a 1065 0965 0664 103c 0064  .<.d.Z.e.e.d.<.d
-00001e70: 115a 1165 0565 0664 123c 0064 115a 1265  .Z.e.e.d.<.d.Z.e
-00001e80: 0565 0664 133c 0064 145a 1365 0965 0664  .e.d.<.d.Z.e.e.d
-00001e90: 153c 0064 165a 1465 0965 0664 173c 0064  .<.d.Z.e.e.d.<.d
-00001ea0: 145a 1565 0965 0664 183c 0064 165a 1665  .Z.e.e.d.<.d.Z.e
-00001eb0: 0965 0664 193c 0064 145a 1765 0965 0664  .e.d.<.d.Z.e.e.d
-00001ec0: 1a3c 0064 165a 1865 0965 0664 1b3c 0064  .<.d.Z.e.e.d.<.d
-00001ed0: 1c5a 1965 0965 0664 1d3c 0064 145a 1a65  .Z.e.e.d.<.d.Z.e
-00001ee0: 0965 0664 1e3c 0064 025a 1b65 0565 0664  .e.d.<.d.Z.e.e.d
-00001ef0: 1f3c 0064 205a 1c65 0565 0664 213c 0064  .<.d Z.e.e.d!<.d
-00001f00: 115a 1d65 0565 0664 223c 0064 115a 1e65  .Z.e.e.d"<.d.Z.e
-00001f10: 0565 0664 233c 0064 245a 1f65 2065 0664  .e.d#<.d$Z.e e.d
-00001f20: 253c 0064 265a 2165 2065 0664 273c 0064  %<.d&Z!e e.d'<.d
-00001f30: 285a 2265 2065 0664 293c 0064 2a53 0029  (Z"e e.d)<.d*S.)
-00001f40: 2bda 2158 6762 6f6f 7374 5475 6e65 5061  +.!XgboostTunePa
-00001f50: 7261 6d73 5265 6772 6573 7369 6f6e 436f  ramsRegressionCo
-00001f60: 6e66 6967 7235 0000 0072 3600 0000 7237  nfigr5...r6...r7
-00001f70: 0000 00e9 0600 0000 7239 0000 0072 3a00  ........r9...r:.
-00001f80: 0000 723b 0000 0072 3c00 0000 723d 0000  ..r;...r<...r=..
-00001f90: 0072 3e00 0000 723f 0000 0072 4000 0000  .r>...r?...r@...
-00001fa0: 7241 0000 0072 4200 0000 7243 0000 0072  rA...rB...rC...r
-00001fb0: 4400 0000 7201 0000 0072 4500 0000 7246  D...r....rE...rF
-00001fc0: 0000 0072 4700 0000 7248 0000 0072 4900  ...rG...rH...rI.
-00001fd0: 0000 724a 0000 0072 4b00 0000 724c 0000  ..rJ...rK...rL..
-00001fe0: 0072 4d00 0000 724e 0000 0072 4f00 0000  .rM...rN...rO...
-00001ff0: 7250 0000 0072 5100 0000 7253 0000 0072  rP...rQ...rS...r
-00002000: 5400 0000 7255 0000 0072 5600 0000 7257  T...rU...rV...rW
-00002010: 0000 007a 1072 6567 3a73 7175 6172 6564  ...z.reg:squared
-00002020: 6572 726f 7272 5800 0000 5a04 726d 7365  errorrX...Z.rmse
-00002030: 725a 0000 0072 5b00 0000 725c 0000 004e  rZ...r[...r\...N
-00002040: 725d 0000 0072 0b00 0000 720b 0000 0072  r]...r....r....r
-00002050: 0b00 0000 720c 0000 0072 5f00 0000 7e00  ....r....r_...~.
-00002060: 0000 725e 0000 0072 5f00 0000 6300 0000  ..r^...r_...c...
-00002070: 0000 0000 0000 0000 0000 0000 000c 0000  ................
-00002080: 0040 0000 0073 5200 0000 6500 5a01 6400  .@...sR...e.Z.d.
-00002090: 5a02 5500 6401 5a03 6402 6403 6404 6404  Z.U.d.Z.d.d.d.d.
-000020a0: 6405 6406 6407 6408 6408 6404 6409 640a  d.d.d.d.d.d.d.d.
-000020b0: 9c0b 5a04 640b 5a05 6506 6507 6508 6509  ..Z.d.Z.e.e.e.e.
-000020c0: 6602 1900 1900 650a 640c 3c00 640d 5a0b  f.....e.d.<.d.Z.
-000020d0: 6509 650a 640e 3c00 640b 5300 290f da17  e.e.d.<.d.S.)...
-000020e0: 5867 626f 6f73 7446 696e 616c 5061 7261  XgboostFinalPara
-000020f0: 6d43 6f6e 6669 677a 1e44 6566 696e 6520  mConfigz.Define 
-00002100: 6669 6e61 6c20 6879 7065 7220 7061 7261  final hyper para
-00002110: 6d65 7465 7273 2e72 5b00 0000 e907 0000  meters.r[.......
-00002120: 0067 9a99 9999 9999 b93f 7242 0000 0072  .g.......?rB...r
-00002130: 4900 0000 e910 0000 0072 2000 0000 7254  I........r ...rT
-00002140: 0000 0029 0b72 5c00 0000 da09 6d61 785f  ...).r\.....max_
-00002150: 6465 7074 68da 0561 6c70 6861 da06 6c61  depth..alpha..la
-00002160: 6d62 6461 da05 6761 6d6d 615a 0973 7562  mbda..gammaZ.sub
-00002170: 7361 6d70 6c65 5a0a 6d61 785f 6c65 6176  sampleZ.max_leav
-00002180: 6573 5a10 636f 6c73 616d 706c 655f 6279  esZ.colsample_by
-00002190: 7472 6565 5a11 636f 6c73 616d 706c 655f  treeZ.colsample_
-000021a0: 6279 6c65 7665 6cda 0365 7461 5a05 7374  bylevel..etaZ.st
-000021b0: 6570 734e da0d 7361 6d70 6c65 5f77 6569  epsN..sample_wei
-000021c0: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
-000021d0: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
-000021e0: 6573 686f 6c64 290c 7208 0000 0072 0900  eshold).r....r..
-000021f0: 0000 720a 0000 0072 2e00 0000 da06 7061  ..r....r......pa
-00002200: 7261 6d73 7269 0000 0072 0400 0000 7202  ramsri...r....r.
-00002210: 0000 0072 3300 0000 7232 0000 0072 3000  ...r3...r2...r0.
-00002220: 0000 726a 0000 0072 0b00 0000 720b 0000  ..rj...r....r...
-00002230: 0072 0b00 0000 720c 0000 0072 6100 0000  .r....r....ra...
-00002240: 9e00 0000 7320 0000 000a 0004 0202 0302  ....s ..........
-00002250: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00002260: 0102 0106 f518 0d10 0172 6100 0000 4e29  .........ra...N)
-00002270: 0e72 2e00 0000 da06 7479 7069 6e67 7202  .r......typingr.
-00002280: 0000 0072 0300 0000 7204 0000 005a 0870  ...r....r....Z.p
-00002290: 7964 616e 7469 6372 0500 0000 5a14 7079  ydanticr....Z.py
-000022a0: 6461 6e74 6963 2e64 6174 6163 6c61 7373  dantic.dataclass
-000022b0: 6573 7206 0000 0072 0700 0000 720d 0000  esr....r....r...
-000022c0: 0072 3400 0000 725f 0000 0072 6100 0000  .r4...r_...ra...
-000022d0: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000022e0: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000022f0: 0000 7314 0000 0004 0014 080c 020c 010e  ..s.............
-00002300: 0310 0410 4b10 2002 2014 01              ....K. . ..
+00000430: 105a 0e65 0f65 0664 113c 0064 0e5a 1065  .Z.e.e.d.<.d.Z.e
+00000440: 0965 0664 123c 0064 135a 1165 1265 0519  .e.d.<.d.Z.e.e..
+00000450: 0065 0664 143c 0064 065a 1365 0965 0664  .e.d.<.d.Z.e.e.d
+00000460: 153c 0064 0e5a 1465 0965 0664 163c 0064  .<.d.Z.e.e.d.<.d
+00000470: 065a 1565 0965 0664 173c 0064 1867 015a  .Z.e.e.d.<.d.g.Z
+00000480: 1665 1765 0519 0065 0664 193c 0064 0c5a  .e.e...e.d.<.d.Z
+00000490: 1865 0565 0664 1a3c 0064 0e5a 1965 0965  .e.e.d.<.d.Z.e.e
+000004a0: 0664 1b3c 0064 1c5a 1a65 0f65 0664 1d3c  .d.<.d.Z.e.e.d.<
+000004b0: 0064 065a 1b65 0965 0664 1e3c 0064 065a  .d.Z.e.e.d.<.d.Z
+000004c0: 1c65 0965 0664 1f3c 0064 205a 1d65 0565  .e.e.d.<.d Z.e.e
+000004d0: 0664 213c 0064 205a 1e65 0565 0664 223c  .d!<.d Z.e.e.d"<
+000004e0: 0064 0e5a 1f65 0965 0664 233c 0064 0e5a  .d.Z.e.e.d#<.d.Z
+000004f0: 2065 0965 0664 243c 0064 025a 2165 0565   e.e.d$<.d.Z!e.e
+00000500: 0664 253c 0064 0e5a 2265 0965 0664 263c  .d%<.d.Z"e.e.d&<
+00000510: 0064 0a5a 2365 0565 0664 273c 0064 205a  .d.Z#e.e.d'<.d Z
+00000520: 2465 0565 0664 283c 0064 295a 2565 2665  $e.e.d(<.d)Z%e&e
+00000530: 0664 2a3c 0064 1353 0029 2bda 0e54 7261  .d*<.d.S.)+..Tra
+00000540: 696e 696e 6743 6f6e 6669 6761 8110 0000  iningConfiga....
+00000550: 4465 6669 6e65 2067 656e 6572 616c 2074  Define general t
+00000560: 7261 696e 696e 6720 7061 7261 6d65 7465  raining paramete
+00000570: 7273 2e0a 0a20 2020 203a 7061 7261 6d20  rs...    :param 
+00000580: 676c 6f62 616c 5f72 616e 646f 6d5f 7374  global_random_st
+00000590: 6174 653a 2047 6c6f 6261 6c20 7261 6e64  ate: Global rand
+000005a0: 6f6d 2073 7461 7465 2074 6f20 7573 6520  om state to use 
+000005b0: 666f 7220 7265 7072 6f64 7563 6962 696c  for reproducibil
+000005c0: 6974 792e 0a20 2020 203a 7061 7261 6d20  ity..    :param 
+000005d0: 696e 6372 6561 7365 5f72 616e 646f 6d5f  increase_random_
+000005e0: 7374 6174 655f 696e 5f62 6c75 6563 6173  state_in_bluecas
+000005f0: 745f 6376 5f62 793a 2049 6e20 426c 7565  t_cv_by: In Blue
+00000600: 4361 7374 4356 206d 756c 7469 706c 6520  CastCV multiple 
+00000610: 6d6f 6465 6c73 2061 7265 2074 7261 696e  models are train
+00000620: 6564 2e20 4465 6669 6e65 2062 7920 686f  ed. Define by ho
+00000630: 7720 6d75 6368 2074 6865 0a20 2020 2020  w much the.     
+00000640: 2020 2072 616e 646f 6d20 7374 6174 6520     random state 
+00000650: 6368 616e 6765 7320 7769 7468 2065 6163  changes with eac
+00000660: 6820 6164 6469 7469 6f6e 616c 206d 6f64  h additional mod
+00000670: 656c 2e0a 2020 2020 3a70 6172 616d 2073  el..    :param s
+00000680: 6875 6666 6c65 5f64 7572 696e 675f 7472  huffle_during_tr
+00000690: 6169 6e69 6e67 3a20 5768 6574 6865 7220  aining: Whether 
+000006a0: 746f 2073 6875 6666 6c65 2074 6865 2064  to shuffle the d
+000006b0: 6174 6120 6475 7269 6e67 2074 7261 696e  ata during train
+000006c0: 696e 6720 7768 656e 2068 7970 6572 7475  ing when hypertu
+000006d0: 6e69 6e67 5f63 765f 666f 6c64 7320 3e20  ning_cv_folds > 
+000006e0: 312e 0a20 2020 203a 7061 7261 6d20 6879  1..    :param hy
+000006f0: 7065 7270 6172 616d 6574 6572 5f74 756e  perparameter_tun
+00000700: 696e 675f 726f 756e 6473 3a20 4e75 6d62  ing_rounds: Numb
+00000710: 6572 206f 6620 6879 7065 7270 6172 616d  er of hyperparam
+00000720: 6574 6572 2074 756e 696e 6720 726f 756e  eter tuning roun
+00000730: 6473 2e20 4e6f 7420 7573 6564 2077 6865  ds. Not used whe
+00000740: 6e20 6375 7374 6f6d 204d 4c20 6d6f 6465  n custom ML mode
+00000750: 6c20 6973 2070 6173 7365 642e 0a20 2020  l is passed..   
+00000760: 203a 7061 7261 6d20 6879 7065 7270 6172   :param hyperpar
+00000770: 616d 6574 6572 5f74 756e 696e 675f 6d61  ameter_tuning_ma
+00000780: 785f 7275 6e74 696d 655f 7365 6373 3a20  x_runtime_secs: 
+00000790: 4d61 7869 6d75 6d20 7275 6e74 696d 6520  Maximum runtime 
+000007a0: 696e 2073 6563 6f6e 6473 2066 6f72 2068  in seconds for h
+000007b0: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
+000007c0: 6e69 6e67 2e20 4e6f 7420 7573 6564 2077  ning. Not used w
+000007d0: 6865 6e0a 2020 2020 2020 2020 6375 7374  hen.        cust
+000007e0: 6f6d 204d 4c20 6d6f 6465 6c20 6973 2070  om ML model is p
+000007f0: 6173 7365 642e 0a20 2020 203a 7061 7261  assed..    :para
+00000800: 6d20 6879 7065 7274 756e 696e 675f 6376  m hypertuning_cv
+00000810: 5f66 6f6c 6473 3a20 4e75 6d62 6572 206f  _folds: Number o
+00000820: 6620 6372 6f73 732d 7661 6c69 6461 7469  f cross-validati
+00000830: 6f6e 2066 6f6c 6473 2074 6f20 7573 6520  on folds to use 
+00000840: 666f 7220 6879 7065 7270 6172 616d 6574  for hyperparamet
+00000850: 6572 2074 756e 696e 672e 204e 6f74 2075  er tuning. Not u
+00000860: 7365 6420 7768 656e 0a20 2020 2020 2020  sed when.       
+00000870: 2063 7573 746f 6d20 4d4c 206d 6f64 656c   custom ML model
+00000880: 2069 7320 7061 7373 6564 2e0a 2020 2020   is passed..    
+00000890: 3a70 6172 616d 2073 616d 706c 655f 6461  :param sample_da
+000008a0: 7461 5f64 7572 696e 675f 7475 6e69 6e67  ta_during_tuning
+000008b0: 3a20 5768 6574 6865 7220 746f 2073 616d  : Whether to sam
+000008c0: 706c 6520 7468 6520 6461 7461 2064 7572  ple the data dur
+000008d0: 696e 6720 7475 6e69 6e67 2e20 4e6f 7420  ing tuning. Not 
+000008e0: 7573 6564 2077 6865 6e20 6375 7374 6f6d  used when custom
+000008f0: 204d 4c20 6d6f 6465 6c20 6973 2070 6173   ML model is pas
+00000900: 7365 642e 0a20 2020 203a 7061 7261 6d20  sed..    :param 
+00000910: 7361 6d70 6c65 5f64 6174 615f 6475 7269  sample_data_duri
+00000920: 6e67 5f74 756e 696e 675f 616c 7068 613a  ng_tuning_alpha:
+00000930: 2041 6c70 6861 2076 616c 7565 2066 6f72   Alpha value for
+00000940: 2073 616d 706c 696e 6720 7468 6520 6461   sampling the da
+00000950: 7461 2064 7572 696e 6720 7475 6e69 6e67  ta during tuning
+00000960: 2e20 5468 6520 6869 6768 6572 2061 6c70  . The higher alp
+00000970: 6861 2074 6865 0a20 2020 2020 2020 2066  ha the.        f
+00000980: 6577 6572 2073 616d 706c 6573 2077 696c  ewer samples wil
+00000990: 6c20 6265 206c 6566 742e 204e 6f74 2075  l be left. Not u
+000009a0: 7365 6420 7768 656e 2063 7573 746f 6d20  sed when custom 
+000009b0: 4d4c 206d 6f64 656c 2069 7320 7061 7373  ML model is pass
+000009c0: 6564 2e0a 2020 2020 3a70 6172 616d 2070  ed..    :param p
+000009d0: 7265 6369 7365 5f63 765f 7475 6e69 6e67  recise_cv_tuning
+000009e0: 3a20 4966 2065 6e61 626c 6564 2077 696c  : If enabled wil
+000009f0: 6c20 7377 6974 6368 2066 726f 6d20 7573  l switch from us
+00000a00: 696e 6720 5867 626f 6f73 7427 7320 6f77  ing Xgboost's ow
+00000a10: 6e20 6376 206d 6574 686f 6420 746f 2061  n cv method to a
+00000a20: 2063 7573 746f 6d20 6372 6f73 7320 7661   custom cross va
+00000a30: 6c69 6461 7469 6f6e 0a20 2020 2020 2020  lidation.       
+00000a40: 2072 6f75 7469 6e65 2e20 5468 6973 2069   routine. This i
+00000a50: 7320 6e65 6564 6564 2077 6865 6e20 7468  s needed when th
+00000a60: 6520 696e 2d66 6f6c 6420 7072 6570 726f  e in-fold prepro
+00000a70: 6365 7373 696e 6720 6973 206e 6563 6573  cessing is neces
+00000a80: 7361 7279 2074 6861 7420 776f 756c 6420  sary that would 
+00000a90: 6361 7573 6520 6f76 6572 6669 7474 696e  cause overfittin
+00000aa0: 6720 7769 7468 2075 7375 616c 2063 762e  g with usual cv.
+00000ab0: 0a20 2020 2020 2020 2054 6869 7320 6861  .        This ha
+00000ac0: 7320 6120 6d75 6368 206c 6f6e 6765 7220  s a much longer 
+00000ad0: 7275 6e74 696d 6520 6173 204f 7074 756e  runtime as Optun
+00000ae0: 6127 7320 7072 756e 696e 6720 6361 6c6c  a's pruning call
+00000af0: 2069 7320 6d69 7373 696e 6720 616e 6420   is missing and 
+00000b00: 616c 6c20 7472 6961 6c73 2077 696c 6c20  all trials will 
+00000b10: 7275 6e20 756e 7469 6c20 7468 6520 656e  run until the en
+00000b20: 642e 0a20 2020 203a 7061 7261 6d20 6561  d..    :param ea
+00000b30: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
+00000b40: 6e64 733a 204e 756d 6265 7220 6f66 2065  nds: Number of e
+00000b50: 6172 6c79 2073 746f 7070 696e 6720 726f  arly stopping ro
+00000b60: 756e 6473 2e20 4e6f 7420 7573 6564 2077  unds. Not used w
+00000b70: 6865 6e20 6375 7374 6f6d 204d 4c20 6d6f  hen custom ML mo
+00000b80: 6465 6c20 6973 2070 6173 7365 642e 2041  del is passed. A
+00000b90: 6c73 6f0a 2020 2020 2020 2020 6e6f 7420  lso.        not 
+00000ba0: 7573 6564 2077 6865 6e20 6879 7065 7274  used when hypert
+00000bb0: 756e 696e 675f 6376 5f66 6f6c 6473 2069  uning_cv_folds i
+00000bc0: 7320 6772 6561 7465 7220 7468 616e 2031  s greater than 1
+00000bd0: 2e0a 2020 2020 3a70 6172 616d 2061 7574  ..    :param aut
+00000be0: 6f74 756e 655f 6d6f 6465 6c3a 2057 6865  otune_model: Whe
+00000bf0: 7468 6572 2074 6f20 6175 746f 7475 6e65  ther to autotune
+00000c00: 2074 6865 206d 6f64 656c 2e20 4e6f 7420   the model. Not 
+00000c10: 7573 6564 2077 6865 6e20 6375 7374 6f6d  used when custom
+00000c20: 204d 4c20 6d6f 6465 6c20 6973 2070 6173   ML model is pas
+00000c30: 7365 642e 0a20 2020 203a 7061 7261 6d20  sed..    :param 
+00000c40: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
+00000c50: 656c 6563 7469 6f6e 3a20 5768 6574 6865  election: Whethe
+00000c60: 7220 746f 2065 6e61 626c 6520 7265 6375  r to enable recu
+00000c70: 7273 6976 6520 6665 6174 7572 6520 7365  rsive feature se
+00000c80: 6c65 6374 696f 6e2e 0a20 2020 203a 7061  lection..    :pa
+00000c90: 7261 6d20 6361 6c63 756c 6174 655f 7368  ram calculate_sh
+00000ca0: 6170 5f76 616c 7565 733a 2057 6865 7468  ap_values: Wheth
+00000cb0: 6572 2074 6f20 6361 6c63 756c 6174 6520  er to calculate 
+00000cc0: 7368 6170 2076 616c 7565 732e 2041 6c73  shap values. Als
+00000cd0: 6f20 7573 6564 2077 6865 6e20 6375 7374  o used when cust
+00000ce0: 6f6d 204d 4c20 6d6f 6465 6c20 6973 2070  om ML model is p
+00000cf0: 6173 7365 642e 204e 6f74 0a20 2020 2020  assed. Not.     
+00000d00: 2020 2063 6f6d 7061 7469 626c 6520 7769     compatible wi
+00000d10: 7468 2061 6c6c 204d 4c20 6d6f 6465 6c73  th all ML models
+00000d20: 2e20 5365 6520 7468 6520 5348 4150 2064  . See the SHAP d
+00000d30: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00000d40: 206d 6f72 6520 6465 7461 696c 732e 0a20   more details.. 
+00000d50: 2020 203a 7061 7261 6d20 7368 6170 5f77     :param shap_w
+00000d60: 6174 6572 6661 6c6c 5f69 6e64 6963 6573  aterfall_indices
+00000d70: 3a20 4c69 7374 206f 6620 7361 6d70 6c65  : List of sample
+00000d80: 2069 6e64 6963 6573 2074 6f20 706c 6f74   indices to plot
+00000d90: 2e20 4561 6368 2069 6e64 6578 2072 6570  . Each index rep
+00000da0: 7265 7365 6e74 7320 6120 7361 6d70 6c65  resents a sample
+00000db0: 2028 692e 652e 3a20 5b30 2c20 312c 2034   (i.e.: [0, 1, 4
+00000dc0: 3939 5d29 2e0a 2020 2020 3a70 6172 616d  99])..    :param
+00000dd0: 2073 686f 775f 6465 7065 6e64 656e 6365   show_dependence
+00000de0: 5f70 6c6f 7473 5f6f 665f 746f 705f 6e5f  _plots_of_top_n_
+00000df0: 6665 6174 7572 6573 3a20 4d61 7869 6d75  features: Maximu
+00000e00: 6d20 6e75 6d62 6572 206f 6620 6465 7065  m number of depe
+00000e10: 6e64 656e 6365 2070 6c6f 7473 2074 6f20  ndence plots to 
+00000e20: 7368 6f77 2e20 4e6f 7420 7573 6564 2077  show. Not used w
+00000e30: 6865 6e20 6375 7374 6f6d 204d 4c0a 2020  hen custom ML.  
+00000e40: 2020 2020 2020 6d6f 6465 6c20 6973 2070        model is p
+00000e50: 6173 7365 642e 0a20 2020 203a 7061 7261  assed..    :para
+00000e60: 6d20 7374 6f72 655f 7368 6170 5f76 616c  m store_shap_val
+00000e70: 7565 735f 696e 5f69 6e73 7461 6e63 653a  ues_in_instance:
+00000e80: 2057 6865 7468 6572 2074 6f20 7374 6f72   Whether to stor
+00000e90: 6520 7468 6520 5348 4150 2076 616c 7565  e the SHAP value
+00000ea0: 7320 696e 2074 6865 2042 6c75 6543 6173  s in the BlueCas
+00000eb0: 7420 696e 7374 616e 6365 2e20 4e6f 7420  t instance. Not 
+00000ec0: 6170 706c 6963 6162 6c65 2077 6865 6e0a  applicable when.
+00000ed0: 2020 2020 2020 2020 6375 7374 6f6d 204d          custom M
+00000ee0: 4c20 6d6f 6465 6c20 6973 2075 7365 642e  L model is used.
+00000ef0: 0a20 2020 203a 7061 7261 6d20 7472 6169  .    :param trai
+00000f00: 6e5f 7369 7a65 3a20 5472 6169 6e20 7369  n_size: Train si
+00000f10: 7a65 2074 6f20 7573 6520 666f 7220 7472  ze to use for tr
+00000f20: 6169 6e2d 7465 7374 2073 706c 6974 2e0a  ain-test split..
+00000f30: 2020 2020 3a70 6172 616d 2074 7261 696e      :param train
+00000f40: 5f73 706c 6974 5f73 7472 6174 6966 793a  _split_stratify:
+00000f50: 2057 6865 7468 6572 2074 6f20 7374 7261   Whether to stra
+00000f60: 7469 6679 2074 6865 2074 7261 696e 2d74  tify the train-t
+00000f70: 6573 7420 7370 6c69 742e 204e 6f74 2075  est split. Not u
+00000f80: 7365 6420 7768 656e 2063 7573 746f 6d20  sed when custom 
+00000f90: 4d4c 206d 6f64 656c 2069 7320 7061 7373  ML model is pass
+00000fa0: 6564 2e0a 2020 2020 3a70 6172 616d 2075  ed..    :param u
+00000fb0: 7365 5f66 756c 6c5f 6461 7461 5f66 6f72  se_full_data_for
+00000fc0: 5f66 696e 616c 5f6d 6f64 656c 3a20 5768  _final_model: Wh
+00000fd0: 6574 6865 7220 746f 2075 7365 2074 6865  ether to use the
+00000fe0: 2066 756c 6c20 6461 7461 2066 6f72 2074   full data for t
+00000ff0: 6865 2066 696e 616c 206d 6f64 656c 2e20  he final model. 
+00001000: 5468 6973 206d 6967 6874 2063 6175 7365  This might cause
+00001010: 206f 7665 7266 6974 7469 6e67 2e0a 2020   overfitting..  
+00001020: 2020 2020 2020 4e6f 7420 7573 6564 2077        Not used w
+00001030: 6865 6e20 6375 7374 6f6d 204d 4c20 6d6f  hen custom ML mo
+00001040: 6465 6c20 6973 2070 6173 7365 642e 0a20  del is passed.. 
+00001050: 2020 203a 7061 7261 6d20 6d69 6e5f 6665     :param min_fe
+00001060: 6174 7572 6573 5f74 6f5f 7365 6c65 6374  atures_to_select
+00001070: 3a20 4d69 6e69 6d75 6d20 6e75 6d62 6572  : Minimum number
+00001080: 206f 6620 6665 6174 7572 6573 2074 6f20   of features to 
+00001090: 7365 6c65 6374 2e20 4f6e 6c79 2075 7365  select. Only use
+000010a0: 6420 7768 656e 2065 6e61 626c 655f 6665  d when enable_fe
+000010b0: 6174 7572 655f 7365 6c65 6374 696f 6e20  ature_selection 
+000010c0: 6973 0a20 2020 2020 2020 2054 7275 652e  is.        True.
+000010d0: 0a20 2020 203a 7061 7261 6d20 6361 7264  .    :param card
+000010e0: 696e 616c 6974 795f 7468 7265 7368 6f6c  inality_threshol
+000010f0: 645f 666f 725f 6f6e 6568 6f74 5f65 6e63  d_for_onehot_enc
+00001100: 6f64 696e 673a 2043 6174 6567 6f72 6963  oding: Categoric
+00001110: 616c 2066 6561 7475 7265 7320 7769 7468  al features with
+00001120: 2061 2063 6172 6469 6e61 6c69 7479 206f   a cardinality o
+00001130: 6620 6c65 7373 206f 7220 6571 7561 6c0a  f less or equal.
+00001140: 2020 2020 2020 2020 7468 6973 2074 6872          this thr
+00001150: 6573 686f 6c64 2077 696c 6c20 6265 206f  eshold will be o
+00001160: 6e65 686f 7420 656e 636f 6465 642e 2054  nehot encoded. T
+00001170: 6865 2072 6573 7420 7769 6c6c 2062 6520  he rest will be 
+00001180: 7461 7267 6574 2065 6e63 6f64 6564 2e20  target encoded. 
+00001190: 5769 6c6c 2062 6520 6967 6e6f 7265 6420  Will be ignored 
+000011a0: 6966 0a20 2020 2020 2020 2063 6174 5f65  if.        cat_e
+000011b0: 6e63 6f64 696e 675f 7669 615f 6d6c 5f61  ncoding_via_ml_a
+000011c0: 6c67 6f72 6974 686d 2069 7320 7365 7420  lgorithm is set 
+000011d0: 746f 2074 7275 652e 0a20 2020 203a 7061  to true..    :pa
+000011e0: 7261 6d20 6361 745f 656e 636f 6469 6e67  ram cat_encoding
+000011f0: 5f76 6961 5f6d 6c5f 616c 676f 7269 7468  _via_ml_algorith
+00001200: 6d3a 2057 6865 7468 6572 2074 6f20 7573  m: Whether to us
+00001210: 6520 616e 204d 4c20 616c 676f 7269 7468  e an ML algorith
+00001220: 6d20 666f 7220 6361 7465 676f 7269 6361  m for categorica
+00001230: 6c20 656e 636f 6469 6e67 2e20 4966 2054  l encoding. If T
+00001240: 7275 652c 2074 6865 0a20 2020 2020 2020  rue, the.       
+00001250: 2063 6174 6567 6f72 6963 616c 2065 6e63   categorical enc
+00001260: 6f64 696e 6720 6973 2064 6f6e 6520 7669  oding is done vi
+00001270: 6120 6120 4d4c 2061 6c67 6f72 6974 686d  a a ML algorithm
+00001280: 2e20 4966 2046 616c 7365 2c20 7468 6520  . If False, the 
+00001290: 6361 7465 676f 7269 6361 6c20 656e 636f  categorical enco
+000012a0: 6469 6e67 2069 7320 646f 6e65 2076 6961  ding is done via
+000012b0: 2061 2020 7461 7267 6574 0a20 2020 2020   a  target.     
+000012c0: 2020 2065 6e63 6f64 696e 6720 696e 2074     encoding in t
+000012d0: 6865 2070 7265 7072 6f63 6573 7369 6e67  he preprocessing
+000012e0: 2073 7465 7073 2e20 5365 6520 7468 6520   steps. See the 
+000012f0: 5265 6164 4d65 2066 6f72 206d 6f72 6520  ReadMe for more 
+00001300: 6465 7461 696c 732e 0a20 2020 203a 7061  details..    :pa
+00001310: 7261 6d20 7368 6f77 5f64 6574 6169 6c65  ram show_detaile
+00001320: 645f 7475 6e69 6e67 5f6c 6f67 733a 2057  d_tuning_logs: W
+00001330: 6865 7468 6572 2074 6f20 7368 6f77 2064  hether to show d
+00001340: 6574 6169 6c65 6420 7475 6e69 6e67 206c  etailed tuning l
+00001350: 6f67 732e 204e 6f74 2075 7365 6420 7768  ogs. Not used wh
+00001360: 656e 2063 7573 746f 6d20 4d4c 206d 6f64  en custom ML mod
+00001370: 656c 2069 7320 7061 7373 6564 2e0a 2020  el is passed..  
+00001380: 2020 3a70 6172 616d 2065 6e61 626c 655f    :param enable_
+00001390: 6772 6964 5f73 6561 7263 685f 6669 6e65  grid_search_fine
+000013a0: 5f74 756e 696e 673a 2041 6674 6572 2068  _tuning: After h
+000013b0: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
+000013c0: 6e69 6e67 2072 756e 2047 7269 6473 6561  ning run Gridsea
+000013d0: 7263 6820 7475 6e69 6e67 206f 6e20 6120  rch tuning on a 
+000013e0: 6669 6e65 2d67 7261 696e 6564 2067 7269  fine-grained gri
+000013f0: 640a 2020 2020 2020 2020 6261 7365 6420  d.        based 
+00001400: 6f6e 2074 6865 2070 7265 7669 6f75 7320  on the previous 
+00001410: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
+00001420: 756e 696e 672e 204f 6e6c 7920 706f 7373  uning. Only poss
+00001430: 6962 6c65 2077 6865 6e20 6175 746f 7475  ible when autotu
+00001440: 6e65 5f6d 6f64 656c 2069 7320 5472 7565  ne_model is True
+00001450: 2e0a 2020 2020 3a70 6172 616d 2067 7269  ..    :param gri
+00001460: 6473 6561 7263 685f 6e62 5f70 6172 616d  dsearch_nb_param
+00001470: 6574 6572 735f 7065 725f 6772 6964 3a20  eters_per_grid: 
+00001480: 4465 6369 6465 7320 686f 7720 6d61 6e79  Decides how many
+00001490: 2073 7465 7073 2074 6865 2067 7269 6420   steps the grid 
+000014a0: 7368 616c 6c20 6861 7665 2070 6572 2070  shall have per p
+000014b0: 6172 616d 6574 6572 2e0a 2020 2020 3a70  arameter..    :p
+000014c0: 6172 616d 2067 7269 6473 6561 7263 685f  aram gridsearch_
+000014d0: 7475 6e69 6e67 5f6d 6178 5f72 756e 7469  tuning_max_runti
+000014e0: 6d65 5f73 6563 733a 2053 6574 7320 7468  me_secs: Sets th
+000014f0: 6520 6d61 7869 6d75 6d20 7469 6d65 2069  e maximum time i
+00001500: 6e20 7365 636f 6e64 7320 7468 6520 7475  n seconds the tu
+00001510: 6e69 6e67 2073 6861 6c6c 2072 756e 2e20  ning shall run. 
+00001520: 5468 6973 2077 696c 6c20 6669 6e69 7368  This will finish
+00001530: 0a20 2020 2020 2020 2074 6865 206c 6174  .        the lat
+00001540: 6573 7420 7472 6961 6c20 6e64 2077 696c  est trial nd wil
+00001550: 6c20 6578 6365 6564 2074 6869 7320 6c69  l exceed this li
+00001560: 6d69 7420 7468 6f75 6768 2e0a 2020 2020  mit though..    
+00001570: 3a70 6172 616d 2065 7870 6572 696d 656e  :param experimen
+00001580: 745f 6e61 6d65 3a20 4e61 6d65 206f 6620  t_name: Name of 
+00001590: 7468 6520 6578 7065 7269 6d65 6e74 2e20  the experiment. 
+000015a0: 5769 6c6c 2062 6520 6c6f 6767 6564 2069  Will be logged i
+000015b0: 6e73 6964 6520 7468 6520 4578 7065 7269  nside the Experi
+000015c0: 6d65 6e74 5472 6163 6b65 722e 0a20 2020  mentTracker..   
+000015d0: 20e9 0a00 0000 da13 676c 6f62 616c 5f72   .......global_r
+000015e0: 616e 646f 6d5f 7374 6174 65e9 2100 0000  andom_state.!...
+000015f0: da27 696e 6372 6561 7365 5f72 616e 646f  .'increase_rando
+00001600: 6d5f 7374 6174 655f 696e 5f62 6c75 6563  m_state_in_bluec
+00001610: 6173 745f 6376 5f62 7954 da17 7368 7566  ast_cv_byT..shuf
+00001620: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
+00001630: 696e 67e9 c800 0000 da1c 6879 7065 7270  ing.......hyperp
+00001640: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
+00001650: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
+00001660: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
+00001670: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
+00001680: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
+00001690: 756e 696e 675f 6376 5f66 6f6c 6473 46da  uning_cv_foldsF.
+000016a0: 1973 616d 706c 655f 6461 7461 5f64 7572  .sample_data_dur
+000016b0: 696e 675f 7475 6e69 6e67 e79a 9999 9999  ing_tuning......
+000016c0: 99b9 3fda 1f73 616d 706c 655f 6461 7461  ..?..sample_data
+000016d0: 5f64 7572 696e 675f 7475 6e69 6e67 5f61  _during_tuning_a
+000016e0: 6c70 6861 da11 7072 6563 6973 655f 6376  lpha..precise_cv
+000016f0: 5f74 756e 696e 674e da15 6561 726c 795f  _tuningN..early_
+00001700: 7374 6f70 7069 6e67 5f72 6f75 6e64 73da  stopping_rounds.
+00001710: 0e61 7574 6f74 756e 655f 6d6f 6465 6cda  .autotune_model.
+00001720: 1865 6e61 626c 655f 6665 6174 7572 655f  .enable_feature_
+00001730: 7365 6c65 6374 696f 6eda 1563 616c 6375  selection..calcu
+00001740: 6c61 7465 5f73 6861 705f 7661 6c75 6573  late_shap_values
+00001750: 7201 0000 00da 1673 6861 705f 7761 7465  r......shap_wate
+00001760: 7266 616c 6c5f 696e 6469 6365 73da 2773  rfall_indices.'s
+00001770: 686f 775f 6465 7065 6e64 656e 6365 5f70  how_dependence_p
+00001780: 6c6f 7473 5f6f 665f 746f 705f 6e5f 6665  lots_of_top_n_fe
+00001790: 6174 7572 6573 da1d 7374 6f72 655f 7368  atures..store_sh
+000017a0: 6170 5f76 616c 7565 735f 696e 5f69 6e73  ap_values_in_ins
+000017b0: 7461 6e63 65e7 9a99 9999 9999 e93f da0a  tance........?..
+000017c0: 7472 6169 6e5f 7369 7a65 da14 7472 6169  train_size..trai
+000017d0: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
+000017e0: da1d 7573 655f 6675 6c6c 5f64 6174 615f  ..use_full_data_
+000017f0: 666f 725f 6669 6e61 6c5f 6d6f 6465 6ce9  for_final_model.
+00001800: 0500 0000 da16 6d69 6e5f 6665 6174 7572  ......min_featur
+00001810: 6573 5f74 6f5f 7365 6c65 6374 da29 6361  es_to_select.)ca
+00001820: 7264 696e 616c 6974 795f 7468 7265 7368  rdinality_thresh
+00001830: 6f6c 645f 666f 725f 6f6e 6568 6f74 5f65  old_for_onehot_e
+00001840: 6e63 6f64 696e 67da 1d63 6174 5f65 6e63  ncoding..cat_enc
+00001850: 6f64 696e 675f 7669 615f 6d6c 5f61 6c67  oding_via_ml_alg
+00001860: 6f72 6974 686d da19 7368 6f77 5f64 6574  orithm..show_det
+00001870: 6169 6c65 645f 7475 6e69 6e67 5f6c 6f67  ailed_tuning_log
+00001880: 73da 1f6f 7074 756e 615f 7361 6d70 6c65  s..optuna_sample
+00001890: 725f 6e5f 7374 6172 7475 705f 7472 6961  r_n_startup_tria
+000018a0: 6c73 da1e 656e 6162 6c65 5f67 7269 645f  ls..enable_grid_
+000018b0: 7365 6172 6368 5f66 696e 655f 7475 6e69  search_fine_tuni
+000018c0: 6e67 da22 6772 6964 7365 6172 6368 5f74  ng."gridsearch_t
+000018d0: 756e 696e 675f 6d61 785f 7275 6e74 696d  uning_max_runtim
+000018e0: 655f 7365 6373 da21 6772 6964 7365 6172  e_secs.!gridsear
+000018f0: 6368 5f6e 625f 7061 7261 6d65 7465 7273  ch_nb_parameters
+00001900: 5f70 6572 5f67 7269 647a 0e6e 6577 2065  _per_gridz.new e
+00001910: 7870 6572 696d 656e 74da 0f65 7870 6572  xperiment..exper
+00001920: 696d 656e 745f 6e61 6d65 2927 7208 0000  iment_name)'r...
+00001930: 0072 0900 0000 720a 0000 00da 075f 5f64  .r....r......__d
+00001940: 6f63 5f5f 720f 0000 00da 0369 6e74 da0f  oc__r......int..
+00001950: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00001960: 1100 0000 7212 0000 00da 0462 6f6f 6c72  ....r......boolr
+00001970: 1400 0000 7215 0000 0072 1700 0000 7218  ....r....r....r.
+00001980: 0000 0072 1a00 0000 da05 666c 6f61 7472  ...r......floatr
+00001990: 1b00 0000 721c 0000 0072 0400 0000 721d  ....r....r....r.
+000019a0: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+000019b0: 0000 7203 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
+000019c0: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+000019d0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+000019e0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+000019f0: 0000 0072 2f00 0000 7230 0000 00da 0373  ...r/...r0.....s
+00001a00: 7472 720b 0000 0072 0b00 0000 720b 0000  trr....r....r...
+00001a10: 0072 0c00 0000 720d 0000 0013 0000 0073  .r....r........s
+00001a20: 3c00 0000 0a00 0401 0c31 0c01 0c01 0c01  <........1......
+00001a30: 0c01 0c01 0c01 0c01 0c01 1001 0c01 0c01  ................
+00001a40: 0c01 1201 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001a50: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1001  ................
+00001a60: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001a70: 0000 0000 0000 0300 0000 4000 0000 7356  ..........@...sV
+00001a80: 0100 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00001a90: 0364 025a 0465 0565 0664 033c 0064 045a  .d.Z.e.e.d.<.d.Z
+00001aa0: 0765 0565 0664 053c 0064 065a 0865 0965  .e.e.d.<.d.Z.e.e
+00001ab0: 0664 073c 0064 085a 0a65 0965 0664 093c  .d.<.d.Z.e.e.d.<
+00001ac0: 0064 065a 0b65 0965 0664 0a3c 0064 085a  .d.Z.e.e.d.<.d.Z
+00001ad0: 0c65 0965 0664 0b3c 0064 065a 0d65 0965  .e.e.d.<.d.Z.e.e
+00001ae0: 0664 0c3c 0064 065a 0e65 0965 0664 0d3c  .d.<.d.Z.e.e.d.<
+00001af0: 0064 0e5a 0f65 0965 0664 0f3c 0064 105a  .d.Z.e.e.d.<.d.Z
+00001b00: 1065 0965 0664 113c 0064 125a 1165 0565  .e.e.d.<.d.Z.e.e
+00001b10: 0664 133c 0064 145a 1265 0565 0664 153c  .d.<.d.Z.e.e.d.<
+00001b20: 0064 165a 1365 0965 0664 173c 0064 105a  .d.Z.e.e.d.<.d.Z
+00001b30: 1465 0965 0664 183c 0064 165a 1565 0965  .e.e.d.<.d.Z.e.e
+00001b40: 0664 193c 0064 105a 1665 0965 0664 1a3c  .d.<.d.Z.e.e.d.<
+00001b50: 0064 105a 1765 0965 0664 1b3c 0064 105a  .d.Z.e.e.d.<.d.Z
+00001b60: 1865 0965 0664 1c3c 0064 1d5a 1965 0965  .e.e.d.<.d.Z.e.e
+00001b70: 0664 1e3c 0064 165a 1a65 0965 0664 1f3c  .d.<.d.Z.e.e.d.<
+00001b80: 0064 205a 1b65 0565 0664 213c 0064 225a  .d Z.e.e.d!<.d"Z
+00001b90: 1c65 0565 0664 233c 0064 245a 1d65 0565  .e.e.d#<.d$Z.e.e
+00001ba0: 0664 253c 0064 245a 1e65 0565 0664 263c  .d%<.d$Z.e.e.d&<
+00001bb0: 0064 275a 1f65 2065 0664 283c 0064 295a  .d'Z.e e.d(<.d)Z
+00001bc0: 2165 2065 0664 2a3c 0064 2b5a 2265 2065  !e e.d*<.d+Z"e e
+00001bd0: 0664 2c3c 0064 2d53 0029 2eda 1758 6762  .d,<.d-S.)...Xgb
+00001be0: 6f6f 7374 5475 6e65 5061 7261 6d73 436f  oostTuneParamsCo
+00001bf0: 6e66 6967 fa2a 4465 6669 6e65 2068 7970  nfig.*Define hyp
+00001c00: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
+00001c10: 6e67 2073 6561 7263 6820 7370 6163 652e  ng search space.
+00001c20: e902 0000 00da 0d6d 6178 5f64 6570 7468  .......max_depth
+00001c30: 5f6d 696e e90c 0000 00da 0d6d 6178 5f64  _min.......max_d
+00001c40: 6570 7468 5f6d 6178 e73a 8c30 e28e 7945  epth_max.:.0..yE
+00001c50: 3eda 0961 6c70 6861 5f6d 696e e700 0000  >..alpha_min....
+00001c60: 0000 0024 40da 0961 6c70 6861 5f6d 6178  ...$@..alpha_max
+00001c70: da0a 6c61 6d62 6461 5f6d 696e da0a 6c61  ..lambda_min..la
+00001c80: 6d62 6461 5f6d 6178 da09 6761 6d6d 615f  mbda_max..gamma_
+00001c90: 6d69 6eda 0967 616d 6d61 5f6d 6178 e700  min..gamma_max..
+00001ca0: 0000 0000 0000 00da 0d73 7562 7361 6d70  .........subsamp
+00001cb0: 6c65 5f6d 696e e700 0000 0000 00f0 3fda  le_min........?.
+00001cc0: 0d73 7562 7361 6d70 6c65 5f6d 6178 7216  .subsample_maxr.
+00001cd0: 0000 00da 146d 696e 5f63 6869 6c64 5f77  .....min_child_w
+00001ce0: 6569 6768 745f 6d69 6e72 0e00 0000 da14  eight_minr......
+00001cf0: 6d69 6e5f 6368 696c 645f 7765 6967 6874  min_child_weight
+00001d00: 5f6d 6178 e733 3333 3333 33d3 3fda 0e73  _max.333333.?..s
+00001d10: 7562 5f73 616d 706c 655f 6d69 6eda 0e73  ub_sample_min..s
+00001d20: 7562 5f73 616d 706c 655f 6d61 78da 1663  ub_sample_max..c
+00001d30: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
+00001d40: 655f 6d69 6eda 1663 6f6c 5f73 616d 706c  e_min..col_sampl
+00001d50: 655f 6279 5f74 7265 655f 6d61 78da 1763  e_by_tree_max..c
+00001d60: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
+00001d70: 656c 5f6d 696e da17 636f 6c5f 7361 6d70  el_min..col_samp
+00001d80: 6c65 5f62 795f 6c65 7665 6c5f 6d61 78e7  le_by_level_max.
+00001d90: fca9 f1d2 4d62 503f da07 6574 615f 6d69  ....MbP?..eta_mi
+00001da0: 6eda 0765 7461 5f6d 6178 e932 0000 00da  n..eta_max.2....
+00001db0: 0973 7465 7073 5f6d 696e e9e8 0300 00da  .steps_min......
+00001dc0: 0973 7465 7073 5f6d 6178 7201 0000 00da  .steps_maxr.....
+00001dd0: 2676 6572 626f 7369 7479 5f64 7572 696e  &verbosity_durin
+00001de0: 675f 6879 7065 7270 6172 616d 6574 6572  g_hyperparameter
+00001df0: 5f74 756e 696e 67da 2576 6572 626f 7369  _tuning.%verbosi
+00001e00: 7479 5f64 7572 696e 675f 6669 6e61 6c5f  ty_during_final_
+00001e10: 6d6f 6465 6c5f 7472 6169 6e69 6e67 7a0e  model_trainingz.
+00001e20: 6d75 6c74 693a 736f 6674 7072 6f62 da11  multi:softprob..
+00001e30: 7867 626f 6f73 745f 6f62 6a65 6374 6976  xgboost_objectiv
+00001e40: 65da 086d 6c6f 676c 6f73 73da 1378 6762  e..mlogloss..xgb
+00001e50: 6f6f 7374 5f65 7661 6c5f 6d65 7472 6963  oost_eval_metric
+00001e60: da06 6762 7472 6565 da07 626f 6f73 7465  ..gbtree..booste
+00001e70: 724e a923 7208 0000 0072 0900 0000 720a  rN.#r....r....r.
+00001e80: 0000 0072 3100 0000 723a 0000 0072 3200  ...r1...r:...r2.
+00001e90: 0000 7233 0000 0072 3c00 0000 723e 0000  ..r3...r<...r>..
+00001ea0: 0072 3500 0000 7240 0000 0072 4100 0000  .r5...r@...rA...
+00001eb0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+00001ec0: 4600 0000 7248 0000 0072 4900 0000 724a  F...rH...rI...rJ
+00001ed0: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
+00001ee0: 0000 724f 0000 0072 5000 0000 7251 0000  ..rO...rP...rQ..
+00001ef0: 0072 5300 0000 7254 0000 0072 5600 0000  .rS...rT...rV...
+00001f00: 7258 0000 0072 5900 0000 725a 0000 0072  rX...rY...rZ...r
+00001f10: 5b00 0000 7236 0000 0072 5d00 0000 725f  [...r6...r]...r_
+00001f20: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00001f30: 0000 720c 0000 0072 3700 0000 6300 0000  ..r....r7...c...
+00001f40: f33a 0000 000a 0004 010c 020c 010c 010c  .:..............
+00001f50: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001f60: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001f70: 010c 010c 010c 010c 010c 010c 0110 0172  ...............r
+00001f80: 3700 0000 6300 0000 0000 0000 0000 0000  7...c...........
+00001f90: 0000 0000 0003 0000 0040 0000 0073 5601  .........@...sV.
+00001fa0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00001fb0: 6402 5a04 6505 6506 6403 3c00 6404 5a07  d.Z.e.e.d.<.d.Z.
+00001fc0: 6505 6506 6405 3c00 6406 5a08 6509 6506  e.e.d.<.d.Z.e.e.
+00001fd0: 6407 3c00 6408 5a0a 6509 6506 6409 3c00  d.<.d.Z.e.e.d.<.
+00001fe0: 6406 5a0b 6509 6506 640a 3c00 6408 5a0c  d.Z.e.e.d.<.d.Z.
+00001ff0: 6509 6506 640b 3c00 6406 5a0d 6509 6506  e.e.d.<.d.Z.e.e.
+00002000: 640c 3c00 6408 5a0e 6509 6506 640d 3c00  d.<.d.Z.e.e.d.<.
+00002010: 640e 5a0f 6509 6506 640f 3c00 6410 5a10  d.Z.e.e.d.<.d.Z.
+00002020: 6509 6506 6411 3c00 6412 5a11 6505 6506  e.e.d.<.d.Z.e.e.
+00002030: 6413 3c00 6412 5a12 6505 6506 6414 3c00  d.<.d.Z.e.e.d.<.
+00002040: 6415 5a13 6509 6506 6416 3c00 6410 5a14  d.Z.e.e.d.<.d.Z.
+00002050: 6509 6506 6417 3c00 6415 5a15 6509 6506  e.e.d.<.d.Z.e.e.
+00002060: 6418 3c00 6410 5a16 6509 6506 6419 3c00  d.<.d.Z.e.e.d.<.
+00002070: 6410 5a17 6509 6506 641a 3c00 6410 5a18  d.Z.e.e.d.<.d.Z.
+00002080: 6509 6506 641b 3c00 641c 5a19 6509 6506  e.e.d.<.d.Z.e.e.
+00002090: 641d 3c00 6415 5a1a 6509 6506 641e 3c00  d.<.d.Z.e.e.d.<.
+000020a0: 6402 5a1b 6505 6506 641f 3c00 6420 5a1c  d.Z.e.e.d.<.d Z.
+000020b0: 6505 6506 6421 3c00 6422 5a1d 6505 6506  e.e.d!<.d"Z.e.e.
+000020c0: 6423 3c00 6422 5a1e 6505 6506 6424 3c00  d#<.d"Z.e.e.d$<.
+000020d0: 6425 5a1f 6520 6506 6426 3c00 6427 5a21  d%Z.e e.d&<.d'Z!
+000020e0: 6520 6506 6428 3c00 6429 5a22 6520 6506  e e.d(<.d)Z"e e.
+000020f0: 642a 3c00 642b 5300 292c da21 5867 626f  d*<.d+S.),.!Xgbo
+00002100: 6f73 7454 756e 6550 6172 616d 7352 6567  ostTuneParamsReg
+00002110: 7265 7373 696f 6e43 6f6e 6669 6772 3800  ressionConfigr8.
+00002120: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
+00002130: 0072 3c00 0000 723d 0000 0072 3e00 0000  .r<...r=...r>...
+00002140: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
+00002150: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
+00002160: 0000 0072 4600 0000 7247 0000 0072 4800  ...rF...rG...rH.
+00002170: 0000 7216 0000 0072 4900 0000 724a 0000  ..r....rI...rJ..
+00002180: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
+00002190: 724e 0000 0072 4f00 0000 7250 0000 0072  rN...rO...rP...r
+000021a0: 5100 0000 7252 0000 0072 5300 0000 7254  Q...rR...rS...rT
+000021b0: 0000 0072 5600 0000 7257 0000 0072 5800  ...rV...rW...rX.
+000021c0: 0000 7201 0000 0072 5900 0000 725a 0000  ..r....rY...rZ..
+000021d0: 007a 1072 6567 3a73 7175 6172 6564 6572  .z.reg:squareder
+000021e0: 726f 7272 5b00 0000 5a04 726d 7365 725d  rorr[...Z.rmser]
+000021f0: 0000 0072 5e00 0000 725f 0000 004e 7260  ...r^...r_...Nr`
+00002200: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00002210: 0000 720c 0000 0072 6200 0000 8300 0000  ..r....rb.......
+00002220: 7261 0000 0072 6200 0000 6300 0000 0000  ra...rb...c.....
+00002230: 0000 0000 0000 0000 0000 000c 0000 0040  ...............@
+00002240: 0000 0073 5200 0000 6500 5a01 6400 5a02  ...sR...e.Z.d.Z.
+00002250: 5500 6401 5a03 6402 6403 6404 6404 6405  U.d.Z.d.d.d.d.d.
+00002260: 6406 6407 6408 6408 6404 6409 640a 9c0b  d.d.d.d.d.d.d...
+00002270: 5a04 640b 5a05 6506 6507 6508 6509 6602  Z.d.Z.e.e.e.e.f.
+00002280: 1900 1900 650a 640c 3c00 640d 5a0b 6509  ....e.d.<.d.Z.e.
+00002290: 650a 640e 3c00 640b 5300 290f da17 5867  e.d.<.d.S.)...Xg
+000022a0: 626f 6f73 7446 696e 616c 5061 7261 6d43  boostFinalParamC
+000022b0: 6f6e 6669 677a 1e44 6566 696e 6520 6669  onfigz.Define fi
+000022c0: 6e61 6c20 6879 7065 7220 7061 7261 6d65  nal hyper parame
+000022d0: 7465 7273 2e72 5e00 0000 e907 0000 0072  ters.r^........r
+000022e0: 1900 0000 7245 0000 0072 4700 0000 7216  ....rE...rG...r.
+000022f0: 0000 0072 2300 0000 7257 0000 0029 0b72  ...r#...rW...).r
+00002300: 5f00 0000 da09 6d61 785f 6465 7074 68da  _.....max_depth.
+00002310: 0561 6c70 6861 da06 6c61 6d62 6461 da05  .alpha..lambda..
+00002320: 6761 6d6d 615a 0973 7562 7361 6d70 6c65  gammaZ.subsample
+00002330: 5a10 6d69 6e5f 6368 696c 645f 7765 6967  Z.min_child_weig
+00002340: 6874 5a10 636f 6c73 616d 706c 655f 6279  htZ.colsample_by
+00002350: 7472 6565 5a11 636f 6c73 616d 706c 655f  treeZ.colsample_
+00002360: 6279 6c65 7665 6cda 0365 7461 5a05 7374  bylevel..etaZ.st
+00002370: 6570 734e da0d 7361 6d70 6c65 5f77 6569  epsN..sample_wei
+00002380: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
+00002390: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
+000023a0: 6573 686f 6c64 290c 7208 0000 0072 0900  eshold).r....r..
+000023b0: 0000 720a 0000 0072 3100 0000 da06 7061  ..r....r1.....pa
+000023c0: 7261 6d73 726a 0000 0072 0400 0000 7202  ramsrj...r....r.
+000023d0: 0000 0072 3600 0000 7235 0000 0072 3300  ...r6...r5...r3.
+000023e0: 0000 726b 0000 0072 0b00 0000 720b 0000  ..rk...r....r...
+000023f0: 0072 0b00 0000 720c 0000 0072 6300 0000  .r....r....rc...
+00002400: a300 0000 7320 0000 000a 0004 0202 0302  ....s ..........
+00002410: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00002420: 0102 0106 f518 0d10 0172 6300 0000 4e29  .........rc...N)
+00002430: 0e72 3100 0000 da06 7479 7069 6e67 7202  .r1.....typingr.
+00002440: 0000 0072 0300 0000 7204 0000 005a 0870  ...r....r....Z.p
+00002450: 7964 616e 7469 6372 0500 0000 5a14 7079  ydanticr....Z.py
+00002460: 6461 6e74 6963 2e64 6174 6163 6c61 7373  dantic.dataclass
+00002470: 6573 7206 0000 0072 0700 0000 720d 0000  esr....r....r...
+00002480: 0072 3700 0000 7262 0000 0072 6300 0000  .r7...rb...rc...
+00002490: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+000024a0: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000024b0: 0000 7314 0000 0004 0014 080c 020c 010e  ..s.............
+000024c0: 0310 0410 5010 2002 2014 01              ....P. . ..
```

### Comparing `bluecast-1.1/bluecast/config/__pycache__/training_config.cpython-38.pyc` & `bluecast-1.2.4/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/config/base_classes.py` & `bluecast-1.2.4/bluecast/config/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/config/training_config.py` & `bluecast-1.2.4/bluecast/config/training_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         random state changes with each additional model.
     :param shuffle_during_training: Whether to shuffle the data during training when hypertuning_cv_folds > 1.
     :param hyperparameter_tuning_rounds: Number of hyperparameter tuning rounds. Not used when custom ML model is passed.
     :param hyperparameter_tuning_max_runtime_secs: Maximum runtime in seconds for hyperparameter tuning. Not used when
         custom ML model is passed.
     :param hypertuning_cv_folds: Number of cross-validation folds to use for hyperparameter tuning. Not used when
         custom ML model is passed.
+    :param sample_data_during_tuning: Whether to sample the data during tuning. Not used when custom ML model is passed.
+    :param sample_data_during_tuning_alpha: Alpha value for sampling the data during tuning. The higher alpha the
+        fewer samples will be left. Not used when custom ML model is passed.
     :param precise_cv_tuning: If enabled will switch from using Xgboost's own cv method to a custom cross validation
         routine. This is needed when the in-fold preprocessing is necessary that would cause overfitting with usual cv.
         This has a much longer runtime as Optuna's pruning call is missing and all trials will run until the end.
     :param early_stopping_rounds: Number of early stopping rounds. Not used when custom ML model is passed. Also
         not used when hypertuning_cv_folds is greater than 1.
     :param autotune_model: Whether to autotune the model. Not used when custom ML model is passed.
     :param enable_feature_selection: Whether to enable recursive feature selection.
@@ -65,25 +68,27 @@
 
     global_random_state: int = 10
     increase_random_state_in_bluecast_cv_by: int = 33
     shuffle_during_training: bool = True
     hyperparameter_tuning_rounds: int = 200
     hyperparameter_tuning_max_runtime_secs: int = 3600
     hypertuning_cv_folds: int = 1
+    sample_data_during_tuning: bool = False
+    sample_data_during_tuning_alpha: float = 0.1
     precise_cv_tuning: bool = False
     early_stopping_rounds: Optional[int] = None
     autotune_model: bool = True
     enable_feature_selection: bool = False
     calculate_shap_values: bool = True
     shap_waterfall_indices: List[int] = [0]
     show_dependence_plots_of_top_n_features: int = 1
     store_shap_values_in_instance: bool = False
     train_size: float = 0.8
     train_split_stratify: bool = True
-    use_full_data_for_final_model: bool = False
+    use_full_data_for_final_model: bool = True
     min_features_to_select: int = 5
     cardinality_threshold_for_onehot_encoding: int = 5
     cat_encoding_via_ml_algorithm: bool = False
     show_detailed_tuning_logs: bool = False
     optuna_sampler_n_startup_trials: int = 10
     enable_grid_search_fine_tuning: bool = False
     gridsearch_tuning_max_runtime_secs: int = 3600
@@ -99,22 +104,22 @@
     alpha_min: float = 1e-8
     alpha_max: float = 10.0
     lambda_min: float = 1e-8
     lambda_max: float = 10.0
     gamma_min: float = 1e-8
     gamma_max: float = 10.0
     subsample_min: float = 0.0
-    subsample_max: float = 10.0
-    max_leaves_min: int = 0
-    max_leaves_max: int = 0
+    subsample_max: float = 1.0
+    min_child_weight_min: int = 1
+    min_child_weight_max: int = 1
     sub_sample_min: float = 0.3
     sub_sample_max: float = 1.0
     col_sample_by_tree_min: float = 0.3
     col_sample_by_tree_max: float = 1.0
-    col_sample_by_level_min: float = 0.3
+    col_sample_by_level_min: float = 1.0
     col_sample_by_level_max: float = 1.0
     eta_min: float = 0.001
     eta_max: float = 0.3
     steps_min: int = 50
     steps_max: int = 1000
     verbosity_during_hyperparameter_tuning: int = 0
     verbosity_during_final_model_training: int = 0
@@ -131,22 +136,22 @@
     alpha_min: float = 1e-8
     alpha_max: float = 10.0
     lambda_min: float = 1e-8
     lambda_max: float = 10.0
     gamma_min: float = 1e-8
     gamma_max: float = 10.0
     subsample_min: float = 0.0
-    subsample_max: float = 10.0
-    max_leaves_min: int = 0
-    max_leaves_max: int = 0
+    subsample_max: float = 1.0
+    min_child_weight_min: int = 1
+    min_child_weight_max: int = 1
     sub_sample_min: float = 0.3
     sub_sample_max: float = 1.0
     col_sample_by_tree_min: float = 0.3
     col_sample_by_tree_max: float = 1.0
-    col_sample_by_level_min: float = 0.3
+    col_sample_by_level_min: float = 1.0
     col_sample_by_level_max: float = 1.0
     eta_min: float = 0.001
     eta_max: float = 0.3
     steps_min: int = 2
     steps_max: int = 1000
     verbosity_during_hyperparameter_tuning: int = 0
     verbosity_during_final_model_training: int = 0
@@ -162,15 +167,15 @@
     params = {
         "booster": "gbtree",
         "max_depth": 7,  # maximum depth of the decision trees being trained
         "alpha": 0.1,
         "lambda": 0.1,
         "gamma": 0.0,
         "subsample": 1.0,
-        "max_leaves": 16,
+        "min_child_weight": 1,
         "colsample_bytree": 0.8,
         "colsample_bylevel": 0.8,
         "eta": 0.1,
         "steps": 1000,
     }
     sample_weight: Optional[Dict[str, float]] = None
     classification_threshold: float = 0.5
```

### Comparing `bluecast-1.1/bluecast/conformal_prediction/__pycache__/base_classes.cpython-310.pyc` & `bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/__pycache__/conformal_prediction.cpython-310.pyc` & `bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/conformal_prediction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/__pycache__/conformal_prediction_regression.cpython-310.pyc` & `bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/conformal_prediction_regression.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/__pycache__/nonconformity_measures.cpython-310.pyc` & `bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/nonconformity_measures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/__pycache__/nonconformity_measures_regression.cpython-310.pyc` & `bluecast-1.2.4/bluecast/conformal_prediction/__pycache__/nonconformity_measures_regression.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/base_classes.py` & `bluecast-1.2.4/bluecast/conformal_prediction/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/conformal_prediction.py` & `bluecast-1.2.4/bluecast/conformal_prediction/conformal_prediction.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/conformal_prediction_regression.py` & `bluecast-1.2.4/bluecast/conformal_prediction/conformal_prediction_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/effectiveness_nonconformity_measures.py` & `bluecast-1.2.4/bluecast/conformal_prediction/effectiveness_nonconformity_measures.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/evaluation.py` & `bluecast-1.2.4/bluecast/conformal_prediction/evaluation.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/nonconformity_measures.py` & `bluecast-1.2.4/bluecast/conformal_prediction/nonconformity_measures.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/conformal_prediction/nonconformity_measures_regression.py` & `bluecast-1.2.4/bluecast/conformal_prediction/nonconformity_measures_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/__pycache__/analyse.cpython-310.pyc` & `bluecast-1.2.4/bluecast/eda/__pycache__/analyse.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/__pycache__/analyse.cpython-38.pyc` & `bluecast-1.2.4/bluecast/eda/__pycache__/analyse.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/__pycache__/data_leakage_checks.cpython-310.pyc` & `bluecast-1.2.4/bluecast/eda/__pycache__/data_leakage_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/__pycache__/data_leakage_checks.cpython-38.pyc` & `bluecast-1.2.4/bluecast/eda/__pycache__/data_leakage_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/analyse.py` & `bluecast-1.2.4/bluecast/eda/analyse.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/eda/data_leakage_checks.py` & `bluecast-1.2.4/bluecast/eda/data_leakage_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-1.2.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc` & `bluecast-1.2.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-1.2.4/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-1.2.4/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/eval_metrics.py` & `bluecast-1.2.4/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/evaluation/shap_values.py` & `bluecast-1.2.4/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/experimentation/__pycache__/tracking.cpython-310.pyc` & `bluecast-1.2.4/bluecast/experimentation/__pycache__/tracking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/experimentation/__pycache__/tracking.cpython-38.pyc` & `bluecast-1.2.4/bluecast/experimentation/__pycache__/tracking.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/experimentation/tracking.py` & `bluecast-1.2.4/bluecast/experimentation/tracking.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-1.2.4/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 26 07:23:40 2024 UTC, .py size: 3185 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,198 +1,247 @@
-00000000: 6f0d 0d0a 0000 0000 7c56 2b66 710c 0000  o.......|V+fq...
+00000000: 6f0d 0d0a 0000 0000 d056 3866 3b0f 0000  o........V8f;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 000b 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 0100 6401 6402 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6401 6402 6c09 5a0a 6401 6402 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 5a0c 6405 6505 650d 650d 6602 1900 6602  Z.d.e.e.e.f...f.
 00000080: 6406 6407 8404 5a0e 6408 650d 6405 6402  d.d...Z.d.e.d.d.
 00000090: 6604 6409 640a 8404 5a0f 0902 090b 090c  f.d.d...Z.......
-000000a0: 6415 640d 6504 640e 6506 650d 1900 640f  d.d.e.d.e.e...d.
+000000a0: 641a 640d 6504 640e 6506 650d 1900 640f  d.d.e.d.e.e...d.
 000000b0: 650d 6410 650d 6405 6402 660a 6411 6412  e.d.e.d.d.f.d.d.
-000000c0: 8405 5a10 0902 090b 090c 6415 640e 6506  ..Z.......d.d.e.
+000000c0: 8405 5a10 0902 090b 090c 641a 640e 6506  ..Z.......d.d.e.
 000000d0: 650d 1900 640f 650d 6410 650d 6405 6504  e...d.e.d.e.d.e.
-000000e0: 6608 6413 6414 8405 5a11 6402 5300 2916  f.d.d...Z.d.S.).
-000000f0: 7a12 4765 6e65 7261 6c20 7574 696c 6974  z.General utilit
-00000100: 6965 732e e900 0000 004e 2901 da08 6461  ies......N)...da
-00000110: 7465 7469 6d65 2903 da03 416e 79da 0444  tetime)...Any..D
-00000120: 6963 74da 084f 7074 696f 6e61 6cda 0672  ict..Optional..r
-00000130: 6574 7572 6e63 0000 0000 0000 0000 0000  eturnc..........
-00000140: 0000 0500 0000 0a00 0000 4300 0000 731a  ..........C...s.
-00000150: 0100 0074 0074 01a0 02a1 009b 0064 019d  ...t.t.......d..
-00000160: 0283 0101 0074 036a 04a0 0564 0264 03a1  .....t.j...d.d..
-00000170: 027d 0074 036a 046a 0664 0364 0264 048d  .}.t.j.j.d.d.d..
-00000180: 027d 0174 076a 087c 007c 0164 058d 027d  .}.t.j.|.|.d...}
-00000190: 027a 1364 0664 0769 017d 0374 076a 097c  .z.d.d.i.}.t.j.|
-000001a0: 037c 0264 0364 088d 0301 0074 0a64 0983  .|.d.d.....t.d..
-000001b0: 0101 007c 0357 0053 0004 0074 0b79 3b01  ...|.W.S...t.y;.
-000001c0: 0001 0001 0059 006e 0177 007a 1364 0a64  .....Y.n.w.z.d.d
-000001d0: 0b69 017d 0374 076a 097c 037c 0264 0364  .i.}.t.j.|.|.d.d
-000001e0: 088d 0301 0074 0a64 0983 0101 007c 0357  .....t.d.....|.W
-000001f0: 0053 0004 0074 0b79 5801 0001 0001 0059  .S...t.yX......Y
-00000200: 006e 0177 007a 1364 0a64 0c69 017d 0374  .n.w.z.d.d.i.}.t
-00000210: 076a 097c 037c 0264 0364 088d 0301 0074  .j.|.|.d.d.....t
-00000220: 0a64 0983 0101 007c 0357 0053 0004 0074  .d.....|.W.S...t
-00000230: 0b79 8c01 007d 0401 007a 1474 0a7c 0483  .y...}...z.t.|..
-00000240: 0101 0064 0a64 0d69 017d 0374 0a64 0e83  ...d.d.i.}.t.d..
-00000250: 0101 007c 0357 0006 0059 0064 007d 047e  ...|.W...Y.d.}.~
-00000260: 0453 0064 007d 047e 0477 0177 0029 0f4e  .S.d.}.~.w.w.).N
-00000270: 7a2f 3a20 5374 6172 7420 6368 6563 6b69  z/: Start checki
-00000280: 6e67 2069 6620 4750 5520 6973 2061 7661  ng if GPU is ava
-00000290: 696c 6162 6c65 2066 6f72 2075 7361 6765  ilable for usage
-000002a0: 2ee9 3200 0000 e902 0000 0029 01da 0473  ..2........)...s
-000002b0: 697a 6529 01da 056c 6162 656c da06 6465  ize)...label..de
-000002c0: 7669 6365 da04 6375 6461 2901 5a0f 6e75  vice..cuda).Z.nu
-000002d0: 6d5f 626f 6f73 745f 726f 756e 647a 1158  m_boost_roundz.X
-000002e0: 6762 6f6f 7374 2075 7365 7320 4750 552e  gboost uses GPU.
-000002f0: 5a0b 7472 6565 5f6d 6574 686f 645a 0867  Z.tree_methodZ.g
-00000300: 7075 5f68 6973 745a 0367 7075 da05 6578  pu_histZ.gpu..ex
-00000310: 6163 747a 1158 6762 6f6f 7374 2075 7365  actz.Xgboost use
-00000320: 7320 4350 552e 290c da06 6c6f 6767 6572  s CPU.)...logger
-00000330: 7202 0000 00da 0675 7463 6e6f 77da 026e  r......utcnow..n
-00000340: 70da 0672 616e 646f 6dda 0472 616e 64da  p..random..rand.
-00000350: 0772 616e 6469 6e74 da03 7867 625a 0744  .randint..xgbZ.D
-00000360: 4d61 7472 6978 5a05 7472 6169 6eda 0570  MatrixZ.train..p
-00000370: 7269 6e74 da09 4578 6365 7074 696f 6e29  rint..Exception)
-00000380: 05da 0464 6174 6172 0a00 0000 5a07 645f  ...datar....Z.d_
-00000390: 7472 6169 6eda 0670 6172 616d 73da 0165  train..params..e
-000003a0: a900 721a 0000 00fa 4a2f 686f 6d65 2f74  ..r.....J/home/t
-000003b0: 686f 6d61 732f 4964 6561 5072 6f6a 6563  homas/IdeaProjec
-000003c0: 7473 2f42 6c75 6543 6173 742f 626c 7565  ts/BlueCast/blue
-000003d0: 6361 7374 2f67 656e 6572 616c 5f75 7469  cast/general_uti
-000003e0: 6c73 2f67 656e 6572 616c 5f75 7469 6c73  ls/general_utils
-000003f0: 2e70 79da 1163 6865 636b 5f67 7075 5f73  .py..check_gpu_s
-00000400: 7570 706f 7274 0c00 0000 7340 0000 0012  upport....s@....
-00000410: 010e 0110 010e 0102 0208 0110 0108 0106  ................
-00000420: 010c 0104 0102 ff02 0308 0110 0108 0106  ................
-00000430: 010c 0104 0102 ff02 0308 0110 0108 0106  ................
-00000440: 010e 0108 0108 0108 0110 0108 8002 fc72  ...............r
-00000450: 1c00 0000 da07 6d65 7373 6167 6563 0100  ......messagec..
-00000460: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00000470: 0000 4300 0000 7326 0000 0074 006a 0164  ..C...s&...t.j.d
-00000480: 0164 0264 0364 048d 0301 0074 00a0 027c  .d.d.d.....t...|
-00000490: 00a1 0101 0074 037c 0083 0101 0064 0053  .....t.|.....d.S
-000004a0: 0029 054e 7a0c 626c 7565 6361 7374 2e6c  .).Nz.bluecast.l
-000004b0: 6f67 da01 777a 2625 286e 616d 6529 7320  og..wz&%(name)s 
-000004c0: 2d20 2528 6c65 7665 6c6e 616d 6529 7320  - %(levelname)s 
-000004d0: 2d20 2528 6d65 7373 6167 6529 7329 03da  - %(message)s)..
-000004e0: 0866 696c 656e 616d 65da 0866 696c 656d  .filename..filem
-000004f0: 6f64 65da 0666 6f72 6d61 7429 04da 076c  ode..format)...l
-00000500: 6f67 6769 6e67 da0b 6261 7369 6343 6f6e  ogging..basicCon
-00000510: 6669 67da 0469 6e66 6f72 1500 0000 2901  fig..infor....).
-00000520: 721d 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00000530: 1b00 0000 720e 0000 002e 0000 0073 0e00  ....r........s..
-00000540: 0000 0401 0201 0201 0201 06fd 0a05 0c01  ................
-00000550: 720e 0000 00da 0f61 7574 6f6d 6c5f 696e  r......automl_in
-00000560: 7374 616e 6365 fa04 2e64 6174 da0e 636c  stance...dat..cl
-00000570: 6173 735f 696e 7374 616e 6365 da09 6669  ass_instance..fi
-00000580: 6c65 5f70 6174 68da 0966 696c 655f 6e61  le_path..file_na
-00000590: 6d65 da09 6669 6c65 5f74 7970 6563 0400  me..file_typec..
-000005a0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000005b0: 0000 4300 0000 734e 0000 0074 0074 01a0  ..C...sN...t.t..
-000005c0: 02a1 009b 0064 019d 0283 0101 007c 0172  .....d.......|.r
-000005d0: 127c 017c 0217 007c 0317 007d 046e 047c  .|.|...|...}.n.|
-000005e0: 027c 0317 007d 0474 037c 0464 0283 027d  .|...}.t.|.d...}
-000005f0: 0574 04a0 057c 007c 05a1 0201 007c 05a0  .t...|.|.....|..
-00000600: 06a1 0001 0064 0353 0029 0461 5301 0000  .....d.S.).aS...
-00000610: 0a20 2020 2054 616b 6573 2061 2070 7265  .    Takes a pre
-00000620: 7472 6169 6e65 6420 6d6f 6465 6c20 616e  trained model an
-00000630: 6420 7361 7665 7320 6974 2076 6961 2064  d saves it via d
-00000640: 696c 6c2e 0a20 2020 203a 7061 7261 6d20  ill..    :param 
-00000650: 636c 6173 735f 696e 7374 616e 6365 3a20  class_instance: 
-00000660: 5461 6b65 7320 696e 7374 616e 6365 206f  Takes instance o
-00000670: 6620 6120 426c 7565 4361 7374 2063 6c61  f a BlueCast cla
-00000680: 7373 2e0a 2020 2020 3a70 6172 616d 2066  ss..    :param f
-00000690: 696c 655f 7061 7468 3a20 5461 6b65 7320  ile_path: Takes 
-000006a0: 6120 7374 7269 6e67 2063 6f6e 7461 696e  a string contain
-000006b0: 696e 6720 7468 6520 6675 6c6c 2061 6273  ing the full abs
-000006c0: 6f6c 7574 6520 7061 7468 2e0a 2020 2020  olute path..    
-000006d0: 3a70 6172 616d 2066 696c 655f 6e61 6d65  :param file_name
-000006e0: 3a20 5461 6b65 7320 6120 7374 7269 6e67  : Takes a string
-000006f0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00000700: 7768 6f6c 6520 6669 6c65 206e 616d 652e  whole file name.
-00000710: 0a20 2020 203a 7061 7261 6d20 6669 6c65  .    :param file
-00000720: 5f74 7970 653a 2054 616b 6573 2074 6865  _type: Takes the
-00000730: 2065 7870 6563 7465 6420 7479 7065 206f   expected type o
-00000740: 6620 6669 6c65 2074 6f20 6578 706f 7274  f file to export
-00000750: 2e0a 2020 2020 3a72 6574 7572 6e3a 0a20  ..    :return:. 
-00000760: 2020 207a 1e3a 2053 7461 7274 2073 6176     z.: Start sav
-00000770: 696e 6720 636c 6173 7320 696e 7374 616e  ing class instan
-00000780: 6365 2eda 0277 624e 2907 720e 0000 0072  ce...wbN).r....r
-00000790: 0200 0000 720f 0000 00da 046f 7065 6eda  ....r......open.
-000007a0: 0670 6963 6b6c 65da 0464 756d 70da 0563  .pickle..dump..c
-000007b0: 6c6f 7365 2906 7227 0000 0072 2800 0000  lose).r'...r(...
-000007c0: 7229 0000 0072 2a00 0000 da09 6675 6c6c  r)...r*.....full
-000007d0: 5f70 6174 68da 0b66 696c 6568 616e 646c  _path..filehandl
-000007e0: 6572 721a 0000 0072 1a00 0000 721b 0000  err....r....r...
-000007f0: 00da 1273 6176 655f 746f 5f70 726f 6475  ...save_to_produ
-00000800: 6374 696f 6e38 0000 0073 0e00 0000 120e  ction8...s......
-00000810: 0401 0e01 0802 0a01 0c01 0c01 7232 0000  ............r2..
-00000820: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
-00000830: 0000 0b00 0000 4300 0000 73b4 0000 0074  ......C...s....t
-00000840: 0074 01a0 02a1 009b 0064 019d 0283 0101  .t.......d......
-00000850: 007c 0072 107c 007c 0117 007d 036e 027c  .|.r.|.|...}.n.|
-00000860: 017d 037a 1f74 037c 0364 0283 028f 0f7d  .}.z.t.|.d.....}
-00000870: 0474 04a0 057c 04a1 017d 0557 0064 0304  .t...|...}.W.d..
-00000880: 0004 0083 0301 0057 007c 0553 0031 0073  .......W.|.S.1.s
-00000890: 2a77 0101 0001 0001 0059 0001 0057 007c  *w.......Y...W.|
-000008a0: 0553 0004 0074 0679 5901 0001 0001 0074  .S...t.yY......t
-000008b0: 037c 037c 0217 0064 0283 028f 0f7d 0474  .|.|...d.....}.t
-000008c0: 04a0 057c 04a1 017d 0557 0064 0304 0004  ...|...}.W.d....
-000008d0: 0083 0301 0059 007c 0553 0031 0073 5177  .....Y.|.S.1.sQw
-000008e0: 0101 0001 0001 0059 0001 0059 007c 0553  .......Y...Y.|.S
-000008f0: 0077 0029 0461 b201 0000 0a20 2020 204c  .w.).a.....    L
-00000900: 6f61 6420 696e 2061 2070 7265 7472 6169  oad in a pretrai
-00000910: 6e65 6420 6175 746f 206d 6c20 6d6f 6465  ned auto ml mode
-00000920: 6c2e 2054 6869 7320 6675 6e63 7469 6f6e  l. This function
-00000930: 2077 696c 6c20 7472 7920 746f 206c 6f61   will try to loa
-00000940: 6420 7468 6520 6d6f 6465 6c20 6173 2070  d the model as p
-00000950: 726f 7669 6465 642e 0a20 2020 2049 7420  rovided..    It 
-00000960: 6861 7320 6120 6661 6c6c 6261 636b 206c  has a fallback l
-00000970: 6f67 6963 2074 6f20 696d 7075 7465 202e  ogic to impute .
-00000980: 6461 7420 6173 2066 696c 655f 7479 7065  dat as file_type
-00000990: 2069 6e20 6361 7365 2074 6865 2069 6d70   in case the imp
-000009a0: 6f72 7420 6661 696c 7320 696e 6974 6961  ort fails initia
-000009b0: 6c6c 792e 0a20 2020 203a 7061 7261 6d20  lly..    :param 
-000009c0: 6669 6c65 5f70 6174 683a 2054 616b 6573  file_path: Takes
-000009d0: 2061 2073 7472 696e 6720 636f 6e74 6169   a string contai
-000009e0: 6e69 6e67 2074 6865 2066 756c 6c20 6162  ning the full ab
-000009f0: 736f 6c75 7465 2070 6174 682e 0a20 2020  solute path..   
-00000a00: 203a 7061 7261 6d20 6669 6c65 5f6e 616d   :param file_nam
-00000a10: 653a 2054 616b 6573 2061 2073 7472 696e  e: Takes a strin
-00000a20: 6720 636f 6e74 6169 6e69 6e67 2074 6865  g containing the
-00000a30: 2077 686f 6c65 2066 696c 6520 6e61 6d65   whole file name
-00000a40: 2e0a 2020 2020 3a70 6172 616d 2066 696c  ..    :param fil
-00000a50: 655f 7479 7065 3a20 5461 6b65 7320 7468  e_type: Takes th
-00000a60: 6520 6578 7065 6374 6564 2074 7970 6520  e expected type 
-00000a70: 6f66 2066 696c 6520 746f 2069 6d70 6f72  of file to impor
-00000a80: 742e 0a20 2020 203a 7265 7475 726e 3a20  t..    :return: 
-00000a90: 5468 6520 6c6f 6164 6564 206d 6f64 656c  The loaded model
-00000aa0: 206f 626a 6563 740a 2020 2020 7a1f 3a20   object.    z.: 
-00000ab0: 5374 6172 7420 6c6f 6164 696e 6720 636c  Start loading cl
-00000ac0: 6173 7320 696e 7374 616e 6365 2eda 0272  ass instance...r
-00000ad0: 624e 2907 720e 0000 0072 0200 0000 720f  bN).r....r....r.
-00000ae0: 0000 0072 2c00 0000 722d 0000 00da 046c  ...r,...r-.....l
-00000af0: 6f61 6472 1600 0000 2906 7228 0000 0072  oadr....).r(...r
-00000b00: 2900 0000 722a 0000 0072 3000 0000 7231  )...r*...r0...r1
-00000b10: 0000 005a 0c61 7574 6f6d 6c5f 6d6f 6465  ...Z.automl_mode
-00000b20: 6c72 1a00 0000 721a 0000 0072 1b00 0000  lr....r....r....
-00000b30: da13 6c6f 6164 5f66 6f72 5f70 726f 6475  ..load_for_produ
-00000b40: 6374 696f 6e50 0000 0073 2600 0000 120d  ctionP...s&.....
-00000b50: 0401 0a01 0402 0201 0c01 0c01 0cff 0405  ................
-00000b60: 12fb 0405 0cfd 1001 0c01 0cff 0402 12fe  ................
-00000b70: 0402 02fd 7235 0000 0029 034e 7225 0000  ....r5...).Nr%..
-00000b80: 0072 2600 0000 2912 da07 5f5f 646f 635f  .r&...)...__doc_
-00000b90: 5f72 2200 0000 7202 0000 00da 0674 7970  _r"...r......typ
-00000ba0: 696e 6772 0300 0000 7204 0000 0072 0500  ingr....r....r..
-00000bb0: 0000 5a04 6469 6c6c 722d 0000 00da 056e  ..Z.dillr-.....n
-00000bc0: 756d 7079 7210 0000 005a 0778 6762 6f6f  umpyr....Z.xgboo
-00000bd0: 7374 7214 0000 00da 0373 7472 721c 0000  str......strr...
-00000be0: 0072 0e00 0000 7232 0000 0072 3500 0000  .r....r2...r5...
-00000bf0: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00000c00: 1b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000c10: 0000 7346 0000 0004 0008 020c 0114 0108  ..sF............
-00000c20: 0208 0108 0116 0312 2202 0c02 0102 0104  ........".......
-00000c30: fc02 0102 ff06 0202 fe02 0302 fd02 0402  ................
-00000c40: fc02 050a fb02 1902 0102 0104 fd06 0102  ................
-00000c50: ff02 0202 fe02 0302 fd02 040e fc         .............
+000000e0: 6608 6413 6414 8405 5a11 641b 6416 6512  f.d.d...Z.d.d.e.
+000000f0: 6417 6513 6405 6512 6606 6418 6419 8405  d.e.d.e.f.d.d...
+00000100: 5a14 6402 5300 291c 7a12 4765 6e65 7261  Z.d.S.).z.Genera
+00000110: 6c20 7574 696c 6974 6965 732e e900 0000  l utilities.....
+00000120: 004e 2901 da08 6461 7465 7469 6d65 2903  .N)...datetime).
+00000130: da03 416e 79da 0444 6963 74da 084f 7074  ..Any..Dict..Opt
+00000140: 696f 6e61 6cda 0672 6574 7572 6e63 0000  ional..returnc..
+00000150: 0000 0000 0000 0000 0000 0500 0000 0a00  ................
+00000160: 0000 4300 0000 731a 0100 0074 0074 01a0  ..C...s....t.t..
+00000170: 02a1 009b 0064 019d 0283 0101 0074 036a  .....d.......t.j
+00000180: 04a0 0564 0264 03a1 027d 0074 036a 046a  ...d.d...}.t.j.j
+00000190: 0664 0364 0264 048d 027d 0174 076a 087c  .d.d.d...}.t.j.|
+000001a0: 007c 0164 058d 027d 027a 1364 0664 0769  .|.d...}.z.d.d.i
+000001b0: 017d 0374 076a 097c 037c 0264 0364 088d  .}.t.j.|.|.d.d..
+000001c0: 0301 0074 0a64 0983 0101 007c 0357 0053  ...t.d.....|.W.S
+000001d0: 0004 0074 0b79 3b01 0001 0001 0059 006e  ...t.y;......Y.n
+000001e0: 0177 007a 1364 0a64 0b69 017d 0374 076a  .w.z.d.d.i.}.t.j
+000001f0: 097c 037c 0264 0364 088d 0301 0074 0a64  .|.|.d.d.....t.d
+00000200: 0983 0101 007c 0357 0053 0004 0074 0b79  .....|.W.S...t.y
+00000210: 5801 0001 0001 0059 006e 0177 007a 1364  X......Y.n.w.z.d
+00000220: 0a64 0c69 017d 0374 076a 097c 037c 0264  .d.i.}.t.j.|.|.d
+00000230: 0364 088d 0301 0074 0a64 0983 0101 007c  .d.....t.d.....|
+00000240: 0357 0053 0004 0074 0b79 8c01 007d 0401  .W.S...t.y...}..
+00000250: 007a 1474 0a7c 0483 0101 0064 0a64 0d69  .z.t.|.....d.d.i
+00000260: 017d 0374 0a64 0e83 0101 007c 0357 0006  .}.t.d.....|.W..
+00000270: 0059 0064 007d 047e 0453 0064 007d 047e  .Y.d.}.~.S.d.}.~
+00000280: 0477 0177 0029 0f4e 7a2f 3a20 5374 6172  .w.w.).Nz/: Star
+00000290: 7420 6368 6563 6b69 6e67 2069 6620 4750  t checking if GP
+000002a0: 5520 6973 2061 7661 696c 6162 6c65 2066  U is available f
+000002b0: 6f72 2075 7361 6765 2ee9 3200 0000 e902  or usage..2.....
+000002c0: 0000 0029 01da 0473 697a 6529 01da 056c  ...)...size)...l
+000002d0: 6162 656c da06 6465 7669 6365 da04 6375  abel..device..cu
+000002e0: 6461 2901 5a0f 6e75 6d5f 626f 6f73 745f  da).Z.num_boost_
+000002f0: 726f 756e 647a 1158 6762 6f6f 7374 2075  roundz.Xgboost u
+00000300: 7365 7320 4750 552e 5a0b 7472 6565 5f6d  ses GPU.Z.tree_m
+00000310: 6574 686f 645a 0867 7075 5f68 6973 745a  ethodZ.gpu_histZ
+00000320: 0367 7075 da05 6578 6163 747a 1158 6762  .gpu..exactz.Xgb
+00000330: 6f6f 7374 2075 7365 7320 4350 552e 290c  oost uses CPU.).
+00000340: da06 6c6f 6767 6572 7202 0000 00da 0675  ..loggerr......u
+00000350: 7463 6e6f 77da 026e 70da 0672 616e 646f  tcnow..np..rando
+00000360: 6dda 0472 616e 64da 0772 616e 6469 6e74  m..rand..randint
+00000370: da03 7867 625a 0744 4d61 7472 6978 5a05  ..xgbZ.DMatrixZ.
+00000380: 7472 6169 6eda 0570 7269 6e74 da09 4578  train..print..Ex
+00000390: 6365 7074 696f 6e29 05da 0464 6174 6172  ception)...datar
+000003a0: 0a00 0000 5a07 645f 7472 6169 6eda 0670  ....Z.d_train..p
+000003b0: 6172 616d 73da 0165 a900 721a 0000 00fa  arams..e..r.....
+000003c0: 4a2f 686f 6d65 2f74 686f 6d61 732f 4964  J/home/thomas/Id
+000003d0: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
+000003e0: 6173 742f 626c 7565 6361 7374 2f67 656e  ast/bluecast/gen
+000003f0: 6572 616c 5f75 7469 6c73 2f67 656e 6572  eral_utils/gener
+00000400: 616c 5f75 7469 6c73 2e70 79da 1163 6865  al_utils.py..che
+00000410: 636b 5f67 7075 5f73 7570 706f 7274 0c00  ck_gpu_support..
+00000420: 0000 7340 0000 0012 010e 0110 010e 0102  ..s@............
+00000430: 0208 0110 0108 0106 010c 0104 0102 ff02  ................
+00000440: 0308 0110 0108 0106 010c 0104 0102 ff02  ................
+00000450: 0308 0110 0108 0106 010e 0108 0108 0108  ................
+00000460: 0110 0108 8002 fc72 1c00 0000 da07 6d65  .......r......me
+00000470: 7373 6167 6563 0100 0000 0000 0000 0000  ssagec..........
+00000480: 0000 0100 0000 0500 0000 4300 0000 7326  ..........C...s&
+00000490: 0000 0074 006a 0164 0164 0264 0364 048d  ...t.j.d.d.d.d..
+000004a0: 0301 0074 00a0 027c 00a1 0101 0074 037c  ...t...|.....t.|
+000004b0: 0083 0101 0064 0053 0029 054e 7a0c 626c  .....d.S.).Nz.bl
+000004c0: 7565 6361 7374 2e6c 6f67 da01 777a 2625  uecast.log..wz&%
+000004d0: 286e 616d 6529 7320 2d20 2528 6c65 7665  (name)s - %(leve
+000004e0: 6c6e 616d 6529 7320 2d20 2528 6d65 7373  lname)s - %(mess
+000004f0: 6167 6529 7329 03da 0866 696c 656e 616d  age)s)...filenam
+00000500: 65da 0866 696c 656d 6f64 65da 0666 6f72  e..filemode..for
+00000510: 6d61 7429 04da 076c 6f67 6769 6e67 da0b  mat)...logging..
+00000520: 6261 7369 6343 6f6e 6669 67da 0469 6e66  basicConfig..inf
+00000530: 6f72 1500 0000 2901 721d 0000 0072 1a00  or....).r....r..
+00000540: 0000 721a 0000 0072 1b00 0000 720e 0000  ..r....r....r...
+00000550: 002e 0000 0073 0e00 0000 0401 0201 0201  .....s..........
+00000560: 0201 06fd 0a05 0c01 720e 0000 00da 0f61  ........r......a
+00000570: 7574 6f6d 6c5f 696e 7374 616e 6365 fa04  utoml_instance..
+00000580: 2e64 6174 da0e 636c 6173 735f 696e 7374  .dat..class_inst
+00000590: 616e 6365 da09 6669 6c65 5f70 6174 68da  ance..file_path.
+000005a0: 0966 696c 655f 6e61 6d65 da09 6669 6c65  .file_name..file
+000005b0: 5f74 7970 6563 0400 0000 0000 0000 0000  _typec..........
+000005c0: 0000 0600 0000 0400 0000 4300 0000 734e  ..........C...sN
+000005d0: 0000 0074 0074 01a0 02a1 009b 0064 019d  ...t.t.......d..
+000005e0: 0283 0101 007c 0172 127c 017c 0217 007c  .....|.r.|.|...|
+000005f0: 0317 007d 046e 047c 027c 0317 007d 0474  ...}.n.|.|...}.t
+00000600: 037c 0464 0283 027d 0574 04a0 057c 007c  .|.d...}.t...|.|
+00000610: 05a1 0201 007c 05a0 06a1 0001 0064 0353  .....|.......d.S
+00000620: 0029 0461 5301 0000 0a20 2020 2054 616b  .).aS....    Tak
+00000630: 6573 2061 2070 7265 7472 6169 6e65 6420  es a pretrained 
+00000640: 6d6f 6465 6c20 616e 6420 7361 7665 7320  model and saves 
+00000650: 6974 2076 6961 2064 696c 6c2e 0a20 2020  it via dill..   
+00000660: 203a 7061 7261 6d20 636c 6173 735f 696e   :param class_in
+00000670: 7374 616e 6365 3a20 5461 6b65 7320 696e  stance: Takes in
+00000680: 7374 616e 6365 206f 6620 6120 426c 7565  stance of a Blue
+00000690: 4361 7374 2063 6c61 7373 2e0a 2020 2020  Cast class..    
+000006a0: 3a70 6172 616d 2066 696c 655f 7061 7468  :param file_path
+000006b0: 3a20 5461 6b65 7320 6120 7374 7269 6e67  : Takes a string
+000006c0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+000006d0: 6675 6c6c 2061 6273 6f6c 7574 6520 7061  full absolute pa
+000006e0: 7468 2e0a 2020 2020 3a70 6172 616d 2066  th..    :param f
+000006f0: 696c 655f 6e61 6d65 3a20 5461 6b65 7320  ile_name: Takes 
+00000700: 6120 7374 7269 6e67 2063 6f6e 7461 696e  a string contain
+00000710: 696e 6720 7468 6520 7768 6f6c 6520 6669  ing the whole fi
+00000720: 6c65 206e 616d 652e 0a20 2020 203a 7061  le name..    :pa
+00000730: 7261 6d20 6669 6c65 5f74 7970 653a 2054  ram file_type: T
+00000740: 616b 6573 2074 6865 2065 7870 6563 7465  akes the expecte
+00000750: 6420 7479 7065 206f 6620 6669 6c65 2074  d type of file t
+00000760: 6f20 6578 706f 7274 2e0a 2020 2020 3a72  o export..    :r
+00000770: 6574 7572 6e3a 0a20 2020 207a 1e3a 2053  eturn:.    z.: S
+00000780: 7461 7274 2073 6176 696e 6720 636c 6173  tart saving clas
+00000790: 7320 696e 7374 616e 6365 2eda 0277 624e  s instance...wbN
+000007a0: 2907 720e 0000 0072 0200 0000 720f 0000  ).r....r....r...
+000007b0: 00da 046f 7065 6eda 0670 6963 6b6c 65da  ...open..pickle.
+000007c0: 0464 756d 70da 0563 6c6f 7365 2906 7227  .dump..close).r'
+000007d0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+000007e0: 0000 da09 6675 6c6c 5f70 6174 68da 0b66  ....full_path..f
+000007f0: 696c 6568 616e 646c 6572 721a 0000 0072  ilehandlerr....r
+00000800: 1a00 0000 721b 0000 00da 1273 6176 655f  ....r......save_
+00000810: 746f 5f70 726f 6475 6374 696f 6e38 0000  to_production8..
+00000820: 0073 0e00 0000 120e 0401 0e01 0802 0a01  .s..............
+00000830: 0c01 0c01 7232 0000 0063 0300 0000 0000  ....r2...c......
+00000840: 0000 0000 0000 0600 0000 0b00 0000 4300  ..............C.
+00000850: 0000 73b4 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
+00000860: 0064 019d 0283 0101 007c 0072 107c 007c  .d.......|.r.|.|
+00000870: 0117 007d 036e 027c 017d 037a 1f74 037c  ...}.n.|.}.z.t.|
+00000880: 0364 0283 028f 0f7d 0474 04a0 057c 04a1  .d.....}.t...|..
+00000890: 017d 0557 0064 0304 0004 0083 0301 0057  .}.W.d.........W
+000008a0: 007c 0553 0031 0073 2a77 0101 0001 0001  .|.S.1.s*w......
+000008b0: 0059 0001 0057 007c 0553 0004 0074 0679  .Y...W.|.S...t.y
+000008c0: 5901 0001 0001 0074 037c 037c 0217 0064  Y......t.|.|...d
+000008d0: 0283 028f 0f7d 0474 04a0 057c 04a1 017d  .....}.t...|...}
+000008e0: 0557 0064 0304 0004 0083 0301 0059 007c  .W.d.........Y.|
+000008f0: 0553 0031 0073 5177 0101 0001 0001 0059  .S.1.sQw.......Y
+00000900: 0001 0059 007c 0553 0077 0029 0461 b201  ...Y.|.S.w.).a..
+00000910: 0000 0a20 2020 204c 6f61 6420 696e 2061  ...    Load in a
+00000920: 2070 7265 7472 6169 6e65 6420 6175 746f   pretrained auto
+00000930: 206d 6c20 6d6f 6465 6c2e 2054 6869 7320   ml model. This 
+00000940: 6675 6e63 7469 6f6e 2077 696c 6c20 7472  function will tr
+00000950: 7920 746f 206c 6f61 6420 7468 6520 6d6f  y to load the mo
+00000960: 6465 6c20 6173 2070 726f 7669 6465 642e  del as provided.
+00000970: 0a20 2020 2049 7420 6861 7320 6120 6661  .    It has a fa
+00000980: 6c6c 6261 636b 206c 6f67 6963 2074 6f20  llback logic to 
+00000990: 696d 7075 7465 202e 6461 7420 6173 2066  impute .dat as f
+000009a0: 696c 655f 7479 7065 2069 6e20 6361 7365  ile_type in case
+000009b0: 2074 6865 2069 6d70 6f72 7420 6661 696c   the import fail
+000009c0: 7320 696e 6974 6961 6c6c 792e 0a20 2020  s initially..   
+000009d0: 203a 7061 7261 6d20 6669 6c65 5f70 6174   :param file_pat
+000009e0: 683a 2054 616b 6573 2061 2073 7472 696e  h: Takes a strin
+000009f0: 6720 636f 6e74 6169 6e69 6e67 2074 6865  g containing the
+00000a00: 2066 756c 6c20 6162 736f 6c75 7465 2070   full absolute p
+00000a10: 6174 682e 0a20 2020 203a 7061 7261 6d20  ath..    :param 
+00000a20: 6669 6c65 5f6e 616d 653a 2054 616b 6573  file_name: Takes
+00000a30: 2061 2073 7472 696e 6720 636f 6e74 6169   a string contai
+00000a40: 6e69 6e67 2074 6865 2077 686f 6c65 2066  ning the whole f
+00000a50: 696c 6520 6e61 6d65 2e0a 2020 2020 3a70  ile name..    :p
+00000a60: 6172 616d 2066 696c 655f 7479 7065 3a20  aram file_type: 
+00000a70: 5461 6b65 7320 7468 6520 6578 7065 6374  Takes the expect
+00000a80: 6564 2074 7970 6520 6f66 2066 696c 6520  ed type of file 
+00000a90: 746f 2069 6d70 6f72 742e 0a20 2020 203a  to import..    :
+00000aa0: 7265 7475 726e 3a20 5468 6520 6c6f 6164  return: The load
+00000ab0: 6564 206d 6f64 656c 206f 626a 6563 740a  ed model object.
+00000ac0: 2020 2020 7a1f 3a20 5374 6172 7420 6c6f      z.: Start lo
+00000ad0: 6164 696e 6720 636c 6173 7320 696e 7374  ading class inst
+00000ae0: 616e 6365 2eda 0272 624e 2907 720e 0000  ance...rbN).r...
+00000af0: 0072 0200 0000 720f 0000 0072 2c00 0000  .r....r....r,...
+00000b00: 722d 0000 00da 046c 6f61 6472 1600 0000  r-.....loadr....
+00000b10: 2906 7228 0000 0072 2900 0000 722a 0000  ).r(...r)...r*..
+00000b20: 0072 3000 0000 7231 0000 005a 0c61 7574  .r0...r1...Z.aut
+00000b30: 6f6d 6c5f 6d6f 6465 6c72 1a00 0000 721a  oml_modelr....r.
+00000b40: 0000 0072 1b00 0000 da13 6c6f 6164 5f66  ...r......load_f
+00000b50: 6f72 5f70 726f 6475 6374 696f 6e50 0000  or_productionP..
+00000b60: 0073 2600 0000 120d 0401 0a01 0402 0201  .s&.............
+00000b70: 0c01 0c01 0cff 0405 12fb 0405 0cfd 1001  ................
+00000b80: 0c01 0cff 0402 12fe 0402 02fd 7235 0000  ............r5..
+00000b90: 00e7 9a99 9999 9999 b93f da07 6e62 5f72  .........?..nb_r
+00000ba0: 6f77 73da 0561 6c70 6861 6302 0000 0000  ows..alphac.....
+00000bb0: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
+00000bc0: 0000 0073 4400 0000 7400 7401 7c00 7402  ...sD...t.t.|.t.
+00000bd0: a003 7c00 a101 7402 a003 7c00 a101 6401  ..|...t...|...d.
+00000be0: 7c01 1700 1300 1300 1800 6402 8302 8301  |.........d.....
+00000bf0: 7d02 7404 6403 7c00 9b00 6404 7c02 9b00  }.t.d.|...d.|...
+00000c00: 6405 9d05 8301 0100 7c02 5300 2906 61b7  d.......|.S.).a.
+00000c10: 0100 0052 6574 7572 6e20 6e75 6d62 6572  ...Return number
+00000c20: 206f 6620 7361 6d70 6c65 7320 6261 7365   of samples base
+00000c30: 6420 6f6e 206c 6f67 2073 616d 706c 696e  d on log samplin
+00000c40: 672e 0a0a 2020 2020 5769 7468 2074 6865  g...    With the
+00000c50: 2064 6566 6175 6c74 2076 616c 7565 206f   default value o
+00000c60: 6620 616c 7068 612c 2074 6865 2066 756e  f alpha, the fun
+00000c70: 6374 696f 6e20 7769 6c6c 2072 6574 7572  ction will retur
+00000c80: 6e3a 0a20 2020 202a 2039 3620 7361 6d70  n:.    * 96 samp
+00000c90: 6c65 7320 666f 7220 3130 3020 726f 7773  les for 100 rows
+00000ca0: 2e0a 2020 2020 2a20 3936 3020 7361 6d70  ..    * 960 samp
+00000cb0: 6c65 7320 666f 7220 3130 3030 2072 6f77  les for 1000 row
+00000cc0: 732e 0a20 2020 202a 2039 3431 3620 7361  s..    * 9416 sa
+00000cd0: 6d70 6c65 7320 666f 7220 3130 3030 3020  mples for 10000 
+00000ce0: 726f 7773 2e0a 2020 2020 2a20 3837 3236  rows..    * 8726
+00000cf0: 3220 7361 6d70 6c65 7320 666f 7220 3130  2 samples for 10
+00000d00: 3030 3030 2072 6f77 732e 0a20 2020 202a  0000 rows..    *
+00000d10: 2036 3135 3332 3620 7361 6d70 6c65 7320   615326 samples 
+00000d20: 666f 7220 3130 3030 3030 3020 726f 7773  for 1000000 rows
+00000d30: 2e0a 2020 2020 3a70 6172 616d 206e 625f  ..    :param nb_
+00000d40: 726f 7773 3a20 4e75 6d62 6572 206f 6620  rows: Number of 
+00000d50: 726f 7773 2069 6e20 7468 6520 6461 7461  rows in the data
+00000d60: 7365 742e 0a20 2020 203a 7061 7261 6d20  set..    :param 
+00000d70: 616c 7068 613a 2041 6c70 6861 2076 616c  alpha: Alpha val
+00000d80: 7565 2066 6f72 206c 6f67 2073 616d 706c  ue for log sampl
+00000d90: 696e 672e 2048 6967 6865 7220 616c 7068  ing. Higher alph
+00000da0: 6120 7661 6c75 6573 2077 696c 6c20 7265  a values will re
+00000db0: 7375 6c74 2069 6e20 6c65 7373 2073 616d  sult in less sam
+00000dc0: 706c 6573 2e0a 2020 2020 e901 0000 0072  ples..    .....r
+00000dd0: 0100 0000 7a13 446f 776e 2073 616d 706c  ....z.Down sampl
+00000de0: 696e 6720 6672 6f6d 207a 0420 746f 207a  ing from z. to z
+00000df0: 0920 7361 6d70 6c65 732e 2905 da03 696e  . samples.)...in
+00000e00: 74da 0572 6f75 6e64 7210 0000 00da 056c  t..roundr......l
+00000e10: 6f67 3130 720e 0000 0029 0372 3700 0000  og10r....).r7...
+00000e20: 7238 0000 005a 0a6e 625f 7361 6d70 6c65  r8...Z.nb_sample
+00000e30: 7372 1a00 0000 721a 0000 0072 1b00 0000  sr....r....r....
+00000e40: da0c 6c6f 675f 7361 6d70 6c69 6e67 6b00  ..log_samplingk.
+00000e50: 0000 730a 0000 0002 0c24 0104 ff16 0304  ..s......$......
+00000e60: 0172 3d00 0000 2903 4e72 2500 0000 7226  .r=...).Nr%...r&
+00000e70: 0000 0029 0172 3600 0000 2915 da07 5f5f  ...).r6...)...__
+00000e80: 646f 635f 5f72 2200 0000 7202 0000 00da  doc__r"...r.....
+00000e90: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
+00000ea0: 0072 0500 0000 5a04 6469 6c6c 722d 0000  .r....Z.dillr-..
+00000eb0: 00da 056e 756d 7079 7210 0000 005a 0778  ...numpyr....Z.x
+00000ec0: 6762 6f6f 7374 7214 0000 00da 0373 7472  gboostr......str
+00000ed0: 721c 0000 0072 0e00 0000 7232 0000 0072  r....r....r2...r
+00000ee0: 3500 0000 723a 0000 00da 0566 6c6f 6174  5...r:.....float
+00000ef0: 723d 0000 0072 1a00 0000 721a 0000 0072  r=...r....r....r
+00000f00: 1a00 0000 721b 0000 00da 083c 6d6f 6475  ....r......<modu
+00000f10: 6c65 3e01 0000 0073 4800 0000 0400 0802  le>....sH.......
+00000f20: 0c01 1401 0802 0801 0801 1603 1222 020c  ............."..
+00000f30: 0201 0201 04fc 0201 02ff 0602 02fe 0203  ................
+00000f40: 02fd 0204 02fc 0205 0afb 0219 0201 0201  ................
+00000f50: 04fd 0601 02ff 0202 02fe 0203 02fd 0204  ................
+00000f60: 0afc 1c1b                                ....
```

### Comparing `bluecast-1.1/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-1.2.4/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/general_utils/general_utils.py` & `bluecast-1.2.4/bluecast/general_utils/general_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -98,7 +98,26 @@
     try:
         with open(full_path, "rb") as filehandler:
             automl_model = pickle.load(filehandler)
     except Exception:
         with open(full_path + file_type, "rb") as filehandler:
             automl_model = pickle.load(filehandler)
     return automl_model
+
+
+def log_sampling(nb_rows: int, alpha: float = 0.1) -> int:
+    """Return number of samples based on log sampling.
+
+    With the default value of alpha, the function will return:
+    * 96 samples for 100 rows.
+    * 960 samples for 1000 rows.
+    * 9416 samples for 10000 rows.
+    * 87262 samples for 100000 rows.
+    * 615326 samples for 1000000 rows.
+    :param nb_rows: Number of rows in the dataset.
+    :param alpha: Alpha value for log sampling. Higher alpha values will result in less samples.
+    """
+    nb_samples = int(
+        round(nb_rows - (np.log10(nb_rows) ** np.log10(nb_rows) ** (1 + alpha)), 0)
+    )
+    logger(f"Down sampling from {nb_rows} to {nb_samples} samples.")
+    return nb_samples
```

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 27 16:18:20 2024 UTC, .py size: 36227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,1189 +1,1179 @@
-00000000: 6f0d 0d0a 0000 0000 4c25 2d66 838d 0000  o.......L%-f....
+00000000: 6f0d 0d0a 0000 0000 fc61 3866 a38d 0000  o........a8f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6401 6405 6c0d 5a0d 6401 6405 6c0e  Z.d.d.l.Z.d.d.l.
 00000080: 5a0f 6401 6405 6c10 5a11 6401 6406 6c12  Z.d.d.l.Z.d.d.l.
 00000090: 6d13 5a13 0100 6401 6407 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
 000000a0: 0100 6401 6408 6c16 6d17 5a17 0100 6401  ..d.d.l.m.Z...d.
 000000b0: 6409 6c18 6d19 5a19 6d1a 5a1a 6d1b 5a1b  d.l.m.Z.m.Z.m.Z.
 000000c0: 0100 6401 640a 6c1c 6d1d 5a1d 0100 6401  ..d.d.l.m.Z...d.
-000000d0: 640b 6c1e 6d1f 5a1f 6d20 5a20 0100 6401  d.l.m.Z.m Z ..d.
-000000e0: 640c 6c21 6d22 5a22 0100 6401 640d 6c23  d.l!m"Z"..d.d.l#
-000000f0: 6d24 5a24 0100 4700 640e 640f 8400 640f  m$Z$..G.d.d...d.
-00000100: 6522 8303 5a25 6405 5300 2910 6119 0100  e"..Z%d.S.).a...
-00000110: 0058 6762 6f6f 7374 2063 6c61 7373 6966  .Xgboost classif
-00000120: 6963 6174 696f 6e20 6d6f 6465 6c2e 0a0a  ication model...
-00000130: 5468 6973 206d 6f64 756c 6520 636f 6e74  This module cont
-00000140: 6169 6e73 2061 2077 7261 7070 6572 2066  ains a wrapper f
-00000150: 6f72 2074 6865 2058 6762 6f6f 7374 2063  or the Xgboost c
-00000160: 6c61 7373 6966 6963 6174 696f 6e20 6d6f  lassification mo
-00000170: 6465 6c2e 2049 7420 6361 6e20 6265 2075  del. It can be u
-00000180: 7365 6420 746f 2074 7261 696e 2061 6e64  sed to train and
-00000190: 2f6f 7220 7475 6e65 2074 6865 206d 6f64  /or tune the mod
-000001a0: 656c 2e0a 4974 2061 6c73 6f20 6361 6c63  el..It also calc
-000001b0: 756c 6174 6573 2063 6c61 7373 2077 6569  ulates class wei
-000001c0: 6768 7473 2066 6f72 2069 6d62 616c 616e  ghts for imbalan
-000001d0: 6365 6420 6461 7461 7365 7473 2e20 5468  ced datasets. Th
-000001e0: 6520 7765 6967 6874 7320 6d61 7920 6f72  e weights may or
-000001f0: 206d 6179 206e 6f74 2062 6520 7573 6564   may not be used
-00000200: 2064 6565 7065 6e64 696e 6720 6f6e 2074   deepending on t
-00000210: 6865 0a68 7970 6572 7061 7261 6d65 7465  he.hyperparamete
-00000220: 7220 7475 6e69 6e67 2e0a e900 0000 0029  r tuning.......)
-00000230: 01da 0864 6565 7063 6f70 7929 01da 0864  ...deepcopy)...d
-00000240: 6174 6574 696d 6529 06da 0341 6e79 da04  atetime)...Any..
-00000250: 4469 6374 da04 4c69 7374 da07 4c69 7465  Dict..List..Lite
-00000260: 7261 6cda 084f 7074 696f 6e61 6cda 0554  ral..Optional..T
-00000270: 7570 6c65 4e29 01da 116d 6174 7468 6577  upleN)...matthew
-00000280: 735f 636f 7272 636f 6566 2901 da0f 5374  s_corrcoef)...St
-00000290: 7261 7469 6669 6564 4b46 6f6c 6429 01da  ratifiedKFold)..
-000002a0: 0c63 6c61 7373 5f77 6569 6768 7429 03da  .class_weight)..
-000002b0: 0e54 7261 696e 696e 6743 6f6e 6669 67da  .TrainingConfig.
-000002c0: 1758 6762 6f6f 7374 4669 6e61 6c50 6172  .XgboostFinalPar
-000002d0: 616d 436f 6e66 6967 da17 5867 626f 6f73  amConfig..Xgboos
-000002e0: 7454 756e 6550 6172 616d 7343 6f6e 6669  tTuneParamsConfi
-000002f0: 6729 01da 1145 7870 6572 696d 656e 7454  g)...ExperimentT
-00000300: 7261 636b 6572 2902 da11 6368 6563 6b5f  racker)...check_
-00000310: 6770 755f 7375 7070 6f72 74da 066c 6f67  gpu_support..log
-00000320: 6765 7229 01da 1042 6173 6543 6c61 7373  ger)...BaseClass
-00000330: 4d6c 4d6f 6465 6c29 01da 1343 7573 746f  MlModel)...Custo
-00000340: 6d50 7265 7072 6f63 6573 7369 6e67 6300  mPreprocessingc.
-00000350: 0000 0000 0000 0000 0000 0000 0000 000e  ................
-00000360: 0000 0040 0000 0073 a201 0000 6500 5a01  ...@...s....e.Z.
-00000370: 6400 5a02 6401 5a03 0902 0902 0902 0902  d.Z.d.Z.........
-00000380: 0902 6434 6403 6504 6404 1900 6405 6505  ..d4d.e.d...d.e.
-00000390: 6506 1900 6406 6505 6507 1900 6407 6505  e...d.e.e...d.e.
-000003a0: 6508 1900 6408 6505 6509 1900 6409 6505  e...d.e.e...d.e.
-000003b0: 650a 1900 660c 640a 640b 8405 5a0b 640c  e...f.d.d...Z.d.
-000003c0: 650c 6a0d 640d 650e 650f 6510 6602 1900  e.j.d.e.e.e.f...
-000003d0: 6604 640e 640f 8404 5a11 6410 6411 8400  f.d.d...Z.d.d...
-000003e0: 5a12 6412 650c 6a13 6413 650c 6a13 6414  Z.d.e.j.d.e.j.d.
-000003f0: 650c 6a0d 6415 650c 6a0d 640d 6514 6a15  e.j.d.e.j.d.e.j.
-00000400: 660a 6416 6417 8404 5a16 6412 650c 6a13  f.d.d...Z.d.e.j.
-00000410: 6413 650c 6a13 6414 650c 6a0d 6415 650c  d.e.j.d.e.j.d.e.
-00000420: 6a0d 640d 6402 660a 6418 6419 8404 5a17  j.d.d.f.d.d...Z.
-00000430: 641a 641b 8400 5a18 641c 641d 8400 5a19  d.d...Z.d.d...Z.
-00000440: 641e 641f 8400 5a1a 0920 6435 6421 650c  d.d...Z.. d5d!e.
-00000450: 6a13 6422 650c 6a0d 6423 651b 6606 6424  j.d"e.j.d#e.f.d$
-00000460: 6425 8405 5a1c 6426 651d 6510 1900 640d  d%..Z.d&e.e...d.
-00000470: 6510 6604 6427 6428 8404 5a1e 6429 650e  e.f.d'd(..Z.d)e.
-00000480: 650f 651f 6602 1900 6412 650c 6a13 6414  e.e.f...d.e.j.d.
-00000490: 650c 6a0d 6413 650c 6a13 6415 650c 6a0d  e.j.d.e.j.d.e.j.
-000004a0: 642a 651b 660c 642b 642c 8404 5a20 6412  d*e.f.d+d,..Z d.
-000004b0: 650c 6a13 6413 650c 6a13 6414 650c 6a0d  e.j.d.e.j.d.e.j.
-000004c0: 6415 650c 6a0d 640d 6402 660a 642d 642e  d.e.j.d.d.f.d-d.
-000004d0: 8404 5a21 642f 650c 6a13 640d 6522 6523  ..Z!d/e.j.d.e"e#
-000004e0: 6a24 6523 6a24 6602 1900 6604 6430 6431  j$e#j$f...f.d0d1
-000004f0: 8404 5a25 642f 650c 6a13 640d 6523 6a24  ..Z%d/e.j.d.e#j$
-00000500: 6604 6432 6433 8404 5a26 6402 5300 2936  f.d2d3..Z&d.S.)6
-00000510: da0c 5867 626f 6f73 744d 6f64 656c 7a2f  ..XgboostModelz/
-00000520: 5472 6169 6e20 616e 642f 6f72 2074 756e  Train and/or tun
-00000530: 6520 5867 626f 6f73 7420 636c 6173 7369  e Xgboost classi
-00000540: 6669 6361 7469 6f6e 206d 6f64 656c 2e4e  fication model.N
-00000550: da0d 636c 6173 735f 7072 6f62 6c65 6d29  ..class_problem)
-00000560: 02da 0662 696e 6172 79da 0a6d 756c 7469  ...binary..multi
-00000570: 636c 6173 73da 0d63 6f6e 665f 7472 6169  class..conf_trai
-00000580: 6e69 6e67 da0c 636f 6e66 5f78 6762 6f6f  ning..conf_xgboo
-00000590: 7374 da13 636f 6e66 5f70 6172 616d 735f  st..conf_params_
-000005a0: 7867 626f 6f73 74da 1265 7870 6572 696d  xgboost..experim
-000005b0: 656e 745f 7472 6163 6b65 72da 1b63 7573  ent_tracker..cus
-000005c0: 746f 6d5f 696e 5f66 6f6c 645f 7072 6570  tom_in_fold_prep
-000005d0: 726f 6365 7373 6f72 6307 0000 0000 0000  rocessorc.......
-000005e0: 0000 0000 0007 0000 0003 0000 0043 0000  .............C..
-000005f0: 0073 5800 0000 6400 7c00 5f00 7c01 7c00  .sX...d.|._.|.|.
-00000600: 5f01 7c02 7c00 5f02 7c03 7c00 5f03 7c04  _.|.|._.|.|._.|.
-00000610: 7c00 5f04 7c05 7c00 5f05 7c06 7c00 5f06  |._.|.|._.|.|._.
-00000620: 7c00 6a02 7223 7407 6a08 a009 7c00 6a02  |.j.r#t.j...|.j.
-00000630: 6a0a a101 7c00 5f0b 6400 5300 7407 6a08  j...|._.d.S.t.j.
-00000640: a009 6401 a101 7c00 5f0b 6400 5300 2902  ..d...|._.d.S.).
-00000650: 4e72 0100 0000 290c da05 6d6f 6465 6c72  Nr....)...modelr
-00000660: 1600 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00000670: 0000 0072 1c00 0000 721d 0000 00da 026e  ...r....r......n
-00000680: 70da 0672 616e 646f 6dda 0b64 6566 6175  p..random..defau
-00000690: 6c74 5f72 6e67 da13 676c 6f62 616c 5f72  lt_rng..global_r
-000006a0: 616e 646f 6d5f 7374 6174 65da 1072 616e  andom_state..ran
-000006b0: 646f 6d5f 6765 6e65 7261 746f 7229 07da  dom_generator)..
-000006c0: 0473 656c 6672 1600 0000 7219 0000 0072  .selfr....r....r
-000006d0: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-000006e0: 0000 00a9 0072 2500 0000 fa43 2f68 6f6d  .....r%....C/hom
-000006f0: 652f 7468 6f6d 6173 2f49 6465 6150 726f  e/thomas/IdeaPro
-00000700: 6a65 6374 732f 426c 7565 4361 7374 2f62  jects/BlueCast/b
-00000710: 6c75 6563 6173 742f 6d6c 5f6d 6f64 656c  luecast/ml_model
-00000720: 6c69 6e67 2f78 6762 6f6f 7374 2e70 79da  ling/xgboost.py.
-00000730: 085f 5f69 6e69 745f 5f22 0000 0073 1800  .__init__"...s..
-00000740: 0000 0609 0601 0601 0601 0601 0601 0601  ................
-00000750: 0601 0601 0601 0aff 1204 7a15 5867 626f  ..........z.Xgbo
-00000760: 6f73 744d 6f64 656c 2e5f 5f69 6e69 745f  ostModel.__init_
-00000770: 5fda 0179 da06 7265 7475 726e 6302 0000  _..y..returnc...
-00000780: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000790: 0043 0000 0073 1200 0000 7400 6a01 6401  .C...s....t.j.d.
-000007a0: 7c01 6402 8d02 7d02 7c02 5300 2903 7a29  |.d...}.|.S.).z)
-000007b0: 4361 6c63 756c 6174 6520 636c 6173 7320  Calculate class 
-000007c0: 7765 6967 6874 7320 6f66 2074 6172 6765  weights of targe
-000007d0: 7420 636f 6c75 6d6e 2eda 0862 616c 616e  t column...balan
-000007e0: 6365 6429 0272 0c00 0000 7228 0000 0029  ced).r....r(...)
-000007f0: 0272 0c00 0000 da15 636f 6d70 7574 655f  .r......compute_
-00000800: 7361 6d70 6c65 5f77 6569 6768 7429 0372  sample_weight).r
-00000810: 2400 0000 7228 0000 00da 0f63 6c61 7373  $...r(.....class
-00000820: 6573 5f77 6569 6768 7473 7225 0000 0072  es_weightsr%...r
-00000830: 2500 0000 7226 0000 00da 1763 616c 6375  %...r&.....calcu
-00000840: 6c61 7465 5f63 6c61 7373 5f77 6569 6768  late_class_weigh
-00000850: 7473 3900 0000 7308 0000 0004 0204 0106  ts9...s.........
-00000860: ff04 037a 2458 6762 6f6f 7374 4d6f 6465  ...z$XgboostMode
-00000870: 6c2e 6361 6c63 756c 6174 655f 636c 6173  l.calculate_clas
-00000880: 735f 7765 6967 6874 7363 0100 0000 0000  s_weightsc......
-00000890: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000008a0: 0000 73b4 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
-000008b0: 0064 019d 0283 0101 007c 006a 0373 1a74  .d.......|.j.s.t
-000008c0: 0483 007c 005f 0374 0074 01a0 02a1 009b  ...|._.t.t......
-000008d0: 0064 029d 0283 0101 006e 0974 0074 01a0  .d.......n.t.t..
-000008e0: 02a1 009b 0064 039d 0283 0101 007c 006a  .....d.......|.j
-000008f0: 0573 3474 0683 007c 005f 0574 0074 01a0  .s4t...|._.t.t..
-00000900: 02a1 009b 0064 049d 0283 0101 006e 0974  .....d.......n.t
-00000910: 0074 01a0 02a1 009b 0064 059d 0283 0101  .t.......d......
-00000920: 007c 006a 0773 4f74 0883 007c 005f 0774  .|.j.sOt...|._.t
-00000930: 0074 01a0 02a1 009b 0064 069d 0283 0101  .t.......d......
-00000940: 0064 0853 0074 0074 01a0 02a1 009b 0064  .d.S.t.t.......d
-00000950: 079d 0283 0101 0064 0853 0029 097a 364c  .......d.S.).z6L
-00000960: 6f61 6420 6d75 6c74 6970 6c65 2063 6f6e  oad multiple con
-00000970: 6669 6773 206f 7220 6c6f 6164 2064 6566  figs or load def
-00000980: 6175 6c74 2063 6f6e 6669 6773 2069 6e73  ault configs ins
-00000990: 7465 6164 2e7a 323a 2053 7461 7274 206c  tead.z2: Start l
-000009a0: 6f61 6469 6e67 2065 7869 7374 696e 6720  oading existing 
-000009b0: 6f72 2064 6566 6175 6c74 2063 6f6e 6669  or default confi
-000009c0: 6720 6669 6c65 732e 2e7a 1e3a 204c 6f61  g files..z.: Loa
-000009d0: 6420 6465 6661 756c 7420 5472 6169 6e69  d default Traini
-000009e0: 6e67 436f 6e66 6967 2e7a 203a 2046 6f75  ngConfig.z : Fou
-000009f0: 6e64 2070 726f 7669 6465 6420 5472 6169  nd provided Trai
-00000a00: 6e69 6e67 436f 6e66 6967 2e7a 273a 204c  ningConfig.z': L
-00000a10: 6f61 6420 6465 6661 756c 7420 5867 626f  oad default Xgbo
-00000a20: 6f73 7454 756e 6550 6172 616d 7343 6f6e  ostTuneParamsCon
-00000a30: 6669 672e 7a29 3a20 466f 756e 6420 7072  fig.z): Found pr
-00000a40: 6f76 6964 6564 2058 6762 6f6f 7374 5475  ovided XgboostTu
-00000a50: 6e65 5061 7261 6d73 436f 6e66 6967 2e7a  neParamsConfig.z
-00000a60: 273a 204c 6f61 6420 6465 6661 756c 7420  ': Load default 
-00000a70: 5867 626f 6f73 7446 696e 616c 5061 7261  XgboostFinalPara
-00000a80: 6d43 6f6e 6669 672e 7a29 3a20 466f 756e  mConfig.z): Foun
-00000a90: 6420 7072 6f76 6964 6564 2058 6762 6f6f  d provided Xgboo
-00000aa0: 7374 4669 6e61 6c50 6172 616d 436f 6e66  stFinalParamConf
-00000ab0: 6967 2e4e 2909 7212 0000 0072 0300 0000  ig.N).r....r....
-00000ac0: da06 7574 636e 6f77 7219 0000 0072 0d00  ..utcnowr....r..
-00000ad0: 0000 721a 0000 0072 0f00 0000 721b 0000  ..r....r....r...
-00000ae0: 0072 0e00 0000 a901 7224 0000 0072 2500  .r......r$...r%.
-00000af0: 0000 7225 0000 0072 2600 0000 da10 6368  ..r%...r&.....ch
-00000b00: 6563 6b5f 6c6f 6164 5f63 6f6e 6673 4000  eck_load_confs@.
-00000b10: 0000 731a 0000 0012 0206 0108 0114 0112  ..s.............
-00000b20: 0206 0208 0114 0112 0206 0208 0116 0116  ................
-00000b30: 027a 1d58 6762 6f6f 7374 4d6f 6465 6c2e  .z.XgboostModel.
-00000b40: 6368 6563 6b5f 6c6f 6164 5f63 6f6e 6673  check_load_confs
-00000b50: da07 785f 7472 6169 6eda 0678 5f74 6573  ..x_train..x_tes
-00000b60: 74da 0779 5f74 7261 696e da06 795f 7465  t..y_train..y_te
-00000b70: 7374 6305 0000 0000 0000 0000 0000 0009  stc.............
-00000b80: 0000 0008 0000 0043 0000 0073 9c01 0000  .......C...s....
-00000b90: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
-00000ba0: 0100 7c00 a003 a100 0100 7c00 6a04 7216  ..|.......|.j.r.
-00000bb0: 7c00 6a05 7216 7c00 6a06 731a 7407 6402  |.j.r.|.j.s.t.d.
-00000bc0: 8301 8201 7c00 6a05 6a08 7326 7409 6a0a  ....|.j.j.s&t.j.
-00000bd0: a00b 7409 6a0a 6a0c a101 0100 7c00 6a05  ..t.j.j.....|.j.
-00000be0: 6a0d 7236 7c00 a00e 7c01 7c02 7c03 7c04  j.r6|...|.|.|.|.
-00000bf0: a104 0100 740f 6403 8301 0100 7c00 6a05  ....t.d.....|.j.
-00000c00: 6a10 7246 7c00 a011 7c01 7c02 7c03 7c04  j.rF|...|.|.|.|.
-00000c10: a104 0100 740f 6404 8301 0100 7400 6405  ....t.d.....t.d.
-00000c20: 8301 0100 7c00 6a12 7261 7c00 6a12 a013  ....|.j.ra|.j...
-00000c30: 7c01 7c03 a102 5c02 7d01 7d03 7c00 6a12  |.|...\.}.}.|.j.
-00000c40: 6a14 7c02 7c04 6406 6407 8d03 5c02 7d02  j.|.|.d.d...\.}.
-00000c50: 7d04 7c00 6a05 6a15 727c 7400 7401 a002  }.|.j.j.r|t.t...
-00000c60: a100 9b00 6408 9d02 8301 0100 7416 a017  ....d.......t...
-00000c70: 7c01 7c02 6702 a101 7d01 7416 a017 7c03  |.|.g...}.t...|.
-00000c80: 7c04 6702 a101 7d03 7c00 a018 7c01 7c03  |.g...}.|...|.|.
-00000c90: 7c02 7c04 a104 5c02 7d05 7d06 7c05 6409  |.|...\.}.}.|.d.
-00000ca0: 6602 7c06 640a 6602 6702 7d07 7c00 6a04  f.|.d.f.g.}.|.j.
-00000cb0: 6a19 a01a 640b 640c a102 7d08 7c00 6a05  j...d.d...}.|.j.
-00000cc0: 6a1b 640d 6b02 72b2 7c00 6a1c 72b2 741d  j.d.k.r.|.j.r.t.
-00000cd0: 6a1e 7c00 6a04 6a19 7c05 7c08 7c00 6a05  j.|.j.j.|.|.|.j.
-00000ce0: 6a1f 7c07 7c00 6a1c 6a20 640e 8d06 7c00  j.|.|.j.j d...|.
-00000cf0: 5f21 6e15 7c00 6a1c 72c7 741d 6a1e 7c00  _!n.|.j.r.t.j.|.
-00000d00: 6a04 6a19 7c05 7c08 7c00 6a05 6a1f 7c07  j.j.|.|.|.j.j.|.
-00000d10: 7c00 6a1c 6a20 640e 8d06 7c00 5f21 7400  |.j.j d...|._!t.
-00000d20: 640f 8301 0100 7c00 6a21 5300 2910 7a3f  d.....|.j!S.).z?
-00000d30: 5472 6169 6e20 5867 626f 6f73 7420 6d6f  Train Xgboost mo
-00000d40: 6465 6c2e 2049 6e63 6c75 6465 7320 6879  del. Includes hy
-00000d50: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
-00000d60: 696e 6720 6f6e 2064 6566 6175 6c74 2e7a  ing on default.z
-00000d70: 1e3a 2053 7461 7274 2066 6974 7469 6e67  .: Start fitting
-00000d80: 2058 6762 6f6f 7374 206d 6f64 656c 2efa   Xgboost model..
-00000d90: 4063 6f6e 665f 7061 7261 6d73 5f78 6762  @conf_params_xgb
-00000da0: 6f6f 7374 2c20 636f 6e66 5f74 7261 696e  oost, conf_train
-00000db0: 696e 6720 6f72 2065 7870 6572 696d 656e  ing or experimen
-00000dc0: 745f 7472 6163 6b65 7220 6973 204e 6f6e  t_tracker is Non
-00000dd0: 657a 1e46 696e 6973 6865 6420 6879 7065  ez.Finished hype
-00000de0: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
-00000df0: 677a 2046 696e 6973 6865 6420 4772 6964  gz Finished Grid
-00000e00: 2073 6561 7263 6820 6669 6e65 2074 756e   search fine tun
-00000e10: 696e 677a 1a53 7461 7274 2066 696e 616c  ingz.Start final
-00000e20: 206d 6f64 656c 2074 7261 696e 696e 6746   model trainingF
-00000e30: a901 da0e 7072 6564 6963 746f 6e5f 6d6f  ....predicton_mo
-00000e40: 6465 7a7f 3a20 556e 696f 6e20 7472 6169  dez.: Union trai
-00000e50: 6e20 616e 6420 7465 7374 2064 6174 6120  n and test data 
-00000e60: 666f 7220 6669 6e61 6c20 6d6f 6465 6c20  for final model 
-00000e70: 7472 6169 6e69 6e67 2062 6173 6564 206f  training based o
-00000e80: 6e20 5472 6169 6e69 6e67 436f 6e66 6967  n TrainingConfig
-00000e90: 0a20 2020 2020 2020 2020 2020 2020 7061  .             pa
-00000ea0: 7261 6d20 2775 7365 5f66 756c 6c5f 6461  ram 'use_full_da
-00000eb0: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
-00000ec0: 656c 27da 0574 7261 696e da04 7465 7374  el'..train..test
-00000ed0: da05 7374 6570 73e9 2c01 0000 e901 0000  ..steps.,.......
-00000ee0: 00a9 04da 0f6e 756d 5f62 6f6f 7374 5f72  .....num_boost_r
-00000ef0: 6f75 6e64 da15 6561 726c 795f 7374 6f70  ound..early_stop
-00000f00: 7069 6e67 5f72 6f75 6e64 73da 0565 7661  ping_rounds..eva
-00000f10: 6c73 da0c 7665 7262 6f73 655f 6576 616c  ls..verbose_eval
-00000f20: 7a11 4669 6e69 7368 6564 2074 7261 696e  z.Finished train
-00000f30: 696e 6729 2272 1200 0000 7203 0000 0072  ing)"r....r....r
-00000f40: 2e00 0000 7230 0000 0072 1b00 0000 7219  ....r0...r....r.
-00000f50: 0000 0072 1c00 0000 da0a 5661 6c75 6545  ...r......ValueE
-00000f60: 7272 6f72 da19 7368 6f77 5f64 6574 6169  rror..show_detai
-00000f70: 6c65 645f 7475 6e69 6e67 5f6c 6f67 73da  led_tuning_logs.
-00000f80: 066f 7074 756e 61da 076c 6f67 6769 6e67  .optuna..logging
-00000f90: 5a0d 7365 745f 7665 7262 6f73 6974 79da  Z.set_verbosity.
-00000fa0: 0757 4152 4e49 4e47 da0e 6175 746f 7475  .WARNING..autotu
-00000fb0: 6e65 5f6d 6f64 656c da08 6175 746f 7475  ne_model..autotu
-00000fc0: 6e65 da05 7072 696e 74da 1e65 6e61 626c  ne..print..enabl
-00000fd0: 655f 6772 6964 5f73 6561 7263 685f 6669  e_grid_search_fi
-00000fe0: 6e65 5f74 756e 696e 67da 0966 696e 655f  ne_tuning..fine_
-00000ff0: 7475 6e65 721d 0000 00da 0d66 6974 5f74  tuner......fit_t
-00001000: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
-00001010: 6f72 6dda 1d75 7365 5f66 756c 6c5f 6461  orm..use_full_da
-00001020: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
-00001030: 656c da02 7064 da06 636f 6e63 6174 da11  el..pd..concat..
-00001040: 6372 6561 7465 5f64 5f6d 6174 7269 6365  create_d_matrice
-00001050: 73da 0670 6172 616d 73da 0370 6f70 da14  s..params..pop..
-00001060: 6879 7065 7274 756e 696e 675f 6376 5f66  hypertuning_cv_f
-00001070: 6f6c 6473 721a 0000 00da 0378 6762 7238  oldsr......xgbr8
-00001080: 0000 0072 3f00 0000 da25 7665 7262 6f73  ...r?....%verbos
-00001090: 6974 795f 6475 7269 6e67 5f66 696e 616c  ity_during_final
-000010a0: 5f6d 6f64 656c 5f74 7261 696e 696e 6772  _model_trainingr
-000010b0: 1e00 0000 2909 7224 0000 0072 3100 0000  ....).r$...r1...
-000010c0: 7232 0000 0072 3300 0000 7234 0000 00da  r2...r3...r4....
-000010d0: 0764 5f74 7261 696e da06 645f 7465 7374  .d_train..d_test
-000010e0: da08 6576 616c 5f73 6574 723a 0000 0072  ..eval_setr:...r
-000010f0: 2500 0000 7225 0000 0072 2600 0000 da03  %...r%...r&.....
-00001100: 6669 7455 0000 0073 7000 0000 1208 0801  fitU...sp.......
-00001110: 0403 02ff 0402 02fe 0403 02fd 0205 0201  ................
-00001120: 04ff 0804 1001 0802 1001 0801 0802 1001  ................
-00001130: 0801 0802 0601 0601 0401 08ff 0603 0601  ................
-00001140: 0aff 0804 0201 0c01 04ff 0e04 0e01 1402  ................
-00001150: 1001 1002 1202 0401 0601 0201 0201 0601  ................
-00001160: 0201 0601 0afa 0608 0401 0601 0201 0201  ................
-00001170: 0601 0201 0601 08fa 0808 0601 7a10 5867  ............z.Xg
-00001180: 626f 6f73 744d 6f64 656c 2e66 6974 6305  boostModel.fitc.
-00001190: 0000 0000 0000 0000 0000 000b 0000 000f  ................
-000011a0: 0000 0003 0000 0073 ba01 0000 7400 7401  .......s....t.t.
-000011b0: a002 a100 9b00 6401 9d02 8301 0100 8800  ......d.........
-000011c0: 6a03 7212 8800 6a04 7212 8800 6a05 7316  j.r...j.r...j.s.
-000011d0: 7406 6402 8301 8201 7407 8300 8901 8800  t.d.....t.......
-000011e0: a008 a100 0100 8800 6a03 7229 8800 6a04  ........j.r)..j.
-000011f0: 7229 8800 6a09 7229 8800 6a05 732d 7406  r)..j.r)..j.s-t.
-00001200: 6403 8301 8201 8700 8701 8702 8703 8704  d...............
-00001210: 8705 6606 6404 6405 8408 7d05 6406 7d06  ..f.d.d...}.d.}.
-00001220: 740a 6a0b 6a0c 6407 8800 6a04 6a0d 8800  t.j.j.d...j.j...
-00001230: 6a04 6a0e 6408 8d03 7d07 740a 6a0f 6409  j.j.d...}.t.j.d.
-00001240: 7c07 7c06 9b00 640a 9d02 640b 8d03 7d08  |.|...d...d...}.
-00001250: 7c08 6a10 7c05 8800 6a04 6a11 8800 6a04  |.j.|...j.j...j.
-00001260: 6a12 6407 6407 640c 8d05 0100 7a16 740a  j.d.d.d.....z.t.
-00001270: 6a13 a014 7c08 a101 7d09 7c09 a015 a100  j...|...}.|.....
-00001280: 0100 740a 6a13 a016 7c08 a101 7d09 7c09  ..t.j...|...}.|.
-00001290: a015 a100 0100 5700 6e0c 0400 7417 7418  ......W.n...t.t.
-000012a0: 7406 6603 7982 0100 0100 0100 5900 6e01  t.f.y.......Y.n.
-000012b0: 7700 7c08 6a19 6a1a 7d0a 8800 6a04 6a1b  w.|.j.j.}...j.j.
-000012c0: 640d 6b04 7293 7c0a 640e 1900 8800 6a04  d.k.r.|.d.....j.
-000012d0: 5f0d 8800 6a09 6a1c 8800 6a09 6a1d 8800  _...j.j...j.j...
-000012e0: 6a09 6a1e 8805 a01f a100 7c0a 640f 1900  j.j.......|.d...
-000012f0: 7c0a 6410 1900 7c0a 6411 1900 7c0a 6412  |.d...|.d...|.d.
-00001300: 1900 7c0a 6413 1900 7c0a 6414 1900 7c0a  ..|.d...|.d...|.
-00001310: 6415 1900 7c0a 6416 1900 7c0a 6417 1900  d...|.d...|.d...
-00001320: 7c0a 6418 1900 6419 9c0e 8800 6a03 5f1a  |.d...d.....j._.
-00001330: 6900 8800 6a03 6a1a a501 8801 a501 8800  i...j.j.........
-00001340: 6a03 5f1a 7400 641a 8800 6a03 6a1a 9b00  j._.t.d...j.j...
-00001350: 9d02 8301 0100 7c0a 641b 1900 8800 6a03  ......|.d.....j.
-00001360: 5f20 641c 5300 291d 7a7b 5475 6e65 2068  _ d.S.).z{Tune h
-00001370: 7970 6572 7061 7261 6d65 7465 7273 2e0a  yperparameters..
-00001380: 0a20 2020 2020 2020 2041 6e20 616c 7465  .        An alte
-00001390: 726e 6174 6976 6520 636f 6e66 6967 2063  rnative config c
-000013a0: 616e 2062 6520 7072 6f76 6964 6564 2074  an be provided t
-000013b0: 6f20 6f76 6572 7772 6974 6520 7468 6520  o overwrite the 
-000013c0: 6879 7065 7270 6172 616d 6574 6572 2073  hyperparameter s
-000013d0: 6561 7263 6820 7370 6163 652e 0a20 2020  earch space..   
-000013e0: 2020 2020 207a 2f3a 2053 7461 7274 2068       z/: Start h
-000013f0: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
-00001400: 6e69 6e67 206f 6620 5867 626f 6f73 7420  ning of Xgboost 
-00001410: 6d6f 6465 6c2e 7235 0000 00fa 4f41 7420  model.r5....OAt 
-00001420: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
-00001430: 2063 6f6e 6669 6773 206f 7220 6578 7065   configs or expe
-00001440: 7269 6d65 6e74 5f74 7261 636b 6572 2069  riment_tracker i
-00001450: 7320 4e6f 6e65 2c20 7768 6963 6820 6973  s None, which is
-00001460: 206e 6f74 2061 6c6c 6f77 6564 6301 0000   not allowedc...
-00001470: 0000 0000 0000 0000 000c 0000 0013 0000  ................
-00001480: 0013 0000 0073 9402 0000 8800 6a00 6a01  .....s......j.j.
-00001490: 8800 6a00 6a02 8800 6a00 6a03 8805 a004  ..j.j...j.j.....
-000014a0: a100 7c00 6a05 6401 8800 6a00 6a06 8800  ..|.j.d...j.j...
-000014b0: 6a00 6a07 6402 6403 8d04 7c00 6a08 6404  j.j.d.d...|.j.d.
-000014c0: 8800 6a00 6a09 8800 6a00 6a0a 6402 6403  ..j.j...j.j.d.d.
-000014d0: 8d04 7c00 6a05 6405 8800 6a00 6a0b 8800  ..|.j.d...j.j...
-000014e0: 6a00 6a0c 6402 6403 8d04 7c00 6a05 6406  j.j.d.d...|.j.d.
-000014f0: 8800 6a00 6a0d 8800 6a00 6a0e 6402 6403  ..j.j...j.j.d.d.
-00001500: 8d04 7c00 6a05 6407 8800 6a00 6a0f 8800  ..|.j.d...j.j...
-00001510: 6a00 6a10 6402 6403 8d04 7c00 a008 6408  j.j.d.d...|...d.
-00001520: 8800 6a00 6a11 8800 6a00 6a12 a103 7c00  ..j.j...j.j...|.
-00001530: a005 6409 8800 6a00 6a13 8800 6a00 6a14  ..d...j.j...j.j.
-00001540: a103 7c00 a005 640a 8800 6a00 6a15 8800  ..|...d...j.j...
-00001550: 6a00 6a16 a103 7c00 a005 640b 8800 6a00  j.j...|...d...j.
-00001560: 6a17 8800 6a00 6a18 a103 7c00 6a08 640c  j...j.j...|.j.d.
-00001570: 8800 6a00 6a19 8800 6a00 6a1a 6402 6403  ..j.j...j.j.d.d.
-00001580: 8d04 640d 9c0e 7d01 6900 7c01 a501 8801  ..d...}.i.|.....
-00001590: a501 7d01 7c00 a01b 640e 6402 640f 6702  ..}.|...d.d.d.g.
-000015a0: a102 7d02 7c02 72a0 8800 a01c 8805 a101  ..}.|.r.........
-000015b0: 7d03 741d 6a1e 8803 8805 7c03 8800 6a1f  }.t.j.....|...j.
-000015c0: 6a20 6410 8d04 7d04 6e0a 741d 6a1e 8803  j d...}.n.t.j...
-000015d0: 8805 8800 6a1f 6a20 6411 8d03 7d04 741d  ....j.j d...}.t.
-000015e0: 6a1e 8802 8804 8800 6a1f 6a20 6411 8d03  j.......j.j d...
-000015f0: 7d05 7421 6a22 a023 7c00 6412 a102 7d06  }.t!j".#|.d...}.
-00001600: 7c01 a024 640c 6413 a102 7d07 8800 6a1f  |..$d.d...}...j.
-00001610: 6a25 6414 6b02 72d1 8800 a026 7c04 7c05  j%d.k.r....&|.|.
-00001620: 8804 7c01 7c07 7c06 a106 5300 8800 6a1f  ..|.|.|...S...j.
-00001630: 6a25 6414 6b04 72f4 8800 6a1f 6a27 72f4  j%d.k.r...j.j'r.
-00001640: 7c00 a01b 6415 8700 6601 6416 6417 8408  |...d...f.d.d...
-00001650: 7428 6418 8301 4400 8301 a102 7d08 8800  t(d...D.....}...
-00001660: a029 7c01 8803 8805 8802 8804 7c08 a106  .)|.........|...
-00001670: 5300 7c00 a01b 6415 8700 6601 6419 6417  S.|...d...f.d.d.
-00001680: 8408 7428 6418 8301 4400 8301 a102 7d08  ..t(d...D.....}.
-00001690: 741d 6a2a 7c01 7c04 7c07 8800 6a1f 6a2b  t.j*|.|.|...j.j+
-000016a0: 8800 6a1f 6a25 6402 7c08 7c06 6701 8800  ..j.j%d.|.|.g...
-000016b0: 6a1f 6a2c 641a 8d09 7d09 7c09 641b 1900  j.j,d...}.|.d...
-000016c0: a02d a100 7c09 641b 1900 a02e a100 641c  .-..|.d.......d.
-000016d0: 1300 1700 7d0a 742f 8800 6a30 6a31 8301  ....}.t/..j0j1..
-000016e0: 641d 6b02 9001 7232 641d 7d0b 6e08 8800  d.k...r2d.}.n...
-000016f0: 6a30 6a31 641e 1900 6414 1700 7d0b 8800  j0j1d...d...}...
-00001700: 6a30 6a32 7c0b 641f 8800 6a1f 7c01 7c0a  j0j2|.d...j.|.|.
-00001710: 6420 640f 6421 8d07 0100 7c0a 5300 2922  d d.d!....|.S.)"
-00001720: 4eda 0365 7461 54a9 01da 036c 6f67 da09  N..etaT....log..
-00001730: 6d61 785f 6465 7074 68da 0561 6c70 6861  max_depth..alpha
-00001740: da06 6c61 6d62 6461 da05 6761 6d6d 61da  ..lambda..gamma.
-00001750: 0a6d 6178 5f6c 6561 7665 73da 0973 7562  .max_leaves..sub
-00001760: 7361 6d70 6c65 da10 636f 6c73 616d 706c  sample..colsampl
-00001770: 655f 6279 7472 6565 da11 636f 6c73 616d  e_bytree..colsam
-00001780: 706c 655f 6279 6c65 7665 6c72 3a00 0000  ple_bylevelr:...
-00001790: 290e da09 6f62 6a65 6374 6976 65da 0762  )...objective..b
-000017a0: 6f6f 7374 6572 da0b 6576 616c 5f6d 6574  ooster..eval_met
-000017b0: 7269 63da 096e 756d 5f63 6c61 7373 725c  ric..num_classr\
-000017c0: 0000 0072 5f00 0000 7260 0000 0072 6100  ...r_...r`...ra.
-000017d0: 0000 7262 0000 0072 6300 0000 7264 0000  ..rb...rc...rd..
-000017e0: 0072 6500 0000 7266 0000 0072 3a00 0000  .re...rf...r:...
-000017f0: da0d 7361 6d70 6c65 5f77 6569 6768 7446  ..sample_weightF
-00001800: a903 da05 6c61 6265 6cda 0677 6569 6768  ....label..weigh
-00001810: 74da 1265 6e61 626c 655f 6361 7465 676f  t..enable_catego
-00001820: 7269 6361 6ca9 0272 6d00 0000 726f 0000  rical..rm...ro..
-00001830: 00fa 0d74 6573 742d 6d6c 6f67 6c6f 7373  ...test-mlogloss
-00001840: 723b 0000 0072 3c00 0000 da0b 7261 6e64  r;...r<.....rand
-00001850: 6f6d 5f73 6565 6463 0100 0000 0000 0000  om_seedc........
-00001860: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-00001870: f318 0000 0067 007c 005d 087d 0188 006a  .....g.|.].}...j
-00001880: 006a 017c 0117 0091 0271 0253 0072 2500  .j.|.....q.S.r%.
-00001890: 0000 a902 7219 0000 0072 2200 0000 a902  ....r....r".....
-000018a0: da02 2e30 da01 6972 2f00 0000 7225 0000  ...0..ir/...r%..
-000018b0: 0072 2600 0000 da0a 3c6c 6973 7463 6f6d  .r&.....<listcom
-000018c0: 703e 2801 0000 f302 0000 0018 007a 3c58  p>(..........z<X
-000018d0: 6762 6f6f 7374 4d6f 6465 6c2e 6175 746f  gboostModel.auto
-000018e0: 7475 6e65 2e3c 6c6f 6361 6c73 3e2e 6f62  tune.<locals>.ob
-000018f0: 6a65 6374 6976 652e 3c6c 6f63 616c 733e  jective.<locals>
-00001900: 2e3c 6c69 7374 636f 6d70 3ee9 6400 0000  .<listcomp>.d...
-00001910: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001920: 0004 0000 0013 0000 0072 7300 0000 7225  .........rs...r%
-00001930: 0000 0072 7400 0000 7275 0000 0072 2f00  ...rt...ru...r/.
-00001940: 0000 7225 0000 0072 2600 0000 7278 0000  ..r%...r&...rx..
-00001950: 0031 0100 0072 7900 0000 a909 7252 0000  .1...ry.....rR..
-00001960: 00da 0664 7472 6169 6e72 3e00 0000 723f  ...dtrainr>...r?
-00001970: 0000 00da 056e 666f 6c64 da09 6173 5f70  .....nfold..as_p
-00001980: 616e 6461 73da 0473 6565 64da 0963 616c  andas..seed..cal
-00001990: 6c62 6163 6b73 da07 7368 7566 666c 65fa  lbacks..shuffle.
-000019a0: 1274 6573 742d 6d6c 6f67 6c6f 7373 2d6d  .test-mlogloss-m
-000019b0: 6561 6ee7 6666 6666 6666 e63f 7201 0000  ean.ffffff.?r...
-000019c0: 00e9 ffff ffff da08 6376 5f73 636f 7265  ........cv_score
-000019d0: fa13 6164 6a75 7374 6564 206d 6c20 6c6f  ..adjusted ml lo
-000019e0: 676c 6f73 73a9 07da 0d65 7870 6572 696d  gloss....experim
-000019f0: 656e 745f 6964 da0e 7363 6f72 655f 6361  ent_id..score_ca
-00001a00: 7465 676f 7279 da0f 7472 6169 6e69 6e67  tegory..training
-00001a10: 5f63 6f6e 6669 67da 106d 6f64 656c 5f70  _config..model_p
-00001a20: 6172 616d 6574 6572 73da 0b65 7661 6c5f  arameters..eval_
-00001a30: 7363 6f72 6573 da0b 6d65 7472 6963 5f75  scores..metric_u
-00001a40: 7365 64da 176d 6574 7269 635f 6869 6768  sed..metric_high
-00001a50: 6572 5f69 735f 6265 7474 6572 2933 721a  er_is_better)3r.
-00001a60: 0000 00da 1178 6762 6f6f 7374 5f6f 626a  .....xgboost_obj
-00001a70: 6563 7469 7665 7268 0000 00da 1378 6762  ectiverh.....xgb
-00001a80: 6f6f 7374 5f65 7661 6c5f 6d65 7472 6963  oost_eval_metric
-00001a90: da07 6e75 6e69 7175 65da 0d73 7567 6765  ..nunique..sugge
-00001aa0: 7374 5f66 6c6f 6174 da07 6574 615f 6d69  st_float..eta_mi
-00001ab0: 6eda 0765 7461 5f6d 6178 5a0b 7375 6767  n..eta_maxZ.sugg
-00001ac0: 6573 745f 696e 74da 0d6d 6178 5f64 6570  est_int..max_dep
-00001ad0: 7468 5f6d 696e da0d 6d61 785f 6465 7074  th_min..max_dept
-00001ae0: 685f 6d61 78da 0961 6c70 6861 5f6d 696e  h_max..alpha_min
-00001af0: da09 616c 7068 615f 6d61 78da 0a6c 616d  ..alpha_max..lam
-00001b00: 6264 615f 6d69 6eda 0a6c 616d 6264 615f  bda_min..lambda_
-00001b10: 6d61 78da 0967 616d 6d61 5f6d 696e da09  max..gamma_min..
-00001b20: 6761 6d6d 615f 6d61 78da 0e6d 6178 5f6c  gamma_max..max_l
-00001b30: 6561 7665 735f 6d69 6eda 0e6d 6178 5f6c  eaves_min..max_l
-00001b40: 6561 7665 735f 6d61 78da 0e73 7562 5f73  eaves_max..sub_s
-00001b50: 616d 706c 655f 6d69 6eda 0e73 7562 5f73  ample_min..sub_s
-00001b60: 616d 706c 655f 6d61 78da 1663 6f6c 5f73  ample_max..col_s
-00001b70: 616d 706c 655f 6279 5f74 7265 655f 6d69  ample_by_tree_mi
-00001b80: 6eda 1663 6f6c 5f73 616d 706c 655f 6279  n..col_sample_by
-00001b90: 5f74 7265 655f 6d61 78da 1763 6f6c 5f73  _tree_max..col_s
-00001ba0: 616d 706c 655f 6279 5f6c 6576 656c 5f6d  ample_by_level_m
-00001bb0: 696e da17 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
-00001bc0: 795f 6c65 7665 6c5f 6d61 78da 0973 7465  y_level_max..ste
-00001bd0: 7073 5f6d 696e da09 7374 6570 735f 6d61  ps_min..steps_ma
-00001be0: 785a 1373 7567 6765 7374 5f63 6174 6567  xZ.suggest_categ
-00001bf0: 6f72 6963 616c 722d 0000 0072 5500 0000  oricalr-...rU...
-00001c00: da07 444d 6174 7269 7872 1900 0000 da1d  ..DMatrixr......
-00001c10: 6361 745f 656e 636f 6469 6e67 5f76 6961  cat_encoding_via
-00001c20: 5f6d 6c5f 616c 676f 7269 7468 6d72 4400  _ml_algorithmrD.
-00001c30: 0000 da0b 696e 7465 6772 6174 696f 6eda  ....integration.
-00001c40: 1658 4742 6f6f 7374 5072 756e 696e 6743  .XGBoostPruningC
-00001c50: 616c 6c62 6163 6b72 5300 0000 7254 0000  allbackrS...rT..
-00001c60: 00da 1774 7261 696e 5f73 696e 676c 655f  ...train_single_
-00001c70: 666f 6c64 5f6d 6f64 656c da11 7072 6563  fold_model..prec
-00001c80: 6973 655f 6376 5f74 756e 696e 67da 0572  ise_cv_tuning..r
-00001c90: 616e 6765 da12 5f66 696e 655f 7475 6e65  ange.._fine_tune
-00001ca0: 5f70 7265 6369 7365 da02 6376 723f 0000  _precise..cvr?..
-00001cb0: 00da 1773 6875 6666 6c65 5f64 7572 696e  ...shuffle_durin
-00001cc0: 675f 7472 6169 6e69 6e67 da04 6d65 616e  g_training..mean
-00001cd0: da03 7374 64da 036c 656e 721c 0000 0072  ..std..lenr....r
-00001ce0: 8800 0000 da0b 6164 645f 7265 7375 6c74  ......add_result
-00001cf0: 7329 0cda 0574 7269 616c da05 7061 7261  s)...trial..para
-00001d00: 6d72 6b00 0000 722c 0000 0072 5700 0000  mrk...r,...rW...
-00001d10: 7258 0000 00da 1070 7275 6e69 6e67 5f63  rX.....pruning_c
-00001d20: 616c 6c62 6163 6b72 3a00 0000 7272 0000  allbackr:...rr..
-00001d30: 00da 0672 6573 756c 74da 0e61 646a 7573  ...result..adjus
-00001d40: 7465 645f 7363 6f72 65da 066e 6577 5f69  ted_score..new_i
-00001d50: 64a9 0672 2400 0000 5a08 7472 6169 6e5f  d..r$...Z.train_
-00001d60: 6f6e 7232 0000 0072 3100 0000 7234 0000  onr2...r1...r4..
-00001d70: 0072 3300 0000 7225 0000 0072 2600 0000  .r3...r%...r&...
-00001d80: 7267 0000 00c2 0000 0073 0401 0000 0602  rg.......s......
-00001d90: 0601 0601 0601 0401 0201 0601 0601 0201  ................
-00001da0: 04fc 0406 0201 0601 0601 0201 04fc 0406  ................
-00001db0: 0201 0601 0601 0201 04fc 0406 0201 0601  ................
-00001dc0: 0601 0201 04fc 0406 0201 0601 0601 0201  ................
-00001dd0: 04fc 0406 0201 0601 0601 02fd 0405 0201  ................
-00001de0: 0601 0601 02fd 0405 0201 0601 0601 02fd  ................
-00001df0: 0405 0201 0601 0601 02fd 0405 0201 0601  ................
-00001e00: 0601 0201 04fc 06c9 0c3e 1001 0401 0a01  .........>......
-00001e10: 0401 0201 0201 0201 0601 08fc 0407 0201  ................
-00001e20: 0201 0601 06fd 0406 0201 0201 0601 06fd  ................
-00001e30: 0606 0401 04ff 0c04 0c02 0401 0c01 04ff  ................
-00001e40: 0c04 0601 02ff 0403 0201 1401 04fe 0405  ................
-00001e50: 0c01 04ff 0404 0201 1401 04fe 0404 0201  ................
-00001e60: 0201 0201 0601 0601 0201 0201 0401 0601  ................
-00001e70: 06f7 0a0c 0e01 04ff 1205 0601 1002 0601  ................
-00001e80: 0201 0201 0401 0201 0201 0201 0201 06f9  ................
-00001e90: 040a 7a28 5867 626f 6f73 744d 6f64 656c  ..z(XgboostModel
-00001ea0: 2e61 7574 6f74 756e 652e 3c6c 6f63 616c  .autotune.<local
-00001eb0: 733e 2e6f 626a 6563 7469 7665 da07 7867  s>.objective..xg
-00001ec0: 626f 6f73 7454 2903 5a0c 6d75 6c74 6976  boostT).Z.multiv
-00001ed0: 6172 6961 7465 727f 0000 005a 106e 5f73  ariater....Z.n_s
-00001ee0: 7461 7274 7570 5f74 7269 616c 73da 086d  tartup_trials..m
-00001ef0: 696e 696d 697a 657a 0720 7475 6e69 6e67  inimizez. tuning
-00001f00: 2903 da09 6469 7265 6374 696f 6eda 0773  )...direction..s
-00001f10: 616d 706c 6572 5a0a 7374 7564 795f 6e61  amplerZ.study_na
-00001f20: 6d65 a904 da08 6e5f 7472 6961 6c73 da07  me....n_trials..
-00001f30: 7469 6d65 6f75 745a 0e67 635f 6166 7465  timeoutZ.gc_afte
-00001f40: 725f 7472 6961 6c5a 1173 686f 775f 7072  r_trialZ.show_pr
-00001f50: 6f67 7265 7373 5f62 6172 723c 0000 0072  ogress_barr<...r
-00001f60: 7200 0000 725f 0000 0072 6000 0000 7261  r...r_...r`...ra
-00001f70: 0000 0072 6200 0000 7263 0000 0072 6400  ...rb...rc...rd.
-00001f80: 0000 7265 0000 0072 6600 0000 725c 0000  ..re...rf...r\..
-00001f90: 0072 3a00 0000 290e 7267 0000 0072 6800  .r:...).rg...rh.
-00001fa0: 0000 7269 0000 0072 6a00 0000 725f 0000  ..ri...rj...r_..
-00001fb0: 0072 6000 0000 7261 0000 0072 6200 0000  .r`...ra...rb...
-00001fc0: 7263 0000 0072 6400 0000 7265 0000 0072  rc...rd...re...r
-00001fd0: 6600 0000 725c 0000 0072 3a00 0000 fa0d  f...r\...r:.....
-00001fe0: 4265 7374 2070 6172 616d 733a 2072 6b00  Best params: rk.
-00001ff0: 0000 4e29 2172 1200 0000 7203 0000 0072  ..N)!r....r....r
-00002000: 2e00 0000 721b 0000 0072 1900 0000 721c  ....r....r....r.
-00002010: 0000 0072 4200 0000 7211 0000 0072 3000  ...rB...r....r0.
-00002020: 0000 721a 0000 0072 4400 0000 da08 7361  ..r....rD.....sa
-00002030: 6d70 6c65 7273 5a0a 5450 4553 616d 706c  mplersZ.TPESampl
-00002040: 6572 7222 0000 00da 1f6f 7074 756e 615f  err".....optuna_
-00002050: 7361 6d70 6c65 725f 6e5f 7374 6172 7475  sampler_n_startu
-00002060: 705f 7472 6961 6c73 da0c 6372 6561 7465  p_trials..create
-00002070: 5f73 7475 6479 da08 6f70 7469 6d69 7a65  _study..optimize
-00002080: da1c 6879 7065 7270 6172 616d 6574 6572  ..hyperparameter
-00002090: 5f74 756e 696e 675f 726f 756e 6473 da26  _tuning_rounds.&
-000020a0: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
-000020b0: 756e 696e 675f 6d61 785f 7275 6e74 696d  uning_max_runtim
-000020c0: 655f 7365 6373 da0d 7669 7375 616c 697a  e_secs..visualiz
-000020d0: 6174 696f 6eda 1970 6c6f 745f 6f70 7469  ation..plot_opti
-000020e0: 6d69 7a61 7469 6f6e 5f68 6973 746f 7279  mization_history
-000020f0: da04 7368 6f77 da16 706c 6f74 5f70 6172  ..show..plot_par
-00002100: 616d 5f69 6d70 6f72 7461 6e63 6573 da11  am_importances..
-00002110: 5a65 726f 4469 7669 7369 6f6e 4572 726f  ZeroDivisionErro
-00002120: 72da 0c52 756e 7469 6d65 4572 726f 72da  r..RuntimeError.
-00002130: 0a62 6573 745f 7472 6961 6c72 5200 0000  .best_trialrR...
-00002140: 7254 0000 0072 8f00 0000 7268 0000 0072  rT...r....rh...r
-00002150: 9000 0000 7291 0000 0072 6b00 0000 290b  ....r....rk...).
-00002160: 7224 0000 0072 3100 0000 7232 0000 0072  r$...r1...r2...r
-00002170: 3300 0000 7234 0000 0072 6700 0000 da09  3...r4...rg.....
-00002180: 616c 676f 7269 7468 6d72 bf00 0000 da05  algorithmr......
-00002190: 7374 7564 79da 0366 6967 5a12 7867 626f  study..figZ.xgbo
-000021a0: 6f73 745f 6265 7374 5f70 6172 616d 7225  ost_best_paramr%
-000021b0: 0000 0072 bb00 0000 7226 0000 0072 4800  ...r....r&...rH.
-000021c0: 0000 9f00 0000 73a0 0000 0012 0b04 0202  ......s.........
-000021d0: ff04 0202 fe04 0302 fd02 0502 0104 ff06  ................
-000021e0: 0408 0204 0302 ff04 0202 fe04 0302 fd04  ................
-000021f0: 0402 fc02 0602 0104 ff16 0400 7f04 1306  ................
-00002200: 0102 0106 0106 0106 fd04 0502 0102 0108  ................
-00002210: 0106 fd04 0602 0106 0106 0102 0102 0106  ................
-00002220: fb02 070c 0108 0106 0102 0104 ff0c 0312  ................
-00002230: 0104 0102 ff08 030c 010c 0106 0306 0106  ................
-00002240: 0106 0102 0102 0102 ff06 0306 0106 0106  ................
-00002250: 0106 0106 0106 0106 0106 010a f002 1206  ................
-00002260: 0102 ff02 0208 fe12 0410 017a 1558 6762  ...........z.Xgb
-00002270: 6f6f 7374 4d6f 6465 6c2e 6175 746f 7475  oostModel.autotu
-00002280: 6e65 6301 0000 0000 0000 0000 0000 0002  nec.............
-00002290: 0000 0003 0000 0043 0000 0073 5e00 0000  .......C...s^...
-000022a0: 7c00 6a00 6a01 7217 7c00 6a00 6a02 6401  |.j.j.r.|.j.j.d.
-000022b0: 6b02 730e 7c00 6a00 6a03 7217 7c00 6a04  k.s.|.j.j.r.|.j.
-000022c0: 6a05 6402 6403 8d01 7d01 7c01 5300 7c00  j.d.d...}.|.S.|.
-000022d0: 6a00 6a01 722a 7c00 6a00 6a02 6401 6b04  j.j.r*|.j.j.d.k.
-000022e0: 722a 7c00 6a04 6a05 6404 6403 8d01 7d01  r*|.j.j.d.d...}.
-000022f0: 7c01 5300 7406 6a07 7d01 7c01 5300 2905  |.S.t.j.}.|.S.).
-00002300: 4e72 3c00 0000 da0f 6d61 7474 6865 775f  Nr<.....matthew_
-00002310: 696e 7665 7273 6529 01da 0d74 6172 6765  inverse)...targe
-00002320: 745f 6d65 7472 6963 7286 0000 0029 0872  t_metricr....).r
-00002330: 1900 0000 7247 0000 0072 5400 0000 72ac  ....rG...rT...r.
-00002340: 0000 0072 1c00 0000 da0e 6765 745f 6265  ...r......get_be
-00002350: 7374 5f73 636f 7265 721f 0000 00da 0369  st_scorer......i
-00002360: 6e66 2902 7224 0000 00da 1262 6573 745f  nf).r$.....best_
-00002370: 7363 6f72 655f 6376 5f67 7269 6472 2500  score_cv_gridr%.
-00002380: 0000 7225 0000 0072 2600 0000 72d6 0000  ..r%...r&...r...
-00002390: 008e 0100 0073 2200 0000 0801 0c01 0601  .....s".........
-000023a0: 02ff 0603 0201 06ff 040c 06f8 02ff 0c02  ................
-000023b0: 0602 0201 06ff 0405 06ff 0401 7a1b 5867  ............z.Xg
-000023c0: 626f 6f73 744d 6f64 656c 2e67 6574 5f62  boostModel.get_b
-000023d0: 6573 745f 7363 6f72 6563 0500 0000 0000  est_scorec......
-000023e0: 0000 0000 0000 0800 0000 0600 0000 4300  ..............C.
-000023f0: 0000 735a 0000 007c 006a 006a 0172 157c  ..sZ...|.j.j.r.|
-00002400: 00a0 027c 02a1 017d 0574 036a 047c 017c  ...|...}.t.j.|.|
-00002410: 027c 057c 006a 056a 0664 018d 047d 066e  .|.|.j.j.d...}.n
-00002420: 0a74 036a 047c 017c 027c 006a 056a 0664  .t.j.|.|.|.j.j.d
-00002430: 028d 037d 0674 036a 047c 037c 047c 006a  ...}.t.j.|.|.|.j
-00002440: 056a 0664 028d 037d 077c 067c 0766 0253  .j.d...}.|.|.f.S
-00002450: 0029 034e 726c 0000 0072 7000 0000 2907  .).Nrl...rp...).
-00002460: 721b 0000 0072 6b00 0000 722d 0000 0072  r....rk...r-...r
-00002470: 5500 0000 72a7 0000 0072 1900 0000 72a8  U...r....r....r.
-00002480: 0000 0029 0872 2400 0000 7231 0000 0072  ...).r$...r1...r
-00002490: 3300 0000 7232 0000 0072 3400 0000 722c  3...r2...r4...r,
-000024a0: 0000 0072 5700 0000 7258 0000 0072 2500  ...rW...rX...r%.
-000024b0: 0000 7225 0000 0072 2600 0000 7251 0000  ..r%...r&...rQ..
-000024c0: 00a1 0100 0073 2600 0000 0801 0a01 0401  .....s&.........
-000024d0: 0201 0201 0201 0601 08fc 0407 0201 0201  ................
-000024e0: 0601 06fd 0405 0201 0201 0601 06fd 0805  ................
-000024f0: 7a1e 5867 626f 6f73 744d 6f64 656c 2e63  z.XgboostModel.c
-00002500: 7265 6174 655f 645f 6d61 7472 6963 6573  reate_d_matrices
-00002510: 6307 0000 0000 0000 0000 0000 000d 0000  c...............
-00002520: 0009 0000 0043 0000 0073 ac00 0000 7c01  .....C...s....|.
-00002530: 6401 6602 7c02 6402 6602 6702 7d07 7400  d.f.|.d.f.g.}.t.
-00002540: 6a01 7c04 7c01 7c05 7c00 6a02 6a03 7c07  j.|.|.|.|.j.j.|.
-00002550: 7c06 6701 7c00 6a04 6a05 6403 8d07 7d08  |.g.|.j.j.d...}.
-00002560: 7c08 a006 7c02 a101 7d09 7407 a008 6404  |...|...}.t...d.
-00002570: 6405 8400 7c09 4400 8301 a101 7d0a 7409  d...|.D.....}.t.
-00002580: 7c03 a00a a100 7c0a a00a a100 8302 6406  |.....|.......d.
-00002590: 1400 7d0b 740b 7c00 6a0c 6a0d 8301 6407  ..}.t.|.j.j...d.
-000025a0: 6b02 723e 6407 7d0c 6e08 7c00 6a0c 6a0d  k.r>d.}.n.|.j.j.
-000025b0: 6406 1900 6408 1700 7d0c 7c00 6a0c 6a0e  d...d...}.|.j.j.
-000025c0: 7c0c 6409 7c00 6a02 7c04 7c0b 640a 640b  |.d.|.j.|.|.d.d.
-000025d0: 640c 8d07 0100 7c0b 5300 290d 4e72 3800  d.....|.S.).Nr8.
-000025e0: 0000 7239 0000 0029 0572 3e00 0000 723f  ..r9...).r>...r?
-000025f0: 0000 0072 4000 0000 7280 0000 0072 4100  ...r@...r....rA.
-00002600: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00002610: 0000 0005 0000 0053 0000 00f3 1600 0000  .......S........
-00002620: 6700 7c00 5d07 7d01 7400 a001 7c01 a101  g.|.].}.t...|...
-00002630: 9102 7102 5300 7225 0000 00a9 0272 1f00  ..q.S.r%.....r..
-00002640: 0000 da06 6172 676d 6178 a902 7276 0000  ....argmax..rv..
-00002650: 00da 046c 696e 6572 2500 0000 7225 0000  ...liner%...r%..
-00002660: 0072 2600 0000 7278 0000 00c5 0100 00f3  .r&...rx........
-00002670: 0200 0000 1600 7a38 5867 626f 6f73 744d  ......z8XgboostM
-00002680: 6f64 656c 2e74 7261 696e 5f73 696e 676c  odel.train_singl
-00002690: 655f 666f 6c64 5f6d 6f64 656c 2e3c 6c6f  e_fold_model.<lo
-000026a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000026b0: 7284 0000 0072 0100 0000 723c 0000 00da  r....r....r<....
-000026c0: 1773 696d 706c 655f 7472 6169 6e5f 7465  .simple_train_te
-000026d0: 7374 5f73 636f 7265 72d4 0000 0046 7287  st_scorer....Fr.
-000026e0: 0000 0029 0f72 5500 0000 7238 0000 0072  ...).rU...r8...r
-000026f0: 1900 0000 723f 0000 0072 1a00 0000 da26  ....r?...r.....&
-00002700: 7665 7262 6f73 6974 795f 6475 7269 6e67  verbosity_during
-00002710: 5f68 7970 6572 7061 7261 6d65 7465 725f  _hyperparameter_
-00002720: 7475 6e69 6e67 da07 7072 6564 6963 7472  tuning..predictr
-00002730: 1f00 0000 da07 6173 6172 7261 7972 0a00  ......asarrayr..
-00002740: 0000 da06 746f 6c69 7374 72b3 0000 0072  ....tolistr....r
-00002750: 1c00 0000 7288 0000 0072 b400 0000 290d  ....r....r....).
-00002760: 7224 0000 0072 5700 0000 7258 0000 0072  r$...rW...rX...r
-00002770: 3400 0000 72b6 0000 0072 3a00 0000 72b7  4...r....r:...r.
-00002780: 0000 0072 5900 0000 721e 0000 00da 0570  ...rY...r......p
-00002790: 7265 6473 da0b 7072 6564 5f6c 6162 656c  reds..pred_label
-000027a0: 735a 076d 6174 7468 6577 72ba 0000 0072  sZ.matthewr....r
-000027b0: 2500 0000 7225 0000 0072 2600 0000 72ab  %...r%...r&...r.
-000027c0: 0000 00b7 0100 0073 3400 0000 1003 0401  .......s4.......
-000027d0: 0201 0201 0201 0601 0201 0401 0601 06f9  ................
-000027e0: 0a09 1401 1601 1003 0601 1002 0601 0201  ................
-000027f0: 0201 0401 0201 0201 0201 0201 06f9 0409  ................
-00002800: 7a24 5867 626f 6f73 744d 6f64 656c 2e74  z$XgboostModel.t
-00002810: 7261 696e 5f73 696e 676c 655f 666f 6c64  rain_single_fold
-00002820: 5f6d 6f64 656c 727a 0000 00da 0765 7661  _modelrz.....eva
-00002830: 6c5f 6466 da06 795f 7472 7565 da0a 6974  l_df..y_true..it
-00002840: 6572 6174 696f 6e73 6305 0000 0000 0000  erationsc.......
-00002850: 0000 0000 0011 0000 0007 0000 0043 0000  .............C..
-00002860: 0073 ae00 0000 6700 7d05 7400 7c04 8301  .s....g.}.t.|...
-00002870: 4400 5d4e 7d06 6401 6402 7c06 1400 0202  D.]N}.d.d.|.....
-00002880: 7d07 7d08 7c02 6a01 5c02 7d09 7d0a 7c00  }.}.|.j.\.}.}.|.
-00002890: 6a02 a003 7c07 7c08 7c09 7c0a 6702 a103  j...|.|.|.|.g...
-000028a0: 7d0b 7c02 7c0b 1700 7d0c 7c00 6a04 7230  }.|.|...}.|.j.r0
-000028b0: 7405 6a06 7c0c 7c03 7c00 6a04 6a07 6403  t.j.|.|.|.j.j.d.
-000028c0: 8d03 7d0d 6e04 7408 6404 8301 8201 7c01  ..}.n.t.d.....|.
-000028d0: a009 7c0d a101 7d0e 740a a00b 6405 6406  ..|...}.t...d.d.
-000028e0: 8400 7c0e 4400 8301 a101 7d0f 740c 7c03  ..|.D.....}.t.|.
-000028f0: 6a0d a00e a100 7c0f a00e a100 8302 6407  j.....|.......d.
-00002900: 1400 7d10 7c05 a00f 7c10 a101 0100 7106  ..}.|...|.....q.
-00002910: 7c05 5300 2908 619f 0100 0046 756e 6374  |.S.).a....Funct
-00002920: 696f 6e20 746f 2061 6464 2069 6e63 7265  ion to add incre
-00002930: 6173 696e 6720 6e6f 6973 6520 616e 6420  asing noise and 
-00002940: 6576 616c 7561 7465 2069 742e 0a0a 2020  evaluate it...  
-00002950: 2020 2020 2020 5468 6520 6675 6e63 7469        The functi
-00002960: 6f6e 2065 7870 6563 7473 2061 2074 7261  on expects a tra
-00002970: 696e 6564 206d 6f64 656c 2061 6e64 2061  ined model and a
-00002980: 2064 6174 6166 7261 6d65 2077 6974 6820   dataframe with 
-00002990: 7468 6520 7361 6d65 2063 6f6c 756d 6e73  the same columns
-000029a0: 2061 7320 7468 6520 7472 6169 6e69 6e67   as the training
-000029b0: 2064 6174 612e 0a20 2020 2020 2020 2054   data..        T
-000029c0: 6865 2074 7261 696e 696e 6720 6461 7461  he training data
-000029d0: 2073 686f 756c 6420 6265 206e 6f72 6d61   should be norma
-000029e0: 6c6c 7920 6469 7374 7269 6275 7465 6420  lly distributed 
-000029f0: 2863 6f6e 7369 6465 7220 7573 696e 6720  (consider using 
-00002a00: 6120 706f 7765 7220 7472 616e 7366 6f72  a power transfor
-00002a10: 6d65 7220 7769 7468 2079 656f 2d6a 6f68  mer with yeo-joh
-00002a20: 6e73 6f6e 292e 0a0a 2020 2020 2020 2020  nson)...        
-00002a30: 5468 6520 6675 6e63 7469 6f6e 2077 696c  The function wil
-00002a40: 6c20 6170 706c 7920 696e 6372 6561 7369  l apply increasi
-00002a50: 6e67 6c79 206e 6f69 7365 2074 6f20 7468  ngly noise to th
-00002a60: 6520 6576 616c 2064 6174 6166 7261 6d65  e eval dataframe
-00002a70: 2061 6e64 2065 7661 6c75 6174 6520 7468   and evaluate th
-00002a80: 6520 6d6f 6465 6c20 6f6e 2069 742e 0a0a  e model on it...
-00002a90: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-00002aa0: 6120 6c69 7374 206f 6620 6c6f 7373 6573  a list of losses
-00002ab0: 2e0a 2020 2020 2020 2020 7201 0000 0067  ..        r....g
-00002ac0: 9a99 9999 9999 c93f 7270 0000 007a 214e  .......?rp...z!N
-00002ad0: 6f20 7472 6169 6e69 6e67 5f63 6f6e 6669  o training_confi
-00002ae0: 6720 636f 756c 6420 6265 2066 6f75 6e64  g could be found
-00002af0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002b00: 0005 0000 0053 0000 0072 d900 0000 7225  .....S...r....r%
-00002b10: 0000 0072 da00 0000 72dc 0000 0072 2500  ...r....r....r%.
-00002b20: 0000 7225 0000 0072 2600 0000 7278 0000  ..r%...r&...rx..
-00002b30: 00f4 0100 0072 de00 0000 7a3b 5867 626f  .....r....z;Xgbo
-00002b40: 6f73 744d 6f64 656c 2e69 6e63 7265 6173  ostModel.increas
-00002b50: 696e 675f 6e6f 6973 655f 6576 616c 7561  ing_noise_evalua
-00002b60: 746f 722e 3c6c 6f63 616c 733e 2e3c 6c69  tor.<locals>.<li
-00002b70: 7374 636f 6d70 3e72 8400 0000 2910 72ad  stcomp>r....).r.
-00002b80: 0000 00da 0573 6861 7065 7223 0000 00da  .....shaper#....
-00002b90: 066e 6f72 6d61 6c72 1900 0000 7255 0000  .normalr....rU..
-00002ba0: 0072 a700 0000 72a8 0000 0072 4200 0000  .r....r....rB...
-00002bb0: 72e1 0000 0072 1f00 0000 72e2 0000 0072  r....r....r....r
-00002bc0: 0a00 0000 da06 7661 6c75 6573 72e3 0000  ......valuesr...
-00002bd0: 00da 0661 7070 656e 6429 1172 2400 0000  ...append).r$...
-00002be0: da08 6d6c 5f6d 6f64 656c 72e6 0000 0072  ..ml_modelr....r
-00002bf0: e700 0000 72e8 0000 00da 066c 6f73 7365  ....r......losse
-00002c00: 7372 7700 0000 da02 6d75 da05 7369 676d  srw.....mu..sigm
-00002c10: 61da 014e da01 44da 056e 6f69 7365 5a0b  a..N..D..noiseZ.
-00002c20: 6576 616c 5f64 665f 6d6f 645a 0664 5f65  eval_df_modZ.d_e
-00002c30: 7661 6cda 0579 5f68 6174 da09 795f 636c  val..y_hat..y_cl
-00002c40: 6173 7365 73da 046c 6f73 7372 2500 0000  asses..lossr%...
-00002c50: 7225 0000 0072 2600 0000 da1a 696e 6372  r%...r&.....incr
-00002c60: 6561 7369 6e67 5f6e 6f69 7365 5f65 7661  easing_noise_eva
-00002c70: 6c75 6174 6f72 d801 0000 7324 0000 0004  luator....s$....
-00002c80: 0d0c 010e 010a 0114 0108 0106 0104 0102  ................
-00002c90: 0102 0106 0108 fd08 060a 0114 0118 020c  ................
-00002ca0: 0104 027a 2758 6762 6f6f 7374 4d6f 6465  ...z'XgboostMode
-00002cb0: 6c2e 696e 6372 6561 7369 6e67 5f6e 6f69  l.increasing_noi
-00002cc0: 7365 5f65 7661 6c75 6174 6f72 72ee 0000  se_evaluatorr...
-00002cd0: 0063 0200 0000 0000 0000 0000 0000 0600  .c..............
-00002ce0: 0000 0600 0000 4300 0000 738c 0000 0064  ......C...s....d
-00002cf0: 017d 0274 0074 017c 0183 0183 0144 005d  .}.t.t.|.....D.]
-00002d00: 1c7d 037c 0364 0217 0074 017c 0183 0164  .}.|.d...t.|...d
-00002d10: 0218 006b 0472 1601 006e 0f7c 017c 0319  ...k.r...n.|.|..
-00002d20: 007c 017c 0364 0217 0019 006b 0472 247c  .|.|.d.....k.r$|
-00002d30: 0264 0237 007d 0271 087c 0264 016b 0272  .d.7.}.q.|.d.k.r
-00002d40: 2d64 037d 047c 0453 0074 017c 0183 017d  -d.}.|.S.t.|...}
-00002d50: 057c 0164 0119 0074 02a0 037c 0164 047c  .|.d...t...|.d.|
-00002d60: 0285 0219 00a1 017c 057c 057c 0218 001b  .......|.|.|....
-00002d70: 0013 0018 007d 047c 0453 0029 0561 4201  .....}.|.S.).aB.
-00002d80: 0000 4361 6c63 756c 6174 6520 6120 7765  ..Calculate a we
-00002d90: 6967 6874 6564 206c 6f73 7320 6261 7365  ighted loss base
-00002da0: 6420 6f6e 2074 6865 206e 756d 6265 7220  d on the number 
-00002db0: 6f66 2074 696d 6573 2074 6865 206c 6f73  of times the los
-00002dc0: 7320 6465 6372 6561 7365 642e 0a0a 2020  s decreased...  
-00002dd0: 2020 2020 2020 4578 7065 6374 7320 6120        Expects a 
-00002de0: 6c69 7374 206f 6620 6c6f 7373 6573 2063  list of losses c
-00002df0: 6f6d 696e 6720 6672 6f6d 2069 6e63 7265  oming from incre
-00002e00: 6173 696e 675f 6e6f 6973 655f 6576 616c  asing_noise_eval
-00002e10: 7561 746f 722e 2043 6865 636b 7320 686f  uator. Checks ho
-00002e20: 7720 6d61 6e79 2074 696d 6573 2074 6865  w many times the
-00002e30: 206c 6f73 7320 6465 6372 6561 7365 6420   loss decreased 
-00002e40: 616e 640a 2020 2020 2020 2020 6361 6c63  and.        calc
-00002e50: 756c 6174 6573 2061 2077 6569 6768 7465  ulates a weighte
-00002e60: 6420 6c6f 7373 2062 6173 6564 206f 6e20  d loss based on 
-00002e70: 7468 6520 6e75 6d62 6572 206f 6620 7469  the number of ti
-00002e80: 6d65 7320 7468 6520 6c6f 7373 2064 6563  mes the loss dec
-00002e90: 7265 6173 6564 2e0a 0a20 2020 2020 2020  reased...       
-00002ea0: 2052 6574 7572 6e73 2074 6865 2077 6569   Returns the wei
-00002eb0: 6768 7465 6420 6c6f 7373 2e0a 2020 2020  ghted loss..    
-00002ec0: 2020 2020 7201 0000 0072 3c00 0000 69e7      r....r<...i.
-00002ed0: 0300 004e 2904 72ad 0000 0072 b300 0000  ...N).r....r....
-00002ee0: 721f 0000 0072 b200 0000 2906 7224 0000  r....r....).r$..
-00002ef0: 0072 ee00 0000 5a11 6e62 5f6c 6f73 735f  .r....Z.nb_loss_
-00002f00: 6465 6372 6561 7365 64da 0369 6478 da0d  decreased..idx..
-00002f10: 7765 6967 6874 6564 5f6c 6f73 735a 096e  weighted_lossZ.n
-00002f20: 625f 6c6f 7373 6573 7225 0000 0072 2500  b_lossesr%...r%.
-00002f30: 0000 7226 0000 00da 2063 6f6e 7374 616e  ..r&.... constan
-00002f40: 745f 6c6f 7373 5f64 6567 7265 6761 7469  t_loss_degregati
-00002f50: 6f6e 5f66 6163 746f 72fb 0100 0073 1e00  on_factor....s..
-00002f60: 0000 0408 1001 1401 0401 1401 0801 0280  ................
-00002f70: 0803 0401 040a 08f8 1601 0a01 06ff 0407  ................
-00002f80: 7a2d 5867 626f 6f73 744d 6f64 656c 2e63  z-XgboostModel.c
-00002f90: 6f6e 7374 616e 745f 6c6f 7373 5f64 6567  onstant_loss_deg
-00002fa0: 7265 6761 7469 6f6e 5f66 6163 746f 72da  regation_factor.
-00002fb0: 0c74 756e 6564 5f70 6172 616d 7372 7200  .tuned_paramsrr.
-00002fc0: 0000 6307 0000 0000 0000 0000 0000 001c  ..c.............
-00002fd0: 0000 0009 0000 0043 0000 0073 0a02 0000  .......C...s....
-00002fe0: 7c01 a000 6401 6402 a102 7d07 7c00 6a01  |...d.d...}.|.j.
-00002ff0: 7311 7402 8300 7c00 5f01 7403 6403 8301  s.t...|._.t.d...
-00003000: 0100 7404 7c00 6a01 6a05 6404 7c06 6405  ..t.|.j.j.d.|.d.
-00003010: 8d03 7d08 6700 7d09 7406 7c08 a007 7c02  ..}.g.}.t.|...|.
-00003020: 7c03 a008 7409 a101 a102 8301 4400 5daa  |...t.......D.].
-00003030: 5c02 7d0a 5c02 7d0b 7d0c 7c02 6a0a 7c0b  \.}.\.}.}.|.j.|.
-00003040: 1900 7c02 6a0a 7c0c 1900 0202 7d0d 7d0e  ..|.j.|.....}.}.
-00003050: 7c03 6a0a 7c0b 1900 7c03 6a0a 7c0c 1900  |.j.|...|.j.|...
-00003060: 0202 7d0f 7d10 7c00 6a0b 7264 7c00 6a0b  ..}.}.|.j.rd|.j.
-00003070: a00c 7c0d 7c0f a102 5c02 7d0d 7d0f 7c00  ..|.|...\.}.}.|.
-00003080: 6a0b a00d 7c04 7c05 a102 5c02 7d11 7d12  j...|.|...\.}.}.
-00003090: 7c00 6a0b 6a0d 7c0e 7c10 6406 6407 8d03  |.j.j.|.|.d.d...
-000030a0: 5c02 7d0e 7d10 6e05 7c04 7c05 0202 7d11  \.}.}.n.|.|...}.
-000030b0: 7d12 740e 6a0f 7c0e 7c10 7c00 6a01 6a10  }.t.j.|.|.|.j.j.
-000030c0: 6408 8d03 7d13 7c00 6a11 737e 7412 8300  d...}.|.j.s~t...
-000030d0: 7c00 5f11 7403 6409 8301 0100 7c00 6a11  |._.t.d.....|.j.
-000030e0: 6a13 7293 7c00 a014 7c0f a101 7d14 740e  j.r.|...|...}.t.
-000030f0: 6a0f 7c0d 7c0f 7c14 7c00 6a01 6a10 640a  j.|.|.|.|.j.j.d.
-00003100: 8d04 7d15 6e0a 740e 6a0f 7c0d 7c0f 7c00  ..}.n.t.j.|.|.|.
-00003110: 6a01 6a10 6408 8d03 7d15 7c15 640b 6602  j.j.d...}.|.d.f.
-00003120: 7c13 640c 6602 6702 7d16 7c00 6a15 73b0  |.d.f.g.}.|.j.s.
-00003130: 7416 8300 7c00 5f15 7403 640d 8301 0100  t...|._.t.d.....
-00003140: 740e 6a17 7c01 7c15 7c07 7c00 6a01 6a18  t.j.|.|.|.|.j.j.
-00003150: 7c16 7c00 6a15 6a19 640e 8d06 7d17 7c00  |.|.j.j.d...}.|.
-00003160: a01a 7c17 7c11 7c12 640f a104 7d18 7c00  ..|.|.|.d...}.|.
-00003170: a01b 7c18 a101 7d19 7c09 a01c 7c19 a101  ..|...}.|...|...
-00003180: 0100 7127 741d a01e 741d a01f 7c09 a101  ..q't...t...|...
-00003190: a101 7d1a 7c00 6a20 9001 7203 7c00 6a01  ..}.|.j ..r.|.j.
-000031a0: 9001 7203 7421 7c00 6a20 6a22 8301 6410  ..r.t!|.j j"..d.
-000031b0: 6b02 72ed 6410 7d1b 6e08 7c00 6a20 6a22  k.r.d.}.n.|.j j"
-000031c0: 6411 1900 6412 1700 7d1b 7c00 6a20 6a23  d...d...}.|.j j#
-000031d0: 7c1b 6413 7c00 6a01 7c01 7c1a 6414 6406  |.d.|.j.|.|.d.d.
-000031e0: 6415 8d07 0100 7c1a 5300 2916 4e72 3a00  d.....|.S.).Nr:.
-000031f0: 0000 723b 0000 007a 3e43 6f75 6c64 206e  ..r;...z>Could n
-00003200: 6f74 2066 696e 6420 5472 6169 6e69 6e67  ot find Training
-00003210: 2063 6f6e 6669 672e 2046 616c 6c69 6e67   config. Falling
-00003220: 2062 6163 6b20 746f 2064 6566 6175 6c74   back to default
-00003230: 2076 616c 7565 7354 2903 da08 6e5f 7370   valuesT)...n_sp
-00003240: 6c69 7473 7281 0000 00da 0c72 616e 646f  litsr......rando
-00003250: 6d5f 7374 6174 6546 7236 0000 0072 7000  m_stateFr6...rp.
-00003260: 0000 7a49 436f 756c 6420 6e6f 7420 6669  ..zICould not fi
-00003270: 6e64 2058 6762 6f6f 7374 4669 6e61 6c50  nd XgboostFinalP
-00003280: 6172 616d 436f 6e66 6967 2e20 4661 6c6c  aramConfig. Fall
-00003290: 696e 6720 6261 636b 2074 6f20 6465 6661  ing back to defa
-000032a0: 756c 7420 7365 7474 696e 6773 2e72 6c00  ult settings.rl.
-000032b0: 0000 7238 0000 0072 3900 0000 7a41 436f  ..r8...r9...zACo
-000032c0: 756c 6420 6e6f 7420 6669 6e64 2058 6762  uld not find Xgb
-000032d0: 6f6f 7374 5475 6e65 5061 7261 6d73 436f  oostTuneParamsCo
-000032e0: 6e66 6967 2e20 4661 6c6c 696e 6720 6261  nfig. Falling ba
-000032f0: 636b 2074 6f20 6465 6661 756c 7473 2e72  ck to defaults.r
-00003300: 3d00 0000 727a 0000 0072 0100 0000 7284  =...rz...r....r.
-00003310: 0000 0072 3c00 0000 da09 6f6f 665f 7363  ...r<.....oof_sc
-00003320: 6f72 6572 d400 0000 7287 0000 0029 2472  orer....r....)$r
-00003330: 5300 0000 7219 0000 0072 0d00 0000 7212  S...r....r....r.
-00003340: 0000 0072 0b00 0000 7254 0000 00da 0965  ...r....rT.....e
-00003350: 6e75 6d65 7261 7465 da05 7370 6c69 74da  numerate..split.
-00003360: 0661 7374 7970 65da 0369 6e74 da04 696c  .astype..int..il
-00003370: 6f63 721d 0000 0072 4c00 0000 724d 0000  ocr....rL...rM..
-00003380: 0072 5500 0000 72a7 0000 0072 a800 0000  .rU...r....r....
-00003390: 721b 0000 0072 0e00 0000 726b 0000 0072  r....r....rk...r
-000033a0: 2d00 0000 721a 0000 0072 0f00 0000 7238  -...r....r....r8
-000033b0: 0000 0072 3f00 0000 72e0 0000 0072 f700  ...r?...r....r..
-000033c0: 0000 72fa 0000 0072 ec00 0000 721f 0000  ..r....r....r...
-000033d0: 0072 b100 0000 72e2 0000 0072 1c00 0000  .r....r....r....
-000033e0: 72b3 0000 0072 8800 0000 72b4 0000 0029  r....r....r....)
-000033f0: 1c72 2400 0000 72fb 0000 0072 3100 0000  .r$...r....r1...
-00003400: 7233 0000 0072 3200 0000 7234 0000 0072  r3...r2...r4...r
-00003410: 7200 0000 723a 0000 005a 0a73 7472 6174  r...r:...Z.strat
-00003420: 6966 6965 725a 0b66 6f6c 645f 6c6f 7373  ifierZ.fold_loss
-00003430: 6573 da03 5f66 6e5a 0774 726e 5f69 6478  es.._fnZ.trn_idx
-00003440: 5a07 7661 6c5f 6964 785a 0c58 5f74 7261  Z.val_idxZ.X_tra
-00003450: 696e 5f66 6f6c 645a 0a58 5f76 616c 5f66  in_foldZ.X_val_f
-00003460: 6f6c 645a 0c79 5f74 7261 696e 5f66 6f6c  oldZ.y_train_fol
-00003470: 645a 0a79 5f76 616c 5f66 6f6c 645a 0b58  dZ.y_val_foldZ.X
-00003480: 5f74 6573 745f 666f 6c64 5a0b 795f 7465  _test_foldZ.y_te
-00003490: 7374 5f66 6f6c 6472 5800 0000 722c 0000  st_foldrX...r,..
-000034a0: 0072 5700 0000 7259 0000 0072 1e00 0000  .rW...rY...r....
-000034b0: 72ee 0000 005a 1963 6f6e 7374 616e 745f  r....Z.constant_
-000034c0: 6c6f 7373 5f64 6567 7265 6761 7469 6f6e  loss_degregation
-000034d0: 5a0d 6d61 7474 6865 7773 5f6d 6561 6e72  Z.matthews_meanr
-000034e0: ba00 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
-000034f0: 0000 0072 ae00 0000 1802 0000 73bc 0000  ...r........s...
-00003500: 000c 0906 0208 0108 0102 0206 0102 0102  ................
-00003510: 0106 fd04 0602 0110 0110 ff08 0408 0106  ................
-00003520: fe08 0508 0106 fe06 0406 0404 0102 ff02  ................
-00003530: fd02 0102 010c 0702 fd02 0102 0106 0506  ................
-00003540: 0104 ff02 fd02 0104 010a 0504 0202 0102  ................
-00003550: 0106 0106 fd06 0608 0102 0102 0104 ff08  ................
-00003560: 040a 0104 0102 0102 0102 0106 0108 fc04  ................
-00003570: 0702 0102 0106 0106 fd10 0506 0208 0102  ................
-00003580: 0102 0104 ff04 0302 0102 0102 0106 0102  ................
-00003590: 0106 0106 fa04 0e08 0104 ff0a 030c 0110  ................
-000035a0: 0410 0210 0206 0110 0206 0102 0102 0104  ................
-000035b0: 0102 0102 0102 0102 0106 f904 097a 1f58  .............z.X
-000035c0: 6762 6f6f 7374 4d6f 6465 6c2e 5f66 696e  gboostModel._fin
-000035d0: 655f 7475 6e65 5f70 7265 6369 7365 6305  e_tune_precisec.
-000035e0: 0000 0000 0000 0000 0000 000c 0000 000a  ................
-000035f0: 0000 0003 0000 0073 8802 0000 7400 7401  .......s....t.t.
-00003600: a002 a100 9b00 6401 9d02 8301 0100 8800  ......d.........
-00003610: 6a03 7215 8800 6a04 7215 8800 6a05 7215  j.r...j.r...j.r.
-00003620: 8800 6a06 7319 7407 6402 8301 8201 8700  ..j.s.t.d.......
-00003630: 8701 8702 8703 8704 6605 6403 6404 8408  ........f.d.d...
-00003640: 7d05 8800 a008 a100 0100 7409 8800 6a03  }.........t...j.
-00003650: 6a0a 6405 1900 740b 8302 72a7 7409 8800  j.d...t...r.t...
-00003660: 6a03 6a0a 6406 1900 740b 8302 72a7 7409  j.j.d...t...r.t.
-00003670: 8800 6a03 6a0a 6407 1900 740b 8302 72a7  ..j.j.d...t...r.
-00003680: 7409 8800 6a03 6a0a 6408 1900 740b 8302  t...j.j.d...t...
-00003690: 72a7 740c 6a0d 8800 6a03 6a0a 6405 1900  r.t.j...j.j.d...
-000036a0: 6409 1400 8800 6a03 6a0a 6405 1900 640a  d.....j.j.d...d.
-000036b0: 1400 8800 6a04 6a0e 740b 640b 8d04 740c  ....j.j.t.d...t.
-000036c0: 6a0d 8800 6a03 6a0a 6406 1900 6409 1400  j...j.j.d...d...
-000036d0: 8800 6a03 6a0a 6406 1900 640a 1400 8800  ..j.j.d...d.....
-000036e0: 6a04 6a0e 740b 640b 8d04 740c 6a0d 8800  j.j.t.d...t.j...
-000036f0: 6a03 6a0a 6407 1900 6409 1400 8800 6a03  j.j.d...d.....j.
-00003700: 6a0a 6407 1900 640a 1400 8800 6a04 6a0e  j.d...d.....j.j.
-00003710: 740b 640b 8d04 740c 6a0d 8800 6a03 6a0a  t.d...t.j...j.j.
-00003720: 6408 1900 6409 1400 8800 6a03 6a0a 6408  d...d.....j.j.d.
-00003730: 1900 640a 1400 8800 6a04 6a0e 740b 640b  ..d.....j.j.t.d.
-00003740: 8d04 640c 9c04 7d06 6e04 7407 640d 8301  ..d...}.n.t.d...
-00003750: 0100 8800 a00f a100 7d07 7410 6a11 640e  ........}.t.j.d.
-00003760: 7410 6a12 a013 7c06 a101 640f 8d02 7d08  t.j...|...d...}.
-00003770: 7c08 6a14 7c05 8800 6a04 6a0e 7415 7c06  |.j.|...j.j.t.|.
-00003780: a016 a100 8301 1300 8800 6a04 6a17 6410  ..........j.j.d.
-00003790: 6410 6411 8d05 0100 7a16 7410 6a18 a019  d.d.....z.t.j...
-000037a0: 7c08 a101 7d09 7c09 a01a a100 0100 7410  |...}.|.......t.
-000037b0: 6a18 a01b 7c08 a101 7d09 7c09 a01a a100  j...|...}.|.....
-000037c0: 0100 5700 6e0c 0400 741c 741d 7407 6603  ..W.n...t.t.t.f.
-000037d0: 79f0 0100 0100 0100 5900 6e01 7700 8800  y.......Y.n.w...
-000037e0: a00f a100 7d0a 7c0a 7c07 6b00 73fe 8800  ....}.|.|.k.s...
-000037f0: 6a04 6a1e 9001 7338 7c08 6a1f 6a0a 7d0b  j.j...s8|.j.j.}.
-00003800: 7c0b 6405 1900 8800 6a03 6a0a 6405 3c00  |.d.....j.j.d.<.
-00003810: 7c0b 6406 1900 8800 6a03 6a0a 6406 3c00  |.d.....j.j.d.<.
-00003820: 7c0b 6407 1900 8800 6a03 6a0a 6407 3c00  |.d.....j.j.d.<.
-00003830: 7c0b 6408 1900 8800 6a03 6a0a 6408 3c00  |.d.....j.j.d.<.
-00003840: 7400 6412 7c07 9b00 6413 7c0a 9b00 6414  t.d.|...d.|...d.
-00003850: 9d05 8301 0100 7400 6415 8800 6a03 6a0a  ......t.d...j.j.
-00003860: 9b00 9d02 8301 0100 6400 5300 7400 6416  ........d.S.t.d.
-00003870: 7c07 9b00 6417 7c0a 9b00 9d04 8301 0100  |...d.|.........
-00003880: 6400 5300 2918 4e7a 313a 2053 7461 7274  d.S.).Nz1: Start
-00003890: 2067 7269 6420 7365 6172 6368 2066 696e   grid search fin
-000038a0: 6520 7475 6e69 6e67 206f 6620 5867 626f  e tuning of Xgbo
-000038b0: 6f73 7420 6d6f 6465 6c2e 725b 0000 0063  ost model.r[...c
-000038c0: 0100 0000 0000 0000 0000 0000 0d00 0000  ................
-000038d0: 0b00 0000 1300 0000 73de 0100 0088 00a0  ........s.......
-000038e0: 0088 0288 0488 0188 03a1 045c 027d 017d  ...........\.}.}
-000038f0: 0274 016a 02a0 037c 0064 01a1 027d 0374  .t.j...|.d...}.t
-00003900: 0488 006a 056a 0683 017d 047c 006a 0764  ...j.j...}.|.j.d
-00003910: 0288 006a 056a 0664 0219 0064 0314 0088  ...j.j.d...d....
-00003920: 006a 056a 0664 0219 0064 0414 0064 0564  .j.j.d...d...d.d
-00003930: 068d 047d 057c 006a 0764 0788 006a 056a  ...}.|.j.d...j.j
-00003940: 0664 0719 0064 0314 0088 006a 056a 0664  .d...d.....j.j.d
-00003950: 0719 0064 0414 0064 0564 068d 047d 067c  ...d...d.d...}.|
-00003960: 006a 0764 0888 006a 056a 0664 0819 0064  .j.d...j.j.d...d
-00003970: 0314 0088 006a 056a 0664 0819 0064 0414  .....j.j.d...d..
-00003980: 0064 0564 068d 047d 077c 006a 0764 0988  .d.d...}.|.j.d..
-00003990: 006a 056a 0664 0919 0064 0314 0088 006a  .j.j.d...d.....j
-000039a0: 056a 0664 0919 0064 0414 0064 0564 068d  .j.d...d...d.d..
-000039b0: 047d 087c 057c 0464 023c 007c 067c 0464  .}.|.|.d.<.|.|.d
-000039c0: 073c 007c 077c 0464 083c 007c 087c 0464  .<.|.|.d.<.|.|.d
-000039d0: 093c 007c 04a0 0864 0a64 0ba1 027d 0988  .<.|...d.d...}..
-000039e0: 006a 096a 0a64 0c6b 0272 9188 00a0 0b7c  .j.j.d.k.r.....|
-000039f0: 017c 0288 037c 047c 097c 03a1 0653 0088  .|...|.|.|...S..
-00003a00: 006a 096a 0a64 0c6b 0472 a788 006a 096a  .j.j.d.k.r...j.j
-00003a10: 0c72 a788 00a0 0d7c 0488 0288 0488 0188  .r.....|........
-00003a20: 0388 006a 096a 0ea1 0653 0074 0f6a 107c  ...j.j...S.t.j.|
-00003a30: 047c 017c 0988 006a 096a 1188 006a 096a  .|.|...j.j...j.j
-00003a40: 0a64 0588 006a 096a 0e7c 0367 0188 006a  .d...j.j.|.g...j
-00003a50: 096a 1264 0d8d 097d 0a7c 0a64 0e19 00a0  .j.d...}.|.d....
-00003a60: 13a1 007c 0a64 0e19 00a0 14a1 0064 0f13  ...|.d.......d..
-00003a70: 0017 007d 0b74 1588 006a 166a 1783 0164  ...}.t...j.j...d
-00003a80: 106b 0272 d764 107d 0c6e 0888 006a 166a  .k.r.d.}.n...j.j
-00003a90: 1764 1119 0064 0c17 007d 0c88 006a 166a  .d...d...}...j.j
-00003aa0: 187c 0c64 1288 006a 097c 047c 0b64 1364  .|.d...j.|.|.d.d
-00003ab0: 1464 158d 0701 007c 0b53 0029 164e 7271  .d.....|.S.).Nrq
-00003ac0: 0000 0072 6000 0000 e7cd cccc cccc ccec  ...r`...........
-00003ad0: 3fe7 9a99 9999 9999 f13f 5472 5d00 0000  ?........?Tr]...
-00003ae0: 7261 0000 0072 6200 0000 725c 0000 0072  ra...rb...r\...r
-00003af0: 3a00 0000 723b 0000 0072 3c00 0000 727b  :...r;...r<...r{
-00003b00: 0000 0072 8200 0000 7283 0000 0072 0100  ...r....r....r..
-00003b10: 0000 7284 0000 0072 8500 0000 7286 0000  ..r....r....r...
-00003b20: 0046 7287 0000 0029 1972 5100 0000 7244  .Fr....).rQ...rD
-00003b30: 0000 0072 a900 0000 72aa 0000 0072 0200  ...r....r....r..
-00003b40: 0000 721b 0000 0072 5200 0000 7292 0000  ..r....rR...r...
-00003b50: 0072 5300 0000 7219 0000 0072 5400 0000  .rS...r....rT...
-00003b60: 72ab 0000 0072 ac00 0000 72ae 0000 0072  r....r....r....r
-00003b70: 2200 0000 7255 0000 0072 af00 0000 723f  "...rU...r....r?
-00003b80: 0000 0072 b000 0000 72b1 0000 0072 b200  ...r....r....r..
-00003b90: 0000 72b3 0000 0072 1c00 0000 7288 0000  ..r....r....r...
-00003ba0: 0072 b400 0000 290d 72b5 0000 0072 5700  .r....).r....rW.
-00003bb0: 0000 7258 0000 0072 b700 0000 72fb 0000  ..rX...r....r...
-00003bc0: 005a 0b61 6c70 6861 5f73 7061 6365 5a0c  .Z.alpha_spaceZ.
-00003bd0: 6c61 6d62 6461 5f73 7061 6365 5a0b 6761  lambda_spaceZ.ga
-00003be0: 6d6d 615f 7370 6163 655a 0965 7461 5f73  mma_spaceZ.eta_s
-00003bf0: 7061 6365 723a 0000 0072 b800 0000 72b9  pacer:...r....r.
-00003c00: 0000 0072 ba00 0000 a905 7224 0000 0072  ...r......r$...r
-00003c10: 3200 0000 7231 0000 0072 3400 0000 7233  2...r1...r4...r3
-00003c20: 0000 0072 2500 0000 7226 0000 0072 6700  ...r%...r&...rg.
-00003c30: 0000 a902 0000 7398 0000 0014 0106 0204  ......s.........
-00003c40: 0104 ff0c 0404 0102 010e 010e 0102 0106  ................
-00003c50: fc04 0602 010e 010e 0102 0106 fc04 0602  ................
-00003c60: 010e 010e 0102 0106 fc04 0602 010e 010e  ................
-00003c70: 0102 0106 fc08 0708 0108 0108 010c 020c  ................
-00003c80: 0204 010c 0104 ff0c 0406 0102 ff04 0302  ................
-00003c90: 0102 0102 0102 0102 0106 0104 fa04 0902  ................
-00003ca0: 0102 0102 0106 0106 0102 0106 0104 0106  ................
-00003cb0: 0106 f70a 0c0e 0104 ff10 0506 0110 0206  ................
-00003cc0: 0102 0102 0104 0102 0102 0102 0102 0106  ................
-00003cd0: f904 0a7a 2958 6762 6f6f 7374 4d6f 6465  ...z)XgboostMode
-00003ce0: 6c2e 6669 6e65 5f74 756e 652e 3c6c 6f63  l.fine_tune.<loc
-00003cf0: 616c 733e 2e6f 626a 6563 7469 7665 7260  als>.objectiver`
-00003d00: 0000 0072 6100 0000 7262 0000 0072 5c00  ...ra...rb...r\.
-00003d10: 0000 7205 0100 0072 0601 0000 2901 da05  ..r....r....)...
-00003d20: 6474 7970 6529 0472 6000 0000 7261 0000  dtype).r`...ra..
-00003d30: 0072 6200 0000 725c 0000 007a 2953 6f6d  .rb...r\...z)Som
-00003d40: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
-00003d50: 206e 6f74 2066 6c6f 6174 7320 6f72 2073   not floats or s
-00003d60: 7472 696e 6773 72bd 0000 0029 0272 be00  tringsr....).r..
-00003d70: 0000 72bf 0000 0054 72c0 0000 007a 2647  ..r....Tr....z&G
-00003d80: 7269 6420 7365 6172 6368 2069 6d70 726f  rid search impro
-00003d90: 7665 6420 6576 616c 206d 6574 7269 6320  ved eval metric 
-00003da0: 6672 6f6d 207a 0420 746f 20da 012e 72c3  from z. to ...r.
-00003db0: 0000 007a 2d47 7269 6420 7365 6172 6368  ...z-Grid search
-00003dc0: 2063 6f75 6c64 206e 6f74 2069 6d70 726f   could not impro
-00003dd0: 7665 2065 7661 6c20 6d65 7472 6963 206f  ve eval metric o
-00003de0: 6620 7a19 2e20 4265 7374 2073 636f 7265  f z.. Best score
-00003df0: 2072 6561 6368 6564 2077 6173 2029 2072   reached was ) r
-00003e00: 1200 0000 7203 0000 0072 2e00 0000 721b  ....r....r....r.
-00003e10: 0000 0072 1900 0000 721a 0000 0072 1c00  ...r....r....r..
-00003e20: 0000 7242 0000 0072 3000 0000 da0a 6973  ..rB...r0.....is
-00003e30: 696e 7374 616e 6365 7252 0000 00da 0566  instancerR.....f
-00003e40: 6c6f 6174 721f 0000 00da 086c 696e 7370  loatr......linsp
-00003e50: 6163 65da 2167 7269 6473 6561 7263 685f  ace.!gridsearch_
-00003e60: 6e62 5f70 6172 616d 6574 6572 735f 7065  nb_parameters_pe
-00003e70: 725f 6772 6964 72d6 0000 0072 4400 0000  r_gridr....rD...
-00003e80: 72c6 0000 0072 c400 0000 5a0b 4772 6964  r....r....Z.Grid
-00003e90: 5361 6d70 6c65 7272 c700 0000 72b3 0000  Samplerr....r...
-00003ea0: 00da 046b 6579 73da 2267 7269 6473 6561  ...keys."gridsea
-00003eb0: 7263 685f 7475 6e69 6e67 5f6d 6178 5f72  rch_tuning_max_r
-00003ec0: 756e 7469 6d65 5f73 6563 7372 ca00 0000  untime_secsr....
-00003ed0: 72cb 0000 0072 cc00 0000 72cd 0000 0072  r....r....r....r
-00003ee0: ce00 0000 72cf 0000 0072 4700 0000 72d0  ....r....rG...r.
-00003ef0: 0000 0029 0c72 2400 0000 7231 0000 0072  ...).r$...r1...r
-00003f00: 3200 0000 7233 0000 0072 3400 0000 7267  2...r3...r4...rg
-00003f10: 0000 005a 0c73 6561 7263 685f 7370 6163  ...Z.search_spac
-00003f20: 655a 0d62 6573 745f 7363 6f72 655f 6376  eZ.best_score_cv
-00003f30: 72d2 0000 0072 d300 0000 72d8 0000 005a  r....r....r....Z
-00003f40: 1778 6762 6f6f 7374 5f67 7269 645f 6265  .xgboost_grid_be
-00003f50: 7374 5f70 6172 616d 7225 0000 0072 0701  st_paramr%...r..
-00003f60: 0000 7226 0000 0072 4b00 0000 9702 0000  ..r&...rK.......
-00003f70: 73ae 0000 0012 0704 0202 ff04 0202 fe04  s...............
-00003f80: 0302 fd04 0402 fc02 0602 0104 ff14 0408  ................
-00003f90: 5a10 0202 ff10 0202 fe10 0302 fd10 0402  Z...............
-00003fa0: fc04 070a 0102 0102 ff0e 0206 0102 0104  ................
-00003fb0: fb04 070e 010e 0106 0102 0104 fc04 060e  ................
-00003fc0: 010e 0106 0102 0104 fc04 060e 010e 0106  ................
-00003fd0: 0102 0104 fc08 ec08 1c08 0204 020c 0106  ................
-00003fe0: ff04 0302 0106 010a 0102 ff06 0202 0102  ................
-00003ff0: 0106 fa02 090c 0108 010c 010c 0112 0104  ................
-00004000: 0102 ff08 0312 0208 0110 0102 0102 010c  ................
-00004010: ff10 0310 0102 0110 0104 ff16 0302 020e  ................
-00004020: 0108 ff7a 1658 6762 6f6f 7374 4d6f 6465  ...z.XgboostMode
-00004030: 6c2e 6669 6e65 5f74 756e 65da 0264 6663  l.fine_tune..dfc
-00004040: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00004050: 0500 0000 4300 0000 73d0 0000 0074 0074  ....C...s....t.t
-00004060: 01a0 02a1 009b 0064 019d 0283 0101 007c  .......d.......|
-00004070: 006a 0372 0f7c 006a 0473 1374 0564 0283  .j.r.|.j.s.t.d..
-00004080: 0182 017c 006a 0672 217c 006a 066a 077c  ...|.j.r!|.j.j.|
-00004090: 0164 0364 0464 058d 035c 027d 017d 0274  .d.d.d...\.}.}.t
-000040a0: 086a 097c 017c 006a 046a 0a64 068d 027d  .j.|.|.j.j.d...}
-000040b0: 037c 006a 0b73 3174 0c64 0783 0182 017c  .|.j.s1t.d.....|
-000040c0: 006a 0d73 3874 0c64 0883 0182 017c 006a  .j.s8t.d.....|.j
-000040d0: 0ba0 0e7c 03a1 017d 047c 006a 0f64 096b  ...|...}.|.j.d.k
-000040e0: 0272 5474 10a0 1164 0a64 0b84 007c 0444  .rTt...d.d...|.D
-000040f0: 0083 01a1 017d 057c 057c 006a 0d6a 126b  .....}.|.|.j.j.k
-00004100: 047d 066e 0c7c 047d 0574 10a0 1164 0c64  .}.n.|.}.t...d.d
-00004110: 0b84 007c 0444 0083 01a1 017d 0674 0064  ...|.D.....}.t.d
-00004120: 0d83 0101 007c 057c 0666 0253 0029 0e7a  .....|.|.f.S.).z
-00004130: 1750 7265 6469 6374 206f 6e20 756e 7365  .Predict on unse
-00004140: 656e 2064 6174 612e fa33 3a20 5374 6172  en data..3: Star
-00004150: 7420 7072 6564 6963 7469 6e67 206f 6e20  t predicting on 
-00004160: 6e65 7720 6461 7461 2075 7369 6e67 2058  new data using X
-00004170: 6762 6f6f 7374 206d 6f64 656c 2efa 2c63  gboost model..,c
-00004180: 6f6e 665f 7061 7261 6d73 5f78 6762 6f6f  onf_params_xgboo
-00004190: 7374 206f 7220 636f 6e66 5f74 7261 696e  st or conf_train
-000041a0: 696e 6720 6973 204e 6f6e 654e 5472 3600  ing is NoneNTr6.
-000041b0: 0000 a901 726f 0000 00fa 204e 6f20 7472  ....ro.... No tr
-000041c0: 6169 6e65 6420 6d6f 6465 6c20 6861 7320  ained model has 
-000041d0: 6265 656e 2066 6f75 6e64 2efa 2b4e 6f20  been found..+No 
-000041e0: 6d6f 6465 6c20 636f 6e66 6967 7572 6174  model configurat
-000041f0: 696f 6e20 6669 6c65 2068 6173 2062 6565  ion file has bee
-00004200: 6e20 666f 756e 642e 7217 0000 0063 0100  n found.r....c..
-00004210: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00004220: 0000 5300 0000 f314 0000 0067 007c 005d  ..S........g.|.]
-00004230: 067d 017c 0164 0019 0091 0271 0253 00a9  .}.|.d.....q.S..
-00004240: 0172 3c00 0000 7225 0000 0072 dc00 0000  .r<...r%...r....
-00004250: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00004260: 7800 0000 6b03 0000 f302 0000 0014 007a  x...k..........z
-00004270: 2858 6762 6f6f 7374 4d6f 6465 6c2e 7072  (XgboostModel.pr
-00004280: 6564 6963 742e 3c6c 6f63 616c 733e 2e3c  edict.<locals>.<
-00004290: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
-000042a0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-000042b0: 0000 72d9 0000 0072 2500 0000 72da 0000  ..r....r%...r...
-000042c0: 0072 dc00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-000042d0: 7226 0000 0072 7800 0000 7103 0000 72de  r&...rx...q...r.
-000042e0: 0000 00fa 1346 696e 6973 6865 6420 7072  .....Finished pr
-000042f0: 6564 6963 7469 6e67 2913 7212 0000 0072  edicting).r....r
-00004300: 0300 0000 722e 0000 0072 1a00 0000 7219  ....r....r....r.
-00004310: 0000 0072 4200 0000 721d 0000 0072 4d00  ...rB...r....rM.
-00004320: 0000 7255 0000 0072 a700 0000 72a8 0000  ..rU...r....r...
-00004330: 0072 1e00 0000 da09 4578 6365 7074 696f  .r......Exceptio
-00004340: 6e72 1b00 0000 72e1 0000 0072 1600 0000  nr....r....r....
-00004350: 721f 0000 0072 e200 0000 da18 636c 6173  r....r......clas
-00004360: 7369 6669 6361 7469 6f6e 5f74 6872 6573  sification_thres
-00004370: 686f 6c64 2907 7224 0000 0072 1001 0000  hold).r$...r....
-00004380: da01 5f72 5800 0000 da0d 7061 7274 6961  .._rX.....partia
-00004390: 6c5f 7072 6f62 73da 0f70 7265 6469 6374  l_probs..predict
-000043a0: 6564 5f70 726f 6273 5a11 7072 6564 6963  ed_probsZ.predic
-000043b0: 7465 645f 636c 6173 7365 7372 2500 0000  ted_classesr%...
-000043c0: 7225 0000 0072 2600 0000 72e1 0000 0051  r%...r&...r....Q
-000043d0: 0300 0073 3400 0000 0202 0c01 04ff 0c03  ...s4...........
-000043e0: 0801 0602 0601 0601 0aff 0404 0201 0601  ................
-000043f0: 06fe 0605 0801 0602 0801 0c02 0a01 1401  ................
-00004400: 0a02 04ff 0404 1401 0801 0801 7a14 5867  ............z.Xg
-00004410: 626f 6f73 744d 6f64 656c 2e70 7265 6469  boostModel.predi
-00004420: 6374 6302 0000 0000 0000 0000 0000 0006  ctc.............
-00004430: 0000 0005 0000 0043 0000 0073 ac00 0000  .......C...s....
-00004440: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
-00004450: 0100 7c00 6a03 720f 7c00 6a04 7313 7405  ..|.j.r.|.j.s.t.
-00004460: 6402 8301 8201 7c00 6a06 7221 7c00 6a06  d.....|.j.r!|.j.
-00004470: 6a07 7c01 6403 6404 6405 8d03 5c02 7d01  j.|.d.d.d...\.}.
-00004480: 7d02 7408 6a09 7c01 7c00 6a04 6a0a 6406  }.t.j.|.|.j.j.d.
-00004490: 8d02 7d03 7c00 6a0b 7331 740c 6407 8301  ..}.|.j.s1t.d...
-000044a0: 8201 7c00 6a0d 7338 740c 6408 8301 8201  ..|.j.s8t.d.....
-000044b0: 7c00 6a0b a00e 7c03 a101 7d04 7c00 6a0f  |.j...|...}.|.j.
-000044c0: 6409 6b02 724e 7410 a011 640a 640b 8400  d.k.rNt...d.d...
-000044d0: 7c04 4400 8301 a101 7d05 6e02 7c04 7d05  |.D.....}.n.|.}.
-000044e0: 7400 640c 8301 0100 7c05 5300 290d 7a24  t.d.....|.S.).z$
-000044f0: 5072 6564 6963 7420 636c 6173 7320 7363  Predict class sc
-00004500: 6f72 6573 206f 6e20 756e 7365 656e 2064  ores on unseen d
-00004510: 6174 612e 7211 0100 0072 1201 0000 4e54  ata.r....r....NT
-00004520: 7236 0000 0072 1301 0000 7214 0100 0072  r6...r....r....r
-00004530: 1501 0000 7217 0000 0063 0100 0000 0000  ....r....c......
-00004540: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00004550: 0000 7216 0100 0072 1701 0000 7225 0000  ..r....r....r%..
-00004560: 0072 dc00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00004570: 7226 0000 0072 7800 0000 8f03 0000 7218  r&...rx.......r.
-00004580: 0100 007a 2e58 6762 6f6f 7374 4d6f 6465  ...z.XgboostMode
-00004590: 6c2e 7072 6564 6963 745f 7072 6f62 612e  l.predict_proba.
-000045a0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000045b0: 6d70 3e72 1901 0000 2912 7212 0000 0072  mp>r....).r....r
-000045c0: 0300 0000 722e 0000 0072 1a00 0000 7219  ....r....r....r.
-000045d0: 0000 0072 4200 0000 721d 0000 0072 4d00  ...rB...r....rM.
-000045e0: 0000 7255 0000 0072 a700 0000 72a8 0000  ..rU...r....r...
-000045f0: 0072 1e00 0000 721a 0100 0072 1b00 0000  .r....r....r....
-00004600: 72e1 0000 0072 1600 0000 721f 0000 0072  r....r....r....r
-00004610: e200 0000 2906 7224 0000 0072 1001 0000  ....).r$...r....
-00004620: 721c 0100 0072 5800 0000 721d 0100 0072  r....rX...r....r
-00004630: 1e01 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
-00004640: 0000 00da 0d70 7265 6469 6374 5f70 726f  .....predict_pro
-00004650: 6261 7503 0000 732e 0000 0002 020c 0104  bau...s.........
-00004660: ff0c 0308 0106 0206 0106 010a ff04 0402  ................
-00004670: 0106 0106 fe06 0508 0106 0208 010c 020a  ................
-00004680: 0116 0104 0208 0104 017a 1a58 6762 6f6f  .........z.Xgboo
-00004690: 7374 4d6f 6465 6c2e 7072 6564 6963 745f  stModel.predict_
-000046a0: 7072 6f62 6129 054e 4e4e 4e4e 2901 727a  proba).NNNNN).rz
-000046b0: 0000 0029 27da 085f 5f6e 616d 655f 5fda  ...)'..__name__.
-000046c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000046d0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000046e0: 5f5f 7207 0000 0072 0800 0000 720d 0000  __r....r....r...
-000046f0: 0072 0f00 0000 720e 0000 0072 1000 0000  .r....r....r....
-00004700: 7214 0000 0072 2700 0000 724f 0000 00da  r....r'...rO....
-00004710: 0653 6572 6965 7372 0500 0000 da03 7374  .Seriesr......st
-00004720: 7272 0b01 0000 722d 0000 0072 3000 0000  rr....r-...r0...
-00004730: da09 4461 7461 4672 616d 6572 5500 0000  ..DataFramerU...
-00004740: da07 426f 6f73 7465 7272 5a00 0000 7248  ..BoosterrZ...rH
-00004750: 0000 0072 d600 0000 7251 0000 0072 ab00  ...r....rQ...r..
-00004760: 0000 7202 0100 0072 f700 0000 7206 0000  ..r....r....r...
-00004770: 0072 fa00 0000 7204 0000 0072 ae00 0000  .r....r....r....
-00004780: 724b 0000 0072 0900 0000 721f 0000 00da  rK...r....r.....
-00004790: 076e 6461 7272 6179 72e1 0000 0072 1f01  .ndarrayr....r..
-000047a0: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-000047b0: 0072 2600 0000 7215 0000 001f 0000 0073  .r&...r........s
-000047c0: a800 0000 0800 0401 0205 0201 0201 0201  ................
-000047d0: 0201 04f9 0602 02fe 0603 02fd 0604 02fc  ................
-000047e0: 0605 02fb 0606 02fa 0607 0af9 1c17 0807  ................
-000047f0: 0215 0402 02fe 0403 02fd 0404 02fc 0405  ................
-00004800: 02fb 0406 0afa 024a 0402 02fe 0403 02fd  .......J........
-00004810: 0404 02fc 0405 02fb 0206 0afa 007f 0870  ...............p
-00004820: 0813 0816 0222 04ff 0401 02ff 0401 02ff  ....."..........
-00004830: 0201 0aff 1623 021d 0a02 02fe 0403 02fd  .....#..........
-00004840: 0404 02fc 0405 02fb 0406 02fa 0207 0af9  ................
-00004850: 027f 0402 02fe 0403 02fd 0404 02fc 0405  ................
-00004860: 02fb 0206 0afa 007f 203b 1a24 7215 0000  ........ ;.$r...
-00004870: 0029 2672 2301 0000 da04 636f 7079 7202  .)&r#.....copyr.
-00004880: 0000 0072 0300 0000 da06 7479 7069 6e67  ...r......typing
-00004890: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-000048a0: 0700 0000 7208 0000 0072 0900 0000 da05  ....r....r......
-000048b0: 6e75 6d70 7972 1f00 0000 7244 0000 00da  numpyr....rD....
-000048c0: 0670 616e 6461 7372 4f00 0000 72bc 0000  .pandasrO...r...
-000048d0: 0072 5500 0000 da0f 736b 6c65 6172 6e2e  .rU.....sklearn.
-000048e0: 6d65 7472 6963 7372 0a00 0000 da17 736b  metricsr......sk
-000048f0: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
-00004900: 6374 696f 6e72 0b00 0000 da0d 736b 6c65  ctionr......skle
-00004910: 6172 6e2e 7574 696c 7372 0c00 0000 da1f  arn.utilsr......
-00004920: 626c 7565 6361 7374 2e63 6f6e 6669 672e  bluecast.config.
-00004930: 7472 6169 6e69 6e67 5f63 6f6e 6669 6772  training_configr
-00004940: 0d00 0000 720e 0000 0072 0f00 0000 da21  ....r....r.....!
-00004950: 626c 7565 6361 7374 2e65 7870 6572 696d  bluecast.experim
-00004960: 656e 7461 7469 6f6e 2e74 7261 636b 696e  entation.trackin
-00004970: 6772 1000 0000 da24 626c 7565 6361 7374  gr.....$bluecast
-00004980: 2e67 656e 6572 616c 5f75 7469 6c73 2e67  .general_utils.g
-00004990: 656e 6572 616c 5f75 7469 6c73 7211 0000  eneral_utilsr...
-000049a0: 0072 1200 0000 5a22 626c 7565 6361 7374  .r....Z"bluecast
-000049b0: 2e6d 6c5f 6d6f 6465 6c6c 696e 672e 6261  .ml_modelling.ba
-000049c0: 7365 5f63 6c61 7373 6573 7213 0000 00da  se_classesr.....
-000049d0: 1d62 6c75 6563 6173 742e 7072 6570 726f  .bluecast.prepro
-000049e0: 6365 7373 696e 672e 6375 7374 6f6d 7214  cessing.customr.
-000049f0: 0000 0072 1500 0000 7225 0000 0072 2500  ...r....r%...r%.
-00004a00: 0000 7225 0000 0072 2600 0000 da08 3c6d  ..r%...r&.....<m
-00004a10: 6f64 756c 653e 0100 0000 7322 0000 0004  odule>....s"....
-00004a20: 000c 070c 0120 0108 0208 0108 0108 010c  ..... ..........
-00004a30: 010c 010c 0114 020c 0510 010c 010c 0114  ................
-00004a40: 03                                       .
+000000d0: 640b 6c1e 6d1f 5a1f 6d20 5a20 6d21 5a21  d.l.m.Z.m Z m!Z!
+000000e0: 0100 6401 640c 6c22 6d23 5a23 0100 6401  ..d.d.l"m#Z#..d.
+000000f0: 640d 6c24 6d25 5a25 0100 4700 640e 640f  d.l$m%Z%..G.d.d.
+00000100: 8400 640f 6523 8303 5a26 6405 5300 2910  ..d.e#..Z&d.S.).
+00000110: 6119 0100 0058 6762 6f6f 7374 2063 6c61  a....Xgboost cla
+00000120: 7373 6966 6963 6174 696f 6e20 6d6f 6465  ssification mode
+00000130: 6c2e 0a0a 5468 6973 206d 6f64 756c 6520  l...This module 
+00000140: 636f 6e74 6169 6e73 2061 2077 7261 7070  contains a wrapp
+00000150: 6572 2066 6f72 2074 6865 2058 6762 6f6f  er for the Xgboo
+00000160: 7374 2063 6c61 7373 6966 6963 6174 696f  st classificatio
+00000170: 6e20 6d6f 6465 6c2e 2049 7420 6361 6e20  n model. It can 
+00000180: 6265 2075 7365 6420 746f 2074 7261 696e  be used to train
+00000190: 2061 6e64 2f6f 7220 7475 6e65 2074 6865   and/or tune the
+000001a0: 206d 6f64 656c 2e0a 4974 2061 6c73 6f20   model..It also 
+000001b0: 6361 6c63 756c 6174 6573 2063 6c61 7373  calculates class
+000001c0: 2077 6569 6768 7473 2066 6f72 2069 6d62   weights for imb
+000001d0: 616c 616e 6365 6420 6461 7461 7365 7473  alanced datasets
+000001e0: 2e20 5468 6520 7765 6967 6874 7320 6d61  . The weights ma
+000001f0: 7920 6f72 206d 6179 206e 6f74 2062 6520  y or may not be 
+00000200: 7573 6564 2064 6565 7065 6e64 696e 6720  used deepending 
+00000210: 6f6e 2074 6865 0a68 7970 6572 7061 7261  on the.hyperpara
+00000220: 6d65 7465 7220 7475 6e69 6e67 2e0a e900  meter tuning....
+00000230: 0000 0029 01da 0864 6565 7063 6f70 7929  ...)...deepcopy)
+00000240: 01da 0864 6174 6574 696d 6529 06da 0341  ...datetime)...A
+00000250: 6e79 da04 4469 6374 da04 4c69 7374 da07  ny..Dict..List..
+00000260: 4c69 7465 7261 6cda 084f 7074 696f 6e61  Literal..Optiona
+00000270: 6cda 0554 7570 6c65 4e29 01da 116d 6174  l..TupleN)...mat
+00000280: 7468 6577 735f 636f 7272 636f 6566 2901  thews_corrcoef).
+00000290: da0f 5374 7261 7469 6669 6564 4b46 6f6c  ..StratifiedKFol
+000002a0: 6429 01da 0c63 6c61 7373 5f77 6569 6768  d)...class_weigh
+000002b0: 7429 03da 0e54 7261 696e 696e 6743 6f6e  t)...TrainingCon
+000002c0: 6669 67da 1758 6762 6f6f 7374 4669 6e61  fig..XgboostFina
+000002d0: 6c50 6172 616d 436f 6e66 6967 da17 5867  lParamConfig..Xg
+000002e0: 626f 6f73 7454 756e 6550 6172 616d 7343  boostTuneParamsC
+000002f0: 6f6e 6669 6729 01da 1145 7870 6572 696d  onfig)...Experim
+00000300: 656e 7454 7261 636b 6572 2903 da11 6368  entTracker)...ch
+00000310: 6563 6b5f 6770 755f 7375 7070 6f72 74da  eck_gpu_support.
+00000320: 0c6c 6f67 5f73 616d 706c 696e 67da 066c  .log_sampling..l
+00000330: 6f67 6765 7229 01da 1042 6173 6543 6c61  ogger)...BaseCla
+00000340: 7373 4d6c 4d6f 6465 6c29 01da 1343 7573  ssMlModel)...Cus
+00000350: 746f 6d50 7265 7072 6f63 6573 7369 6e67  tomPreprocessing
+00000360: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000370: 000e 0000 0040 0000 0073 9e01 0000 6500  .....@...s....e.
+00000380: 5a01 6400 5a02 6401 5a03 0902 0902 0902  Z.d.Z.d.Z.......
+00000390: 0902 0902 6433 6403 6504 6404 1900 6405  ....d3d.e.d...d.
+000003a0: 6505 6506 1900 6406 6505 6507 1900 6407  e.e...d.e.e...d.
+000003b0: 6505 6508 1900 6408 6505 6509 1900 6409  e.e...d.e.e...d.
+000003c0: 6505 650a 1900 660c 640a 640b 8405 5a0b  e.e...f.d.d...Z.
+000003d0: 640c 650c 6a0d 640d 650e 650f 6510 6602  d.e.j.d.e.e.e.f.
+000003e0: 1900 6604 640e 640f 8404 5a11 6410 6411  ..f.d.d...Z.d.d.
+000003f0: 8400 5a12 6412 650c 6a13 6413 650c 6a13  ..Z.d.e.j.d.e.j.
+00000400: 6414 650c 6a0d 6415 650c 6a0d 640d 6514  d.e.j.d.e.j.d.e.
+00000410: 6a15 660a 6416 6417 8404 5a16 6412 650c  j.f.d.d...Z.d.e.
+00000420: 6a13 6413 650c 6a13 6414 650c 6a0d 6415  j.d.e.j.d.e.j.d.
+00000430: 650c 6a0d 640d 6402 660a 6418 6419 8404  e.j.d.d.f.d.d...
+00000440: 5a17 641a 641b 8400 5a18 641c 641d 8400  Z.d.d...Z.d.d...
+00000450: 5a19 641e 641f 8400 5a1a 0920 6434 6421  Z.d.d...Z.. d4d!
+00000460: 650c 6a13 6422 650c 6a0d 6423 651b 6606  e.j.d"e.j.d#e.f.
+00000470: 6424 6425 8405 5a1c 6426 651d 6510 1900  d$d%..Z.d&e.e...
+00000480: 640d 6510 6604 6427 6428 8404 5a1e 6429  d.e.f.d'd(..Z.d)
+00000490: 650e 650f 651f 6602 1900 6412 650c 6a13  e.e.e.f...d.e.j.
+000004a0: 6414 650c 6a0d 6413 650c 6a13 6415 650c  d.e.j.d.e.j.d.e.
+000004b0: 6a0d 660a 642a 642b 8404 5a20 6412 650c  j.f.d*d+..Z d.e.
+000004c0: 6a13 6413 650c 6a13 6414 650c 6a0d 6415  j.d.e.j.d.e.j.d.
+000004d0: 650c 6a0d 640d 6402 660a 642c 642d 8404  e.j.d.d.f.d,d-..
+000004e0: 5a21 642e 650c 6a13 640d 6522 6523 6a24  Z!d.e.j.d.e"e#j$
+000004f0: 6523 6a24 6602 1900 6604 642f 6430 8404  e#j$f...f.d/d0..
+00000500: 5a25 642e 650c 6a13 640d 6523 6a24 6604  Z%d.e.j.d.e#j$f.
+00000510: 6431 6432 8404 5a26 6402 5300 2935 da0c  d1d2..Z&d.S.)5..
+00000520: 5867 626f 6f73 744d 6f64 656c 7a2f 5472  XgboostModelz/Tr
+00000530: 6169 6e20 616e 642f 6f72 2074 756e 6520  ain and/or tune 
+00000540: 5867 626f 6f73 7420 636c 6173 7369 6669  Xgboost classifi
+00000550: 6361 7469 6f6e 206d 6f64 656c 2e4e da0d  cation model.N..
+00000560: 636c 6173 735f 7072 6f62 6c65 6d29 02da  class_problem)..
+00000570: 0662 696e 6172 79da 0a6d 756c 7469 636c  .binary..multicl
+00000580: 6173 73da 0d63 6f6e 665f 7472 6169 6e69  ass..conf_traini
+00000590: 6e67 da0c 636f 6e66 5f78 6762 6f6f 7374  ng..conf_xgboost
+000005a0: da13 636f 6e66 5f70 6172 616d 735f 7867  ..conf_params_xg
+000005b0: 626f 6f73 74da 1265 7870 6572 696d 656e  boost..experimen
+000005c0: 745f 7472 6163 6b65 72da 1b63 7573 746f  t_tracker..custo
+000005d0: 6d5f 696e 5f66 6f6c 645f 7072 6570 726f  m_in_fold_prepro
+000005e0: 6365 7373 6f72 6307 0000 0000 0000 0000  cessorc.........
+000005f0: 0000 0007 0000 0003 0000 0043 0000 0073  ...........C...s
+00000600: 5800 0000 6400 7c00 5f00 7c01 7c00 5f01  X...d.|._.|.|._.
+00000610: 7c02 7c00 5f02 7c03 7c00 5f03 7c04 7c00  |.|._.|.|._.|.|.
+00000620: 5f04 7c05 7c00 5f05 7c06 7c00 5f06 7c00  _.|.|._.|.|._.|.
+00000630: 6a02 7223 7407 6a08 a009 7c00 6a02 6a0a  j.r#t.j...|.j.j.
+00000640: a101 7c00 5f0b 6400 5300 7407 6a08 a009  ..|._.d.S.t.j...
+00000650: 6401 a101 7c00 5f0b 6400 5300 2902 4e72  d...|._.d.S.).Nr
+00000660: 0100 0000 290c da05 6d6f 6465 6c72 1700  ....)...modelr..
+00000670: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000680: 0072 1d00 0000 721e 0000 00da 026e 70da  .r....r......np.
+00000690: 0672 616e 646f 6dda 0b64 6566 6175 6c74  .random..default
+000006a0: 5f72 6e67 da13 676c 6f62 616c 5f72 616e  _rng..global_ran
+000006b0: 646f 6d5f 7374 6174 65da 1072 616e 646f  dom_state..rando
+000006c0: 6d5f 6765 6e65 7261 746f 7229 07da 0473  m_generator)...s
+000006d0: 656c 6672 1700 0000 721a 0000 0072 1b00  elfr....r....r..
+000006e0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000006f0: 00a9 0072 2600 0000 fa43 2f68 6f6d 652f  ...r&....C/home/
+00000700: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
+00000710: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
+00000720: 6563 6173 742f 6d6c 5f6d 6f64 656c 6c69  ecast/ml_modelli
+00000730: 6e67 2f78 6762 6f6f 7374 2e70 79da 085f  ng/xgboost.py.._
+00000740: 5f69 6e69 745f 5f22 0000 0073 1800 0000  _init__"...s....
+00000750: 0609 0601 0601 0601 0601 0601 0601 0601  ................
+00000760: 0601 0601 0aff 1204 7a15 5867 626f 6f73  ........z.Xgboos
+00000770: 744d 6f64 656c 2e5f 5f69 6e69 745f 5fda  tModel.__init__.
+00000780: 0179 da06 7265 7475 726e 6302 0000 0000  .y..returnc.....
+00000790: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+000007a0: 0000 0073 1200 0000 7400 6a01 6401 7c01  ...s....t.j.d.|.
+000007b0: 6402 8d02 7d02 7c02 5300 2903 7a29 4361  d...}.|.S.).z)Ca
+000007c0: 6c63 756c 6174 6520 636c 6173 7320 7765  lculate class we
+000007d0: 6967 6874 7320 6f66 2074 6172 6765 7420  ights of target 
+000007e0: 636f 6c75 6d6e 2eda 0862 616c 616e 6365  column...balance
+000007f0: 6429 0272 0c00 0000 7229 0000 0029 0272  d).r....r)...).r
+00000800: 0c00 0000 da15 636f 6d70 7574 655f 7361  ......compute_sa
+00000810: 6d70 6c65 5f77 6569 6768 7429 0372 2500  mple_weight).r%.
+00000820: 0000 7229 0000 00da 0f63 6c61 7373 6573  ..r).....classes
+00000830: 5f77 6569 6768 7473 7226 0000 0072 2600  _weightsr&...r&.
+00000840: 0000 7227 0000 00da 1763 616c 6375 6c61  ..r'.....calcula
+00000850: 7465 5f63 6c61 7373 5f77 6569 6768 7473  te_class_weights
+00000860: 3900 0000 7308 0000 0004 0204 0106 ff04  9...s...........
+00000870: 037a 2458 6762 6f6f 7374 4d6f 6465 6c2e  .z$XgboostModel.
+00000880: 6361 6c63 756c 6174 655f 636c 6173 735f  calculate_class_
+00000890: 7765 6967 6874 7363 0100 0000 0000 0000  weightsc........
+000008a0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000008b0: 73b4 0000 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
+000008c0: 019d 0283 0101 007c 006a 0373 1a74 0483  .......|.j.s.t..
+000008d0: 007c 005f 0374 0074 01a0 02a1 009b 0064  .|._.t.t.......d
+000008e0: 029d 0283 0101 006e 0974 0074 01a0 02a1  .......n.t.t....
+000008f0: 009b 0064 039d 0283 0101 007c 006a 0573  ...d.......|.j.s
+00000900: 3474 0683 007c 005f 0574 0074 01a0 02a1  4t...|._.t.t....
+00000910: 009b 0064 049d 0283 0101 006e 0974 0074  ...d.......n.t.t
+00000920: 01a0 02a1 009b 0064 059d 0283 0101 007c  .......d.......|
+00000930: 006a 0773 4f74 0883 007c 005f 0774 0074  .j.sOt...|._.t.t
+00000940: 01a0 02a1 009b 0064 069d 0283 0101 0064  .......d.......d
+00000950: 0853 0074 0074 01a0 02a1 009b 0064 079d  .S.t.t.......d..
+00000960: 0283 0101 0064 0853 0029 097a 364c 6f61  .....d.S.).z6Loa
+00000970: 6420 6d75 6c74 6970 6c65 2063 6f6e 6669  d multiple confi
+00000980: 6773 206f 7220 6c6f 6164 2064 6566 6175  gs or load defau
+00000990: 6c74 2063 6f6e 6669 6773 2069 6e73 7465  lt configs inste
+000009a0: 6164 2e7a 323a 2053 7461 7274 206c 6f61  ad.z2: Start loa
+000009b0: 6469 6e67 2065 7869 7374 696e 6720 6f72  ding existing or
+000009c0: 2064 6566 6175 6c74 2063 6f6e 6669 6720   default config 
+000009d0: 6669 6c65 732e 2e7a 1e3a 204c 6f61 6420  files..z.: Load 
+000009e0: 6465 6661 756c 7420 5472 6169 6e69 6e67  default Training
+000009f0: 436f 6e66 6967 2e7a 203a 2046 6f75 6e64  Config.z : Found
+00000a00: 2070 726f 7669 6465 6420 5472 6169 6e69   provided Traini
+00000a10: 6e67 436f 6e66 6967 2e7a 273a 204c 6f61  ngConfig.z': Loa
+00000a20: 6420 6465 6661 756c 7420 5867 626f 6f73  d default Xgboos
+00000a30: 7454 756e 6550 6172 616d 7343 6f6e 6669  tTuneParamsConfi
+00000a40: 672e 7a29 3a20 466f 756e 6420 7072 6f76  g.z): Found prov
+00000a50: 6964 6564 2058 6762 6f6f 7374 5475 6e65  ided XgboostTune
+00000a60: 5061 7261 6d73 436f 6e66 6967 2e7a 273a  ParamsConfig.z':
+00000a70: 204c 6f61 6420 6465 6661 756c 7420 5867   Load default Xg
+00000a80: 626f 6f73 7446 696e 616c 5061 7261 6d43  boostFinalParamC
+00000a90: 6f6e 6669 672e 7a29 3a20 466f 756e 6420  onfig.z): Found 
+00000aa0: 7072 6f76 6964 6564 2058 6762 6f6f 7374  provided Xgboost
+00000ab0: 4669 6e61 6c50 6172 616d 436f 6e66 6967  FinalParamConfig
+00000ac0: 2e4e 2909 7213 0000 0072 0300 0000 da06  .N).r....r......
+00000ad0: 7574 636e 6f77 721a 0000 0072 0d00 0000  utcnowr....r....
+00000ae0: 721b 0000 0072 0f00 0000 721c 0000 0072  r....r....r....r
+00000af0: 0e00 0000 2901 7225 0000 0072 2600 0000  ....).r%...r&...
+00000b00: 7226 0000 0072 2700 0000 da10 6368 6563  r&...r'.....chec
+00000b10: 6b5f 6c6f 6164 5f63 6f6e 6673 4000 0000  k_load_confs@...
+00000b20: 731a 0000 0012 0206 0108 0114 0112 0206  s...............
+00000b30: 0208 0114 0112 0206 0208 0116 0116 027a  ...............z
+00000b40: 1d58 6762 6f6f 7374 4d6f 6465 6c2e 6368  .XgboostModel.ch
+00000b50: 6563 6b5f 6c6f 6164 5f63 6f6e 6673 da07  eck_load_confs..
+00000b60: 785f 7472 6169 6eda 0678 5f74 6573 74da  x_train..x_test.
+00000b70: 0779 5f74 7261 696e da06 795f 7465 7374  .y_train..y_test
+00000b80: 6305 0000 0000 0000 0000 0000 0009 0000  c...............
+00000b90: 0008 0000 0043 0000 0073 9c01 0000 7400  .....C...s....t.
+00000ba0: 7401 a002 a100 9b00 6401 9d02 8301 0100  t.......d.......
+00000bb0: 7c00 a003 a100 0100 7c00 6a04 7216 7c00  |.......|.j.r.|.
+00000bc0: 6a05 7216 7c00 6a06 731a 7407 6402 8301  j.r.|.j.s.t.d...
+00000bd0: 8201 7c00 6a05 6a08 7326 7409 6a0a a00b  ..|.j.j.s&t.j...
+00000be0: 7409 6a0a 6a0c a101 0100 7c00 6a05 6a0d  t.j.j.....|.j.j.
+00000bf0: 7236 7c00 a00e 7c01 7c02 7c03 7c04 a104  r6|...|.|.|.|...
+00000c00: 0100 740f 6403 8301 0100 7c00 6a05 6a10  ..t.d.....|.j.j.
+00000c10: 7246 7c00 a011 7c01 7c02 7c03 7c04 a104  rF|...|.|.|.|...
+00000c20: 0100 740f 6404 8301 0100 7400 6405 8301  ..t.d.....t.d...
+00000c30: 0100 7c00 6a12 7261 7c00 6a12 a013 7c01  ..|.j.ra|.j...|.
+00000c40: 7c03 a102 5c02 7d01 7d03 7c00 6a12 6a14  |...\.}.}.|.j.j.
+00000c50: 7c02 7c04 6406 6407 8d03 5c02 7d02 7d04  |.|.d.d...\.}.}.
+00000c60: 7c00 6a05 6a15 727c 7400 7401 a002 a100  |.j.j.r|t.t.....
+00000c70: 9b00 6408 9d02 8301 0100 7416 a017 7c01  ..d.......t...|.
+00000c80: 7c02 6702 a101 7d01 7416 a017 7c03 7c04  |.g...}.t...|.|.
+00000c90: 6702 a101 7d03 7c00 a018 7c01 7c03 7c02  g...}.|...|.|.|.
+00000ca0: 7c04 a104 5c02 7d05 7d06 7c05 6409 6602  |...\.}.}.|.d.f.
+00000cb0: 7c06 640a 6602 6702 7d07 7c00 6a04 6a19  |.d.f.g.}.|.j.j.
+00000cc0: a01a 640b 640c a102 7d08 7c00 6a05 6a1b  ..d.d...}.|.j.j.
+00000cd0: 640d 6b02 72b2 7c00 6a1c 72b2 741d 6a1e  d.k.r.|.j.r.t.j.
+00000ce0: 7c00 6a04 6a19 7c05 7c08 7c00 6a05 6a1f  |.j.j.|.|.|.j.j.
+00000cf0: 7c07 7c00 6a1c 6a20 640e 8d06 7c00 5f21  |.|.j.j d...|._!
+00000d00: 6e15 7c00 6a1c 72c7 741d 6a1e 7c00 6a04  n.|.j.r.t.j.|.j.
+00000d10: 6a19 7c05 7c08 7c00 6a05 6a1f 7c07 7c00  j.|.|.|.j.j.|.|.
+00000d20: 6a1c 6a20 640e 8d06 7c00 5f21 7400 640f  j.j d...|._!t.d.
+00000d30: 8301 0100 7c00 6a21 5300 2910 7a3f 5472  ....|.j!S.).z?Tr
+00000d40: 6169 6e20 5867 626f 6f73 7420 6d6f 6465  ain Xgboost mode
+00000d50: 6c2e 2049 6e63 6c75 6465 7320 6879 7065  l. Includes hype
+00000d60: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
+00000d70: 6720 6f6e 2064 6566 6175 6c74 2e7a 1e3a  g on default.z.:
+00000d80: 2053 7461 7274 2066 6974 7469 6e67 2058   Start fitting X
+00000d90: 6762 6f6f 7374 206d 6f64 656c 2efa 4063  gboost model..@c
+00000da0: 6f6e 665f 7061 7261 6d73 5f78 6762 6f6f  onf_params_xgboo
+00000db0: 7374 2c20 636f 6e66 5f74 7261 696e 696e  st, conf_trainin
+00000dc0: 6720 6f72 2065 7870 6572 696d 656e 745f  g or experiment_
+00000dd0: 7472 6163 6b65 7220 6973 204e 6f6e 657a  tracker is Nonez
+00000de0: 1e46 696e 6973 6865 6420 6879 7065 7270  .Finished hyperp
+00000df0: 6172 616d 6574 6572 2074 756e 696e 677a  arameter tuningz
+00000e00: 2046 696e 6973 6865 6420 4772 6964 2073   Finished Grid s
+00000e10: 6561 7263 6820 6669 6e65 2074 756e 696e  earch fine tunin
+00000e20: 677a 1a53 7461 7274 2066 696e 616c 206d  gz.Start final m
+00000e30: 6f64 656c 2074 7261 696e 696e 6746 a901  odel trainingF..
+00000e40: da0e 7072 6564 6963 746f 6e5f 6d6f 6465  ..predicton_mode
+00000e50: 7a7f 3a20 556e 696f 6e20 7472 6169 6e20  z.: Union train 
+00000e60: 616e 6420 7465 7374 2064 6174 6120 666f  and test data fo
+00000e70: 7220 6669 6e61 6c20 6d6f 6465 6c20 7472  r final model tr
+00000e80: 6169 6e69 6e67 2062 6173 6564 206f 6e20  aining based on 
+00000e90: 5472 6169 6e69 6e67 436f 6e66 6967 0a20  TrainingConfig. 
+00000ea0: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00000eb0: 6d20 2775 7365 5f66 756c 6c5f 6461 7461  m 'use_full_data
+00000ec0: 5f66 6f72 5f66 696e 616c 5f6d 6f64 656c  _for_final_model
+00000ed0: 27da 0574 7261 696e da04 7465 7374 da05  '..train..test..
+00000ee0: 7374 6570 73e9 2c01 0000 e901 0000 00a9  steps.,.........
+00000ef0: 04da 0f6e 756d 5f62 6f6f 7374 5f72 6f75  ...num_boost_rou
+00000f00: 6e64 da15 6561 726c 795f 7374 6f70 7069  nd..early_stoppi
+00000f10: 6e67 5f72 6f75 6e64 73da 0565 7661 6c73  ng_rounds..evals
+00000f20: da0c 7665 7262 6f73 655f 6576 616c 7a11  ..verbose_evalz.
+00000f30: 4669 6e69 7368 6564 2074 7261 696e 696e  Finished trainin
+00000f40: 6729 2272 1300 0000 7203 0000 0072 2f00  g)"r....r....r/.
+00000f50: 0000 7230 0000 0072 1c00 0000 721a 0000  ..r0...r....r...
+00000f60: 0072 1d00 0000 da0a 5661 6c75 6545 7272  .r......ValueErr
+00000f70: 6f72 da19 7368 6f77 5f64 6574 6169 6c65  or..show_detaile
+00000f80: 645f 7475 6e69 6e67 5f6c 6f67 73da 066f  d_tuning_logs..o
+00000f90: 7074 756e 61da 076c 6f67 6769 6e67 5a0d  ptuna..loggingZ.
+00000fa0: 7365 745f 7665 7262 6f73 6974 79da 0757  set_verbosity..W
+00000fb0: 4152 4e49 4e47 da0e 6175 746f 7475 6e65  ARNING..autotune
+00000fc0: 5f6d 6f64 656c da08 6175 746f 7475 6e65  _model..autotune
+00000fd0: da05 7072 696e 74da 1e65 6e61 626c 655f  ..print..enable_
+00000fe0: 6772 6964 5f73 6561 7263 685f 6669 6e65  grid_search_fine
+00000ff0: 5f74 756e 696e 67da 0966 696e 655f 7475  _tuning..fine_tu
+00001000: 6e65 721e 0000 00da 0d66 6974 5f74 7261  ner......fit_tra
+00001010: 6e73 666f 726d da09 7472 616e 7366 6f72  nsform..transfor
+00001020: 6dda 1d75 7365 5f66 756c 6c5f 6461 7461  m..use_full_data
+00001030: 5f66 6f72 5f66 696e 616c 5f6d 6f64 656c  _for_final_model
+00001040: da02 7064 da06 636f 6e63 6174 da11 6372  ..pd..concat..cr
+00001050: 6561 7465 5f64 5f6d 6174 7269 6365 73da  eate_d_matrices.
+00001060: 0670 6172 616d 73da 0370 6f70 da14 6879  .params..pop..hy
+00001070: 7065 7274 756e 696e 675f 6376 5f66 6f6c  pertuning_cv_fol
+00001080: 6473 721b 0000 00da 0378 6762 7238 0000  dsr......xgbr8..
+00001090: 0072 3f00 0000 da25 7665 7262 6f73 6974  .r?....%verbosit
+000010a0: 795f 6475 7269 6e67 5f66 696e 616c 5f6d  y_during_final_m
+000010b0: 6f64 656c 5f74 7261 696e 696e 6772 1f00  odel_trainingr..
+000010c0: 0000 2909 7225 0000 0072 3100 0000 7232  ..).r%...r1...r2
+000010d0: 0000 0072 3300 0000 7234 0000 00da 0764  ...r3...r4.....d
+000010e0: 5f74 7261 696e da06 645f 7465 7374 da08  _train..d_test..
+000010f0: 6576 616c 5f73 6574 723a 0000 0072 2600  eval_setr:...r&.
+00001100: 0000 7226 0000 0072 2700 0000 da03 6669  ..r&...r'.....fi
+00001110: 7455 0000 0073 7000 0000 1208 0801 0403  tU...sp.........
+00001120: 02ff 0402 02fe 0403 02fd 0205 0201 04ff  ................
+00001130: 0804 1001 0802 1001 0801 0802 1001 0801  ................
+00001140: 0802 0601 0601 0401 08ff 0603 0601 0aff  ................
+00001150: 0804 0201 0c01 04ff 0e04 0e01 1402 1001  ................
+00001160: 1002 1202 0401 0601 0201 0201 0601 0201  ................
+00001170: 0601 0afa 0608 0401 0601 0201 0201 0601  ................
+00001180: 0201 0601 08fa 0808 0601 7a10 5867 626f  ..........z.Xgbo
+00001190: 6f73 744d 6f64 656c 2e66 6974 6305 0000  ostModel.fitc...
+000011a0: 0000 0000 0000 0000 000d 0000 000f 0000  ................
+000011b0: 0003 0000 0073 1202 0000 7400 7401 a002  .....s....t.t...
+000011c0: a100 9b00 6401 9d02 8301 0100 8800 6a03  ....d.........j.
+000011d0: 7212 8800 6a04 7212 8800 6a05 7316 7406  r...j.r...j.s.t.
+000011e0: 6402 8301 8201 7407 8300 8901 8800 a008  d.....t.........
+000011f0: a100 0100 8800 6a03 7229 8800 6a04 7229  ......j.r)..j.r)
+00001200: 8800 6a09 7229 8800 6a05 732d 7406 6403  ..j.r)..j.s-t.d.
+00001210: 8301 8201 8800 6a04 6a0a 7265 740b 740c  ......j.j.ret.t.
+00001220: 8803 6a0d 8301 8800 6a04 6a0e 6404 8d02  ..j.....j.j.d...
+00001230: 7d05 740b 740c 8802 6a0d 8301 8800 6a04  }.t.t...j.....j.
+00001240: 6a0e 6404 8d02 7d06 8803 6a0f 7c05 8800  j.d...}...j.|...
+00001250: 6a04 6a10 6405 8d02 8903 8805 6a11 8803  j.j.d.......j...
+00001260: 6a0d 1900 8905 8802 6a0f 7c06 8800 6a04  j.......j.|...j.
+00001270: 6a10 6405 8d02 8902 8804 6a11 8802 6a0d  j.d.......j...j.
+00001280: 1900 8904 8700 8701 8702 8703 8704 8705  ................
+00001290: 6606 6406 6407 8408 7d07 6408 7d08 7412  f.d.d...}.d.}.t.
+000012a0: 6a13 6a14 6409 8800 6a04 6a10 8800 6a04  j.j.d...j.j...j.
+000012b0: 6a15 640a 8d03 7d09 7412 6a16 640b 7c09  j.d...}.t.j.d.|.
+000012c0: 7c08 9b00 640c 9d02 640d 8d03 7d0a 7c0a  |...d...d...}.|.
+000012d0: 6a17 7c07 8800 6a04 6a18 8800 6a04 6a19  j.|...j.j...j.j.
+000012e0: 6409 6409 640e 8d05 0100 7a16 7412 6a1a  d.d.d.....z.t.j.
+000012f0: a01b 7c0a a101 7d0b 7c0b a01c a100 0100  ..|...}.|.......
+00001300: 7412 6a1a a01d 7c0a a101 7d0b 7c0b a01c  t.j...|...}.|...
+00001310: a100 0100 5700 6e0c 0400 741e 741f 7406  ....W.n...t.t.t.
+00001320: 6603 79ba 0100 0100 0100 5900 6e01 7700  f.y.......Y.n.w.
+00001330: 7c0a 6a20 6a21 7d0c 8800 6a09 6a22 8800  |.j j!}...j.j"..
+00001340: 6a09 6a23 8800 6a09 6a24 8805 a025 a100  j.j#..j.j$...%..
+00001350: 7c0c 640f 1900 7c0c 6410 1900 7c0c 6411  |.d...|.d...|.d.
+00001360: 1900 7c0c 6412 1900 7c0c 6413 1900 7c0c  ..|.d...|.d...|.
+00001370: 6414 1900 7c0c 6415 1900 7c0c 6416 1900  d...|.d...|.d...
+00001380: 7c0c 6417 1900 7c0c 6418 1900 6419 9c0e  |.d...|.d...d...
+00001390: 8800 6a03 5f21 6900 8800 6a03 6a21 a501  ..j._!i...j.j!..
+000013a0: 8801 a501 8800 6a03 5f21 7400 641a 8800  ......j._!t.d...
+000013b0: 6a03 6a21 9b00 9d02 8301 0100 7c0c 641b  j.j!........|.d.
+000013c0: 1900 8800 6a03 5f26 641c 5300 291d 7a7b  ....j._&d.S.).z{
+000013d0: 5475 6e65 2068 7970 6572 7061 7261 6d65  Tune hyperparame
+000013e0: 7465 7273 2e0a 0a20 2020 2020 2020 2041  ters...        A
+000013f0: 6e20 616c 7465 726e 6174 6976 6520 636f  n alternative co
+00001400: 6e66 6967 2063 616e 2062 6520 7072 6f76  nfig can be prov
+00001410: 6964 6564 2074 6f20 6f76 6572 7772 6974  ided to overwrit
+00001420: 6520 7468 6520 6879 7065 7270 6172 616d  e the hyperparam
+00001430: 6574 6572 2073 6561 7263 6820 7370 6163  eter search spac
+00001440: 652e 0a20 2020 2020 2020 207a 2f3a 2053  e..        z/: S
+00001450: 7461 7274 2068 7970 6572 7061 7261 6d65  tart hyperparame
+00001460: 7465 7220 7475 6e69 6e67 206f 6620 5867  ter tuning of Xg
+00001470: 626f 6f73 7420 6d6f 6465 6c2e 7235 0000  boost model.r5..
+00001480: 00fa 4f41 7420 6c65 6173 7420 6f6e 6520  ..OAt least one 
+00001490: 6f66 2074 6865 2063 6f6e 6669 6773 206f  of the configs o
+000014a0: 7220 6578 7065 7269 6d65 6e74 5f74 7261  r experiment_tra
+000014b0: 636b 6572 2069 7320 4e6f 6e65 2c20 7768  cker is None, wh
+000014c0: 6963 6820 6973 206e 6f74 2061 6c6c 6f77  ich is not allow
+000014d0: 6564 2901 da05 616c 7068 6129 01da 0c72  ed)...alpha)...r
+000014e0: 616e 646f 6d5f 7374 6174 6563 0100 0000  andom_statec....
+000014f0: 0000 0000 0000 0000 0b00 0000 1300 0000  ................
+00001500: 1300 0000 734a 0200 0088 006a 006a 0188  ....sJ.....j.j..
+00001510: 006a 006a 0288 006a 006a 0388 05a0 04a1  .j.j...j.j......
+00001520: 007c 006a 0564 0188 006a 006a 0688 006a  .|.j.d...j.j...j
+00001530: 006a 0764 0264 038d 047c 006a 0864 0488  .j.d.d...|.j.d..
+00001540: 006a 006a 0988 006a 006a 0a64 0264 038d  .j.j...j.j.d.d..
+00001550: 047c 006a 0564 0588 006a 006a 0b88 006a  .|.j.d...j.j...j
+00001560: 006a 0c64 0264 038d 047c 006a 0564 0688  .j.d.d...|.j.d..
+00001570: 006a 006a 0d88 006a 006a 0e64 0264 038d  .j.j...j.j.d.d..
+00001580: 047c 006a 0564 0788 006a 006a 0f88 006a  .|.j.d...j.j...j
+00001590: 006a 1064 0264 038d 047c 00a0 0864 0888  .j.d.d...|...d..
+000015a0: 006a 006a 1188 006a 006a 12a1 037c 00a0  .j.j...j.j...|..
+000015b0: 0564 0988 006a 006a 1388 006a 006a 14a1  .d...j.j...j.j..
+000015c0: 037c 00a0 0564 0a88 006a 006a 1588 006a  .|...d...j.j...j
+000015d0: 006a 16a1 037c 00a0 0564 0b88 006a 006a  .j...|...d...j.j
+000015e0: 1788 006a 006a 18a1 037c 006a 0864 0c88  ...j.j...|.j.d..
+000015f0: 006a 006a 1988 006a 006a 1a64 0264 038d  .j.j...j.j.d.d..
+00001600: 0464 0d9c 0e7d 0169 007c 01a5 0188 01a5  .d...}.i.|......
+00001610: 017d 017c 00a0 1b64 0e64 0264 0f67 02a1  .}.|...d.d.d.g..
+00001620: 027d 027c 0272 a088 00a0 1c88 05a1 017d  .}.|.r.........}
+00001630: 0374 1d6a 1e88 0388 057c 0388 006a 1f6a  .t.j.....|...j.j
+00001640: 2064 108d 047d 046e 0a74 1d6a 1e88 0388   d...}.n.t.j....
+00001650: 0588 006a 1f6a 2064 118d 037d 0474 1d6a  ...j.j d...}.t.j
+00001660: 1e88 0288 0488 006a 1f6a 2064 118d 037d  .......j.j d...}
+00001670: 0574 216a 22a0 237c 0064 12a1 027d 067c  .t!j".#|.d...}.|
+00001680: 01a0 2464 0c64 13a1 027d 0788 006a 1f6a  ..$d.d...}...j.j
+00001690: 2564 146b 0272 d188 00a0 267c 047c 0588  %d.k.r....&|.|..
+000016a0: 047c 017c 077c 06a1 0653 0088 006a 1f6a  .|.|.|...S...j.j
+000016b0: 2564 146b 0472 e488 006a 1f6a 2772 e488  %d.k.r...j.j'r..
+000016c0: 00a0 287c 0188 0388 0588 0288 04a1 0553  ..(|...........S
+000016d0: 0074 1d6a 297c 017c 047c 0788 006a 1f6a  .t.j)|.|.|...j.j
+000016e0: 2a88 006a 1f6a 2564 0288 006a 1f6a 2b7c  *..j.j%d...j.j+|
+000016f0: 0667 0188 006a 1f6a 2c64 158d 097d 087c  .g...j.j,d...}.|
+00001700: 0864 1619 00a0 2da1 007d 0974 2e88 006a  .d....-..}.t...j
+00001710: 2f6a 3083 0164 176b 0290 0172 0d64 177d  /j0..d.k...r.d.}
+00001720: 0a6e 0888 006a 2f6a 3064 1819 0064 1417  .n...j/j0d...d..
+00001730: 007d 0a88 006a 2f6a 317c 0a64 1988 006a  .}...j/j1|.d...j
+00001740: 1f7c 017c 0964 1a64 0f64 1b8d 0701 007c  .|.|.d.d.d.....|
+00001750: 0953 0029 1c4e da03 6574 6154 a901 da03  .S.).N..etaT....
+00001760: 6c6f 67da 096d 6178 5f64 6570 7468 725c  log..max_depthr\
+00001770: 0000 00da 066c 616d 6264 61da 0567 616d  .....lambda..gam
+00001780: 6d61 da10 6d69 6e5f 6368 696c 645f 7765  ma..min_child_we
+00001790: 6967 6874 da09 7375 6273 616d 706c 65da  ight..subsample.
+000017a0: 1063 6f6c 7361 6d70 6c65 5f62 7974 7265  .colsample_bytre
+000017b0: 65da 1163 6f6c 7361 6d70 6c65 5f62 796c  e..colsample_byl
+000017c0: 6576 656c 723a 0000 0029 0eda 096f 626a  evelr:...)...obj
+000017d0: 6563 7469 7665 da07 626f 6f73 7465 72da  ective..booster.
+000017e0: 0b65 7661 6c5f 6d65 7472 6963 da09 6e75  .eval_metric..nu
+000017f0: 6d5f 636c 6173 7372 5e00 0000 7261 0000  m_classr^...ra..
+00001800: 0072 5c00 0000 7262 0000 0072 6300 0000  .r\...rb...rc...
+00001810: 7264 0000 0072 6500 0000 7266 0000 0072  rd...re...rf...r
+00001820: 6700 0000 723a 0000 00da 0d73 616d 706c  g...r:.....sampl
+00001830: 655f 7765 6967 6874 46a9 03da 056c 6162  e_weightF....lab
+00001840: 656c da06 7765 6967 6874 da12 656e 6162  el..weight..enab
+00001850: 6c65 5f63 6174 6567 6f72 6963 616c a902  le_categorical..
+00001860: 726e 0000 0072 7000 0000 fa0d 7465 7374  rn...rp.....test
+00001870: 2d6d 6c6f 676c 6f73 7372 3b00 0000 723c  -mloglossr;...r<
+00001880: 0000 00a9 0972 5200 0000 da06 6474 7261  .....rR.....dtra
+00001890: 696e 723e 0000 0072 3f00 0000 da05 6e66  inr>...r?.....nf
+000018a0: 6f6c 64da 0961 735f 7061 6e64 6173 da04  old..as_pandas..
+000018b0: 7365 6564 da09 6361 6c6c 6261 636b 73da  seed..callbacks.
+000018c0: 0773 6875 6666 6c65 fa12 7465 7374 2d6d  .shuffle..test-m
+000018d0: 6c6f 676c 6f73 732d 6d65 616e 7201 0000  logloss-meanr...
+000018e0: 00e9 ffff ffff da08 6376 5f73 636f 7265  ........cv_score
+000018f0: fa13 6164 6a75 7374 6564 206d 6c20 6c6f  ..adjusted ml lo
+00001900: 676c 6f73 73a9 07da 0d65 7870 6572 696d  gloss....experim
+00001910: 656e 745f 6964 da0e 7363 6f72 655f 6361  ent_id..score_ca
+00001920: 7465 676f 7279 da0f 7472 6169 6e69 6e67  tegory..training
+00001930: 5f63 6f6e 6669 67da 106d 6f64 656c 5f70  _config..model_p
+00001940: 6172 616d 6574 6572 73da 0b65 7661 6c5f  arameters..eval_
+00001950: 7363 6f72 6573 da0b 6d65 7472 6963 5f75  scores..metric_u
+00001960: 7365 64da 176d 6574 7269 635f 6869 6768  sed..metric_high
+00001970: 6572 5f69 735f 6265 7474 6572 2932 721b  er_is_better)2r.
+00001980: 0000 00da 1178 6762 6f6f 7374 5f6f 626a  .....xgboost_obj
+00001990: 6563 7469 7665 7269 0000 00da 1378 6762  ectiveri.....xgb
+000019a0: 6f6f 7374 5f65 7661 6c5f 6d65 7472 6963  oost_eval_metric
+000019b0: da07 6e75 6e69 7175 65da 0d73 7567 6765  ..nunique..sugge
+000019c0: 7374 5f66 6c6f 6174 da07 6574 615f 6d69  st_float..eta_mi
+000019d0: 6eda 0765 7461 5f6d 6178 5a0b 7375 6767  n..eta_maxZ.sugg
+000019e0: 6573 745f 696e 74da 0d6d 6178 5f64 6570  est_int..max_dep
+000019f0: 7468 5f6d 696e da0d 6d61 785f 6465 7074  th_min..max_dept
+00001a00: 685f 6d61 78da 0961 6c70 6861 5f6d 696e  h_max..alpha_min
+00001a10: da09 616c 7068 615f 6d61 78da 0a6c 616d  ..alpha_max..lam
+00001a20: 6264 615f 6d69 6eda 0a6c 616d 6264 615f  bda_min..lambda_
+00001a30: 6d61 78da 0967 616d 6d61 5f6d 696e da09  max..gamma_min..
+00001a40: 6761 6d6d 615f 6d61 78da 146d 696e 5f63  gamma_max..min_c
+00001a50: 6869 6c64 5f77 6569 6768 745f 6d69 6eda  hild_weight_min.
+00001a60: 146d 696e 5f63 6869 6c64 5f77 6569 6768  .min_child_weigh
+00001a70: 745f 6d61 78da 0e73 7562 5f73 616d 706c  t_max..sub_sampl
+00001a80: 655f 6d69 6eda 0e73 7562 5f73 616d 706c  e_min..sub_sampl
+00001a90: 655f 6d61 78da 1663 6f6c 5f73 616d 706c  e_max..col_sampl
+00001aa0: 655f 6279 5f74 7265 655f 6d69 6eda 1663  e_by_tree_min..c
+00001ab0: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
+00001ac0: 655f 6d61 78da 1763 6f6c 5f73 616d 706c  e_max..col_sampl
+00001ad0: 655f 6279 5f6c 6576 656c 5f6d 696e da17  e_by_level_min..
+00001ae0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
+00001af0: 7665 6c5f 6d61 78da 0973 7465 7073 5f6d  vel_max..steps_m
+00001b00: 696e da09 7374 6570 735f 6d61 785a 1373  in..steps_maxZ.s
+00001b10: 7567 6765 7374 5f63 6174 6567 6f72 6963  uggest_categoric
+00001b20: 616c 722e 0000 0072 5500 0000 da07 444d  alr....rU.....DM
+00001b30: 6174 7269 7872 1a00 0000 da1d 6361 745f  atrixr......cat_
+00001b40: 656e 636f 6469 6e67 5f76 6961 5f6d 6c5f  encoding_via_ml_
+00001b50: 616c 676f 7269 7468 6d72 4400 0000 da0b  algorithmrD.....
+00001b60: 696e 7465 6772 6174 696f 6eda 1658 4742  integration..XGB
+00001b70: 6f6f 7374 5072 756e 696e 6743 616c 6c62  oostPruningCallb
+00001b80: 6163 6b72 5300 0000 7254 0000 00da 1774  ackrS...rT.....t
+00001b90: 7261 696e 5f73 696e 676c 655f 666f 6c64  rain_single_fold
+00001ba0: 5f6d 6f64 656c da11 7072 6563 6973 655f  _model..precise_
+00001bb0: 6376 5f74 756e 696e 67da 125f 6669 6e65  cv_tuning.._fine
+00001bc0: 5f74 756e 655f 7072 6563 6973 65da 0263  _tune_precise..c
+00001bd0: 7672 3f00 0000 7223 0000 00da 1773 6875  vr?...r#.....shu
+00001be0: 6666 6c65 5f64 7572 696e 675f 7472 6169  ffle_during_trai
+00001bf0: 6e69 6e67 da04 6d65 616e da03 6c65 6e72  ning..mean..lenr
+00001c00: 1d00 0000 727f 0000 00da 0b61 6464 5f72  ....r......add_r
+00001c10: 6573 756c 7473 290b da05 7472 6961 6cda  esults)...trial.
+00001c20: 0570 6172 616d 726c 0000 0072 2d00 0000  .paramrl...r-...
+00001c30: 7257 0000 0072 5800 0000 da10 7072 756e  rW...rX.....prun
+00001c40: 696e 675f 6361 6c6c 6261 636b 723a 0000  ing_callbackr:..
+00001c50: 00da 0672 6573 756c 74da 0e61 646a 7573  ...result..adjus
+00001c60: 7465 645f 7363 6f72 65da 066e 6577 5f69  ted_score..new_i
+00001c70: 64a9 0672 2500 0000 5a08 7472 6169 6e5f  d..r%...Z.train_
+00001c80: 6f6e 7232 0000 0072 3100 0000 7234 0000  onr2...r1...r4..
+00001c90: 0072 3300 0000 7226 0000 0072 2700 0000  .r3...r&...r'...
+00001ca0: 7268 0000 00d5 0000 0073 ec00 0000 0602  rh.......s......
+00001cb0: 0601 0601 0601 0401 0201 0601 0601 0201  ................
+00001cc0: 04fc 0406 0201 0601 0601 0201 04fc 0406  ................
+00001cd0: 0201 0601 0601 0201 04fc 0406 0201 0601  ................
+00001ce0: 0601 0201 04fc 0406 0201 0601 0601 0201  ................
+00001cf0: 04fc 0406 0201 0601 0601 02fd 0405 0201  ................
+00001d00: 0601 0601 02fd 0405 0201 0601 0601 02fd  ................
+00001d10: 0405 0201 0601 0601 02fd 0405 0201 0601  ................
+00001d20: 0601 0201 04fc 06c9 0c3e 1001 0402 0a01  .........>......
+00001d30: 0401 0201 0201 0201 0601 08fc 0407 0201  ................
+00001d40: 0201 0601 06fd 0406 0201 0201 0601 06fd  ................
+00001d50: 0606 0401 04ff 0c04 0c02 0401 0c01 04ff  ................
+00001d60: 0c04 0601 02ff 1204 0402 0201 0201 0201  ................
+00001d70: 0601 0601 0201 0601 0401 0601 06f7 0c0c  ................
+00001d80: 1203 0601 1002 0601 0201 0201 0401 0201  ................
+00001d90: 0201 0201 0201 06f9 040a 7a28 5867 626f  ..........z(Xgbo
+00001da0: 6f73 744d 6f64 656c 2e61 7574 6f74 756e  ostModel.autotun
+00001db0: 652e 3c6c 6f63 616c 733e 2e6f 626a 6563  e.<locals>.objec
+00001dc0: 7469 7665 da07 7867 626f 6f73 7454 2903  tive..xgboostT).
+00001dd0: 5a0c 6d75 6c74 6976 6172 6961 7465 7277  Z.multivariaterw
+00001de0: 0000 005a 106e 5f73 7461 7274 7570 5f74  ...Z.n_startup_t
+00001df0: 7269 616c 73da 086d 696e 696d 697a 657a  rials..minimizez
+00001e00: 0720 7475 6e69 6e67 2903 da09 6469 7265  . tuning)...dire
+00001e10: 6374 696f 6eda 0773 616d 706c 6572 5a0a  ction..samplerZ.
+00001e20: 7374 7564 795f 6e61 6d65 a904 da08 6e5f  study_name....n_
+00001e30: 7472 6961 6c73 da07 7469 6d65 6f75 745a  trials..timeoutZ
+00001e40: 0e67 635f 6166 7465 725f 7472 6961 6c5a  .gc_after_trialZ
+00001e50: 1173 686f 775f 7072 6f67 7265 7373 5f62  .show_progress_b
+00001e60: 6172 7261 0000 0072 5c00 0000 7262 0000  arra...r\...rb..
+00001e70: 0072 6300 0000 7264 0000 0072 6500 0000  .rc...rd...re...
+00001e80: 7266 0000 0072 6700 0000 725e 0000 0072  rf...rg...r^...r
+00001e90: 3a00 0000 290e 7268 0000 0072 6900 0000  :...).rh...ri...
+00001ea0: 726a 0000 0072 6b00 0000 7261 0000 0072  rj...rk...ra...r
+00001eb0: 5c00 0000 7262 0000 0072 6300 0000 7264  \...rb...rc...rd
+00001ec0: 0000 0072 6500 0000 7266 0000 0072 6700  ...re...rf...rg.
+00001ed0: 0000 725e 0000 0072 3a00 0000 fa0d 4265  ..r^...r:.....Be
+00001ee0: 7374 2070 6172 616d 733a 2072 6c00 0000  st params: rl...
+00001ef0: 4e29 2772 1300 0000 7203 0000 0072 2f00  N)'r....r....r/.
+00001f00: 0000 721c 0000 0072 1a00 0000 721d 0000  ..r....r....r...
+00001f10: 0072 4200 0000 7211 0000 0072 3000 0000  .rB...r....r0...
+00001f20: 721b 0000 00da 1973 616d 706c 655f 6461  r......sample_da
+00001f30: 7461 5f64 7572 696e 675f 7475 6e69 6e67  ta_during_tuning
+00001f40: 7212 0000 0072 a800 0000 da05 696e 6465  r....r......inde
+00001f50: 78da 1f73 616d 706c 655f 6461 7461 5f64  x..sample_data_d
+00001f60: 7572 696e 675f 7475 6e69 6e67 5f61 6c70  uring_tuning_alp
+00001f70: 6861 da06 7361 6d70 6c65 7223 0000 00da  ha..sampler#....
+00001f80: 036c 6f63 7244 0000 00da 0873 616d 706c  .locrD.....sampl
+00001f90: 6572 735a 0a54 5045 5361 6d70 6c65 72da  ersZ.TPESampler.
+00001fa0: 1f6f 7074 756e 615f 7361 6d70 6c65 725f  .optuna_sampler_
+00001fb0: 6e5f 7374 6172 7475 705f 7472 6961 6c73  n_startup_trials
+00001fc0: da0c 6372 6561 7465 5f73 7475 6479 da08  ..create_study..
+00001fd0: 6f70 7469 6d69 7a65 da1c 6879 7065 7270  optimize..hyperp
+00001fe0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
+00001ff0: 726f 756e 6473 da26 6879 7065 7270 6172  rounds.&hyperpar
+00002000: 616d 6574 6572 5f74 756e 696e 675f 6d61  ameter_tuning_ma
+00002010: 785f 7275 6e74 696d 655f 7365 6373 da0d  x_runtime_secs..
+00002020: 7669 7375 616c 697a 6174 696f 6eda 1970  visualization..p
+00002030: 6c6f 745f 6f70 7469 6d69 7a61 7469 6f6e  lot_optimization
+00002040: 5f68 6973 746f 7279 da04 7368 6f77 da16  _history..show..
+00002050: 706c 6f74 5f70 6172 616d 5f69 6d70 6f72  plot_param_impor
+00002060: 7461 6e63 6573 da11 5a65 726f 4469 7669  tances..ZeroDivi
+00002070: 7369 6f6e 4572 726f 72da 0c52 756e 7469  sionError..Runti
+00002080: 6d65 4572 726f 72da 0a62 6573 745f 7472  meError..best_tr
+00002090: 6961 6c72 5200 0000 7286 0000 0072 6900  ialrR...r....ri.
+000020a0: 0000 7287 0000 0072 8800 0000 726c 0000  ..r....r....rl..
+000020b0: 0029 0d72 2500 0000 7231 0000 0072 3200  .).r%...r1...r2.
+000020c0: 0000 7233 0000 0072 3400 0000 5a10 6e62  ..r3...r4...Z.nb
+000020d0: 5f73 616d 706c 6573 5f74 7261 696e 5a0f  _samples_trainZ.
+000020e0: 6e62 5f73 616d 706c 6573 5f74 6573 7472  nb_samples_testr
+000020f0: 6800 0000 da09 616c 676f 7269 7468 6d72  h.....algorithmr
+00002100: b400 0000 da05 7374 7564 79da 0366 6967  ......study..fig
+00002110: 5a12 7867 626f 6f73 745f 6265 7374 5f70  Z.xgboost_best_p
+00002120: 6172 616d 7226 0000 0072 b000 0000 7227  aramr&...r....r'
+00002130: 0000 0072 4800 0000 9f00 0000 73be 0000  ...rH.......s...
+00002140: 0012 0b04 0202 ff04 0202 fe04 0302 fd02  ................
+00002150: 0502 0104 ff06 0408 0204 0302 ff04 0202  ................
+00002160: fe04 0302 fd04 0402 fc02 0602 0104 ff08  ................
+00002170: 0402 0108 0106 0106 fe02 0408 0106 0106  ................
+00002180: fe04 0508 0106 ff0c 0304 0108 0106 ff0c  ................
+00002190: 0316 0200 7f04 0806 0102 0106 0106 0106  ................
+000021a0: fd04 0502 0102 0108 0106 fd04 0602 0106  ................
+000021b0: 0106 0102 0102 0106 fb02 070c 0108 0106  ................
+000021c0: 0102 0104 ff0c 0312 0104 0102 ff08 0306  ................
+000021d0: 0306 0106 0106 0102 0102 0102 ff06 0306  ................
+000021e0: 0106 0106 0106 0106 0106 0106 0106 010a  ................
+000021f0: f002 1206 0102 ff02 0208 fe12 0410 017a  ...............z
+00002200: 1558 6762 6f6f 7374 4d6f 6465 6c2e 6175  .XgboostModel.au
+00002210: 746f 7475 6e65 6301 0000 0000 0000 0000  totunec.........
+00002220: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00002230: 5e00 0000 7c00 6a00 6a01 7217 7c00 6a00  ^...|.j.j.r.|.j.
+00002240: 6a02 6401 6b02 730e 7c00 6a00 6a03 7217  j.d.k.s.|.j.j.r.
+00002250: 7c00 6a04 6a05 6402 6403 8d01 7d01 7c01  |.j.j.d.d...}.|.
+00002260: 5300 7c00 6a00 6a01 722a 7c00 6a00 6a02  S.|.j.j.r*|.j.j.
+00002270: 6401 6b04 722a 7c00 6a04 6a05 6404 6403  d.k.r*|.j.j.d.d.
+00002280: 8d01 7d01 7c01 5300 7406 6a07 7d01 7c01  ..}.|.S.t.j.}.|.
+00002290: 5300 2905 4e72 3c00 0000 da0f 6d61 7474  S.).Nr<.....matt
+000022a0: 6865 775f 696e 7665 7273 6529 01da 0d74  hew_inverse)...t
+000022b0: 6172 6765 745f 6d65 7472 6963 727d 0000  arget_metricr}..
+000022c0: 0029 0872 1a00 0000 7247 0000 0072 5400  .).r....rG...rT.
+000022d0: 0000 72a3 0000 0072 1d00 0000 da0e 6765  ..r....r......ge
+000022e0: 745f 6265 7374 5f73 636f 7265 7220 0000  t_best_scorer ..
+000022f0: 00da 0369 6e66 2902 7225 0000 00da 1262  ...inf).r%.....b
+00002300: 6573 745f 7363 6f72 655f 6376 5f67 7269  est_score_cv_gri
+00002310: 6472 2600 0000 7226 0000 0072 2700 0000  dr&...r&...r'...
+00002320: 72d0 0000 0094 0100 0073 2200 0000 0801  r........s".....
+00002330: 0c01 0601 02ff 0603 0201 06ff 040c 06f8  ................
+00002340: 02ff 0c02 0602 0201 06ff 0405 06ff 0401  ................
+00002350: 7a1b 5867 626f 6f73 744d 6f64 656c 2e67  z.XgboostModel.g
+00002360: 6574 5f62 6573 745f 7363 6f72 6563 0500  et_best_scorec..
+00002370: 0000 0000 0000 0000 0000 0800 0000 0600  ................
+00002380: 0000 4300 0000 735a 0000 007c 006a 006a  ..C...sZ...|.j.j
+00002390: 0172 157c 00a0 027c 02a1 017d 0574 036a  .r.|...|...}.t.j
+000023a0: 047c 017c 027c 057c 006a 056a 0664 018d  .|.|.|.|.j.j.d..
+000023b0: 047d 066e 0a74 036a 047c 017c 027c 006a  .}.n.t.j.|.|.|.j
+000023c0: 056a 0664 028d 037d 0674 036a 047c 037c  .j.d...}.t.j.|.|
+000023d0: 047c 006a 056a 0664 028d 037d 077c 067c  .|.j.j.d...}.|.|
+000023e0: 0766 0253 0029 034e 726d 0000 0072 7100  .f.S.).Nrm...rq.
+000023f0: 0000 2907 721c 0000 0072 6c00 0000 722e  ..).r....rl...r.
+00002400: 0000 0072 5500 0000 729e 0000 0072 1a00  ...rU...r....r..
+00002410: 0000 729f 0000 0029 0872 2500 0000 7231  ..r....).r%...r1
+00002420: 0000 0072 3300 0000 7232 0000 0072 3400  ...r3...r2...r4.
+00002430: 0000 722d 0000 0072 5700 0000 7258 0000  ..r-...rW...rX..
+00002440: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00002450: 7251 0000 00a7 0100 0073 2600 0000 0801  rQ.......s&.....
+00002460: 0a01 0401 0201 0201 0201 0601 08fc 0407  ................
+00002470: 0201 0201 0601 06fd 0405 0201 0201 0601  ................
+00002480: 06fd 0805 7a1e 5867 626f 6f73 744d 6f64  ....z.XgboostMod
+00002490: 656c 2e63 7265 6174 655f 645f 6d61 7472  el.create_d_matr
+000024a0: 6963 6573 6307 0000 0000 0000 0000 0000  icesc...........
+000024b0: 000d 0000 0009 0000 0043 0000 0073 ac00  .........C...s..
+000024c0: 0000 7c01 6401 6602 7c02 6402 6602 6702  ..|.d.f.|.d.f.g.
+000024d0: 7d07 7400 6a01 7c04 7c01 7c05 7c00 6a02  }.t.j.|.|.|.|.j.
+000024e0: 6a03 7c07 7c06 6701 7c00 6a04 6a05 6403  j.|.|.g.|.j.j.d.
+000024f0: 8d07 7d08 7c08 a006 7c02 a101 7d09 7407  ..}.|...|...}.t.
+00002500: a008 6404 6405 8400 7c09 4400 8301 a101  ..d.d...|.D.....
+00002510: 7d0a 7409 7c03 a00a a100 7c0a a00a a100  }.t.|.....|.....
+00002520: 8302 6406 1400 7d0b 740b 7c00 6a0c 6a0d  ..d...}.t.|.j.j.
+00002530: 8301 6407 6b02 723e 6407 7d0c 6e08 7c00  ..d.k.r>d.}.n.|.
+00002540: 6a0c 6a0d 6406 1900 6408 1700 7d0c 7c00  j.j.d...d...}.|.
+00002550: 6a0c 6a0e 7c0c 6409 7c00 6a02 7c04 7c0b  j.j.|.d.|.j.|.|.
+00002560: 640a 640b 640c 8d07 0100 7c0b 5300 290d  d.d.d.....|.S.).
+00002570: 4e72 3800 0000 7239 0000 0029 0572 3e00  Nr8...r9...).r>.
+00002580: 0000 723f 0000 0072 4000 0000 7278 0000  ..r?...r@...rx..
+00002590: 0072 4100 0000 6301 0000 0000 0000 0000  .rA...c.........
+000025a0: 0000 0002 0000 0005 0000 0053 0000 00f3  ...........S....
+000025b0: 1600 0000 6700 7c00 5d07 7d01 7400 a001  ....g.|.].}.t...
+000025c0: 7c01 a101 9102 7102 5300 7226 0000 00a9  |.....q.S.r&....
+000025d0: 0272 2000 0000 da06 6172 676d 6178 a902  .r .....argmax..
+000025e0: da02 2e30 da04 6c69 6e65 7226 0000 0072  ...0..liner&...r
+000025f0: 2600 0000 7227 0000 00da 0a3c 6c69 7374  &...r'.....<list
+00002600: 636f 6d70 3ecb 0100 00f3 0200 0000 1600  comp>...........
+00002610: 7a38 5867 626f 6f73 744d 6f64 656c 2e74  z8XgboostModel.t
+00002620: 7261 696e 5f73 696e 676c 655f 666f 6c64  rain_single_fold
+00002630: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
+00002640: 3c6c 6973 7463 6f6d 703e 727b 0000 0072  <listcomp>r{...r
+00002650: 0100 0000 723c 0000 00da 1773 696d 706c  ....r<.....simpl
+00002660: 655f 7472 6169 6e5f 7465 7374 5f73 636f  e_train_test_sco
+00002670: 7265 72ce 0000 0046 727e 0000 0029 0f72  rer....Fr~...).r
+00002680: 5500 0000 7238 0000 0072 1a00 0000 723f  U...r8...r....r?
+00002690: 0000 0072 1b00 0000 da26 7665 7262 6f73  ...r.....&verbos
+000026a0: 6974 795f 6475 7269 6e67 5f68 7970 6572  ity_during_hyper
+000026b0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+000026c0: da07 7072 6564 6963 7472 2000 0000 da07  ..predictr .....
+000026d0: 6173 6172 7261 7972 0a00 0000 da06 746f  asarrayr......to
+000026e0: 6c69 7374 72a8 0000 0072 1d00 0000 727f  listr....r....r.
+000026f0: 0000 0072 a900 0000 290d 7225 0000 0072  ...r....).r%...r
+00002700: 5700 0000 7258 0000 0072 3400 0000 72ab  W...rX...r4...r.
+00002710: 0000 0072 3a00 0000 72ac 0000 0072 5900  ...r:...r....rY.
+00002720: 0000 721f 0000 00da 0570 7265 6473 da0b  ..r......preds..
+00002730: 7072 6564 5f6c 6162 656c 735a 076d 6174  pred_labelsZ.mat
+00002740: 7468 6577 72af 0000 0072 2600 0000 7226  thewr....r&...r&
+00002750: 0000 0072 2700 0000 72a2 0000 00bd 0100  ...r'...r.......
+00002760: 0073 3400 0000 1003 0401 0201 0201 0201  .s4.............
+00002770: 0601 0201 0401 0601 06f9 0a09 1401 1601  ................
+00002780: 1003 0601 1002 0601 0201 0201 0401 0201  ................
+00002790: 0201 0201 0201 06f9 0409 7a24 5867 626f  ..........z$Xgbo
+000027a0: 6f73 744d 6f64 656c 2e74 7261 696e 5f73  ostModel.train_s
+000027b0: 696e 676c 655f 666f 6c64 5f6d 6f64 656c  ingle_fold_model
+000027c0: e964 0000 00da 0765 7661 6c5f 6466 da06  .d.....eval_df..
+000027d0: 795f 7472 7565 da0a 6974 6572 6174 696f  y_true..iteratio
+000027e0: 6e73 6305 0000 0000 0000 0000 0000 0011  nsc.............
+000027f0: 0000 0007 0000 0043 0000 0073 ae00 0000  .......C...s....
+00002800: 6700 7d05 7400 7c04 8301 4400 5d4e 7d06  g.}.t.|...D.]N}.
+00002810: 6401 6402 7c06 1400 0202 7d07 7d08 7c02  d.d.|.....}.}.|.
+00002820: 6a01 5c02 7d09 7d0a 7c00 6a02 a003 7c07  j.\.}.}.|.j...|.
+00002830: 7c08 7c09 7c0a 6702 a103 7d0b 7c02 7c0b  |.|.|.g...}.|.|.
+00002840: 1700 7d0c 7c00 6a04 7230 7405 6a06 7c0c  ..}.|.j.r0t.j.|.
+00002850: 7c03 7c00 6a04 6a07 6403 8d03 7d0d 6e04  |.|.j.j.d...}.n.
+00002860: 7408 6404 8301 8201 7c01 a009 7c0d a101  t.d.....|...|...
+00002870: 7d0e 740a a00b 6405 6406 8400 7c0e 4400  }.t...d.d...|.D.
+00002880: 8301 a101 7d0f 740c 7c03 6a0d a00e a100  ....}.t.|.j.....
+00002890: 7c0f a00e a100 8302 6407 1400 7d10 7c05  |.......d...}.|.
+000028a0: a00f 7c10 a101 0100 7106 7c05 5300 2908  ..|.....q.|.S.).
+000028b0: 619f 0100 0046 756e 6374 696f 6e20 746f  a....Function to
+000028c0: 2061 6464 2069 6e63 7265 6173 696e 6720   add increasing 
+000028d0: 6e6f 6973 6520 616e 6420 6576 616c 7561  noise and evalua
+000028e0: 7465 2069 742e 0a0a 2020 2020 2020 2020  te it...        
+000028f0: 5468 6520 6675 6e63 7469 6f6e 2065 7870  The function exp
+00002900: 6563 7473 2061 2074 7261 696e 6564 206d  ects a trained m
+00002910: 6f64 656c 2061 6e64 2061 2064 6174 6166  odel and a dataf
+00002920: 7261 6d65 2077 6974 6820 7468 6520 7361  rame with the sa
+00002930: 6d65 2063 6f6c 756d 6e73 2061 7320 7468  me columns as th
+00002940: 6520 7472 6169 6e69 6e67 2064 6174 612e  e training data.
+00002950: 0a20 2020 2020 2020 2054 6865 2074 7261  .        The tra
+00002960: 696e 696e 6720 6461 7461 2073 686f 756c  ining data shoul
+00002970: 6420 6265 206e 6f72 6d61 6c6c 7920 6469  d be normally di
+00002980: 7374 7269 6275 7465 6420 2863 6f6e 7369  stributed (consi
+00002990: 6465 7220 7573 696e 6720 6120 706f 7765  der using a powe
+000029a0: 7220 7472 616e 7366 6f72 6d65 7220 7769  r transformer wi
+000029b0: 7468 2079 656f 2d6a 6f68 6e73 6f6e 292e  th yeo-johnson).
+000029c0: 0a0a 2020 2020 2020 2020 5468 6520 6675  ..        The fu
+000029d0: 6e63 7469 6f6e 2077 696c 6c20 6170 706c  nction will appl
+000029e0: 7920 696e 6372 6561 7369 6e67 6c79 206e  y increasingly n
+000029f0: 6f69 7365 2074 6f20 7468 6520 6576 616c  oise to the eval
+00002a00: 2064 6174 6166 7261 6d65 2061 6e64 2065   dataframe and e
+00002a10: 7661 6c75 6174 6520 7468 6520 6d6f 6465  valuate the mode
+00002a20: 6c20 6f6e 2069 742e 0a0a 2020 2020 2020  l on it...      
+00002a30: 2020 5265 7475 726e 7320 6120 6c69 7374    Returns a list
+00002a40: 206f 6620 6c6f 7373 6573 2e0a 2020 2020   of losses..    
+00002a50: 2020 2020 7201 0000 0067 9a99 9999 9999      r....g......
+00002a60: c93f 7271 0000 007a 214e 6f20 7472 6169  .?rq...z!No trai
+00002a70: 6e69 6e67 5f63 6f6e 6669 6720 636f 756c  ning_config coul
+00002a80: 6420 6265 2066 6f75 6e64 6301 0000 0000  d be foundc.....
+00002a90: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00002aa0: 0000 0072 d300 0000 7226 0000 0072 d400  ...r....r&...r..
+00002ab0: 0000 72d6 0000 0072 2600 0000 7226 0000  ..r....r&...r&..
+00002ac0: 0072 2700 0000 72d9 0000 00fa 0100 0072  .r'...r........r
+00002ad0: da00 0000 7a3b 5867 626f 6f73 744d 6f64  ....z;XgboostMod
+00002ae0: 656c 2e69 6e63 7265 6173 696e 675f 6e6f  el.increasing_no
+00002af0: 6973 655f 6576 616c 7561 746f 722e 3c6c  ise_evaluator.<l
+00002b00: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00002b10: 3e72 7b00 0000 2910 da05 7261 6e67 65da  >r{...)...range.
+00002b20: 0573 6861 7065 7224 0000 00da 066e 6f72  .shaper$.....nor
+00002b30: 6d61 6c72 1a00 0000 7255 0000 0072 9e00  malr....rU...r..
+00002b40: 0000 729f 0000 0072 4200 0000 72dd 0000  ..r....rB...r...
+00002b50: 0072 2000 0000 72de 0000 0072 0a00 0000  .r ...r....r....
+00002b60: da06 7661 6c75 6573 72df 0000 00da 0661  ..valuesr......a
+00002b70: 7070 656e 6429 1172 2500 0000 da08 6d6c  ppend).r%.....ml
+00002b80: 5f6d 6f64 656c 72e3 0000 0072 e400 0000  _modelr....r....
+00002b90: 72e5 0000 00da 066c 6f73 7365 73da 0169  r......losses..i
+00002ba0: da02 6d75 da05 7369 676d 61da 014e da01  ..mu..sigma..N..
+00002bb0: 44da 056e 6f69 7365 5a0b 6576 616c 5f64  D..noiseZ.eval_d
+00002bc0: 665f 6d6f 645a 0664 5f65 7661 6cda 0579  f_modZ.d_eval..y
+00002bd0: 5f68 6174 da09 795f 636c 6173 7365 73da  _hat..y_classes.
+00002be0: 046c 6f73 7372 2600 0000 7226 0000 0072  .lossr&...r&...r
+00002bf0: 2700 0000 da1a 696e 6372 6561 7369 6e67  '.....increasing
+00002c00: 5f6e 6f69 7365 5f65 7661 6c75 6174 6f72  _noise_evaluator
+00002c10: de01 0000 7324 0000 0004 0d0c 010e 010a  ....s$..........
+00002c20: 0114 0108 0106 0104 0102 0102 0106 0108  ................
+00002c30: fd08 060a 0114 0118 020c 0104 027a 2758  .............z'X
+00002c40: 6762 6f6f 7374 4d6f 6465 6c2e 696e 6372  gboostModel.incr
+00002c50: 6561 7369 6e67 5f6e 6f69 7365 5f65 7661  easing_noise_eva
+00002c60: 6c75 6174 6f72 72ec 0000 0063 0200 0000  luatorr....c....
+00002c70: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+00002c80: 4300 0000 738c 0000 0064 017d 0274 0074  C...s....d.}.t.t
+00002c90: 017c 0183 0183 0144 005d 1c7d 037c 0364  .|.....D.].}.|.d
+00002ca0: 0217 0074 017c 0183 0164 0218 006b 0472  ...t.|...d...k.r
+00002cb0: 1601 006e 0f7c 017c 0319 007c 017c 0364  ...n.|.|...|.|.d
+00002cc0: 0217 0019 006b 0472 247c 0264 0237 007d  .....k.r$|.d.7.}
+00002cd0: 0271 087c 0264 016b 0272 2d64 037d 047c  .q.|.d.k.r-d.}.|
+00002ce0: 0453 0074 017c 0183 017d 057c 0164 0119  .S.t.|...}.|.d..
+00002cf0: 0074 02a0 037c 0164 047c 0285 0219 00a1  .t...|.d.|......
+00002d00: 017c 057c 057c 0218 001b 0013 0018 007d  .|.|.|.........}
+00002d10: 047c 0453 0029 0561 4201 0000 4361 6c63  .|.S.).aB...Calc
+00002d20: 756c 6174 6520 6120 7765 6967 6874 6564  ulate a weighted
+00002d30: 206c 6f73 7320 6261 7365 6420 6f6e 2074   loss based on t
+00002d40: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
+00002d50: 6573 2074 6865 206c 6f73 7320 6465 6372  es the loss decr
+00002d60: 6561 7365 642e 0a0a 2020 2020 2020 2020  eased...        
+00002d70: 4578 7065 6374 7320 6120 6c69 7374 206f  Expects a list o
+00002d80: 6620 6c6f 7373 6573 2063 6f6d 696e 6720  f losses coming 
+00002d90: 6672 6f6d 2069 6e63 7265 6173 696e 675f  from increasing_
+00002da0: 6e6f 6973 655f 6576 616c 7561 746f 722e  noise_evaluator.
+00002db0: 2043 6865 636b 7320 686f 7720 6d61 6e79   Checks how many
+00002dc0: 2074 696d 6573 2074 6865 206c 6f73 7320   times the loss 
+00002dd0: 6465 6372 6561 7365 6420 616e 640a 2020  decreased and.  
+00002de0: 2020 2020 2020 6361 6c63 756c 6174 6573        calculates
+00002df0: 2061 2077 6569 6768 7465 6420 6c6f 7373   a weighted loss
+00002e00: 2062 6173 6564 206f 6e20 7468 6520 6e75   based on the nu
+00002e10: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
+00002e20: 6520 6c6f 7373 2064 6563 7265 6173 6564  e loss decreased
+00002e30: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00002e40: 6e73 2074 6865 2077 6569 6768 7465 6420  ns the weighted 
+00002e50: 6c6f 7373 2e0a 2020 2020 2020 2020 7201  loss..        r.
+00002e60: 0000 0072 3c00 0000 69e7 0300 004e 2904  ...r<...i....N).
+00002e70: 72e6 0000 0072 a800 0000 7220 0000 00da  r....r....r ....
+00002e80: 0373 7464 2906 7225 0000 0072 ec00 0000  .std).r%...r....
+00002e90: 5a11 6e62 5f6c 6f73 735f 6465 6372 6561  Z.nb_loss_decrea
+00002ea0: 7365 64da 0369 6478 da0d 7765 6967 6874  sed..idx..weight
+00002eb0: 6564 5f6c 6f73 735a 096e 625f 6c6f 7373  ed_lossZ.nb_loss
+00002ec0: 6573 7226 0000 0072 2600 0000 7227 0000  esr&...r&...r'..
+00002ed0: 00da 2063 6f6e 7374 616e 745f 6c6f 7373  .. constant_loss
+00002ee0: 5f64 6567 7265 6761 7469 6f6e 5f66 6163  _degregation_fac
+00002ef0: 746f 7201 0200 0073 1e00 0000 0408 1001  tor....s........
+00002f00: 1401 0401 1401 0801 0280 0803 0401 040a  ................
+00002f10: 08f8 1601 0a01 06ff 0407 7a2d 5867 626f  ..........z-Xgbo
+00002f20: 6f73 744d 6f64 656c 2e63 6f6e 7374 616e  ostModel.constan
+00002f30: 745f 6c6f 7373 5f64 6567 7265 6761 7469  t_loss_degregati
+00002f40: 6f6e 5f66 6163 746f 72da 0c74 756e 6564  on_factor..tuned
+00002f50: 5f70 6172 616d 7363 0600 0000 0000 0000  _paramsc........
+00002f60: 0000 0000 1b00 0000 0900 0000 4300 0000  ............C...
+00002f70: 730e 0200 007c 01a0 0064 0164 02a1 027d  s....|...d.d...}
+00002f80: 067c 006a 0173 1174 0283 007c 005f 0174  .|.j.s.t...|._.t
+00002f90: 0364 0383 0101 0074 047c 006a 016a 0564  .d.....t.|.j.j.d
+00002fa0: 047c 006a 016a 0664 058d 037d 0767 007d  .|.j.j.d...}.g.}
+00002fb0: 0874 077c 07a0 087c 027c 03a0 0974 0aa1  .t.|...|.|...t..
+00002fc0: 01a1 0283 0144 005d aa5c 027d 095c 027d  .....D.].\.}.\.}
+00002fd0: 0a7d 0b7c 026a 0b7c 0a19 007c 026a 0b7c  .}.|.j.|...|.j.|
+00002fe0: 0b19 0002 027d 0c7d 0d7c 036a 0b7c 0a19  .....}.}.|.j.|..
+00002ff0: 007c 036a 0b7c 0b19 0002 027d 0e7d 0f7c  .|.j.|.....}.}.|
+00003000: 006a 0c72 667c 006a 0ca0 0d7c 0c7c 0ea1  .j.rf|.j...|.|..
+00003010: 025c 027d 0c7d 0e7c 006a 0ca0 0e7c 047c  .\.}.}.|.j...|.|
+00003020: 05a1 025c 027d 107d 117c 006a 0c6a 0e7c  ...\.}.}.|.j.j.|
+00003030: 0d7c 0f64 0664 078d 035c 027d 0d7d 0f6e  .|.d.d...\.}.}.n
+00003040: 057c 047c 0502 027d 107d 1174 0f6a 107c  .|.|...}.}.t.j.|
+00003050: 0d7c 0f7c 006a 016a 1164 088d 037d 127c  .|.|.j.j.d...}.|
+00003060: 006a 1273 8074 1383 007c 005f 1274 0364  .j.s.t...|._.t.d
+00003070: 0983 0101 007c 006a 126a 1472 957c 00a0  .....|.j.j.r.|..
+00003080: 157c 0ea1 017d 1374 0f6a 107c 0c7c 0e7c  .|...}.t.j.|.|.|
+00003090: 137c 006a 016a 1164 0a8d 047d 146e 0a74  .|.j.j.d...}.n.t
+000030a0: 0f6a 107c 0c7c 0e7c 006a 016a 1164 088d  .j.|.|.|.j.j.d..
+000030b0: 037d 147c 1464 0b66 027c 1264 0c66 0267  .}.|.d.f.|.d.f.g
+000030c0: 027d 157c 006a 1673 b274 1783 007c 005f  .}.|.j.s.t...|._
+000030d0: 1674 0364 0d83 0101 0074 0f6a 187c 017c  .t.d.....t.j.|.|
+000030e0: 147c 067c 006a 016a 197c 157c 006a 166a  .|.|.j.j.|.|.j.j
+000030f0: 1a64 0e8d 067d 167c 00a0 1b7c 167c 107c  .d...}.|...|.|.|
+00003100: 1164 0fa1 047d 177c 00a0 1c7c 17a1 017d  .d...}.|...|...}
+00003110: 187c 08a0 1d7c 18a1 0101 0071 2974 1ea0  .|...|.....q)t..
+00003120: 1f74 1ea0 207c 08a1 01a1 017d 197c 006a  .t.. |.....}.|.j
+00003130: 2190 0172 057c 006a 0190 0172 0574 227c  !..r.|.j...r.t"|
+00003140: 006a 216a 2383 0164 106b 0272 ef64 107d  .j!j#..d.k.r.d.}
+00003150: 1a6e 087c 006a 216a 2364 1119 0064 1217  .n.|.j!j#d...d..
+00003160: 007d 1a7c 006a 216a 247c 1a64 137c 006a  .}.|.j!j$|.d.|.j
+00003170: 017c 017c 1964 1464 0664 158d 0701 007c  .|.|.d.d.d.....|
+00003180: 1953 0029 164e 723a 0000 0072 3b00 0000  .S.).Nr:...r;...
+00003190: 7a3e 436f 756c 6420 6e6f 7420 6669 6e64  z>Could not find
+000031a0: 2054 7261 696e 696e 6720 636f 6e66 6967   Training config
+000031b0: 2e20 4661 6c6c 696e 6720 6261 636b 2074  . Falling back t
+000031c0: 6f20 6465 6661 756c 7420 7661 6c75 6573  o default values
+000031d0: 5429 03da 086e 5f73 706c 6974 7372 7900  T)...n_splitsry.
+000031e0: 0000 725d 0000 0046 7236 0000 0072 7100  ..r]...Fr6...rq.
+000031f0: 0000 7a49 436f 756c 6420 6e6f 7420 6669  ..zICould not fi
+00003200: 6e64 2058 6762 6f6f 7374 4669 6e61 6c50  nd XgboostFinalP
+00003210: 6172 616d 436f 6e66 6967 2e20 4661 6c6c  aramConfig. Fall
+00003220: 696e 6720 6261 636b 2074 6f20 6465 6661  ing back to defa
+00003230: 756c 7420 7365 7474 696e 6773 2e72 6d00  ult settings.rm.
+00003240: 0000 7238 0000 0072 3900 0000 7a41 436f  ..r8...r9...zACo
+00003250: 756c 6420 6e6f 7420 6669 6e64 2058 6762  uld not find Xgb
+00003260: 6f6f 7374 5475 6e65 5061 7261 6d73 436f  oostTuneParamsCo
+00003270: 6e66 6967 2e20 4661 6c6c 696e 6720 6261  nfig. Falling ba
+00003280: 636b 2074 6f20 6465 6661 756c 7473 2e72  ck to defaults.r
+00003290: 3d00 0000 72e2 0000 0072 0100 0000 727b  =...r....r....r{
+000032a0: 0000 0072 3c00 0000 da09 6f6f 665f 7363  ...r<.....oof_sc
+000032b0: 6f72 6572 ce00 0000 727e 0000 0029 2572  orer....r~...)%r
+000032c0: 5300 0000 721a 0000 0072 0d00 0000 7213  S...r....r....r.
+000032d0: 0000 0072 0b00 0000 7254 0000 0072 2300  ...r....rT...r#.
+000032e0: 0000 da09 656e 756d 6572 6174 65da 0573  ....enumerate..s
+000032f0: 706c 6974 da06 6173 7479 7065 da03 696e  plit..astype..in
+00003300: 74da 0469 6c6f 6372 1e00 0000 724c 0000  t..ilocr....rL..
+00003310: 0072 4d00 0000 7255 0000 0072 9e00 0000  .rM...rU...r....
+00003320: 729f 0000 0072 1c00 0000 720e 0000 0072  r....r....r....r
+00003330: 6c00 0000 722e 0000 0072 1b00 0000 720f  l...r....r....r.
+00003340: 0000 0072 3800 0000 723f 0000 0072 dc00  ...r8...r?...r..
+00003350: 0000 72f6 0000 0072 fa00 0000 72ea 0000  ..r....r....r...
+00003360: 0072 2000 0000 72a7 0000 0072 de00 0000  .r ...r....r....
+00003370: 721d 0000 0072 a800 0000 727f 0000 0072  r....r....r....r
+00003380: a900 0000 291b 7225 0000 0072 fb00 0000  ....).r%...r....
+00003390: 7231 0000 0072 3300 0000 7232 0000 0072  r1...r3...r2...r
+000033a0: 3400 0000 723a 0000 005a 0a73 7472 6174  4...r:...Z.strat
+000033b0: 6966 6965 725a 0b66 6f6c 645f 6c6f 7373  ifierZ.fold_loss
+000033c0: 6573 da03 5f66 6e5a 0774 726e 5f69 6478  es.._fnZ.trn_idx
+000033d0: 5a07 7661 6c5f 6964 785a 0c58 5f74 7261  Z.val_idxZ.X_tra
+000033e0: 696e 5f66 6f6c 645a 0a58 5f76 616c 5f66  in_foldZ.X_val_f
+000033f0: 6f6c 645a 0c79 5f74 7261 696e 5f66 6f6c  oldZ.y_train_fol
+00003400: 645a 0a79 5f76 616c 5f66 6f6c 645a 0b58  dZ.y_val_foldZ.X
+00003410: 5f74 6573 745f 666f 6c64 5a0b 795f 7465  _test_foldZ.y_te
+00003420: 7374 5f66 6f6c 6472 5800 0000 722d 0000  st_foldrX...r-..
+00003430: 0072 5700 0000 7259 0000 0072 1f00 0000  .rW...rY...r....
+00003440: 72ec 0000 005a 1963 6f6e 7374 616e 745f  r....Z.constant_
+00003450: 6c6f 7373 5f64 6567 7265 6761 7469 6f6e  loss_degregation
+00003460: 5a0d 6d61 7474 6865 7773 5f6d 6561 6e72  Z.matthews_meanr
+00003470: af00 0000 7226 0000 0072 2600 0000 7227  ....r&...r&...r'
+00003480: 0000 0072 a400 0000 1e02 0000 73bc 0000  ...r........s...
+00003490: 000c 0806 0208 0108 0102 0206 0102 0106  ................
+000034a0: 0106 fd04 0602 0110 0110 ff08 0408 0106  ................
+000034b0: fe08 0508 0106 fe06 0406 0404 0102 ff02  ................
+000034c0: fd02 0102 010c 0702 fd02 0102 0106 0506  ................
+000034d0: 0104 ff02 fd02 0104 010a 0504 0202 0102  ................
+000034e0: 0106 0106 fd06 0608 0102 0102 0104 ff08  ................
+000034f0: 040a 0104 0102 0102 0102 0106 0108 fc04  ................
+00003500: 0702 0102 0106 0106 fd10 0506 0208 0102  ................
+00003510: 0102 0104 ff04 0302 0102 0102 0106 0102  ................
+00003520: 0106 0106 fa04 0e08 0104 ff0a 030c 0110  ................
+00003530: 0410 0210 0206 0110 0206 0102 0102 0104  ................
+00003540: 0102 0102 0102 0102 0106 f904 097a 1f58  .............z.X
+00003550: 6762 6f6f 7374 4d6f 6465 6c2e 5f66 696e  gboostModel._fin
+00003560: 655f 7475 6e65 5f70 7265 6369 7365 6305  e_tune_precisec.
+00003570: 0000 0000 0000 0000 0000 000c 0000 000a  ................
+00003580: 0000 0003 0000 0073 8802 0000 7400 7401  .......s....t.t.
+00003590: a002 a100 9b00 6401 9d02 8301 0100 8800  ......d.........
+000035a0: 6a03 7215 8800 6a04 7215 8800 6a05 7215  j.r...j.r...j.r.
+000035b0: 8800 6a06 7319 7407 6402 8301 8201 8700  ..j.s.t.d.......
+000035c0: 8701 8702 8703 8704 6605 6403 6404 8408  ........f.d.d...
+000035d0: 7d05 8800 a008 a100 0100 7409 8800 6a03  }.........t...j.
+000035e0: 6a0a 6405 1900 740b 8302 72a7 7409 8800  j.d...t...r.t...
+000035f0: 6a03 6a0a 6406 1900 740b 8302 72a7 7409  j.j.d...t...r.t.
+00003600: 8800 6a03 6a0a 6407 1900 740b 8302 72a7  ..j.j.d...t...r.
+00003610: 7409 8800 6a03 6a0a 6408 1900 740b 8302  t...j.j.d...t...
+00003620: 72a7 740c 6a0d 8800 6a03 6a0a 6405 1900  r.t.j...j.j.d...
+00003630: 6409 1400 8800 6a03 6a0a 6405 1900 640a  d.....j.j.d...d.
+00003640: 1400 8800 6a04 6a0e 740b 640b 8d04 740c  ....j.j.t.d...t.
+00003650: 6a0d 8800 6a03 6a0a 6406 1900 6409 1400  j...j.j.d...d...
+00003660: 8800 6a03 6a0a 6406 1900 640a 1400 8800  ..j.j.d...d.....
+00003670: 6a04 6a0e 740b 640b 8d04 740c 6a0d 8800  j.j.t.d...t.j...
+00003680: 6a03 6a0a 6407 1900 6409 1400 8800 6a03  j.j.d...d.....j.
+00003690: 6a0a 6407 1900 640a 1400 8800 6a04 6a0e  j.d...d.....j.j.
+000036a0: 740b 640b 8d04 740c 6a0d 8800 6a03 6a0a  t.d...t.j...j.j.
+000036b0: 6408 1900 6409 1400 8800 6a03 6a0a 6408  d...d.....j.j.d.
+000036c0: 1900 640a 1400 8800 6a04 6a0e 740b 640b  ..d.....j.j.t.d.
+000036d0: 8d04 640c 9c04 7d06 6e04 7407 640d 8301  ..d...}.n.t.d...
+000036e0: 0100 8800 a00f a100 7d07 7410 6a11 640e  ........}.t.j.d.
+000036f0: 7410 6a12 a013 7c06 a101 640f 8d02 7d08  t.j...|...d...}.
+00003700: 7c08 6a14 7c05 8800 6a04 6a0e 7415 7c06  |.j.|...j.j.t.|.
+00003710: a016 a100 8301 1300 8800 6a04 6a17 6410  ..........j.j.d.
+00003720: 6410 6411 8d05 0100 7a16 7410 6a18 a019  d.d.....z.t.j...
+00003730: 7c08 a101 7d09 7c09 a01a a100 0100 7410  |...}.|.......t.
+00003740: 6a18 a01b 7c08 a101 7d09 7c09 a01a a100  j...|...}.|.....
+00003750: 0100 5700 6e0c 0400 741c 741d 7407 6603  ..W.n...t.t.t.f.
+00003760: 79f0 0100 0100 0100 5900 6e01 7700 8800  y.......Y.n.w...
+00003770: a00f a100 7d0a 7c0a 7c07 6b00 73fe 8800  ....}.|.|.k.s...
+00003780: 6a04 6a1e 9001 7338 7c08 6a1f 6a0a 7d0b  j.j...s8|.j.j.}.
+00003790: 7c0b 6405 1900 8800 6a03 6a0a 6405 3c00  |.d.....j.j.d.<.
+000037a0: 7c0b 6406 1900 8800 6a03 6a0a 6406 3c00  |.d.....j.j.d.<.
+000037b0: 7c0b 6407 1900 8800 6a03 6a0a 6407 3c00  |.d.....j.j.d.<.
+000037c0: 7c0b 6408 1900 8800 6a03 6a0a 6408 3c00  |.d.....j.j.d.<.
+000037d0: 7400 6412 7c07 9b00 6413 7c0a 9b00 6414  t.d.|...d.|...d.
+000037e0: 9d05 8301 0100 7400 6415 8800 6a03 6a0a  ......t.d...j.j.
+000037f0: 9b00 9d02 8301 0100 6400 5300 7400 6416  ........d.S.t.d.
+00003800: 7c07 9b00 6417 7c0a 9b00 9d04 8301 0100  |...d.|.........
+00003810: 6400 5300 2918 4e7a 313a 2053 7461 7274  d.S.).Nz1: Start
+00003820: 2067 7269 6420 7365 6172 6368 2066 696e   grid search fin
+00003830: 6520 7475 6e69 6e67 206f 6620 5867 626f  e tuning of Xgbo
+00003840: 6f73 7420 6d6f 6465 6c2e 725b 0000 0063  ost model.r[...c
+00003850: 0100 0000 0000 0000 0000 0000 0d00 0000  ................
+00003860: 0b00 0000 1300 0000 73c8 0100 0088 00a0  ........s.......
+00003870: 0088 0288 0488 0188 03a1 045c 027d 017d  ...........\.}.}
+00003880: 0274 016a 02a0 037c 0064 01a1 027d 0374  .t.j...|.d...}.t
+00003890: 0488 006a 056a 0683 017d 047c 006a 0764  ...j.j...}.|.j.d
+000038a0: 0288 006a 056a 0664 0219 0064 0314 0088  ...j.j.d...d....
+000038b0: 006a 056a 0664 0219 0064 0414 0064 0564  .j.j.d...d...d.d
+000038c0: 068d 047d 057c 006a 0764 0788 006a 056a  ...}.|.j.d...j.j
+000038d0: 0664 0719 0064 0314 0088 006a 056a 0664  .d...d.....j.j.d
+000038e0: 0719 0064 0414 0064 0564 068d 047d 067c  ...d...d.d...}.|
+000038f0: 006a 0764 0888 006a 056a 0664 0819 0064  .j.d...j.j.d...d
+00003900: 0314 0088 006a 056a 0664 0819 0064 0414  .....j.j.d...d..
+00003910: 0064 0564 068d 047d 077c 006a 0764 0988  .d.d...}.|.j.d..
+00003920: 006a 056a 0664 0919 0064 0314 0088 006a  .j.j.d...d.....j
+00003930: 056a 0664 0919 0064 0414 0064 0564 068d  .j.d...d...d.d..
+00003940: 047d 087c 057c 0464 023c 007c 067c 0464  .}.|.|.d.<.|.|.d
+00003950: 073c 007c 077c 0464 083c 007c 087c 0464  .<.|.|.d.<.|.|.d
+00003960: 093c 007c 04a0 0864 0a64 0ba1 027d 0988  .<.|...d.d...}..
+00003970: 006a 096a 0a64 0c6b 0272 9188 00a0 0b7c  .j.j.d.k.r.....|
+00003980: 017c 0288 037c 047c 097c 03a1 0653 0088  .|...|.|.|...S..
+00003990: 006a 096a 0a64 0c6b 0472 a488 006a 096a  .j.j.d.k.r...j.j
+000039a0: 0c72 a488 00a0 0d7c 0488 0288 0488 0188  .r.....|........
+000039b0: 03a1 0553 0074 0e6a 0f7c 047c 017c 0988  ...S.t.j.|.|.|..
+000039c0: 006a 096a 1088 006a 096a 0a64 0d88 006a  .j.j...j.j.d...j
+000039d0: 096a 117c 0367 0188 006a 096a 1264 0e8d  .j.|.g...j.j.d..
+000039e0: 097d 0a7c 0a64 0f19 00a0 13a1 007d 0b74  .}.|.d.......}.t
+000039f0: 1488 006a 156a 1683 0164 106b 0272 cc64  ...j.j...d.k.r.d
+00003a00: 107d 0c6e 0888 006a 156a 1664 1119 0064  .}.n...j.j.d...d
+00003a10: 0c17 007d 0c88 006a 156a 177c 0c64 1288  ...}...j.j.|.d..
+00003a20: 006a 097c 047c 0b64 1364 0564 148d 0701  .j.|.|.d.d.d....
+00003a30: 007c 0b53 0029 154e 7272 0000 0072 5c00  .|.S.).Nrr...r\.
+00003a40: 0000 e7cd cccc cccc ccec 3fe7 9a99 9999  ..........?.....
+00003a50: 9999 f13f 4672 5f00 0000 7262 0000 0072  ...?Fr_...rb...r
+00003a60: 6300 0000 725e 0000 0072 3a00 0000 723b  c...r^...r:...r;
+00003a70: 0000 0072 3c00 0000 5472 7300 0000 727a  ...r<...Trs...rz
+00003a80: 0000 0072 0100 0000 727b 0000 0072 7c00  ...r....r{...r|.
+00003a90: 0000 727d 0000 0072 7e00 0000 2918 7251  ..r}...r~...).rQ
+00003aa0: 0000 0072 4400 0000 72a0 0000 0072 a100  ...rD...r....r..
+00003ab0: 0000 7202 0000 0072 1c00 0000 7252 0000  ..r....r....rR..
+00003ac0: 0072 8900 0000 7253 0000 0072 1a00 0000  .r....rS...r....
+00003ad0: 7254 0000 0072 a200 0000 72a3 0000 0072  rT...r....r....r
+00003ae0: a400 0000 7255 0000 0072 a500 0000 723f  ....rU...r....r?
+00003af0: 0000 0072 2300 0000 72a6 0000 0072 a700  ...r#...r....r..
+00003b00: 0000 72a8 0000 0072 1d00 0000 727f 0000  ..r....r....r...
+00003b10: 0072 a900 0000 290d 72aa 0000 0072 5700  .r....).r....rW.
+00003b20: 0000 7258 0000 0072 ac00 0000 72fb 0000  ..rX...r....r...
+00003b30: 005a 0b61 6c70 6861 5f73 7061 6365 5a0c  .Z.alpha_spaceZ.
+00003b40: 6c61 6d62 6461 5f73 7061 6365 5a0b 6761  lambda_spaceZ.ga
+00003b50: 6d6d 615f 7370 6163 655a 0965 7461 5f73  mma_spaceZ.eta_s
+00003b60: 7061 6365 723a 0000 0072 ad00 0000 72ae  pacer:...r....r.
+00003b70: 0000 0072 af00 0000 a905 7225 0000 0072  ...r......r%...r
+00003b80: 3200 0000 7231 0000 0072 3400 0000 7233  2...r1...r4...r3
+00003b90: 0000 0072 2600 0000 7227 0000 0072 6800  ...r&...r'...rh.
+00003ba0: 0000 ae02 0000 7392 0000 0014 0106 0204  ......s.........
+00003bb0: 0104 ff0c 0404 0102 010e 010e 0102 0106  ................
+00003bc0: fc04 0602 010e 010e 0102 0106 fc04 0602  ................
+00003bd0: 010e 010e 0102 0106 fc04 0602 010e 010e  ................
+00003be0: 0102 0106 fc08 0708 0108 0108 010c 020c  ................
+00003bf0: 0204 010c 0104 ff0c 0406 0102 ff04 0302  ................
+00003c00: 0102 0102 0102 0102 0104 fb04 0802 0102  ................
+00003c10: 0102 0106 0106 0102 0106 0104 0106 0106  ................
+00003c20: f70c 0c10 0306 0110 0206 0102 0102 0104  ................
+00003c30: 0102 0102 0102 0102 0106 f904 0a7a 2958  .............z)X
+00003c40: 6762 6f6f 7374 4d6f 6465 6c2e 6669 6e65  gboostModel.fine
+00003c50: 5f74 756e 652e 3c6c 6f63 616c 733e 2e6f  _tune.<locals>.o
+00003c60: 626a 6563 7469 7665 725c 0000 0072 6200  bjectiver\...rb.
+00003c70: 0000 7263 0000 0072 5e00 0000 7204 0100  ..rc...r^...r...
+00003c80: 0072 0501 0000 2901 da05 6474 7970 6529  .r....)...dtype)
+00003c90: 0472 5c00 0000 7262 0000 0072 6300 0000  .r\...rb...rc...
+00003ca0: 725e 0000 007a 2953 6f6d 6520 7061 7261  r^...z)Some para
+00003cb0: 6d65 7465 7273 2061 7265 206e 6f74 2066  meters are not f
+00003cc0: 6c6f 6174 7320 6f72 2073 7472 696e 6773  loats or strings
+00003cd0: 72b2 0000 0029 0272 b300 0000 72b4 0000  r....).r....r...
+00003ce0: 0054 72b5 0000 007a 2647 7269 6420 7365  .Tr....z&Grid se
+00003cf0: 6172 6368 2069 6d70 726f 7665 6420 6576  arch improved ev
+00003d00: 616c 206d 6574 7269 6320 6672 6f6d 207a  al metric from z
+00003d10: 0420 746f 20da 012e 72b8 0000 007a 2d47  . to ...r....z-G
+00003d20: 7269 6420 7365 6172 6368 2063 6f75 6c64  rid search could
+00003d30: 206e 6f74 2069 6d70 726f 7665 2065 7661   not improve eva
+00003d40: 6c20 6d65 7472 6963 206f 6620 7a19 2e20  l metric of z.. 
+00003d50: 4265 7374 2073 636f 7265 2072 6561 6368  Best score reach
+00003d60: 6564 2077 6173 2029 2072 1300 0000 7203  ed was ) r....r.
+00003d70: 0000 0072 2f00 0000 721c 0000 0072 1a00  ...r/...r....r..
+00003d80: 0000 721b 0000 0072 1d00 0000 7242 0000  ..r....r....rB..
+00003d90: 0072 3000 0000 da0a 6973 696e 7374 616e  .r0.....isinstan
+00003da0: 6365 7252 0000 00da 0566 6c6f 6174 7220  cerR.....floatr 
+00003db0: 0000 00da 086c 696e 7370 6163 65da 2167  .....linspace.!g
+00003dc0: 7269 6473 6561 7263 685f 6e62 5f70 6172  ridsearch_nb_par
+00003dd0: 616d 6574 6572 735f 7065 725f 6772 6964  ameters_per_grid
+00003de0: 72d0 0000 0072 4400 0000 72c0 0000 0072  r....rD...r....r
+00003df0: be00 0000 5a0b 4772 6964 5361 6d70 6c65  ....Z.GridSample
+00003e00: 7272 c100 0000 72a8 0000 00da 046b 6579  rr....r......key
+00003e10: 73da 2267 7269 6473 6561 7263 685f 7475  s."gridsearch_tu
+00003e20: 6e69 6e67 5f6d 6178 5f72 756e 7469 6d65  ning_max_runtime
+00003e30: 5f73 6563 7372 c400 0000 72c5 0000 0072  _secsr....r....r
+00003e40: c600 0000 72c7 0000 0072 c800 0000 72c9  ....r....r....r.
+00003e50: 0000 0072 4700 0000 72ca 0000 0029 0c72  ...rG...r....).r
+00003e60: 2500 0000 7231 0000 0072 3200 0000 7233  %...r1...r2...r3
+00003e70: 0000 0072 3400 0000 7268 0000 005a 0c73  ...r4...rh...Z.s
+00003e80: 6561 7263 685f 7370 6163 655a 0d62 6573  earch_spaceZ.bes
+00003e90: 745f 7363 6f72 655f 6376 72cc 0000 0072  t_score_cvr....r
+00003ea0: cd00 0000 72d2 0000 005a 1778 6762 6f6f  ....r....Z.xgboo
+00003eb0: 7374 5f67 7269 645f 6265 7374 5f70 6172  st_grid_best_par
+00003ec0: 616d 7226 0000 0072 0601 0000 7227 0000  amr&...r....r'..
+00003ed0: 0072 4b00 0000 9c02 0000 73ae 0000 0012  .rK.......s.....
+00003ee0: 0704 0202 ff04 0202 fe04 0302 fd04 0402  ................
+00003ef0: fc02 0602 0104 ff14 0408 5710 0202 ff10  ..........W.....
+00003f00: 0202 fe10 0302 fd10 0402 fc04 070a 0102  ................
+00003f10: 0102 ff0e 0206 0102 0104 fb04 070e 010e  ................
+00003f20: 0106 0102 0104 fc04 060e 010e 0106 0102  ................
+00003f30: 0104 fc04 060e 010e 0106 0102 0104 fc08  ................
+00003f40: ec08 1c08 0204 020c 0106 ff04 0302 0106  ................
+00003f50: 010a 0102 ff06 0202 0102 0106 fa02 090c  ................
+00003f60: 0108 010c 010c 0112 0104 0102 ff08 0312  ................
+00003f70: 0208 0110 0102 0102 010c ff10 0310 0102  ................
+00003f80: 0110 0104 ff16 0302 020e 0108 ff7a 1658  .............z.X
+00003f90: 6762 6f6f 7374 4d6f 6465 6c2e 6669 6e65  gboostModel.fine
+00003fa0: 5f74 756e 65da 0264 6663 0200 0000 0000  _tune..dfc......
+00003fb0: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00003fc0: 0000 73d0 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
+00003fd0: 0064 019d 0283 0101 007c 006a 0372 0f7c  .d.......|.j.r.|
+00003fe0: 006a 0473 1374 0564 0283 0182 017c 006a  .j.s.t.d.....|.j
+00003ff0: 0672 217c 006a 066a 077c 0164 0364 0464  .r!|.j.j.|.d.d.d
+00004000: 058d 035c 027d 017d 0274 086a 097c 017c  ...\.}.}.t.j.|.|
+00004010: 006a 046a 0a64 068d 027d 037c 006a 0b73  .j.j.d...}.|.j.s
+00004020: 3174 0c64 0783 0182 017c 006a 0d73 3874  1t.d.....|.j.s8t
+00004030: 0c64 0883 0182 017c 006a 0ba0 0e7c 03a1  .d.....|.j...|..
+00004040: 017d 047c 006a 0f64 096b 0272 5474 10a0  .}.|.j.d.k.rTt..
+00004050: 1164 0a64 0b84 007c 0444 0083 01a1 017d  .d.d...|.D.....}
+00004060: 057c 057c 006a 0d6a 126b 047d 066e 0c7c  .|.|.j.j.k.}.n.|
+00004070: 047d 0574 10a0 1164 0c64 0b84 007c 0444  .}.t...d.d...|.D
+00004080: 0083 01a1 017d 0674 0064 0d83 0101 007c  .....}.t.d.....|
+00004090: 057c 0666 0253 0029 0e7a 1750 7265 6469  .|.f.S.).z.Predi
+000040a0: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
+000040b0: 612e fa33 3a20 5374 6172 7420 7072 6564  a..3: Start pred
+000040c0: 6963 7469 6e67 206f 6e20 6e65 7720 6461  icting on new da
+000040d0: 7461 2075 7369 6e67 2058 6762 6f6f 7374  ta using Xgboost
+000040e0: 206d 6f64 656c 2efa 2c63 6f6e 665f 7061   model..,conf_pa
+000040f0: 7261 6d73 5f78 6762 6f6f 7374 206f 7220  rams_xgboost or 
+00004100: 636f 6e66 5f74 7261 696e 696e 6720 6973  conf_training is
+00004110: 204e 6f6e 654e 5472 3600 0000 a901 7270   NoneNTr6.....rp
+00004120: 0000 00fa 204e 6f20 7472 6169 6e65 6420  .... No trained 
+00004130: 6d6f 6465 6c20 6861 7320 6265 656e 2066  model has been f
+00004140: 6f75 6e64 2efa 2b4e 6f20 6d6f 6465 6c20  ound..+No model 
+00004150: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00004160: 6c65 2068 6173 2062 6565 6e20 666f 756e  le has been foun
+00004170: 642e 7218 0000 0063 0100 0000 0000 0000  d.r....c........
+00004180: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00004190: f314 0000 0067 007c 005d 067d 017c 0164  .....g.|.].}.|.d
+000041a0: 0019 0091 0271 0253 00a9 0172 3c00 0000  .....q.S...r<...
+000041b0: 7226 0000 0072 d600 0000 7226 0000 0072  r&...r....r&...r
+000041c0: 2600 0000 7227 0000 0072 d900 0000 6d03  &...r'...r....m.
+000041d0: 0000 f302 0000 0014 007a 2858 6762 6f6f  .........z(Xgboo
+000041e0: 7374 4d6f 6465 6c2e 7072 6564 6963 742e  stModel.predict.
+000041f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00004200: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
+00004210: 0200 0000 0500 0000 5300 0000 72d3 0000  ........S...r...
+00004220: 0072 2600 0000 72d4 0000 0072 d600 0000  .r&...r....r....
+00004230: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
+00004240: d900 0000 7303 0000 72da 0000 00fa 1346  ....s...r......F
+00004250: 696e 6973 6865 6420 7072 6564 6963 7469  inished predicti
+00004260: 6e67 2913 7213 0000 0072 0300 0000 722f  ng).r....r....r/
+00004270: 0000 0072 1b00 0000 721a 0000 0072 4200  ...r....r....rB.
+00004280: 0000 721e 0000 0072 4d00 0000 7255 0000  ..r....rM...rU..
+00004290: 0072 9e00 0000 729f 0000 0072 1f00 0000  .r....r....r....
+000042a0: da09 4578 6365 7074 696f 6e72 1c00 0000  ..Exceptionr....
+000042b0: 72dd 0000 0072 1700 0000 7220 0000 0072  r....r....r ...r
+000042c0: de00 0000 da18 636c 6173 7369 6669 6361  ......classifica
+000042d0: 7469 6f6e 5f74 6872 6573 686f 6c64 2907  tion_threshold).
+000042e0: 7225 0000 0072 0f01 0000 da01 5f72 5800  r%...r......_rX.
+000042f0: 0000 da0d 7061 7274 6961 6c5f 7072 6f62  ....partial_prob
+00004300: 73da 0f70 7265 6469 6374 6564 5f70 726f  s..predicted_pro
+00004310: 6273 5a11 7072 6564 6963 7465 645f 636c  bsZ.predicted_cl
+00004320: 6173 7365 7372 2600 0000 7226 0000 0072  assesr&...r&...r
+00004330: 2700 0000 72dd 0000 0053 0300 0073 3400  '...r....S...s4.
+00004340: 0000 0202 0c01 04ff 0c03 0801 0602 0601  ................
+00004350: 0601 0aff 0404 0201 0601 06fe 0605 0801  ................
+00004360: 0602 0801 0c02 0a01 1401 0a02 04ff 0404  ................
+00004370: 1401 0801 0801 7a14 5867 626f 6f73 744d  ......z.XgboostM
+00004380: 6f64 656c 2e70 7265 6469 6374 6302 0000  odel.predictc...
+00004390: 0000 0000 0000 0000 0006 0000 0005 0000  ................
+000043a0: 0043 0000 0073 ac00 0000 7400 7401 a002  .C...s....t.t...
+000043b0: a100 9b00 6401 9d02 8301 0100 7c00 6a03  ....d.......|.j.
+000043c0: 720f 7c00 6a04 7313 7405 6402 8301 8201  r.|.j.s.t.d.....
+000043d0: 7c00 6a06 7221 7c00 6a06 6a07 7c01 6403  |.j.r!|.j.j.|.d.
+000043e0: 6404 6405 8d03 5c02 7d01 7d02 7408 6a09  d.d...\.}.}.t.j.
+000043f0: 7c01 7c00 6a04 6a0a 6406 8d02 7d03 7c00  |.|.j.j.d...}.|.
+00004400: 6a0b 7331 740c 6407 8301 8201 7c00 6a0d  j.s1t.d.....|.j.
+00004410: 7338 740c 6408 8301 8201 7c00 6a0b a00e  s8t.d.....|.j...
+00004420: 7c03 a101 7d04 7c00 6a0f 6409 6b02 724e  |...}.|.j.d.k.rN
+00004430: 7410 a011 640a 640b 8400 7c04 4400 8301  t...d.d...|.D...
+00004440: a101 7d05 6e02 7c04 7d05 7400 640c 8301  ..}.n.|.}.t.d...
+00004450: 0100 7c05 5300 290d 7a24 5072 6564 6963  ..|.S.).z$Predic
+00004460: 7420 636c 6173 7320 7363 6f72 6573 206f  t class scores o
+00004470: 6e20 756e 7365 656e 2064 6174 612e 7210  n unseen data.r.
+00004480: 0100 0072 1101 0000 4e54 7236 0000 0072  ...r....NTr6...r
+00004490: 1201 0000 7213 0100 0072 1401 0000 7218  ....r....r....r.
+000044a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000044b0: 0200 0000 0400 0000 5300 0000 7215 0100  ........S...r...
+000044c0: 0072 1601 0000 7226 0000 0072 d600 0000  .r....r&...r....
+000044d0: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
+000044e0: d900 0000 9103 0000 7217 0100 007a 2e58  ........r....z.X
+000044f0: 6762 6f6f 7374 4d6f 6465 6c2e 7072 6564  gboostModel.pred
+00004500: 6963 745f 7072 6f62 612e 3c6c 6f63 616c  ict_proba.<local
+00004510: 733e 2e3c 6c69 7374 636f 6d70 3e72 1801  s>.<listcomp>r..
+00004520: 0000 2912 7213 0000 0072 0300 0000 722f  ..).r....r....r/
+00004530: 0000 0072 1b00 0000 721a 0000 0072 4200  ...r....r....rB.
+00004540: 0000 721e 0000 0072 4d00 0000 7255 0000  ..r....rM...rU..
+00004550: 0072 9e00 0000 729f 0000 0072 1f00 0000  .r....r....r....
+00004560: 7219 0100 0072 1c00 0000 72dd 0000 0072  r....r....r....r
+00004570: 1700 0000 7220 0000 0072 de00 0000 2906  ....r ...r....).
+00004580: 7225 0000 0072 0f01 0000 721b 0100 0072  r%...r....r....r
+00004590: 5800 0000 721c 0100 0072 1d01 0000 7226  X...r....r....r&
+000045a0: 0000 0072 2600 0000 7227 0000 00da 0d70  ...r&...r'.....p
+000045b0: 7265 6469 6374 5f70 726f 6261 7703 0000  redict_probaw...
+000045c0: 732e 0000 0002 020c 0104 ff0c 0308 0106  s...............
+000045d0: 0206 0106 010a ff04 0402 0106 0106 fe06  ................
+000045e0: 0508 0106 0208 010c 020a 0116 0104 0208  ................
+000045f0: 0104 017a 1a58 6762 6f6f 7374 4d6f 6465  ...z.XgboostMode
+00004600: 6c2e 7072 6564 6963 745f 7072 6f62 6129  l.predict_proba)
+00004610: 054e 4e4e 4e4e 2901 72e2 0000 0029 27da  .NNNNN).r....)'.
+00004620: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00004630: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00004640: 655f 5fda 075f 5f64 6f63 5f5f 7207 0000  e__..__doc__r...
+00004650: 0072 0800 0000 720d 0000 0072 0f00 0000  .r....r....r....
+00004660: 720e 0000 0072 1000 0000 7215 0000 0072  r....r....r....r
+00004670: 2800 0000 724f 0000 00da 0653 6572 6965  (...rO.....Serie
+00004680: 7372 0500 0000 da03 7374 7272 0a01 0000  sr......strr....
+00004690: 722e 0000 0072 3000 0000 da09 4461 7461  r....r0.....Data
+000046a0: 4672 616d 6572 5500 0000 da07 426f 6f73  FramerU.....Boos
+000046b0: 7465 7272 5a00 0000 7248 0000 0072 d000  terrZ...rH...r..
+000046c0: 0000 7251 0000 0072 a200 0000 7201 0100  ..rQ...r....r...
+000046d0: 0072 f600 0000 7206 0000 0072 fa00 0000  .r....r....r....
+000046e0: 7204 0000 0072 a400 0000 724b 0000 0072  r....r....rK...r
+000046f0: 0900 0000 7220 0000 00da 076e 6461 7272  ....r .....ndarr
+00004700: 6179 72dd 0000 0072 1e01 0000 7226 0000  ayr....r....r&..
+00004710: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
+00004720: 7216 0000 001f 0000 0073 a400 0000 0800  r........s......
+00004730: 0401 0205 0201 0201 0201 0201 04f9 0602  ................
+00004740: 02fe 0603 02fd 0604 02fc 0605 02fb 0606  ................
+00004750: 02fa 0607 0af9 1c17 0807 0215 0402 02fe  ................
+00004760: 0403 02fd 0404 02fc 0405 02fb 0406 0afa  ................
+00004770: 024a 0402 02fe 0403 02fd 0404 02fc 0405  .J..............
+00004780: 02fb 0206 0afa 007f 0876 0813 0816 0222  .........v....."
+00004790: 04ff 0401 02ff 0401 02ff 0201 0aff 1623  ...............#
+000047a0: 021d 0a02 02fe 0403 02fd 0404 02fc 0405  ................
+000047b0: 02fb 0406 0afa 027e 0402 02fe 0403 02fd  .......~........
+000047c0: 0404 02fc 0405 02fb 0206 0afa 007f 2038  .............. 8
+000047d0: 1a24 7216 0000 0029 2772 2201 0000 da04  .$r....)'r".....
+000047e0: 636f 7079 7202 0000 0072 0300 0000 da06  copyr....r......
+000047f0: 7479 7069 6e67 7204 0000 0072 0500 0000  typingr....r....
+00004800: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00004810: 0900 0000 da05 6e75 6d70 7972 2000 0000  ......numpyr ...
+00004820: 7244 0000 00da 0670 616e 6461 7372 4f00  rD.....pandasrO.
+00004830: 0000 72b1 0000 0072 5500 0000 da0f 736b  ..r....rU.....sk
+00004840: 6c65 6172 6e2e 6d65 7472 6963 7372 0a00  learn.metricsr..
+00004850: 0000 da17 736b 6c65 6172 6e2e 6d6f 6465  ....sklearn.mode
+00004860: 6c5f 7365 6c65 6374 696f 6e72 0b00 0000  l_selectionr....
+00004870: da0d 736b 6c65 6172 6e2e 7574 696c 7372  ..sklearn.utilsr
+00004880: 0c00 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+00004890: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+000048a0: 6f6e 6669 6772 0d00 0000 720e 0000 0072  onfigr....r....r
+000048b0: 0f00 0000 da21 626c 7565 6361 7374 2e65  .....!bluecast.e
+000048c0: 7870 6572 696d 656e 7461 7469 6f6e 2e74  xperimentation.t
+000048d0: 7261 636b 696e 6772 1000 0000 da24 626c  rackingr.....$bl
+000048e0: 7565 6361 7374 2e67 656e 6572 616c 5f75  uecast.general_u
+000048f0: 7469 6c73 2e67 656e 6572 616c 5f75 7469  tils.general_uti
+00004900: 6c73 7211 0000 0072 1200 0000 7213 0000  lsr....r....r...
+00004910: 005a 2262 6c75 6563 6173 742e 6d6c 5f6d  .Z"bluecast.ml_m
+00004920: 6f64 656c 6c69 6e67 2e62 6173 655f 636c  odelling.base_cl
+00004930: 6173 7365 7372 1400 0000 da1d 626c 7565  assesr......blue
+00004940: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
+00004950: 6e67 2e63 7573 746f 6d72 1500 0000 7216  ng.customr....r.
+00004960: 0000 0072 2600 0000 7226 0000 0072 2600  ...r&...r&...r&.
+00004970: 0000 7227 0000 00da 083c 6d6f 6475 6c65  ..r'.....<module
+00004980: 3e01 0000 0073 2200 0000 0400 0c07 0c01  >....s".........
+00004990: 2001 0802 0801 0801 0801 0c01 0c01 0c01   ...............
+000049a0: 1402 0c05 1401 0c01 0c01 1403            ............
```

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-310.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 27 16:18:20 2024 UTC, .py size: 32380 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,1061 +1,1049 @@
-00000000: 6f0d 0d0a 0000 0000 4c25 2d66 7c7e 0000  o.......L%-f|~..
+00000000: 6f0d 0d0a 0000 0000 fc61 3866 a37e 0000  o........a8f.~..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 5a0b 6401  m.Z...d.d.l.Z.d.
 00000070: 6405 6c0c 5a0c 6401 6405 6c0d 5a0e 6401  d.l.Z.d.d.l.Z.d.
 00000080: 6405 6c0f 5a10 6401 6406 6c11 6d12 5a12  d.l.Z.d.d.l.m.Z.
 00000090: 0100 6401 6407 6c13 6d14 5a14 0100 6401  ..d.d.l.m.Z...d.
 000000a0: 6408 6c15 6d16 5a16 6d17 5a17 0100 6401  d.l.m.Z.m.Z...d.
 000000b0: 6409 6c15 6d18 5a19 0100 6401 640a 6c1a  d.l.m.Z...d.d.l.
 000000c0: 6d1b 5a1b 0100 6401 640b 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000d0: 6d1e 5a1e 0100 6401 640c 6c1f 6d20 5a20  m.Z...d.d.l.m Z 
-000000e0: 0100 6401 640d 6c21 6d22 5a22 0100 4700  ..d.d.l!m"Z"..G.
-000000f0: 640e 640f 8400 640f 6520 8303 5a23 6405  d.d...d.e ..Z#d.
-00000100: 5300 2910 6119 0100 0058 6762 6f6f 7374  S.).a....Xgboost
-00000110: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
-00000120: 6d6f 6465 6c2e 0a0a 5468 6973 206d 6f64  model...This mod
-00000130: 756c 6520 636f 6e74 6169 6e73 2061 2077  ule contains a w
-00000140: 7261 7070 6572 2066 6f72 2074 6865 2058  rapper for the X
-00000150: 6762 6f6f 7374 2063 6c61 7373 6966 6963  gboost classific
-00000160: 6174 696f 6e20 6d6f 6465 6c2e 2049 7420  ation model. It 
-00000170: 6361 6e20 6265 2075 7365 6420 746f 2074  can be used to t
-00000180: 7261 696e 2061 6e64 2f6f 7220 7475 6e65  rain and/or tune
-00000190: 2074 6865 206d 6f64 656c 2e0a 4974 2061   the model..It a
-000001a0: 6c73 6f20 6361 6c63 756c 6174 6573 2063  lso calculates c
-000001b0: 6c61 7373 2077 6569 6768 7473 2066 6f72  lass weights for
-000001c0: 2069 6d62 616c 616e 6365 6420 6461 7461   imbalanced data
-000001d0: 7365 7473 2e20 5468 6520 7765 6967 6874  sets. The weight
-000001e0: 7320 6d61 7920 6f72 206d 6179 206e 6f74  s may or may not
-000001f0: 2062 6520 7573 6564 2064 6565 7065 6e64   be used deepend
-00000200: 696e 6720 6f6e 2074 6865 0a68 7970 6572  ing on the.hyper
-00000210: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
-00000220: 2e0a e900 0000 0029 01da 0864 6565 7063  .......)...deepc
-00000230: 6f70 7929 01da 0864 6174 6574 696d 6529  opy)...datetime)
-00000240: 05da 0341 6e79 da04 4469 6374 da04 4c69  ...Any..Dict..Li
-00000250: 7374 da07 4c69 7465 7261 6cda 084f 7074  st..Literal..Opt
-00000260: 696f 6e61 6c4e 2901 da12 6d65 616e 5f73  ionalN)...mean_s
-00000270: 7175 6172 6564 5f65 7272 6f72 2901 da05  quared_error)...
-00000280: 4b46 6f6c 6429 02da 0e54 7261 696e 696e  KFold)...Trainin
-00000290: 6743 6f6e 6669 67da 1758 6762 6f6f 7374  gConfig..Xgboost
-000002a0: 4669 6e61 6c50 6172 616d 436f 6e66 6967  FinalParamConfig
-000002b0: 2901 da21 5867 626f 6f73 7454 756e 6550  )..!XgboostTuneP
-000002c0: 6172 616d 7352 6567 7265 7373 696f 6e43  aramsRegressionC
-000002d0: 6f6e 6669 6729 01da 1145 7870 6572 696d  onfig)...Experim
-000002e0: 656e 7454 7261 636b 6572 2902 da11 6368  entTracker)...ch
-000002f0: 6563 6b5f 6770 755f 7375 7070 6f72 74da  eck_gpu_support.
-00000300: 066c 6f67 6765 7229 01da 1a42 6173 6543  .logger)...BaseC
-00000310: 6c61 7373 4d6c 5265 6772 6573 7369 6f6e  lassMlRegression
-00000320: 4d6f 6465 6c29 01da 1343 7573 746f 6d50  Model)...CustomP
-00000330: 7265 7072 6f63 6573 7369 6e67 6300 0000  reprocessingc...
-00000340: 0000 0000 0000 0000 0000 0000 000e 0000  ................
-00000350: 0040 0000 0073 6601 0000 6500 5a01 6400  .@...sf...e.Z.d.
-00000360: 5a02 6401 5a03 0902 0902 0902 0902 0902  Z.d.Z...........
-00000370: 642f 6403 6504 6404 1900 6405 6505 6506  d/d.e.d...d.e.e.
-00000380: 1900 6406 6505 6507 1900 6407 6505 6508  ..d.e.e...d.e.e.
-00000390: 1900 6408 6505 6509 1900 6409 6505 650a  ..d.e.e...d.e.e.
-000003a0: 1900 660c 640a 640b 8405 5a0b 640c 640d  ..f.d.d...Z.d.d.
-000003b0: 8400 5a0c 640e 650d 6a0e 640f 650d 6a0e  ..Z.d.e.j.d.e.j.
-000003c0: 6410 650d 6a0f 6411 650d 6a0f 6412 6510  d.e.j.d.e.j.d.e.
-000003d0: 6a11 660a 6413 6414 8404 5a12 640e 650d  j.f.d.d...Z.d.e.
-000003e0: 6a0e 640f 650d 6a0e 6410 650d 6a0f 6411  j.d.e.j.d.e.j.d.
-000003f0: 650d 6a0f 6412 6402 660a 6415 6416 8404  e.j.d.d.f.d.d...
-00000400: 5a13 6417 6418 8400 5a14 6419 641a 8400  Z.d.d...Z.d.d...
-00000410: 5a15 641b 641c 8400 5a16 091d 6430 641e  Z.d.d...Z...d0d.
-00000420: 650d 6a0e 641f 650d 6a0f 6420 6517 6606  e.j.d.e.j.d e.f.
-00000430: 6421 6422 8405 5a18 6423 6519 651a 1900  d!d"..Z.d#e.e...
-00000440: 6412 651a 6604 6424 6425 8404 5a1b 6426  d.e.f.d$d%..Z.d&
-00000450: 651c 651d 651e 6602 1900 640e 650d 6a0e  e.e.e.f...d.e.j.
-00000460: 6410 650d 6a0f 640f 650d 6a0e 6411 650d  d.e.j.d.e.j.d.e.
-00000470: 6a0f 6427 6517 660c 6428 6429 8404 5a1f  j.d'e.f.d(d)..Z.
-00000480: 640e 650d 6a0e 640f 650d 6a0e 6410 650d  d.e.j.d.e.j.d.e.
-00000490: 6a0f 6411 650d 6a0f 6412 6402 660a 642a  j.d.e.j.d.d.f.d*
-000004a0: 642b 8404 5a20 642c 650d 6a0e 6412 6521  d+..Z d,e.j.d.e!
-000004b0: 6a22 6604 642d 642e 8404 5a23 6402 5300  j"f.d-d...Z#d.S.
-000004c0: 2931 da16 5867 626f 6f73 744d 6f64 656c  )1..XgboostModel
-000004d0: 5265 6772 6573 7369 6f6e 7a2b 5472 6169  Regressionz+Trai
-000004e0: 6e20 616e 642f 6f72 2074 756e 6520 5867  n and/or tune Xg
-000004f0: 626f 6f73 7420 7265 6772 6573 7369 6f6e  boost regression
-00000500: 206d 6f64 656c 2e4e da0d 636c 6173 735f   model.N..class_
-00000510: 7072 6f62 6c65 6dda 0a72 6567 7265 7373  problem..regress
-00000520: 696f 6eda 0d63 6f6e 665f 7472 6169 6e69  ion..conf_traini
-00000530: 6e67 da0c 636f 6e66 5f78 6762 6f6f 7374  ng..conf_xgboost
-00000540: da13 636f 6e66 5f70 6172 616d 735f 7867  ..conf_params_xg
-00000550: 626f 6f73 74da 1265 7870 6572 696d 656e  boost..experimen
-00000560: 745f 7472 6163 6b65 72da 1b63 7573 746f  t_tracker..custo
-00000570: 6d5f 696e 5f66 6f6c 645f 7072 6570 726f  m_in_fold_prepro
-00000580: 6365 7373 6f72 6307 0000 0000 0000 0000  cessorc.........
-00000590: 0000 0007 0000 0003 0000 0043 0000 0073  ...........C...s
-000005a0: 5800 0000 6400 7c00 5f00 7c01 7c00 5f01  X...d.|._.|.|._.
-000005b0: 7c02 7c00 5f02 7c04 7c00 5f03 7c03 7c00  |.|._.|.|._.|.|.
-000005c0: 5f04 7c05 7c00 5f05 7c06 7c00 5f06 7c00  _.|.|._.|.|._.|.
-000005d0: 6a02 7223 7407 6a08 a009 7c00 6a02 6a0a  j.r#t.j...|.j.j.
-000005e0: a101 7c00 5f0b 6400 5300 7407 6a08 a009  ..|._.d.S.t.j...
-000005f0: 6401 a101 7c00 5f0b 6400 5300 2902 4e72  d...|._.d.S.).Nr
-00000600: 0100 0000 290c da05 6d6f 6465 6c72 1400  ....)...modelr..
-00000610: 0000 7216 0000 0072 1800 0000 7217 0000  ..r....r....r...
-00000620: 0072 1900 0000 721a 0000 00da 026e 70da  .r....r......np.
-00000630: 0672 616e 646f 6dda 0b64 6566 6175 6c74  .random..default
-00000640: 5f72 6e67 da13 676c 6f62 616c 5f72 616e  _rng..global_ran
-00000650: 646f 6d5f 7374 6174 65da 1072 616e 646f  dom_state..rando
-00000660: 6d5f 6765 6e65 7261 746f 7229 07da 0473  m_generator)...s
-00000670: 656c 6672 1400 0000 7216 0000 0072 1700  elfr....r....r..
-00000680: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000690: 00a9 0072 2200 0000 fa4e 2f68 6f6d 652f  ...r"....N/home/
-000006a0: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
-000006b0: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
-000006c0: 6563 6173 742f 6d6c 5f6d 6f64 656c 6c69  ecast/ml_modelli
-000006d0: 6e67 2f78 6762 6f6f 7374 5f72 6567 7265  ng/xgboost_regre
-000006e0: 7373 696f 6e2e 7079 da08 5f5f 696e 6974  ssion.py..__init
-000006f0: 5f5f 2000 0000 7318 0000 0006 0906 0106  __ ...s.........
-00000700: 0106 0106 0106 0206 0106 0106 0106 010a  ................
-00000710: ff12 047a 1f58 6762 6f6f 7374 4d6f 6465  ...z.XgboostMode
-00000720: 6c52 6567 7265 7373 696f 6e2e 5f5f 696e  lRegression.__in
-00000730: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000740: 0001 0000 0003 0000 0043 0000 0073 b400  .........C...s..
-00000750: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
-00000760: 8301 0100 7c00 6a03 731a 7404 8300 7c00  ....|.j.s.t...|.
-00000770: 5f03 7400 7401 a002 a100 9b00 6402 9d02  _.t.t.......d...
-00000780: 8301 0100 6e09 7400 7401 a002 a100 9b00  ....n.t.t.......
-00000790: 6403 9d02 8301 0100 7c00 6a05 7334 7406  d.......|.j.s4t.
-000007a0: 8300 7c00 5f05 7400 7401 a002 a100 9b00  ..|._.t.t.......
-000007b0: 6404 9d02 8301 0100 6e09 7400 7401 a002  d.......n.t.t...
-000007c0: a100 9b00 6405 9d02 8301 0100 7c00 6a07  ....d.......|.j.
-000007d0: 734f 7408 8300 7c00 5f07 7400 7401 a002  sOt...|._.t.t...
-000007e0: a100 9b00 6406 9d02 8301 0100 6408 5300  ....d.......d.S.
-000007f0: 7400 7401 a002 a100 9b00 6407 9d02 8301  t.t.......d.....
-00000800: 0100 6408 5300 2909 7a36 4c6f 6164 206d  ..d.S.).z6Load m
-00000810: 756c 7469 706c 6520 636f 6e66 6967 7320  ultiple configs 
-00000820: 6f72 206c 6f61 6420 6465 6661 756c 7420  or load default 
-00000830: 636f 6e66 6967 7320 696e 7374 6561 642e  configs instead.
-00000840: 7a32 3a20 5374 6172 7420 6c6f 6164 696e  z2: Start loadin
-00000850: 6720 6578 6973 7469 6e67 206f 7220 6465  g existing or de
-00000860: 6661 756c 7420 636f 6e66 6967 2066 696c  fault config fil
-00000870: 6573 2e2e 7a1e 3a20 4c6f 6164 2064 6566  es..z.: Load def
-00000880: 6175 6c74 2054 7261 696e 696e 6743 6f6e  ault TrainingCon
-00000890: 6669 672e 7a20 3a20 466f 756e 6420 7072  fig.z : Found pr
-000008a0: 6f76 6964 6564 2054 7261 696e 696e 6743  ovided TrainingC
-000008b0: 6f6e 6669 672e 7a27 3a20 4c6f 6164 2064  onfig.z': Load d
-000008c0: 6566 6175 6c74 2058 6762 6f6f 7374 5475  efault XgboostTu
-000008d0: 6e65 5061 7261 6d73 436f 6e66 6967 2e7a  neParamsConfig.z
-000008e0: 293a 2046 6f75 6e64 2070 726f 7669 6465  ): Found provide
-000008f0: 6420 5867 626f 6f73 7454 756e 6550 6172  d XgboostTunePar
-00000900: 616d 7343 6f6e 6669 672e 7a27 3a20 4c6f  amsConfig.z': Lo
-00000910: 6164 2064 6566 6175 6c74 2058 6762 6f6f  ad default Xgboo
-00000920: 7374 4669 6e61 6c50 6172 616d 436f 6e66  stFinalParamConf
-00000930: 6967 2e7a 293a 2046 6f75 6e64 2070 726f  ig.z): Found pro
-00000940: 7669 6465 6420 5867 626f 6f73 7446 696e  vided XgboostFin
-00000950: 616c 5061 7261 6d43 6f6e 6669 672e 4e29  alParamConfig.N)
-00000960: 0972 1000 0000 7203 0000 00da 0675 7463  .r....r......utc
-00000970: 6e6f 7772 1600 0000 720b 0000 0072 1700  nowr....r....r..
-00000980: 0000 da17 5867 626f 6f73 7454 756e 6550  ....XgboostTuneP
-00000990: 6172 616d 7343 6f6e 6669 6772 1800 0000  aramsConfigr....
-000009a0: 720c 0000 00a9 0172 2100 0000 7222 0000  r......r!...r"..
-000009b0: 0072 2200 0000 7223 0000 00da 1063 6865  .r"...r#.....che
-000009c0: 636b 5f6c 6f61 645f 636f 6e66 7338 0000  ck_load_confs8..
-000009d0: 0073 1a00 0000 1202 0601 0801 1401 1202  .s..............
-000009e0: 0602 0801 1401 1202 0602 0801 1601 1602  ................
-000009f0: 7a27 5867 626f 6f73 744d 6f64 656c 5265  z'XgboostModelRe
-00000a00: 6772 6573 7369 6f6e 2e63 6865 636b 5f6c  gression.check_l
-00000a10: 6f61 645f 636f 6e66 73da 0778 5f74 7261  oad_confs..x_tra
-00000a20: 696e da06 785f 7465 7374 da07 795f 7472  in..x_test..y_tr
-00000a30: 6169 6eda 0679 5f74 6573 74da 0672 6574  ain..y_test..ret
-00000a40: 7572 6e63 0500 0000 0000 0000 0000 0000  urnc............
-00000a50: 0900 0000 0800 0000 4300 0000 739c 0100  ........C...s...
-00000a60: 0074 0074 01a0 02a1 009b 0064 019d 0283  .t.t.......d....
-00000a70: 0101 007c 00a0 03a1 0001 007c 006a 0472  ...|.......|.j.r
-00000a80: 167c 006a 0572 167c 006a 0673 1a74 0764  .|.j.r.|.j.s.t.d
-00000a90: 0283 0182 017c 006a 056a 0873 2674 096a  .....|.j.j.s&t.j
-00000aa0: 0aa0 0b74 096a 0a6a 0ca1 0101 007c 006a  ...t.j.j.....|.j
-00000ab0: 056a 0d72 367c 00a0 0e7c 017c 027c 037c  .j.r6|...|.|.|.|
-00000ac0: 04a1 0401 0074 0f64 0383 0101 007c 006a  .....t.d.....|.j
-00000ad0: 056a 1072 467c 00a0 117c 017c 027c 037c  .j.rF|...|.|.|.|
-00000ae0: 04a1 0401 0074 0f64 0483 0101 0074 0064  .....t.d.....t.d
-00000af0: 0583 0101 007c 006a 1272 617c 006a 12a0  .....|.j.ra|.j..
-00000b00: 137c 017c 03a1 025c 027d 017d 037c 006a  .|.|...\.}.}.|.j
-00000b10: 126a 147c 027c 0464 0664 078d 035c 027d  .j.|.|.d.d...\.}
-00000b20: 027d 047c 006a 056a 1572 7c74 0074 01a0  .}.|.j.j.r|t.t..
-00000b30: 02a1 009b 0064 089d 0283 0101 0074 16a0  .....d.......t..
-00000b40: 177c 017c 0267 02a1 017d 0174 16a0 177c  .|.|.g...}.t...|
-00000b50: 037c 0467 02a1 017d 037c 00a0 187c 017c  .|.g...}.|...|.|
-00000b60: 037c 027c 04a1 045c 027d 057d 067c 0564  .|.|...\.}.}.|.d
-00000b70: 0966 027c 0664 0a66 0267 027d 077c 006a  .f.|.d.f.g.}.|.j
-00000b80: 046a 19a0 1a64 0b64 0ca1 027d 087c 006a  .j...d.d...}.|.j
-00000b90: 056a 1b64 0d6b 0272 b27c 006a 1c72 b274  .j.d.k.r.|.j.r.t
-00000ba0: 1d6a 1e7c 006a 046a 197c 057c 087c 006a  .j.|.j.j.|.|.|.j
-00000bb0: 056a 1f7c 077c 006a 1c6a 2064 0e8d 067c  .j.|.|.j.j d...|
-00000bc0: 005f 216e 157c 006a 1c72 c774 1d6a 1e7c  ._!n.|.j.r.t.j.|
-00000bd0: 006a 046a 197c 057c 087c 006a 056a 1f7c  .j.j.|.|.|.j.j.|
-00000be0: 077c 006a 1c6a 2064 0e8d 067c 005f 2174  .|.j.j d...|._!t
-00000bf0: 0064 0f83 0101 007c 006a 2153 0029 107a  .d.....|.j!S.).z
-00000c00: 3f54 7261 696e 2058 6762 6f6f 7374 206d  ?Train Xgboost m
-00000c10: 6f64 656c 2e20 496e 636c 7564 6573 2068  odel. Includes h
-00000c20: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
-00000c30: 6e69 6e67 206f 6e20 6465 6661 756c 742e  ning on default.
-00000c40: 7a1e 3a20 5374 6172 7420 6669 7474 696e  z.: Start fittin
-00000c50: 6720 5867 626f 6f73 7420 6d6f 6465 6c2e  g Xgboost model.
-00000c60: fa40 636f 6e66 5f70 6172 616d 735f 7867  .@conf_params_xg
-00000c70: 626f 6f73 742c 2063 6f6e 665f 7472 6169  boost, conf_trai
-00000c80: 6e69 6e67 206f 7220 6578 7065 7269 6d65  ning or experime
-00000c90: 6e74 5f74 7261 636b 6572 2069 7320 4e6f  nt_tracker is No
-00000ca0: 6e65 7a1e 4669 6e69 7368 6564 2068 7970  nez.Finished hyp
-00000cb0: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
-00000cc0: 6e67 7a20 4669 6e69 7368 6564 2047 7269  ngz Finished Gri
-00000cd0: 6420 7365 6172 6368 2066 696e 6520 7475  d search fine tu
-00000ce0: 6e69 6e67 7a1a 5374 6172 7420 6669 6e61  ningz.Start fina
-00000cf0: 6c20 6d6f 6465 6c20 7472 6169 6e69 6e67  l model training
-00000d00: 46a9 01da 0e70 7265 6469 6374 6f6e 5f6d  F....predicton_m
-00000d10: 6f64 657a 7f3a 2055 6e69 6f6e 2074 7261  odez.: Union tra
-00000d20: 696e 2061 6e64 2074 6573 7420 6461 7461  in and test data
-00000d30: 2066 6f72 2066 696e 616c 206d 6f64 656c   for final model
-00000d40: 2074 7261 696e 696e 6720 6261 7365 6420   training based 
-00000d50: 6f6e 2054 7261 696e 696e 6743 6f6e 6669  on TrainingConfi
-00000d60: 670a 2020 2020 2020 2020 2020 2020 2070  g.             p
-00000d70: 6172 616d 2027 7573 655f 6675 6c6c 5f64  aram 'use_full_d
-00000d80: 6174 615f 666f 725f 6669 6e61 6c5f 6d6f  ata_for_final_mo
-00000d90: 6465 6c27 da05 7472 6169 6eda 0474 6573  del'..train..tes
-00000da0: 74da 0573 7465 7073 e92c 0100 00e9 0100  t..steps.,......
-00000db0: 0000 a904 da0f 6e75 6d5f 626f 6f73 745f  ......num_boost_
-00000dc0: 726f 756e 64da 1565 6172 6c79 5f73 746f  round..early_sto
-00000dd0: 7070 696e 675f 726f 756e 6473 da05 6576  pping_rounds..ev
-00000de0: 616c 73da 0c76 6572 626f 7365 5f65 7661  als..verbose_eva
-00000df0: 6c7a 1146 696e 6973 6865 6420 7472 6169  lz.Finished trai
-00000e00: 6e69 6e67 2922 7210 0000 0072 0300 0000  ning)"r....r....
-00000e10: 7225 0000 0072 2800 0000 7218 0000 0072  r%...r(...r....r
-00000e20: 1600 0000 7219 0000 00da 0a56 616c 7565  ....r......Value
-00000e30: 4572 726f 72da 1973 686f 775f 6465 7461  Error..show_deta
-00000e40: 696c 6564 5f74 756e 696e 675f 6c6f 6773  iled_tuning_logs
-00000e50: da06 6f70 7475 6e61 da07 6c6f 6767 696e  ..optuna..loggin
-00000e60: 67da 0d73 6574 5f76 6572 626f 7369 7479  g..set_verbosity
-00000e70: da07 5741 524e 494e 47da 0e61 7574 6f74  ..WARNING..autot
-00000e80: 756e 655f 6d6f 6465 6cda 0861 7574 6f74  une_model..autot
-00000e90: 756e 65da 0570 7269 6e74 da1e 656e 6162  une..print..enab
-00000ea0: 6c65 5f67 7269 645f 7365 6172 6368 5f66  le_grid_search_f
-00000eb0: 696e 655f 7475 6e69 6e67 da09 6669 6e65  ine_tuning..fine
-00000ec0: 5f74 756e 6572 1a00 0000 da0d 6669 745f  _tuner......fit_
-00000ed0: 7472 616e 7366 6f72 6dda 0974 7261 6e73  transform..trans
-00000ee0: 666f 726d da1d 7573 655f 6675 6c6c 5f64  form..use_full_d
-00000ef0: 6174 615f 666f 725f 6669 6e61 6c5f 6d6f  ata_for_final_mo
-00000f00: 6465 6cda 0270 64da 0663 6f6e 6361 74da  del..pd..concat.
-00000f10: 1163 7265 6174 655f 645f 6d61 7472 6963  .create_d_matric
-00000f20: 6573 da06 7061 7261 6d73 da03 706f 70da  es..params..pop.
-00000f30: 1468 7970 6572 7475 6e69 6e67 5f63 765f  .hypertuning_cv_
-00000f40: 666f 6c64 7372 1700 0000 da03 7867 6272  foldsr......xgbr
-00000f50: 3100 0000 7238 0000 00da 2576 6572 626f  1...r8....%verbo
-00000f60: 7369 7479 5f64 7572 696e 675f 6669 6e61  sity_during_fina
-00000f70: 6c5f 6d6f 6465 6c5f 7472 6169 6e69 6e67  l_model_training
-00000f80: 721b 0000 0029 0972 2100 0000 7229 0000  r....).r!...r)..
-00000f90: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000fa0: da07 645f 7472 6169 6eda 0664 5f74 6573  ..d_train..d_tes
-00000fb0: 74da 0865 7661 6c5f 7365 7472 3300 0000  t..eval_setr3...
-00000fc0: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
-00000fd0: 0366 6974 4d00 0000 7370 0000 0012 0808  .fitM...sp......
-00000fe0: 0104 0302 ff04 0202 fe04 0302 fd02 0502  ................
-00000ff0: 0104 ff08 0410 0108 0210 0108 0108 0210  ................
-00001000: 0108 0108 0206 0106 0104 0108 ff06 0306  ................
-00001010: 010a ff08 0402 010c 0104 ff0e 040e 0114  ................
-00001020: 0210 0110 0212 0204 0106 0102 0102 0106  ................
-00001030: 0102 0106 010a fa06 0804 0106 0102 0102  ................
-00001040: 0106 0102 0106 0108 fa08 0806 017a 1a58  .............z.X
-00001050: 6762 6f6f 7374 4d6f 6465 6c52 6567 7265  gboostModelRegre
-00001060: 7373 696f 6e2e 6669 7463 0500 0000 0000  ssion.fitc......
-00001070: 0000 0000 0000 0b00 0000 0e00 0000 0300  ................
-00001080: 0000 73a8 0100 0074 0074 01a0 02a1 009b  ..s....t.t......
-00001090: 0064 019d 0283 0101 0088 006a 0372 1288  .d.........j.r..
-000010a0: 006a 0472 1288 006a 0573 1674 0664 0283  .j.r...j.s.t.d..
-000010b0: 0182 0174 0783 0089 0188 00a0 08a1 0001  ...t............
-000010c0: 0088 006a 0372 2988 006a 0472 2988 006a  ...j.r)..j.r)..j
-000010d0: 0972 2988 006a 0573 2d74 0664 0383 0182  .r)..j.s-t.d....
-000010e0: 0187 0087 0187 0287 0387 0487 0566 0664  .............f.d
-000010f0: 0464 0584 087d 0564 067d 0674 0a6a 0b6a  .d...}.d.}.t.j.j
-00001100: 0c64 0788 006a 046a 0d88 006a 046a 0e64  .d...j.j...j.j.d
-00001110: 088d 037d 0774 0a6a 0f64 097c 077c 069b  ...}.t.j.d.|.|..
-00001120: 0064 0a9d 0264 0b8d 037d 087c 086a 107c  .d...d...}.|.j.|
-00001130: 0588 006a 046a 1188 006a 046a 1264 0764  ...j.j...j.j.d.d
-00001140: 0764 0c8d 0501 007a 1674 0a6a 13a0 147c  .d.....z.t.j...|
-00001150: 08a1 017d 097c 09a0 15a1 0001 0074 0a6a  ...}.|.......t.j
-00001160: 13a0 167c 08a1 017d 097c 09a0 15a1 0001  ...|...}.|......
-00001170: 0057 006e 0c04 0074 1774 1874 0666 0379  .W.n...t.t.t.f.y
-00001180: 8201 0001 0001 0059 006e 0177 007c 086a  .......Y.n.w.|.j
-00001190: 196a 1a7d 0a88 006a 046a 1b64 0d6b 0472  .j.}...j.j.d.k.r
-000011a0: 937c 0a64 0e19 0088 006a 045f 0d88 006a  .|.d.....j._...j
-000011b0: 096a 1c88 006a 096a 1d88 006a 096a 1e7c  .j...j.j...j.j.|
-000011c0: 0a64 0f19 007c 0a64 1019 007c 0a64 1119  .d...|.d...|.d..
-000011d0: 007c 0a64 1219 007c 0a64 1319 007c 0a64  .|.d...|.d...|.d
-000011e0: 1419 007c 0a64 1519 007c 0a64 1619 007c  ...|.d...|.d...|
-000011f0: 0a64 1719 007c 0a64 1819 0064 199c 0d88  .d...|.d...d....
-00001200: 006a 035f 1a69 0088 006a 036a 1aa5 0188  .j._.i...j.j....
-00001210: 01a5 0188 006a 035f 1a74 0064 1a88 006a  .....j._.t.d...j
-00001220: 036a 1a9b 009d 0283 0101 0064 1b53 0029  .j.........d.S.)
-00001230: 1c7a 7b54 756e 6520 6879 7065 7270 6172  .z{Tune hyperpar
-00001240: 616d 6574 6572 732e 0a0a 2020 2020 2020  ameters...      
-00001250: 2020 416e 2061 6c74 6572 6e61 7469 7665    An alternative
-00001260: 2063 6f6e 6669 6720 6361 6e20 6265 2070   config can be p
-00001270: 726f 7669 6465 6420 746f 206f 7665 7277  rovided to overw
-00001280: 7269 7465 2074 6865 2068 7970 6572 7061  rite the hyperpa
-00001290: 7261 6d65 7465 7220 7365 6172 6368 2073  rameter search s
-000012a0: 7061 6365 2e0a 2020 2020 2020 2020 7a2f  pace..        z/
-000012b0: 3a20 5374 6172 7420 6879 7065 7270 6172  : Start hyperpar
-000012c0: 616d 6574 6572 2074 756e 696e 6720 6f66  ameter tuning of
-000012d0: 2058 6762 6f6f 7374 206d 6f64 656c 2e72   Xgboost model.r
-000012e0: 2e00 0000 fa4f 4174 206c 6561 7374 206f  .....OAt least o
-000012f0: 6e65 206f 6620 7468 6520 636f 6e66 6967  ne of the config
-00001300: 7320 6f72 2065 7870 6572 696d 656e 745f  s or experiment_
-00001310: 7472 6163 6b65 7220 6973 204e 6f6e 652c  tracker is None,
-00001320: 2077 6869 6368 2069 7320 6e6f 7420 616c   which is not al
-00001330: 6c6f 7765 6463 0100 0000 0000 0000 0000  lowedc..........
-00001340: 0000 0a00 0000 1200 0000 1300 0000 7358  ..............sX
-00001350: 0200 0088 006a 006a 0188 006a 006a 0288  .....j.j...j.j..
-00001360: 006a 006a 037c 006a 0464 0188 006a 006a  .j.j.|.j.d...j.j
-00001370: 0588 006a 006a 0664 0264 038d 047c 006a  ...j.j.d.d...|.j
-00001380: 0764 0488 006a 006a 0888 006a 006a 0964  .d...j.j...j.j.d
-00001390: 0264 038d 047c 006a 0464 0588 006a 006a  .d...|.j.d...j.j
-000013a0: 0a88 006a 006a 0b64 0264 038d 047c 006a  ...j.j.d.d...|.j
-000013b0: 0464 0688 006a 006a 0c88 006a 006a 0d64  .d...j.j...j.j.d
-000013c0: 0264 038d 047c 006a 0464 0788 006a 006a  .d...|.j.d...j.j
-000013d0: 0c88 006a 006a 0d64 0264 038d 047c 00a0  ...j.j.d.d...|..
-000013e0: 0764 0888 006a 006a 0e88 006a 006a 0fa1  .d...j.j...j.j..
-000013f0: 037c 00a0 0464 0988 006a 006a 1088 006a  .|...d...j.j...j
-00001400: 006a 11a1 037c 00a0 0464 0a88 006a 006a  .j...|...d...j.j
-00001410: 1288 006a 006a 13a1 037c 00a0 0464 0b88  ...j.j...|...d..
-00001420: 006a 006a 1488 006a 006a 15a1 037c 006a  .j.j...j.j...|.j
-00001430: 0764 0c88 006a 006a 1688 006a 006a 1764  .d...j.j...j.j.d
-00001440: 0264 038d 0464 0d9c 0d7d 0169 007c 01a5  .d...d...}.i.|..
-00001450: 0188 01a5 017d 0174 186a 1988 0388 0588  .....}.t.j......
-00001460: 006a 1a6a 1b64 0e8d 037d 0274 186a 1988  .j.j.d...}.t.j..
-00001470: 0288 0488 006a 1a6a 1b64 0e8d 037d 0374  .....j.j.d...}.t
-00001480: 1c6a 1da0 1e7c 0064 0fa1 027d 047c 01a0  .j...|.d...}.|..
-00001490: 1f64 0c64 10a1 027d 0588 006a 1a6a 2064  .d.d...}...j.j d
-000014a0: 116b 0272 b388 00a0 217c 027c 0388 047c  .k.r....!|.|...|
-000014b0: 017c 057c 04a1 0653 0088 006a 1a6a 2064  .|.|...S...j.j d
-000014c0: 116b 0472 d688 006a 1a6a 2272 d67c 00a0  .k.r...j.j"r.|..
-000014d0: 2364 1287 0066 0164 1364 1484 0874 2464  #d...f.d.d...t$d
-000014e0: 1583 0144 0083 01a1 027d 0688 00a0 257c  ...D.....}....%|
-000014f0: 0188 0388 0588 0288 047c 06a1 0653 007c  .........|...S.|
-00001500: 00a0 2364 1287 0066 0164 1664 1484 0874  ..#d...f.d.d...t
-00001510: 2464 1583 0144 0083 01a1 027d 0674 186a  $d...D.....}.t.j
-00001520: 267c 017c 027c 0588 006a 1a6a 2788 006a  &|.|.|...j.j'..j
-00001530: 1a6a 2064 027c 067c 0467 0188 006a 1a6a  .j d.|.|.g...j.j
-00001540: 2864 178d 097d 077c 0764 1819 00a0 29a1  (d...}.|.d....).
-00001550: 007c 0764 1819 00a0 2aa1 0064 1913 0017  .|.d....*..d....
-00001560: 007d 0874 2b88 006a 2c6a 2d83 0164 1a6b  .}.t+..j,j-..d.k
-00001570: 0290 0172 1464 1a7d 096e 0888 006a 2c6a  ...r.d.}.n...j,j
-00001580: 2d64 1b19 0064 1117 007d 0988 006a 2c6a  -d...d...}...j,j
-00001590: 2e7c 0964 1c88 006a 1a7c 017c 0864 1d64  .|.d...j.|.|.d.d
-000015a0: 1e64 1f8d 0701 007c 0853 0029 204e da03  .d.....|.S.) N..
-000015b0: 6574 6154 a901 da03 6c6f 67da 096d 6178  etaT....log..max
-000015c0: 5f64 6570 7468 da05 616c 7068 61da 066c  _depth..alpha..l
-000015d0: 616d 6264 61da 0567 616d 6d61 da0a 6d61  ambda..gamma..ma
-000015e0: 785f 6c65 6176 6573 da09 7375 6273 616d  x_leaves..subsam
-000015f0: 706c 65da 1063 6f6c 7361 6d70 6c65 5f62  ple..colsample_b
-00001600: 7974 7265 65da 1163 6f6c 7361 6d70 6c65  ytree..colsample
-00001610: 5f62 796c 6576 656c 7233 0000 0029 0dda  _bylevelr3...)..
-00001620: 096f 626a 6563 7469 7665 da07 626f 6f73  .objective..boos
-00001630: 7465 72da 0b65 7661 6c5f 6d65 7472 6963  ter..eval_metric
-00001640: 7256 0000 0072 5900 0000 725a 0000 0072  rV...rY...rZ...r
-00001650: 5b00 0000 725c 0000 0072 5d00 0000 725e  [...r\...r]...r^
-00001660: 0000 0072 5f00 0000 7260 0000 0072 3300  ...r_...r`...r3.
-00001670: 0000 a902 da05 6c61 6265 6cda 1265 6e61  ......label..ena
-00001680: 626c 655f 6361 7465 676f 7269 6361 6cfa  ble_categorical.
-00001690: 0974 6573 742d 726d 7365 7234 0000 0072  .test-rmser4...r
-000016a0: 3500 0000 da0b 7261 6e64 6f6d 5f73 6565  5.....random_see
-000016b0: 6463 0100 0000 0000 0000 0000 0000 0200  dc..............
-000016c0: 0000 0400 0000 1300 0000 f318 0000 0067  ...............g
-000016d0: 007c 005d 087d 0188 006a 006a 017c 0117  .|.].}...j.j.|..
-000016e0: 0091 0271 0253 0072 2200 0000 a902 7216  ...q.S.r".....r.
-000016f0: 0000 0072 1f00 0000 a902 da02 2e30 da01  ...r.........0..
-00001700: 6972 2700 0000 7222 0000 0072 2300 0000  ir'...r"...r#...
-00001710: da0a 3c6c 6973 7463 6f6d 703e 1501 0000  ..<listcomp>....
-00001720: f302 0000 0018 007a 4658 6762 6f6f 7374  .......zFXgboost
-00001730: 4d6f 6465 6c52 6567 7265 7373 696f 6e2e  ModelRegression.
-00001740: 6175 746f 7475 6e65 2e3c 6c6f 6361 6c73  autotune.<locals
-00001750: 3e2e 6f62 6a65 6374 6976 652e 3c6c 6f63  >.objective.<loc
-00001760: 616c 733e 2e3c 6c69 7374 636f 6d70 3ee9  als>.<listcomp>.
-00001770: 6400 0000 6301 0000 0000 0000 0000 0000  d...c...........
-00001780: 0002 0000 0004 0000 0013 0000 0072 6900  .............ri.
-00001790: 0000 7222 0000 0072 6a00 0000 726b 0000  ..r"...rj...rk..
-000017a0: 0072 2700 0000 7222 0000 0072 2300 0000  .r'...r"...r#...
-000017b0: 726e 0000 001e 0100 0072 6f00 0000 a909  rn.......ro.....
-000017c0: 724c 0000 00da 0664 7472 6169 6e72 3700  rL.....dtrainr7.
-000017d0: 0000 7238 0000 00da 056e 666f 6c64 da09  ..r8.....nfold..
-000017e0: 6173 5f70 616e 6461 73da 0473 6565 64da  as_pandas..seed.
-000017f0: 0963 616c 6c62 6163 6b73 da07 7368 7566  .callbacks..shuf
-00001800: 666c 65fa 0e74 6573 742d 726d 7365 2d6d  fle..test-rmse-m
-00001810: 6561 6ee7 6666 6666 6666 e63f 7201 0000  ean.ffffff.?r...
-00001820: 00e9 ffff ffff da08 6376 5f73 636f 7265  ........cv_score
-00001830: 7a0d 6164 6a75 7374 6564 2072 6d73 6546  z.adjusted rmseF
-00001840: a907 da0d 6578 7065 7269 6d65 6e74 5f69  ....experiment_i
-00001850: 64da 0e73 636f 7265 5f63 6174 6567 6f72  d..score_categor
-00001860: 79da 0f74 7261 696e 696e 675f 636f 6e66  y..training_conf
-00001870: 6967 da10 6d6f 6465 6c5f 7061 7261 6d65  ig..model_parame
-00001880: 7465 7273 da0b 6576 616c 5f73 636f 7265  ters..eval_score
-00001890: 73da 0b6d 6574 7269 635f 7573 6564 da17  s..metric_used..
-000018a0: 6d65 7472 6963 5f68 6967 6865 725f 6973  metric_higher_is
-000018b0: 5f62 6574 7465 7229 2f72 1700 0000 da11  _better)/r......
-000018c0: 7867 626f 6f73 745f 6f62 6a65 6374 6976  xgboost_objectiv
-000018d0: 6572 6200 0000 da13 7867 626f 6f73 745f  erb.....xgboost_
-000018e0: 6576 616c 5f6d 6574 7269 63da 0d73 7567  eval_metric..sug
-000018f0: 6765 7374 5f66 6c6f 6174 da07 6574 615f  gest_float..eta_
-00001900: 6d69 6eda 0765 7461 5f6d 6178 da0b 7375  min..eta_max..su
-00001910: 6767 6573 745f 696e 74da 0d6d 6178 5f64  ggest_int..max_d
-00001920: 6570 7468 5f6d 696e da0d 6d61 785f 6465  epth_min..max_de
-00001930: 7074 685f 6d61 78da 0961 6c70 6861 5f6d  pth_max..alpha_m
-00001940: 696e da09 616c 7068 615f 6d61 78da 0a6c  in..alpha_max..l
-00001950: 616d 6264 615f 6d69 6eda 0a6c 616d 6264  ambda_min..lambd
-00001960: 615f 6d61 78da 0e6d 6178 5f6c 6561 7665  a_max..max_leave
-00001970: 735f 6d69 6eda 0e6d 6178 5f6c 6561 7665  s_min..max_leave
-00001980: 735f 6d61 78da 0e73 7562 5f73 616d 706c  s_max..sub_sampl
-00001990: 655f 6d69 6eda 0e73 7562 5f73 616d 706c  e_min..sub_sampl
-000019a0: 655f 6d61 78da 1663 6f6c 5f73 616d 706c  e_max..col_sampl
-000019b0: 655f 6279 5f74 7265 655f 6d69 6eda 1663  e_by_tree_min..c
-000019c0: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
-000019d0: 655f 6d61 78da 1763 6f6c 5f73 616d 706c  e_max..col_sampl
-000019e0: 655f 6279 5f6c 6576 656c 5f6d 696e da17  e_by_level_min..
-000019f0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
-00001a00: 7665 6c5f 6d61 78da 0973 7465 7073 5f6d  vel_max..steps_m
-00001a10: 696e da09 7374 6570 735f 6d61 7872 4f00  in..steps_maxrO.
-00001a20: 0000 da07 444d 6174 7269 7872 1600 0000  ....DMatrixr....
-00001a30: da1d 6361 745f 656e 636f 6469 6e67 5f76  ..cat_encoding_v
-00001a40: 6961 5f6d 6c5f 616c 676f 7269 7468 6d72  ia_ml_algorithmr
-00001a50: 3d00 0000 da0b 696e 7465 6772 6174 696f  =.....integratio
-00001a60: 6eda 1658 4742 6f6f 7374 5072 756e 696e  n..XGBoostPrunin
-00001a70: 6743 616c 6c62 6163 6b72 4d00 0000 724e  gCallbackrM...rN
-00001a80: 0000 00da 1774 7261 696e 5f73 696e 676c  .....train_singl
-00001a90: 655f 666f 6c64 5f6d 6f64 656c da11 7072  e_fold_model..pr
-00001aa0: 6563 6973 655f 6376 5f74 756e 696e 67da  ecise_cv_tuning.
-00001ab0: 1373 7567 6765 7374 5f63 6174 6567 6f72  .suggest_categor
-00001ac0: 6963 616c da05 7261 6e67 65da 125f 6669  ical..range.._fi
-00001ad0: 6e65 5f74 756e 655f 7072 6563 6973 65da  ne_tune_precise.
-00001ae0: 0263 7672 3800 0000 da17 7368 7566 666c  .cvr8.....shuffl
-00001af0: 655f 6475 7269 6e67 5f74 7261 696e 696e  e_during_trainin
-00001b00: 67da 046d 6561 6eda 0373 7464 da03 6c65  g..mean..std..le
-00001b10: 6e72 1900 0000 727d 0000 00da 0b61 6464  nr....r}.....add
-00001b20: 5f72 6573 756c 7473 290a da05 7472 6961  _results)...tria
-00001b30: 6cda 0570 6172 616d 7251 0000 0072 5200  l..paramrQ...rR.
-00001b40: 0000 da10 7072 756e 696e 675f 6361 6c6c  ....pruning_call
-00001b50: 6261 636b 7233 0000 0072 6800 0000 da06  backr3...rh.....
-00001b60: 7265 7375 6c74 da0e 6164 6a75 7374 6564  result..adjusted
-00001b70: 5f73 636f 7265 da06 6e65 775f 6964 a906  _score..new_id..
-00001b80: 7221 0000 00da 0874 7261 696e 5f6f 6e72  r!.....train_onr
-00001b90: 2a00 0000 7229 0000 0072 2c00 0000 722b  *...r)...r,...r+
-00001ba0: 0000 0072 2200 0000 7223 0000 0072 6100  ...r"...r#...ra.
-00001bb0: 0000 ba00 0000 73f0 0000 0006 0206 0106  ......s.........
-00001bc0: 0104 0102 0106 0106 0102 0104 fc04 0602  ................
-00001bd0: 0106 0106 0102 0104 fc04 0602 0106 0106  ................
-00001be0: 0102 0104 fc04 0602 0106 0106 0102 0104  ................
-00001bf0: fc04 0602 0106 0106 0102 0104 fc04 0602  ................
-00001c00: 0106 0106 0102 fd04 0502 0106 0106 0102  ................
-00001c10: fd04 0502 0106 0106 0102 fd04 0502 0106  ................
-00001c20: 0106 0102 fd04 0502 0106 0106 0102 0104  ................
-00001c30: fc06 ca0c 3d04 0102 0102 0106 0106 fd04  ....=...........
-00001c40: 0602 0102 0106 0106 fd06 0604 0104 ff0c  ................
-00001c50: 040c 0204 010c 0104 ff0c 0406 0102 ff04  ................
-00001c60: 0302 0114 0104 fe04 050c 0104 ff04 0402  ................
-00001c70: 0114 0104 fe04 0402 0102 0102 0106 0106  ................
-00001c80: 0102 0102 0104 0106 0106 f70a 0c0e 0104  ................
-00001c90: ff12 0506 0110 0206 0102 0102 0104 0102  ................
-00001ca0: 0102 0102 0102 0106 f904 0a7a 3258 6762  ...........z2Xgb
-00001cb0: 6f6f 7374 4d6f 6465 6c52 6567 7265 7373  oostModelRegress
-00001cc0: 696f 6e2e 6175 746f 7475 6e65 2e3c 6c6f  ion.autotune.<lo
-00001cd0: 6361 6c73 3e2e 6f62 6a65 6374 6976 65da  cals>.objective.
-00001ce0: 0778 6762 6f6f 7374 5429 03da 0c6d 756c  .xgboostT)...mul
-00001cf0: 7469 7661 7269 6174 6572 7500 0000 da10  tivariateru.....
-00001d00: 6e5f 7374 6172 7475 705f 7472 6961 6c73  n_startup_trials
-00001d10: da08 6d69 6e69 6d69 7a65 7a07 2074 756e  ..minimizez. tun
-00001d20: 696e 6729 03da 0964 6972 6563 7469 6f6e  ing)...direction
-00001d30: da07 7361 6d70 6c65 72da 0a73 7475 6479  ..sampler..study
-00001d40: 5f6e 616d 65a9 04da 086e 5f74 7269 616c  _name....n_trial
-00001d50: 73da 0774 696d 656f 7574 da0e 6763 5f61  s..timeout..gc_a
-00001d60: 6674 6572 5f74 7269 616c da11 7368 6f77  fter_trial..show
-00001d70: 5f70 726f 6772 6573 735f 6261 7272 3500  _progress_barr5.
-00001d80: 0000 7268 0000 0072 5900 0000 725a 0000  ..rh...rY...rZ..
-00001d90: 0072 5b00 0000 725c 0000 0072 5d00 0000  .r[...r\...r]...
-00001da0: 725e 0000 0072 5f00 0000 7260 0000 0072  r^...r_...r`...r
-00001db0: 5600 0000 7233 0000 0029 0d72 6100 0000  V...r3...).ra...
-00001dc0: 7262 0000 0072 6300 0000 7259 0000 0072  rb...rc...rY...r
-00001dd0: 5a00 0000 725b 0000 0072 5c00 0000 725d  Z...r[...r\...r]
-00001de0: 0000 0072 5e00 0000 725f 0000 0072 6000  ...r^...r_...r`.
-00001df0: 0000 7256 0000 0072 3300 0000 fa0d 4265  ..rV...r3.....Be
-00001e00: 7374 2070 6172 616d 733a 204e 291f 7210  st params: N).r.
-00001e10: 0000 0072 0300 0000 7225 0000 0072 1800  ...r....r%...r..
-00001e20: 0000 7216 0000 0072 1900 0000 723b 0000  ..r....r....r;..
-00001e30: 0072 0f00 0000 7228 0000 0072 1700 0000  .r....r(...r....
-00001e40: 723d 0000 00da 0873 616d 706c 6572 73da  r=.....samplers.
-00001e50: 0a54 5045 5361 6d70 6c65 7272 1f00 0000  .TPESamplerr....
-00001e60: da1f 6f70 7475 6e61 5f73 616d 706c 6572  ..optuna_sampler
-00001e70: 5f6e 5f73 7461 7274 7570 5f74 7269 616c  _n_startup_trial
-00001e80: 73da 0c63 7265 6174 655f 7374 7564 79da  s..create_study.
-00001e90: 086f 7074 696d 697a 65da 1c68 7970 6572  .optimize..hyper
-00001ea0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
-00001eb0: 5f72 6f75 6e64 73da 2668 7970 6572 7061  _rounds.&hyperpa
-00001ec0: 7261 6d65 7465 725f 7475 6e69 6e67 5f6d  rameter_tuning_m
-00001ed0: 6178 5f72 756e 7469 6d65 5f73 6563 73da  ax_runtime_secs.
-00001ee0: 0d76 6973 7561 6c69 7a61 7469 6f6e da19  .visualization..
-00001ef0: 706c 6f74 5f6f 7074 696d 697a 6174 696f  plot_optimizatio
-00001f00: 6e5f 6869 7374 6f72 79da 0473 686f 77da  n_history..show.
-00001f10: 1670 6c6f 745f 7061 7261 6d5f 696d 706f  .plot_param_impo
-00001f20: 7274 616e 6365 73da 115a 6572 6f44 6976  rtances..ZeroDiv
-00001f30: 6973 696f 6e45 7272 6f72 da0c 5275 6e74  isionError..Runt
-00001f40: 696d 6545 7272 6f72 da0a 6265 7374 5f74  imeError..best_t
-00001f50: 7269 616c 724c 0000 0072 4e00 0000 7284  rialrL...rN...r.
-00001f60: 0000 0072 6200 0000 7285 0000 0029 0b72  ...rb...r....).r
-00001f70: 2100 0000 7229 0000 0072 2a00 0000 722b  !...r)...r*...r+
-00001f80: 0000 0072 2c00 0000 7261 0000 00da 0961  ...r,...ra.....a
-00001f90: 6c67 6f72 6974 686d 72b6 0000 00da 0573  lgorithmr......s
-00001fa0: 7475 6479 da03 6669 67da 1278 6762 6f6f  tudy..fig..xgboo
-00001fb0: 7374 5f62 6573 745f 7061 7261 6d72 2200  st_best_paramr".
-00001fc0: 0000 72af 0000 0072 2300 0000 7242 0000  ..r....r#...rB..
-00001fd0: 0097 0000 0073 9c00 0000 120b 0402 02ff  .....s..........
-00001fe0: 0402 02fe 0403 02fd 0205 0201 04ff 0604  ................
-00001ff0: 0802 0403 02ff 0402 02fe 0403 02fd 0404  ................
-00002000: 02fc 0206 0201 04ff 1604 007f 0408 0601  ................
-00002010: 0201 0601 0601 06fd 0405 0201 0201 0801  ................
-00002020: 06fd 0406 0201 0601 0601 0201 0201 06fb  ................
-00002030: 0207 0c01 0801 0601 0201 04ff 0c03 1201  ................
-00002040: 0401 02ff 0803 0c01 0c01 0603 0601 0601  ................
-00002050: 0201 0201 02ff 0603 0601 0601 0601 0601  ................
-00002060: 0601 0601 0601 0601 0af1 0211 0601 02ff  ................
-00002070: 0202 08fe 1604 7a1f 5867 626f 6f73 744d  ......z.XgboostM
-00002080: 6f64 656c 5265 6772 6573 7369 6f6e 2e61  odelRegression.a
-00002090: 7574 6f74 756e 6563 0100 0000 0000 0000  utotunec........
-000020a0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000020b0: 735e 0000 007c 006a 006a 0172 177c 006a  s^...|.j.j.r.|.j
-000020c0: 006a 0264 016b 0273 0e7c 006a 006a 0372  .j.d.k.s.|.j.j.r
-000020d0: 177c 006a 046a 0564 0264 038d 017d 017c  .|.j.j.d.d...}.|
-000020e0: 0153 007c 006a 006a 0172 2a7c 006a 006a  .S.|.j.j.r*|.j.j
-000020f0: 0264 016b 0472 2a7c 006a 046a 0564 0264  .d.k.r*|.j.j.d.d
-00002100: 038d 017d 017c 0153 0074 066a 077d 017c  ...}.|.S.t.j.}.|
-00002110: 0153 0029 044e 7235 0000 00da 1772 6f6f  .S.).Nr5.....roo
-00002120: 745f 6d65 616e 5f73 7175 6172 6564 5f65  t_mean_squared_e
-00002130: 7272 6f72 2901 da0d 7461 7267 6574 5f6d  rror)...target_m
-00002140: 6574 7269 6329 0872 1600 0000 7241 0000  etric).r....rA..
-00002150: 0072 4e00 0000 729f 0000 0072 1900 0000  .rN...r....r....
-00002160: da0e 6765 745f 6265 7374 5f73 636f 7265  ..get_best_score
-00002170: 721c 0000 00da 0369 6e66 2902 7221 0000  r......inf).r!..
-00002180: 00da 1262 6573 745f 7363 6f72 655f 6376  ...best_score_cv
-00002190: 5f67 7269 6472 2200 0000 7222 0000 0072  _gridr"...r"...r
-000021a0: 2300 0000 72d2 0000 0079 0100 0073 2200  #...r....y...s".
-000021b0: 0000 0801 0c01 0601 02ff 0603 0201 06ff  ................
-000021c0: 040c 06f8 02ff 0c02 0602 0201 06ff 0405  ................
-000021d0: 06ff 0401 7a25 5867 626f 6f73 744d 6f64  ....z%XgboostMod
-000021e0: 656c 5265 6772 6573 7369 6f6e 2e67 6574  elRegression.get
-000021f0: 5f62 6573 745f 7363 6f72 6563 0500 0000  _best_scorec....
-00002200: 0000 0000 0000 0000 0700 0000 0500 0000  ................
-00002210: 4300 0000 7330 0000 0074 006a 017c 017c  C...s0...t.j.|.|
-00002220: 027c 006a 026a 0364 018d 037d 0574 006a  .|.j.j.d...}.t.j
-00002230: 017c 037c 047c 006a 026a 0364 018d 037d  .|.|.|.j.j.d...}
-00002240: 067c 057c 0666 0253 0029 024e 7264 0000  .|.|.f.S.).Nrd..
-00002250: 0029 0472 4f00 0000 729a 0000 0072 1600  .).rO...r....r..
-00002260: 0000 729b 0000 0029 0772 2100 0000 7229  ..r....).r!...r)
-00002270: 0000 0072 2b00 0000 722a 0000 0072 2c00  ...r+...r*...r,.
-00002280: 0000 7251 0000 0072 5200 0000 7222 0000  ..rQ...rR...r"..
-00002290: 0072 2200 0000 7223 0000 0072 4b00 0000  .r"...r#...rK...
-000022a0: 8c01 0000 7316 0000 0004 0102 0102 0106  ....s...........
-000022b0: 0106 fd04 0502 0102 0106 0106 fd08 057a  ...............z
-000022c0: 2858 6762 6f6f 7374 4d6f 6465 6c52 6567  (XgboostModelReg
-000022d0: 7265 7373 696f 6e2e 6372 6561 7465 5f64  ression.create_d
-000022e0: 5f6d 6174 7269 6365 7363 0700 0000 0000  _matricesc......
-000022f0: 0000 0000 0000 0c00 0000 0900 0000 4300  ..............C.
-00002300: 0000 7390 0000 007c 0164 0166 027c 0264  ..s....|.d.f.|.d
-00002310: 0266 0267 027d 0774 006a 017c 047c 017c  .f.g.}.t.j.|.|.|
-00002320: 057c 006a 026a 037c 077c 0667 017c 006a  .|.j.j.|.|.g.|.j
-00002330: 046a 0564 038d 077d 087c 08a0 067c 02a1  .j.d...}.|...|..
-00002340: 017d 0974 077c 037c 0964 0464 058d 037d  .}.t.|.|.d.d...}
-00002350: 0a74 087c 006a 096a 0a83 0164 066b 0272  .t.|.j.j...d.k.r
-00002360: 3064 067d 0b6e 087c 006a 096a 0a64 0719  0d.}.n.|.j.j.d..
-00002370: 0064 0817 007d 0b7c 006a 096a 0b7c 0b64  .d...}.|.j.j.|.d
-00002380: 097c 006a 027c 047c 0a64 0a64 0464 0b8d  .|.j.|.|.d.d.d..
-00002390: 0701 007c 0a53 0029 0c4e 7231 0000 0072  ...|.S.).Nr1...r
-000023a0: 3200 0000 2905 7237 0000 0072 3800 0000  2...).r7...r8...
-000023b0: 7239 0000 0072 7600 0000 723a 0000 0046  r9...rv...r:...F
-000023c0: a901 da07 7371 7561 7265 6472 0100 0000  ....squaredr....
-000023d0: 727a 0000 0072 3500 0000 da17 7369 6d70  rz...r5.....simp
-000023e0: 6c65 5f74 7261 696e 5f74 6573 745f 7363  le_train_test_sc
-000023f0: 6f72 6572 d000 0000 727c 0000 0029 0c72  orer....r|...).r
-00002400: 4f00 0000 7231 0000 0072 1600 0000 7238  O...r1...r....r8
-00002410: 0000 0072 1700 0000 da26 7665 7262 6f73  ...r.....&verbos
-00002420: 6974 795f 6475 7269 6e67 5f68 7970 6572  ity_during_hyper
-00002430: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
-00002440: da07 7072 6564 6963 7472 0900 0000 72a7  ..predictr....r.
-00002450: 0000 0072 1900 0000 727d 0000 0072 a800  ...r....r}...r..
-00002460: 0000 290c 7221 0000 0072 5100 0000 7252  ..).r!...rQ...rR
-00002470: 0000 0072 2c00 0000 72aa 0000 0072 3300  ...r,...r....r3.
-00002480: 0000 72ab 0000 0072 5300 0000 721b 0000  ..r....rS...r...
-00002490: 00da 0570 7265 6473 da03 6d73 6572 ae00  ...preds..mser..
-000024a0: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
-000024b0: 0072 9e00 0000 9901 0000 7332 0000 0010  .r........s2....
-000024c0: 0304 0102 0102 0102 0106 0102 0104 0106  ................
-000024d0: 0106 f90a 090e 0110 0306 0110 0206 0102  ................
-000024e0: 0102 0104 0102 0102 0102 0102 0106 f904  ................
-000024f0: 097a 2e58 6762 6f6f 7374 4d6f 6465 6c52  .z.XgboostModelR
-00002500: 6567 7265 7373 696f 6e2e 7472 6169 6e5f  egression.train_
-00002510: 7369 6e67 6c65 5f66 6f6c 645f 6d6f 6465  single_fold_mode
-00002520: 6c72 7000 0000 da07 6576 616c 5f64 66da  lrp.....eval_df.
-00002530: 0679 5f74 7275 65da 0a69 7465 7261 7469  .y_true..iterati
-00002540: 6f6e 7363 0500 0000 0000 0000 0000 0000  onsc............
-00002550: 1000 0000 0700 0000 4300 0000 739a 0000  ........C...s...
-00002560: 0067 007d 0574 007c 0483 0144 005d 447d  .g.}.t.|...D.]D}
-00002570: 0664 0164 027c 0614 0002 027d 077d 087c  .d.d.|.....}.}.|
-00002580: 026a 015c 027d 097d 0a7c 006a 02a0 037c  .j.\.}.}.|.j...|
-00002590: 077c 087c 097c 0a67 02a1 037d 0b7c 027c  .|.|.|.g...}.|.|
-000025a0: 0b17 007d 0c7c 006a 0472 3074 056a 067c  ...}.|.j.r0t.j.|
-000025b0: 0c7c 037c 006a 046a 0764 038d 037d 0d6e  .|.|.j.j.d...}.n
-000025c0: 0474 0864 0483 0182 017c 01a0 097c 0da1  .t.d.....|...|..
-000025d0: 017d 0e74 0a7c 036a 0ba0 0ca1 007c 0ea0  .}.t.|.j.....|..
-000025e0: 0ca1 0064 0564 068d 037d 0f7c 05a0 0d7c  ...d.d...}.|...|
-000025f0: 0fa1 0101 0071 067c 0553 0029 0761 9f01  .....q.|.S.).a..
-00002600: 0000 4675 6e63 7469 6f6e 2074 6f20 6164  ..Function to ad
-00002610: 6420 696e 6372 6561 7369 6e67 206e 6f69  d increasing noi
-00002620: 7365 2061 6e64 2065 7661 6c75 6174 6520  se and evaluate 
-00002630: 6974 2e0a 0a20 2020 2020 2020 2054 6865  it...        The
-00002640: 2066 756e 6374 696f 6e20 6578 7065 6374   function expect
-00002650: 7320 6120 7472 6169 6e65 6420 6d6f 6465  s a trained mode
-00002660: 6c20 616e 6420 6120 6461 7461 6672 616d  l and a datafram
-00002670: 6520 7769 7468 2074 6865 2073 616d 6520  e with the same 
-00002680: 636f 6c75 6d6e 7320 6173 2074 6865 2074  columns as the t
-00002690: 7261 696e 696e 6720 6461 7461 2e0a 2020  raining data..  
-000026a0: 2020 2020 2020 5468 6520 7472 6169 6e69        The traini
-000026b0: 6e67 2064 6174 6120 7368 6f75 6c64 2062  ng data should b
-000026c0: 6520 6e6f 726d 616c 6c79 2064 6973 7472  e normally distr
-000026d0: 6962 7574 6564 2028 636f 6e73 6964 6572  ibuted (consider
-000026e0: 2075 7369 6e67 2061 2070 6f77 6572 2074   using a power t
-000026f0: 7261 6e73 666f 726d 6572 2077 6974 6820  ransformer with 
-00002700: 7965 6f2d 6a6f 686e 736f 6e29 2e0a 0a20  yeo-johnson)... 
-00002710: 2020 2020 2020 2054 6865 2066 756e 6374         The funct
-00002720: 696f 6e20 7769 6c6c 2061 7070 6c79 2069  ion will apply i
-00002730: 6e63 7265 6173 696e 676c 7920 6e6f 6973  ncreasingly nois
-00002740: 6520 746f 2074 6865 2065 7661 6c20 6461  e to the eval da
-00002750: 7461 6672 616d 6520 616e 6420 6576 616c  taframe and eval
-00002760: 7561 7465 2074 6865 206d 6f64 656c 206f  uate the model o
-00002770: 6e20 6974 2e0a 0a20 2020 2020 2020 2052  n it...        R
-00002780: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
-00002790: 206c 6f73 7365 732e 0a20 2020 2020 2020   losses..       
-000027a0: 2072 0100 0000 679a 9999 9999 99c9 3f72   r....g.......?r
-000027b0: 6400 0000 7a21 4e6f 2074 7261 696e 696e  d...z!No trainin
-000027c0: 675f 636f 6e66 6967 2063 6f75 6c64 2062  g_config could b
-000027d0: 6520 666f 756e 6446 72d5 0000 0029 0e72  e foundFr....).r
-000027e0: a100 0000 da05 7368 6170 6572 2000 0000  ......shaper ...
-000027f0: da06 6e6f 726d 616c 7216 0000 0072 4f00  ..normalr....rO.
-00002800: 0000 729a 0000 0072 9b00 0000 723b 0000  ..r....r....r;..
-00002810: 0072 d900 0000 7209 0000 00da 0676 616c  .r....r......val
-00002820: 7565 73da 0674 6f6c 6973 74da 0661 7070  ues..tolist..app
-00002830: 656e 6429 1072 2100 0000 da08 6d6c 5f6d  end).r!.....ml_m
-00002840: 6f64 656c 72dc 0000 0072 dd00 0000 72de  odelr....r....r.
-00002850: 0000 00da 066c 6f73 7365 7372 6d00 0000  .....lossesrm...
-00002860: da02 6d75 da05 7369 676d 61da 014e da01  ..mu..sigma..N..
-00002870: 44da 056e 6f69 7365 da0b 6576 616c 5f64  D..noise..eval_d
-00002880: 665f 6d6f 64da 0664 5f65 7661 6c72 da00  f_mod..d_evalr..
-00002890: 0000 da04 6c6f 7373 7222 0000 0072 2200  ....lossr"...r".
-000028a0: 0000 7223 0000 00da 1a69 6e63 7265 6173  ..r#.....increas
-000028b0: 696e 675f 6e6f 6973 655f 6576 616c 7561  ing_noise_evalua
-000028c0: 746f 72b9 0100 0073 2600 0000 040d 0c01  tor....s&.......
-000028d0: 0e01 0a01 1401 0801 0601 0401 0201 0201  ................
-000028e0: 0601 08fd 0806 0a01 0202 1001 06ff 0c03  ................
-000028f0: 0402 7a31 5867 626f 6f73 744d 6f64 656c  ..z1XgboostModel
-00002900: 5265 6772 6573 7369 6f6e 2e69 6e63 7265  Regression.incre
-00002910: 6173 696e 675f 6e6f 6973 655f 6576 616c  asing_noise_eval
-00002920: 7561 746f 7272 e500 0000 6302 0000 0000  uatorr....c.....
-00002930: 0000 0000 0000 0006 0000 0006 0000 0043  ...............C
-00002940: 0000 0073 8c00 0000 6401 7d02 7400 7401  ...s....d.}.t.t.
-00002950: 7c01 8301 8301 4400 5d1c 7d03 7c03 6402  |.....D.].}.|.d.
-00002960: 1700 7401 7c01 8301 6402 1800 6b04 7216  ..t.|...d...k.r.
-00002970: 0100 6e0f 7c01 7c03 1900 7c01 7c03 6402  ..n.|.|...|.|.d.
-00002980: 1700 1900 6b04 7224 7c02 6402 3700 7d02  ....k.r$|.d.7.}.
-00002990: 7108 7c02 6401 6b02 722d 6403 7d04 7c04  q.|.d.k.r-d.}.|.
-000029a0: 5300 7401 7c01 8301 7d05 7c01 6401 1900  S.t.|...}.|.d...
-000029b0: 7402 a003 7c01 6404 7c02 8502 1900 a101  t...|.d.|.......
-000029c0: 7c05 7c05 7c02 1800 1b00 1300 1800 7d04  |.|.|.........}.
-000029d0: 7c04 5300 2905 6142 0100 0043 616c 6375  |.S.).aB...Calcu
-000029e0: 6c61 7465 2061 2077 6569 6768 7465 6420  late a weighted 
-000029f0: 6c6f 7373 2062 6173 6564 206f 6e20 7468  loss based on th
-00002a00: 6520 6e75 6d62 6572 206f 6620 7469 6d65  e number of time
-00002a10: 7320 7468 6520 6c6f 7373 2064 6563 7265  s the loss decre
-00002a20: 6173 6564 2e0a 0a20 2020 2020 2020 2045  ased...        E
-00002a30: 7870 6563 7473 2061 206c 6973 7420 6f66  xpects a list of
-00002a40: 206c 6f73 7365 7320 636f 6d69 6e67 2066   losses coming f
-00002a50: 726f 6d20 696e 6372 6561 7369 6e67 5f6e  rom increasing_n
-00002a60: 6f69 7365 5f65 7661 6c75 6174 6f72 2e20  oise_evaluator. 
-00002a70: 4368 6563 6b73 2068 6f77 206d 616e 7920  Checks how many 
-00002a80: 7469 6d65 7320 7468 6520 6c6f 7373 2064  times the loss d
-00002a90: 6563 7265 6173 6564 2061 6e64 0a20 2020  ecreased and.   
-00002aa0: 2020 2020 2063 616c 6375 6c61 7465 7320       calculates 
-00002ab0: 6120 7765 6967 6874 6564 206c 6f73 7320  a weighted loss 
-00002ac0: 6261 7365 6420 6f6e 2074 6865 206e 756d  based on the num
-00002ad0: 6265 7220 6f66 2074 696d 6573 2074 6865  ber of times the
-00002ae0: 206c 6f73 7320 6465 6372 6561 7365 642e   loss decreased.
-00002af0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00002b00: 7320 7468 6520 7765 6967 6874 6564 206c  s the weighted l
-00002b10: 6f73 732e 0a20 2020 2020 2020 2072 0100  oss..        r..
-00002b20: 0000 7235 0000 0069 e703 0000 4e29 0472  ..r5...i....N).r
-00002b30: a100 0000 72a7 0000 0072 1c00 0000 72a6  ....r....r....r.
-00002b40: 0000 0029 0672 2100 0000 72e5 0000 00da  ...).r!...r.....
-00002b50: 116e 625f 6c6f 7373 5f64 6563 7265 6173  .nb_loss_decreas
-00002b60: 6564 da03 6964 78da 0d77 6569 6768 7465  ed..idx..weighte
-00002b70: 645f 6c6f 7373 da09 6e62 5f6c 6f73 7365  d_loss..nb_losse
-00002b80: 7372 2200 0000 7222 0000 0072 2300 0000  sr"...r"...r#...
-00002b90: da20 636f 6e73 7461 6e74 5f6c 6f73 735f  . constant_loss_
-00002ba0: 6465 6772 6567 6174 696f 6e5f 6661 6374  degregation_fact
-00002bb0: 6f72 dd01 0000 731e 0000 0004 0810 0114  or....s.........
-00002bc0: 0104 0114 0108 0102 8008 0304 0104 0a08  ................
-00002bd0: f816 010a 0106 ff04 077a 3758 6762 6f6f  .........z7Xgboo
-00002be0: 7374 4d6f 6465 6c52 6567 7265 7373 696f  stModelRegressio
-00002bf0: 6e2e 636f 6e73 7461 6e74 5f6c 6f73 735f  n.constant_loss_
-00002c00: 6465 6772 6567 6174 696f 6e5f 6661 6374  degregation_fact
-00002c10: 6f72 da0c 7475 6e65 645f 7061 7261 6d73  or..tuned_params
-00002c20: 7268 0000 0063 0700 0000 0000 0000 0000  rh...c..........
-00002c30: 0000 1b00 0000 0900 0000 4300 0000 73ea  ..........C...s.
-00002c40: 0100 007c 01a0 0064 0164 02a1 027d 077c  ...|...d.d...}.|
-00002c50: 006a 0173 1174 0283 007c 005f 0174 0364  .j.s.t...|._.t.d
-00002c60: 0383 0101 0074 047c 006a 016a 0564 047c  .....t.|.j.j.d.|
-00002c70: 0664 058d 037d 0867 007d 0974 067c 08a0  .d...}.g.}.t.|..
-00002c80: 077c 027c 03a0 0874 09a1 01a1 0283 0144  .|.|...t.......D
-00002c90: 005d 9c5c 027d 0a5c 027d 0b7d 0c7c 026a  .].\.}.\.}.}.|.j
-00002ca0: 0a7c 0b19 007c 026a 0a7c 0c19 0002 027d  .|...|.j.|.....}
-00002cb0: 0d7d 0e7c 036a 0a7c 0b19 007c 036a 0a7c  .}.|.j.|...|.j.|
-00002cc0: 0c19 0002 027d 0f7d 107c 006a 0b72 647c  .....}.}.|.j.rd|
-00002cd0: 006a 0ba0 0c7c 0d7c 0fa1 025c 027d 0d7d  .j...|.|...\.}.}
-00002ce0: 0f7c 006a 0ba0 0d7c 047c 05a1 025c 027d  .|.j...|.|...\.}
-00002cf0: 117d 127c 006a 0b6a 0d7c 0e7c 1064 0664  .}.|.j.j.|.|.d.d
-00002d00: 078d 035c 027d 0e7d 106e 057c 047c 0502  ...\.}.}.n.|.|..
-00002d10: 027d 117d 1274 0e6a 0f7c 0e7c 107c 006a  .}.}.t.j.|.|.|.j
-00002d20: 016a 1064 088d 037d 137c 006a 1173 7e74  .j.d...}.|.j.s~t
-00002d30: 1283 007c 005f 1174 0364 0983 0101 0074  ...|._.t.d.....t
-00002d40: 0e6a 0f7c 0d7c 0f7c 006a 016a 1064 088d  .j.|.|.|.j.j.d..
-00002d50: 037d 147c 1464 0a66 027c 1364 0b66 0267  .}.|.d.f.|.d.f.g
-00002d60: 027d 157c 006a 1373 9b74 1483 007c 005f  .}.|.j.s.t...|._
-00002d70: 1374 0364 0c83 0101 0074 0e6a 157c 017c  .t.d.....t.j.|.|
-00002d80: 147c 077c 006a 016a 167c 157c 006a 136a  .|.|.j.j.|.|.j.j
-00002d90: 1764 0d8d 067d 1674 0e6a 0f7c 117c 127c  .d...}.t.j.|.|.|
-00002da0: 006a 016a 1064 088d 037d 177c 16a0 187c  .j.j.d...}.|...|
-00002db0: 17a1 017d 187c 09a0 1974 1a7c 127c 1864  ...}.|...t.|.|.d
-00002dc0: 0664 0e8d 03a1 0101 0071 2774 1ba0 1c74  .d.......q't...t
-00002dd0: 1ba0 1d7c 09a1 01a1 017d 197c 006a 1e72  ...|.....}.|.j.r
-00002de0: f37c 006a 0172 f374 1f7c 006a 1e6a 2083  .|.j.r.t.|.j.j .
-00002df0: 0164 0f6b 0272 dd64 0f7d 1a6e 087c 006a  .d.k.r.d.}.n.|.j
-00002e00: 1e6a 2064 1019 0064 1117 007d 1a7c 006a  .j d...d...}.|.j
-00002e10: 1e6a 217c 1a64 127c 006a 017c 017c 1964  .j!|.d.|.j.|.|.d
-00002e20: 1364 0664 148d 0701 007c 1953 0029 154e  .d.d.....|.S.).N
-00002e30: 7233 0000 0072 3400 0000 7a3e 436f 756c  r3...r4...z>Coul
-00002e40: 6420 6e6f 7420 6669 6e64 2054 7261 696e  d not find Train
-00002e50: 696e 6720 636f 6e66 6967 2e20 4661 6c6c  ing config. Fall
-00002e60: 696e 6720 6261 636b 2074 6f20 6465 6661  ing back to defa
-00002e70: 756c 7420 7661 6c75 6573 5429 03da 086e  ult valuesT)...n
-00002e80: 5f73 706c 6974 7372 7700 0000 da0c 7261  _splitsrw.....ra
-00002e90: 6e64 6f6d 5f73 7461 7465 4672 2f00 0000  ndom_stateFr/...
-00002ea0: 7264 0000 007a 4943 6f75 6c64 206e 6f74  rd...zICould not
-00002eb0: 2066 696e 6420 5867 626f 6f73 7446 696e   find XgboostFin
-00002ec0: 616c 5061 7261 6d43 6f6e 6669 672e 2046  alParamConfig. F
-00002ed0: 616c 6c69 6e67 2062 6163 6b20 746f 2064  alling back to d
-00002ee0: 6566 6175 6c74 2073 6574 7469 6e67 732e  efault settings.
-00002ef0: 7231 0000 0072 3200 0000 7a41 436f 756c  r1...r2...zACoul
-00002f00: 6420 6e6f 7420 6669 6e64 2058 6762 6f6f  d not find Xgboo
-00002f10: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
-00002f20: 6967 2e20 4661 6c6c 696e 6720 6261 636b  ig. Falling back
-00002f30: 2074 6f20 6465 6661 756c 7473 2e72 3600   to defaults.r6.
-00002f40: 0000 72d5 0000 0072 0100 0000 727a 0000  ..r....r....rz..
-00002f50: 0072 3500 0000 da09 6f6f 665f 7363 6f72  .r5.....oof_scor
-00002f60: 6572 d000 0000 727c 0000 0029 2272 4d00  er....r|...)"rM.
-00002f70: 0000 7216 0000 0072 0b00 0000 7210 0000  ..r....r....r...
-00002f80: 0072 0a00 0000 724e 0000 00da 0965 6e75  .r....rN.....enu
-00002f90: 6d65 7261 7465 da05 7370 6c69 74da 0661  merate..split..a
-00002fa0: 7374 7970 65da 0369 6e74 da04 696c 6f63  stype..int..iloc
-00002fb0: 721a 0000 0072 4600 0000 7247 0000 0072  r....rF...rG...r
-00002fc0: 4f00 0000 729a 0000 0072 9b00 0000 7218  O...r....r....r.
-00002fd0: 0000 0072 0c00 0000 7217 0000 0072 2600  ...r....r....r&.
-00002fe0: 0000 7231 0000 0072 3800 0000 72d8 0000  ..r1...r8...r...
-00002ff0: 0072 d900 0000 72e3 0000 0072 0900 0000  .r....r....r....
-00003000: 721c 0000 0072 a500 0000 da07 6173 6172  r....r......asar
-00003010: 7261 7972 1900 0000 72a7 0000 0072 7d00  rayr....r....r}.
-00003020: 0000 72a8 0000 0029 1b72 2100 0000 72f4  ..r....).r!...r.
-00003030: 0000 0072 2900 0000 722b 0000 0072 2a00  ...r)...r+...r*.
-00003040: 0000 722c 0000 0072 6800 0000 7233 0000  ..r,...rh...r3..
-00003050: 00da 0a73 7472 6174 6966 6965 72da 0b66  ...stratifier..f
-00003060: 6f6c 645f 6c6f 7373 6573 da03 5f66 6eda  old_losses.._fn.
-00003070: 0774 726e 5f69 6478 da07 7661 6c5f 6964  .trn_idx..val_id
-00003080: 78da 0c58 5f74 7261 696e 5f66 6f6c 64da  x..X_train_fold.
-00003090: 0a58 5f76 616c 5f66 6f6c 64da 0c79 5f74  .X_val_fold..y_t
-000030a0: 7261 696e 5f66 6f6c 64da 0a79 5f76 616c  rain_fold..y_val
-000030b0: 5f66 6f6c 64da 0b58 5f74 6573 745f 666f  _fold..X_test_fo
-000030c0: 6c64 da0b 795f 7465 7374 5f66 6f6c 6472  ld..y_test_foldr
-000030d0: 5200 0000 7251 0000 0072 5300 0000 721b  R...rQ...rS...r.
-000030e0: 0000 0072 ec00 0000 72da 0000 005a 086d  ...r....r....Z.m
-000030f0: 7365 5f6d 6561 6e72 ae00 0000 7222 0000  se_meanr....r"..
-00003100: 0072 2200 0000 7223 0000 0072 a200 0000  .r"...r#...r....
-00003110: fa01 0000 73b0 0000 000c 0906 0208 0108  ....s...........
-00003120: 0102 0206 0102 0102 0106 fd04 0602 0110  ................
-00003130: 0110 ff08 0408 0106 fe08 0508 0106 fe06  ................
-00003140: 0406 0404 0102 ff02 fd02 0102 010c 0702  ................
-00003150: fd02 0102 0106 0506 0104 ff02 fd02 0104  ................
-00003160: 010a 0504 0202 0102 0106 0106 fd06 0608  ................
-00003170: 0102 0102 0104 ff04 0402 0102 0106 0106  ................
-00003180: fd10 0506 0208 0102 0102 0104 ff04 0302  ................
-00003190: 0102 0102 0106 0102 0106 0106 fa04 0802  ................
-000031a0: 0102 0106 0106 fd0a 0516 0110 020c 0210  ................
-000031b0: 0206 0110 0206 0102 0102 0104 0102 0102  ................
-000031c0: 0102 0102 0106 f904 097a 2958 6762 6f6f  .........z)Xgboo
-000031d0: 7374 4d6f 6465 6c52 6567 7265 7373 696f  stModelRegressio
-000031e0: 6e2e 5f66 696e 655f 7475 6e65 5f70 7265  n._fine_tune_pre
-000031f0: 6369 7365 6305 0000 0000 0000 0000 0000  cisec...........
-00003200: 000c 0000 000a 0000 0003 0000 0073 8802  .............s..
-00003210: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
-00003220: 8301 0100 8800 6a03 7215 8800 6a04 7215  ......j.r...j.r.
-00003230: 8800 6a05 7215 8800 6a06 7319 7407 6402  ..j.r...j.s.t.d.
-00003240: 8301 8201 8700 8701 8702 8703 8704 6605  ..............f.
-00003250: 6403 6404 8408 7d05 8800 a008 a100 0100  d.d...}.........
-00003260: 7409 8800 6a03 6a0a 6405 1900 740b 8302  t...j.j.d...t...
-00003270: 72a7 7409 8800 6a03 6a0a 6406 1900 740b  r.t...j.j.d...t.
-00003280: 8302 72a7 7409 8800 6a03 6a0a 6407 1900  ..r.t...j.j.d...
-00003290: 740b 8302 72a7 7409 8800 6a03 6a0a 6408  t...r.t...j.j.d.
-000032a0: 1900 740b 8302 72a7 740c 6a0d 8800 6a03  ..t...r.t.j...j.
-000032b0: 6a0a 6405 1900 6409 1400 8800 6a03 6a0a  j.d...d.....j.j.
-000032c0: 6405 1900 640a 1400 8800 6a04 6a0e 740b  d...d.....j.j.t.
-000032d0: 640b 8d04 740c 6a0d 8800 6a03 6a0a 6406  d...t.j...j.j.d.
-000032e0: 1900 6409 1400 8800 6a03 6a0a 6406 1900  ..d.....j.j.d...
-000032f0: 640a 1400 8800 6a04 6a0e 740b 640b 8d04  d.....j.j.t.d...
-00003300: 740c 6a0d 8800 6a03 6a0a 6407 1900 6409  t.j...j.j.d...d.
-00003310: 1400 8800 6a03 6a0a 6407 1900 640a 1400  ....j.j.d...d...
-00003320: 8800 6a04 6a0e 740b 640b 8d04 740c 6a0d  ..j.j.t.d...t.j.
-00003330: 8800 6a03 6a0a 6408 1900 6409 1400 8800  ..j.j.d...d.....
-00003340: 6a03 6a0a 6408 1900 640a 1400 8800 6a04  j.j.d...d.....j.
-00003350: 6a0e 740b 640b 8d04 640c 9c04 7d06 6e04  j.t.d...d...}.n.
-00003360: 7407 640d 8301 0100 8800 a00f a100 7d07  t.d...........}.
-00003370: 7410 6a11 640e 7410 6a12 a013 7c06 a101  t.j.d.t.j...|...
-00003380: 640f 8d02 7d08 7c08 6a14 7c05 8800 6a04  d...}.|.j.|...j.
-00003390: 6a0e 7415 7c06 a016 a100 8301 1300 8800  j.t.|...........
-000033a0: 6a04 6a17 6410 6410 6411 8d05 0100 7a16  j.j.d.d.d.....z.
-000033b0: 7410 6a18 a019 7c08 a101 7d09 7c09 a01a  t.j...|...}.|...
-000033c0: a100 0100 7410 6a18 a01b 7c08 a101 7d09  ....t.j...|...}.
-000033d0: 7c09 a01a a100 0100 5700 6e0c 0400 741c  |.......W.n...t.
-000033e0: 741d 7407 6603 79f0 0100 0100 0100 5900  t.t.f.y.......Y.
-000033f0: 6e01 7700 8800 a00f a100 7d0a 7c0a 7c07  n.w.......}.|.|.
-00003400: 6b00 73fe 8800 6a04 6a1e 9001 7338 7c08  k.s...j.j...s8|.
-00003410: 6a1f 6a0a 7d0b 7c0b 6405 1900 8800 6a03  j.j.}.|.d.....j.
-00003420: 6a0a 6405 3c00 7c0b 6406 1900 8800 6a03  j.d.<.|.d.....j.
-00003430: 6a0a 6406 3c00 7c0b 6407 1900 8800 6a03  j.d.<.|.d.....j.
-00003440: 6a0a 6407 3c00 7c0b 6408 1900 8800 6a03  j.d.<.|.d.....j.
-00003450: 6a0a 6408 3c00 7400 6412 7c07 9b00 6413  j.d.<.t.d.|...d.
-00003460: 7c0a 9b00 6414 9d05 8301 0100 7400 6415  |...d.......t.d.
-00003470: 8800 6a03 6a0a 9b00 9d02 8301 0100 6400  ..j.j.........d.
-00003480: 5300 7400 6416 7c07 9b00 6417 7c0a 9b00  S.t.d.|...d.|...
-00003490: 9d04 8301 0100 6400 5300 2918 4e7a 313a  ......d.S.).Nz1:
-000034a0: 2053 7461 7274 2067 7269 6420 7365 6172   Start grid sear
-000034b0: 6368 2066 696e 6520 7475 6e69 6e67 206f  ch fine tuning o
-000034c0: 6620 5867 626f 6f73 7420 6d6f 6465 6c2e  f Xgboost model.
-000034d0: 7255 0000 0063 0100 0000 0000 0000 0000  rU...c..........
-000034e0: 0000 0d00 0000 0b00 0000 1300 0000 73de  ..............s.
-000034f0: 0100 0088 00a0 0088 0288 0488 0188 03a1  ................
-00003500: 045c 027d 017d 0274 016a 02a0 037c 0064  .\.}.}.t.j...|.d
-00003510: 01a1 027d 0374 0488 006a 056a 0683 017d  ...}.t...j.j...}
-00003520: 047c 006a 0764 0288 006a 056a 0664 0219  .|.j.d...j.j.d..
-00003530: 0064 0314 0088 006a 056a 0664 0219 0064  .d.....j.j.d...d
-00003540: 0414 0064 0564 068d 047d 057c 006a 0764  ...d.d...}.|.j.d
-00003550: 0788 006a 056a 0664 0719 0064 0314 0088  ...j.j.d...d....
-00003560: 006a 056a 0664 0719 0064 0414 0064 0564  .j.j.d...d...d.d
-00003570: 068d 047d 067c 006a 0764 0888 006a 056a  ...}.|.j.d...j.j
-00003580: 0664 0819 0064 0314 0088 006a 056a 0664  .d...d.....j.j.d
-00003590: 0819 0064 0414 0064 0564 068d 047d 077c  ...d...d.d...}.|
-000035a0: 006a 0764 0988 006a 056a 0664 0919 0064  .j.d...j.j.d...d
-000035b0: 0314 0088 006a 056a 0664 0919 0064 0414  .....j.j.d...d..
-000035c0: 0064 0564 068d 047d 087c 057c 0464 023c  .d.d...}.|.|.d.<
-000035d0: 007c 067c 0464 073c 007c 077c 0464 083c  .|.|.d.<.|.|.d.<
-000035e0: 007c 087c 0464 093c 007c 04a0 0864 0a64  .|.|.d.<.|...d.d
-000035f0: 0ba1 027d 0988 006a 096a 0a64 0c6b 0272  ...}...j.j.d.k.r
-00003600: 9188 00a0 0b7c 017c 0288 037c 047c 097c  .....|.|...|.|.|
-00003610: 03a1 0653 0088 006a 096a 0a64 0c6b 0472  ...S...j.j.d.k.r
-00003620: a788 006a 096a 0c72 a788 00a0 0d7c 0488  ...j.j.r.....|..
-00003630: 0288 0488 0188 0388 006a 096a 0ea1 0653  .........j.j...S
-00003640: 0074 0f6a 107c 047c 017c 0988 006a 096a  .t.j.|.|.|...j.j
-00003650: 1188 006a 096a 0a64 0588 006a 096a 0e7c  ...j.j.d...j.j.|
-00003660: 0367 0188 006a 096a 1264 0d8d 097d 0a7c  .g...j.j.d...}.|
-00003670: 0a64 0e19 00a0 13a1 007c 0a64 0e19 00a0  .d.......|.d....
-00003680: 14a1 0064 0f13 0017 007d 0b74 1588 006a  ...d.....}.t...j
-00003690: 166a 1783 0164 106b 0272 d764 107d 0c6e  .j...d.k.r.d.}.n
-000036a0: 0888 006a 166a 1764 1119 0064 0c17 007d  ...j.j.d...d...}
-000036b0: 0c88 006a 166a 187c 0c64 1288 006a 097c  ...j.j.|.d...j.|
-000036c0: 047c 0b64 1364 1464 158d 0701 007c 0b53  .|.d.d.d.....|.S
-000036d0: 0029 164e 7267 0000 0072 5a00 0000 e7cd  .).Nrg...rZ.....
-000036e0: cccc cccc ccec 3fe7 9a99 9999 9999 f13f  ......?........?
-000036f0: 5472 5700 0000 725b 0000 0072 5c00 0000  TrW...r[...r\...
-00003700: 7256 0000 0072 3300 0000 7234 0000 0072  rV...r3...r4...r
-00003710: 3500 0000 7271 0000 0072 7800 0000 7279  5...rq...rx...ry
-00003720: 0000 0072 0100 0000 727a 0000 0072 7b00  ...r....rz...r{.
-00003730: 0000 72d0 0000 0046 727c 0000 0029 1972  ..r....Fr|...).r
-00003740: 4b00 0000 723d 0000 0072 9c00 0000 729d  K...r=...r....r.
-00003750: 0000 0072 0200 0000 7218 0000 0072 4c00  ...r....r....rL.
-00003760: 0000 7286 0000 0072 4d00 0000 7216 0000  ..r....rM...r...
-00003770: 0072 4e00 0000 729e 0000 0072 9f00 0000  .rN...r....r....
-00003780: 72a2 0000 0072 1f00 0000 724f 0000 0072  r....r....rO...r
-00003790: a300 0000 7238 0000 0072 a400 0000 72a5  ....r8...r....r.
-000037a0: 0000 0072 a600 0000 72a7 0000 0072 1900  ...r....r....r..
-000037b0: 0000 727d 0000 0072 a800 0000 290d 72a9  ..r}...r....).r.
-000037c0: 0000 0072 5100 0000 7252 0000 0072 ab00  ...rQ...rR...r..
-000037d0: 0000 72f4 0000 00da 0b61 6c70 6861 5f73  ..r......alpha_s
-000037e0: 7061 6365 da0c 6c61 6d62 6461 5f73 7061  pace..lambda_spa
-000037f0: 6365 da0b 6761 6d6d 615f 7370 6163 65da  ce..gamma_space.
-00003800: 0965 7461 5f73 7061 6365 7233 0000 0072  .eta_spacer3...r
-00003810: ac00 0000 72ad 0000 0072 ae00 0000 a905  ....r....r......
-00003820: 7221 0000 0072 2a00 0000 7229 0000 0072  r!...r*...r)...r
-00003830: 2c00 0000 722b 0000 0072 2200 0000 7223  ,...r+...r"...r#
-00003840: 0000 0072 6100 0000 7c02 0000 7398 0000  ...ra...|...s...
-00003850: 0014 0106 0204 0104 ff0c 0404 0102 010e  ................
-00003860: 010e 0102 0106 fc04 0602 010e 010e 0102  ................
-00003870: 0106 fc04 0602 010e 010e 0102 0106 fc04  ................
-00003880: 0602 010e 010e 0102 0106 fc08 0708 0108  ................
-00003890: 0108 010c 020c 0204 010c 0104 ff0c 0406  ................
-000038a0: 0102 ff04 0302 0102 0102 0102 0102 0106  ................
-000038b0: 0104 fa04 0902 0102 0102 0106 0106 0102  ................
-000038c0: 0106 0104 0106 0106 f70a 0c0e 0104 ff10  ................
-000038d0: 0506 0110 0206 0102 0102 0104 0102 0102  ................
-000038e0: 0102 0102 0106 f904 0a7a 3358 6762 6f6f  .........z3Xgboo
-000038f0: 7374 4d6f 6465 6c52 6567 7265 7373 696f  stModelRegressio
-00003900: 6e2e 6669 6e65 5f74 756e 652e 3c6c 6f63  n.fine_tune.<loc
-00003910: 616c 733e 2e6f 626a 6563 7469 7665 725a  als>.objectiverZ
-00003920: 0000 0072 5b00 0000 725c 0000 0072 5600  ...r[...r\...rV.
-00003930: 0000 7209 0100 0072 0a01 0000 2901 da05  ..r....r....)...
-00003940: 6474 7970 6529 0472 5a00 0000 725b 0000  dtype).rZ...r[..
-00003950: 0072 5c00 0000 7256 0000 007a 2953 6f6d  .r\...rV...z)Som
-00003960: 6520 7061 7261 6d65 7465 7273 2061 7265  e parameters are
-00003970: 206e 6f74 2066 6c6f 6174 7320 6f72 2073   not floats or s
-00003980: 7472 696e 6773 72b4 0000 0029 0272 b500  tringsr....).r..
-00003990: 0000 72b6 0000 0054 72b8 0000 007a 2647  ..r....Tr....z&G
-000039a0: 7269 6420 7365 6172 6368 2069 6d70 726f  rid search impro
-000039b0: 7665 6420 6576 616c 206d 6574 7269 6320  ved eval metric 
-000039c0: 6672 6f6d 207a 0420 746f 20da 012e 72bd  from z. to ...r.
-000039d0: 0000 007a 2d47 7269 6420 7365 6172 6368  ...z-Grid search
-000039e0: 2063 6f75 6c64 206e 6f74 2069 6d70 726f   could not impro
-000039f0: 7665 2065 7661 6c20 6d65 7472 6963 206f  ve eval metric o
-00003a00: 6620 7a19 2e20 4265 7374 2073 636f 7265  f z.. Best score
-00003a10: 2072 6561 6368 6564 2077 6173 2029 2072   reached was ) r
-00003a20: 1000 0000 7203 0000 0072 2500 0000 7218  ....r....r%...r.
-00003a30: 0000 0072 1600 0000 7217 0000 0072 1900  ...r....r....r..
-00003a40: 0000 723b 0000 0072 2800 0000 da0a 6973  ..r;...r(.....is
-00003a50: 696e 7374 616e 6365 724c 0000 00da 0566  instancerL.....f
-00003a60: 6c6f 6174 721c 0000 00da 086c 696e 7370  loatr......linsp
-00003a70: 6163 65da 2167 7269 6473 6561 7263 685f  ace.!gridsearch_
-00003a80: 6e62 5f70 6172 616d 6574 6572 735f 7065  nb_parameters_pe
-00003a90: 725f 6772 6964 72d2 0000 0072 3d00 0000  r_gridr....r=...
-00003aa0: 72c1 0000 0072 be00 0000 da0b 4772 6964  r....r......Grid
-00003ab0: 5361 6d70 6c65 7272 c200 0000 72a7 0000  Samplerr....r...
-00003ac0: 00da 046b 6579 73da 2267 7269 6473 6561  ...keys."gridsea
-00003ad0: 7263 685f 7475 6e69 6e67 5f6d 6178 5f72  rch_tuning_max_r
-00003ae0: 756e 7469 6d65 5f73 6563 7372 c500 0000  untime_secsr....
-00003af0: 72c6 0000 0072 c700 0000 72c8 0000 0072  r....r....r....r
-00003b00: c900 0000 72ca 0000 0072 4100 0000 72cb  ....r....rA...r.
-00003b10: 0000 0029 0c72 2100 0000 7229 0000 0072  ...).r!...r)...r
-00003b20: 2a00 0000 722b 0000 0072 2c00 0000 7261  *...r+...r,...ra
-00003b30: 0000 00da 0c73 6561 7263 685f 7370 6163  .....search_spac
-00003b40: 65da 0d62 6573 745f 7363 6f72 655f 6376  e..best_score_cv
-00003b50: 72cd 0000 0072 ce00 0000 72d4 0000 00da  r....r....r.....
-00003b60: 1778 6762 6f6f 7374 5f67 7269 645f 6265  .xgboost_grid_be
-00003b70: 7374 5f70 6172 616d 7222 0000 0072 0f01  st_paramr"...r..
-00003b80: 0000 7223 0000 0072 4500 0000 6a02 0000  ..r#...rE...j...
-00003b90: 73ae 0000 0012 0704 0202 ff04 0202 fe04  s...............
-00003ba0: 0302 fd04 0402 fc02 0602 0104 ff14 0408  ................
-00003bb0: 5a10 0202 ff10 0202 fe10 0302 fd10 0402  Z...............
-00003bc0: fc04 070a 0102 0102 ff0e 0206 0102 0104  ................
-00003bd0: fb04 070e 010e 0106 0102 0104 fc04 060e  ................
-00003be0: 010e 0106 0102 0104 fc04 060e 010e 0106  ................
-00003bf0: 0102 0104 fc08 ec08 1c08 0204 020c 0106  ................
-00003c00: ff04 0302 0106 010a 0102 ff06 0202 0102  ................
-00003c10: 0106 fa02 090c 0108 010c 010c 0112 0104  ................
-00003c20: 0102 ff08 0312 0208 0110 0102 0102 010c  ................
-00003c30: ff10 0310 0102 0110 0104 ff16 0302 020e  ................
-00003c40: 0108 ff7a 2058 6762 6f6f 7374 4d6f 6465  ...z XgboostMode
-00003c50: 6c52 6567 7265 7373 696f 6e2e 6669 6e65  lRegression.fine
-00003c60: 5f74 756e 65da 0264 6663 0200 0000 0000  _tune..dfc......
-00003c70: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-00003c80: 0000 7388 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
-00003c90: 0064 019d 0283 0101 007c 006a 0372 0f7c  .d.......|.j.r.|
-00003ca0: 006a 0473 1374 0564 0283 0182 017c 006a  .j.s.t.d.....|.j
-00003cb0: 0672 217c 006a 066a 077c 0164 0364 0464  .r!|.j.j.|.d.d.d
-00003cc0: 058d 035c 027d 017d 0274 086a 097c 017c  ...\.}.}.t.j.|.|
-00003cd0: 006a 046a 0a64 068d 027d 037c 006a 0b73  .j.j.d...}.|.j.s
-00003ce0: 3174 0c64 0783 0182 017c 006a 0d73 3874  1t.d.....|.j.s8t
-00003cf0: 0c64 0883 0182 017c 006a 0ba0 0e7c 03a1  .d.....|.j...|..
-00003d00: 017d 0474 0064 0983 0101 007c 0453 0029  .}.t.d.....|.S.)
-00003d10: 0a7a 1750 7265 6469 6374 206f 6e20 756e  .z.Predict on un
-00003d20: 7365 656e 2064 6174 612e 7a33 3a20 5374  seen data.z3: St
-00003d30: 6172 7420 7072 6564 6963 7469 6e67 206f  art predicting o
-00003d40: 6e20 6e65 7720 6461 7461 2075 7369 6e67  n new data using
-00003d50: 2058 6762 6f6f 7374 206d 6f64 656c 2e7a   Xgboost model.z
-00003d60: 2c63 6f6e 665f 7061 7261 6d73 5f78 6762  ,conf_params_xgb
-00003d70: 6f6f 7374 206f 7220 636f 6e66 5f74 7261  oost or conf_tra
-00003d80: 696e 696e 6720 6973 204e 6f6e 654e 5472  ining is NoneNTr
-00003d90: 2f00 0000 2901 7266 0000 007a 204e 6f20  /...).rf...z No 
-00003da0: 7472 6169 6e65 6420 6d6f 6465 6c20 6861  trained model ha
-00003db0: 7320 6265 656e 2066 6f75 6e64 2e7a 2b4e  s been found.z+N
-00003dc0: 6f20 6d6f 6465 6c20 636f 6e66 6967 7572  o model configur
-00003dd0: 6174 696f 6e20 6669 6c65 2068 6173 2062  ation file has b
-00003de0: 6565 6e20 666f 756e 642e 7a13 4669 6e69  een found.z.Fini
-00003df0: 7368 6564 2070 7265 6469 6374 696e 6729  shed predicting)
-00003e00: 0f72 1000 0000 7203 0000 0072 2500 0000  .r....r....r%...
-00003e10: 7217 0000 0072 1600 0000 723b 0000 0072  r....r....r;...r
-00003e20: 1a00 0000 7247 0000 0072 4f00 0000 729a  ....rG...rO...r.
-00003e30: 0000 0072 9b00 0000 721b 0000 00da 0945  ...r....r......E
-00003e40: 7863 6570 7469 6f6e 7218 0000 0072 d900  xceptionr....r..
-00003e50: 0000 2905 7221 0000 0072 1c01 0000 da01  ..).r!...r......
-00003e60: 5f72 5200 0000 72da 0000 0072 2200 0000  _rR...r....r"...
-00003e70: 7222 0000 0072 2300 0000 72d9 0000 0024  r"...r#...r....$
-00003e80: 0300 0073 2800 0000 0202 0c01 04ff 0c03  ...s(...........
-00003e90: 0801 0602 0601 0601 0aff 0404 0201 0601  ................
-00003ea0: 06fe 0605 0801 0602 0801 0c02 0801 0401  ................
-00003eb0: 7a1e 5867 626f 6f73 744d 6f64 656c 5265  z.XgboostModelRe
-00003ec0: 6772 6573 7369 6f6e 2e70 7265 6469 6374  gression.predict
-00003ed0: 2905 4e4e 4e4e 4e29 0172 7000 0000 2924  ).NNNNN).rp...)$
-00003ee0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00003ef0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00003f00: 6d65 5f5f da07 5f5f 646f 635f 5f72 0700  me__..__doc__r..
-00003f10: 0000 7208 0000 0072 0b00 0000 7226 0000  ..r....r....r&..
-00003f20: 0072 0c00 0000 720e 0000 0072 1200 0000  .r....r....r....
-00003f30: 7224 0000 0072 2800 0000 7249 0000 00da  r$...r(...rI....
-00003f40: 0944 6174 6146 7261 6d65 da06 5365 7269  .DataFrame..Seri
-00003f50: 6573 724f 0000 00da 0742 6f6f 7374 6572  esrO.....Booster
-00003f60: 7254 0000 0072 4200 0000 72d2 0000 0072  rT...rB...r....r
-00003f70: 4b00 0000 729e 0000 0072 fb00 0000 72ee  K...r....r....r.
-00003f80: 0000 0072 0600 0000 7213 0100 0072 f300  ...r....r....r..
-00003f90: 0000 7205 0000 00da 0373 7472 7204 0000  ..r......strr...
-00003fa0: 0072 a200 0000 7245 0000 0072 1c00 0000  .r....rE...r....
-00003fb0: da07 6e64 6172 7261 7972 d900 0000 7222  ..ndarrayr....r"
-00003fc0: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00003fd0: 0000 7213 0000 001d 0000 0073 a400 0000  ..r........s....
-00003fe0: 0800 0401 0205 0201 0201 0201 0201 04f9  ................
-00003ff0: 0602 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-00004000: 0606 02fa 0607 0af9 0818 0215 0402 02fe  ................
-00004010: 0403 02fd 0404 02fc 0405 02fb 0406 0afa  ................
-00004020: 024a 0402 02fe 0403 02fd 0404 02fc 0405  .J..............
-00004030: 02fb 0206 0afa 007f 0863 0813 080d 0221  .........c.....!
-00004040: 04ff 0401 02ff 0401 02ff 0201 0aff 1624  ...............$
-00004050: 021d 0a02 02fe 0403 02fd 0404 02fc 0405  ................
-00004060: 02fb 0406 02fa 0207 0af9 0270 0402 02fe  ...........p....
-00004070: 0403 02fd 0404 02fc 0405 02fb 0206 0afa  ................
-00004080: 007f 1a3b 7213 0000 0029 2472 2201 0000  ...;r....)$r"...
-00004090: da04 636f 7079 7202 0000 0072 0300 0000  ..copyr....r....
-000040a0: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
-000040b0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000040c0: 00da 056e 756d 7079 721c 0000 0072 3d00  ...numpyr....r=.
-000040d0: 0000 da06 7061 6e64 6173 7249 0000 0072  ....pandasrI...r
-000040e0: b100 0000 724f 0000 00da 0f73 6b6c 6561  ....rO.....sklea
-000040f0: 726e 2e6d 6574 7269 6373 7209 0000 00da  rn.metricsr.....
-00004100: 1773 6b6c 6561 726e 2e6d 6f64 656c 5f73  .sklearn.model_s
-00004110: 656c 6563 7469 6f6e 720a 0000 00da 1f62  electionr......b
-00004120: 6c75 6563 6173 742e 636f 6e66 6967 2e74  luecast.config.t
-00004130: 7261 696e 696e 675f 636f 6e66 6967 720b  raining_configr.
-00004140: 0000 0072 0c00 0000 720d 0000 0072 2600  ...r....r....r&.
-00004150: 0000 da21 626c 7565 6361 7374 2e65 7870  ...!bluecast.exp
-00004160: 6572 696d 656e 7461 7469 6f6e 2e74 7261  erimentation.tra
-00004170: 636b 696e 6772 0e00 0000 da24 626c 7565  ckingr.....$blue
-00004180: 6361 7374 2e67 656e 6572 616c 5f75 7469  cast.general_uti
-00004190: 6c73 2e67 656e 6572 616c 5f75 7469 6c73  ls.general_utils
-000041a0: 720f 0000 0072 1000 0000 da22 626c 7565  r....r....."blue
-000041b0: 6361 7374 2e6d 6c5f 6d6f 6465 6c6c 696e  cast.ml_modellin
-000041c0: 672e 6261 7365 5f63 6c61 7373 6573 7211  g.base_classesr.
-000041d0: 0000 00da 1d62 6c75 6563 6173 742e 7072  .....bluecast.pr
-000041e0: 6570 726f 6365 7373 696e 672e 6375 7374  eprocessing.cust
-000041f0: 6f6d 7212 0000 0072 1300 0000 7222 0000  omr....r....r"..
-00004200: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-00004210: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
-00004220: 0000 0004 000c 070c 011c 0108 0208 0108  ................
-00004230: 0108 010c 010c 0110 020c 010c 0310 010c  ................
-00004240: 010c 0114 03                             .....
+000000d0: 6d1e 5a1e 6d1f 5a1f 0100 6401 640c 6c20  m.Z.m.Z...d.d.l 
+000000e0: 6d21 5a21 0100 6401 640d 6c22 6d23 5a23  m!Z!..d.d.l"m#Z#
+000000f0: 0100 4700 640e 640f 8400 640f 6521 8303  ..G.d.d...d.e!..
+00000100: 5a24 6405 5300 2910 6119 0100 0058 6762  Z$d.S.).a....Xgb
+00000110: 6f6f 7374 2063 6c61 7373 6966 6963 6174  oost classificat
+00000120: 696f 6e20 6d6f 6465 6c2e 0a0a 5468 6973  ion model...This
+00000130: 206d 6f64 756c 6520 636f 6e74 6169 6e73   module contains
+00000140: 2061 2077 7261 7070 6572 2066 6f72 2074   a wrapper for t
+00000150: 6865 2058 6762 6f6f 7374 2063 6c61 7373  he Xgboost class
+00000160: 6966 6963 6174 696f 6e20 6d6f 6465 6c2e  ification model.
+00000170: 2049 7420 6361 6e20 6265 2075 7365 6420   It can be used 
+00000180: 746f 2074 7261 696e 2061 6e64 2f6f 7220  to train and/or 
+00000190: 7475 6e65 2074 6865 206d 6f64 656c 2e0a  tune the model..
+000001a0: 4974 2061 6c73 6f20 6361 6c63 756c 6174  It also calculat
+000001b0: 6573 2063 6c61 7373 2077 6569 6768 7473  es class weights
+000001c0: 2066 6f72 2069 6d62 616c 616e 6365 6420   for imbalanced 
+000001d0: 6461 7461 7365 7473 2e20 5468 6520 7765  datasets. The we
+000001e0: 6967 6874 7320 6d61 7920 6f72 206d 6179  ights may or may
+000001f0: 206e 6f74 2062 6520 7573 6564 2064 6565   not be used dee
+00000200: 7065 6e64 696e 6720 6f6e 2074 6865 0a68  pending on the.h
+00000210: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
+00000220: 6e69 6e67 2e0a e900 0000 0029 01da 0864  ning.......)...d
+00000230: 6565 7063 6f70 7929 01da 0864 6174 6574  eepcopy)...datet
+00000240: 696d 6529 05da 0341 6e79 da04 4469 6374  ime)...Any..Dict
+00000250: da04 4c69 7374 da07 4c69 7465 7261 6cda  ..List..Literal.
+00000260: 084f 7074 696f 6e61 6c4e 2901 da12 6d65  .OptionalN)...me
+00000270: 616e 5f73 7175 6172 6564 5f65 7272 6f72  an_squared_error
+00000280: 2901 da05 4b46 6f6c 6429 02da 0e54 7261  )...KFold)...Tra
+00000290: 696e 696e 6743 6f6e 6669 67da 1758 6762  iningConfig..Xgb
+000002a0: 6f6f 7374 4669 6e61 6c50 6172 616d 436f  oostFinalParamCo
+000002b0: 6e66 6967 2901 da21 5867 626f 6f73 7454  nfig)..!XgboostT
+000002c0: 756e 6550 6172 616d 7352 6567 7265 7373  uneParamsRegress
+000002d0: 696f 6e43 6f6e 6669 6729 01da 1145 7870  ionConfig)...Exp
+000002e0: 6572 696d 656e 7454 7261 636b 6572 2903  erimentTracker).
+000002f0: da11 6368 6563 6b5f 6770 755f 7375 7070  ..check_gpu_supp
+00000300: 6f72 74da 0c6c 6f67 5f73 616d 706c 696e  ort..log_samplin
+00000310: 67da 066c 6f67 6765 7229 01da 1a42 6173  g..logger)...Bas
+00000320: 6543 6c61 7373 4d6c 5265 6772 6573 7369  eClassMlRegressi
+00000330: 6f6e 4d6f 6465 6c29 01da 1343 7573 746f  onModel)...Custo
+00000340: 6d50 7265 7072 6f63 6573 7369 6e67 6300  mPreprocessingc.
+00000350: 0000 0000 0000 0000 0000 0000 0000 000e  ................
+00000360: 0000 0040 0000 0073 6201 0000 6500 5a01  ...@...sb...e.Z.
+00000370: 6400 5a02 6401 5a03 0902 0902 0902 0902  d.Z.d.Z.........
+00000380: 0902 642e 6403 6504 6404 1900 6405 6505  ..d.d.e.d...d.e.
+00000390: 6506 1900 6406 6505 6507 1900 6407 6505  e...d.e.e...d.e.
+000003a0: 6508 1900 6408 6505 6509 1900 6409 6505  e...d.e.e...d.e.
+000003b0: 650a 1900 660c 640a 640b 8405 5a0b 640c  e...f.d.d...Z.d.
+000003c0: 640d 8400 5a0c 640e 650d 6a0e 640f 650d  d...Z.d.e.j.d.e.
+000003d0: 6a0e 6410 650d 6a0f 6411 650d 6a0f 6412  j.d.e.j.d.e.j.d.
+000003e0: 6510 6a11 660a 6413 6414 8404 5a12 640e  e.j.f.d.d...Z.d.
+000003f0: 650d 6a0e 640f 650d 6a0e 6410 650d 6a0f  e.j.d.e.j.d.e.j.
+00000400: 6411 650d 6a0f 6412 6402 660a 6415 6416  d.e.j.d.d.f.d.d.
+00000410: 8404 5a13 6417 6418 8400 5a14 6419 641a  ..Z.d.d...Z.d.d.
+00000420: 8400 5a15 641b 641c 8400 5a16 091d 642f  ..Z.d.d...Z...d/
+00000430: 641e 650d 6a0e 641f 650d 6a0f 6420 6517  d.e.j.d.e.j.d e.
+00000440: 6606 6421 6422 8405 5a18 6423 6519 651a  f.d!d"..Z.d#e.e.
+00000450: 1900 6412 651a 6604 6424 6425 8404 5a1b  ..d.e.f.d$d%..Z.
+00000460: 6426 651c 651d 651e 6602 1900 640e 650d  d&e.e.e.f...d.e.
+00000470: 6a0e 6410 650d 6a0f 640f 650d 6a0e 6411  j.d.e.j.d.e.j.d.
+00000480: 650d 6a0f 660a 6427 6428 8404 5a1f 640e  e.j.f.d'd(..Z.d.
+00000490: 650d 6a0e 640f 650d 6a0e 6410 650d 6a0f  e.j.d.e.j.d.e.j.
+000004a0: 6411 650d 6a0f 6412 6402 660a 6429 642a  d.e.j.d.d.f.d)d*
+000004b0: 8404 5a20 642b 650d 6a0e 6412 6521 6a22  ..Z d+e.j.d.e!j"
+000004c0: 6604 642c 642d 8404 5a23 6402 5300 2930  f.d,d-..Z#d.S.)0
+000004d0: da16 5867 626f 6f73 744d 6f64 656c 5265  ..XgboostModelRe
+000004e0: 6772 6573 7369 6f6e 7a2b 5472 6169 6e20  gressionz+Train 
+000004f0: 616e 642f 6f72 2074 756e 6520 5867 626f  and/or tune Xgbo
+00000500: 6f73 7420 7265 6772 6573 7369 6f6e 206d  ost regression m
+00000510: 6f64 656c 2e4e da0d 636c 6173 735f 7072  odel.N..class_pr
+00000520: 6f62 6c65 6dda 0a72 6567 7265 7373 696f  oblem..regressio
+00000530: 6eda 0d63 6f6e 665f 7472 6169 6e69 6e67  n..conf_training
+00000540: da0c 636f 6e66 5f78 6762 6f6f 7374 da13  ..conf_xgboost..
+00000550: 636f 6e66 5f70 6172 616d 735f 7867 626f  conf_params_xgbo
+00000560: 6f73 74da 1265 7870 6572 696d 656e 745f  ost..experiment_
+00000570: 7472 6163 6b65 72da 1b63 7573 746f 6d5f  tracker..custom_
+00000580: 696e 5f66 6f6c 645f 7072 6570 726f 6365  in_fold_preproce
+00000590: 7373 6f72 6307 0000 0000 0000 0000 0000  ssorc...........
+000005a0: 0007 0000 0003 0000 0043 0000 0073 5800  .........C...sX.
+000005b0: 0000 6400 7c00 5f00 7c01 7c00 5f01 7c02  ..d.|._.|.|._.|.
+000005c0: 7c00 5f02 7c04 7c00 5f03 7c03 7c00 5f04  |._.|.|._.|.|._.
+000005d0: 7c05 7c00 5f05 7c06 7c00 5f06 7c00 6a02  |.|._.|.|._.|.j.
+000005e0: 7223 7407 6a08 a009 7c00 6a02 6a0a a101  r#t.j...|.j.j...
+000005f0: 7c00 5f0b 6400 5300 7407 6a08 a009 6401  |._.d.S.t.j...d.
+00000600: a101 7c00 5f0b 6400 5300 2902 4e72 0100  ..|._.d.S.).Nr..
+00000610: 0000 290c da05 6d6f 6465 6c72 1500 0000  ..)...modelr....
+00000620: 7217 0000 0072 1900 0000 7218 0000 0072  r....r....r....r
+00000630: 1a00 0000 721b 0000 00da 026e 70da 0672  ....r......np..r
+00000640: 616e 646f 6dda 0b64 6566 6175 6c74 5f72  andom..default_r
+00000650: 6e67 da13 676c 6f62 616c 5f72 616e 646f  ng..global_rando
+00000660: 6d5f 7374 6174 65da 1072 616e 646f 6d5f  m_state..random_
+00000670: 6765 6e65 7261 746f 7229 07da 0473 656c  generator)...sel
+00000680: 6672 1500 0000 7217 0000 0072 1800 0000  fr....r....r....
+00000690: 7219 0000 0072 1a00 0000 721b 0000 00a9  r....r....r.....
+000006a0: 0072 2300 0000 fa4e 2f68 6f6d 652f 7468  .r#....N/home/th
+000006b0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
+000006c0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
+000006d0: 6173 742f 6d6c 5f6d 6f64 656c 6c69 6e67  ast/ml_modelling
+000006e0: 2f78 6762 6f6f 7374 5f72 6567 7265 7373  /xgboost_regress
+000006f0: 696f 6e2e 7079 da08 5f5f 696e 6974 5f5f  ion.py..__init__
+00000700: 2000 0000 7318 0000 0006 0906 0106 0106   ...s...........
+00000710: 0106 0106 0206 0106 0106 0106 010a ff12  ................
+00000720: 047a 1f58 6762 6f6f 7374 4d6f 6465 6c52  .z.XgboostModelR
+00000730: 6567 7265 7373 696f 6e2e 5f5f 696e 6974  egression.__init
+00000740: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000750: 0000 0003 0000 0043 0000 0073 b400 0000  .......C...s....
+00000760: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
+00000770: 0100 7c00 6a03 731a 7404 8300 7c00 5f03  ..|.j.s.t...|._.
+00000780: 7400 7401 a002 a100 9b00 6402 9d02 8301  t.t.......d.....
+00000790: 0100 6e09 7400 7401 a002 a100 9b00 6403  ..n.t.t.......d.
+000007a0: 9d02 8301 0100 7c00 6a05 7334 7406 8300  ......|.j.s4t...
+000007b0: 7c00 5f05 7400 7401 a002 a100 9b00 6404  |._.t.t.......d.
+000007c0: 9d02 8301 0100 6e09 7400 7401 a002 a100  ......n.t.t.....
+000007d0: 9b00 6405 9d02 8301 0100 7c00 6a07 734f  ..d.......|.j.sO
+000007e0: 7408 8300 7c00 5f07 7400 7401 a002 a100  t...|._.t.t.....
+000007f0: 9b00 6406 9d02 8301 0100 6408 5300 7400  ..d.......d.S.t.
+00000800: 7401 a002 a100 9b00 6407 9d02 8301 0100  t.......d.......
+00000810: 6408 5300 2909 7a36 4c6f 6164 206d 756c  d.S.).z6Load mul
+00000820: 7469 706c 6520 636f 6e66 6967 7320 6f72  tiple configs or
+00000830: 206c 6f61 6420 6465 6661 756c 7420 636f   load default co
+00000840: 6e66 6967 7320 696e 7374 6561 642e 7a32  nfigs instead.z2
+00000850: 3a20 5374 6172 7420 6c6f 6164 696e 6720  : Start loading 
+00000860: 6578 6973 7469 6e67 206f 7220 6465 6661  existing or defa
+00000870: 756c 7420 636f 6e66 6967 2066 696c 6573  ult config files
+00000880: 2e2e 7a1e 3a20 4c6f 6164 2064 6566 6175  ..z.: Load defau
+00000890: 6c74 2054 7261 696e 696e 6743 6f6e 6669  lt TrainingConfi
+000008a0: 672e 7a20 3a20 466f 756e 6420 7072 6f76  g.z : Found prov
+000008b0: 6964 6564 2054 7261 696e 696e 6743 6f6e  ided TrainingCon
+000008c0: 6669 672e 7a27 3a20 4c6f 6164 2064 6566  fig.z': Load def
+000008d0: 6175 6c74 2058 6762 6f6f 7374 5475 6e65  ault XgboostTune
+000008e0: 5061 7261 6d73 436f 6e66 6967 2e7a 293a  ParamsConfig.z):
+000008f0: 2046 6f75 6e64 2070 726f 7669 6465 6420   Found provided 
+00000900: 5867 626f 6f73 7454 756e 6550 6172 616d  XgboostTuneParam
+00000910: 7343 6f6e 6669 672e 7a27 3a20 4c6f 6164  sConfig.z': Load
+00000920: 2064 6566 6175 6c74 2058 6762 6f6f 7374   default Xgboost
+00000930: 4669 6e61 6c50 6172 616d 436f 6e66 6967  FinalParamConfig
+00000940: 2e7a 293a 2046 6f75 6e64 2070 726f 7669  .z): Found provi
+00000950: 6465 6420 5867 626f 6f73 7446 696e 616c  ded XgboostFinal
+00000960: 5061 7261 6d43 6f6e 6669 672e 4e29 0972  ParamConfig.N).r
+00000970: 1100 0000 7203 0000 00da 0675 7463 6e6f  ....r......utcno
+00000980: 7772 1700 0000 720b 0000 0072 1800 0000  wr....r....r....
+00000990: da17 5867 626f 6f73 7454 756e 6550 6172  ..XgboostTunePar
+000009a0: 616d 7343 6f6e 6669 6772 1900 0000 720c  amsConfigr....r.
+000009b0: 0000 0029 0172 2200 0000 7223 0000 0072  ...).r"...r#...r
+000009c0: 2300 0000 7224 0000 00da 1063 6865 636b  #...r$.....check
+000009d0: 5f6c 6f61 645f 636f 6e66 7338 0000 0073  _load_confs8...s
+000009e0: 1a00 0000 1202 0601 0801 1401 1202 0602  ................
+000009f0: 0801 1401 1202 0602 0801 1601 1602 7a27  ..............z'
+00000a00: 5867 626f 6f73 744d 6f64 656c 5265 6772  XgboostModelRegr
+00000a10: 6573 7369 6f6e 2e63 6865 636b 5f6c 6f61  ession.check_loa
+00000a20: 645f 636f 6e66 73da 0778 5f74 7261 696e  d_confs..x_train
+00000a30: da06 785f 7465 7374 da07 795f 7472 6169  ..x_test..y_trai
+00000a40: 6eda 0679 5f74 6573 74da 0672 6574 7572  n..y_test..retur
+00000a50: 6e63 0500 0000 0000 0000 0000 0000 0900  nc..............
+00000a60: 0000 0800 0000 4300 0000 739c 0100 0074  ......C...s....t
+00000a70: 0074 01a0 02a1 009b 0064 019d 0283 0101  .t.......d......
+00000a80: 007c 00a0 03a1 0001 007c 006a 0472 167c  .|.......|.j.r.|
+00000a90: 006a 0572 167c 006a 0673 1a74 0764 0283  .j.r.|.j.s.t.d..
+00000aa0: 0182 017c 006a 056a 0873 2674 096a 0aa0  ...|.j.j.s&t.j..
+00000ab0: 0b74 096a 0a6a 0ca1 0101 007c 006a 056a  .t.j.j.....|.j.j
+00000ac0: 0d72 367c 00a0 0e7c 017c 027c 037c 04a1  .r6|...|.|.|.|..
+00000ad0: 0401 0074 0f64 0383 0101 007c 006a 056a  ...t.d.....|.j.j
+00000ae0: 1072 467c 00a0 117c 017c 027c 037c 04a1  .rF|...|.|.|.|..
+00000af0: 0401 0074 0f64 0483 0101 0074 0064 0583  ...t.d.....t.d..
+00000b00: 0101 007c 006a 1272 617c 006a 12a0 137c  ...|.j.ra|.j...|
+00000b10: 017c 03a1 025c 027d 017d 037c 006a 126a  .|...\.}.}.|.j.j
+00000b20: 147c 027c 0464 0664 078d 035c 027d 027d  .|.|.d.d...\.}.}
+00000b30: 047c 006a 056a 1572 7c74 0074 01a0 02a1  .|.j.j.r|t.t....
+00000b40: 009b 0064 089d 0283 0101 0074 16a0 177c  ...d.......t...|
+00000b50: 017c 0267 02a1 017d 0174 16a0 177c 037c  .|.g...}.t...|.|
+00000b60: 0467 02a1 017d 037c 00a0 187c 017c 037c  .g...}.|...|.|.|
+00000b70: 027c 04a1 045c 027d 057d 067c 0564 0966  .|...\.}.}.|.d.f
+00000b80: 027c 0664 0a66 0267 027d 077c 006a 046a  .|.d.f.g.}.|.j.j
+00000b90: 19a0 1a64 0b64 0ca1 027d 087c 006a 056a  ...d.d...}.|.j.j
+00000ba0: 1b64 0d6b 0272 b27c 006a 1c72 b274 1d6a  .d.k.r.|.j.r.t.j
+00000bb0: 1e7c 006a 046a 197c 057c 087c 006a 056a  .|.j.j.|.|.|.j.j
+00000bc0: 1f7c 077c 006a 1c6a 2064 0e8d 067c 005f  .|.|.j.j d...|._
+00000bd0: 216e 157c 006a 1c72 c774 1d6a 1e7c 006a  !n.|.j.r.t.j.|.j
+00000be0: 046a 197c 057c 087c 006a 056a 1f7c 077c  .j.|.|.|.j.j.|.|
+00000bf0: 006a 1c6a 2064 0e8d 067c 005f 2174 0064  .j.j d...|._!t.d
+00000c00: 0f83 0101 007c 006a 2153 0029 107a 3f54  .....|.j!S.).z?T
+00000c10: 7261 696e 2058 6762 6f6f 7374 206d 6f64  rain Xgboost mod
+00000c20: 656c 2e20 496e 636c 7564 6573 2068 7970  el. Includes hyp
+00000c30: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
+00000c40: 6e67 206f 6e20 6465 6661 756c 742e 7a1e  ng on default.z.
+00000c50: 3a20 5374 6172 7420 6669 7474 696e 6720  : Start fitting 
+00000c60: 5867 626f 6f73 7420 6d6f 6465 6c2e fa40  Xgboost model..@
+00000c70: 636f 6e66 5f70 6172 616d 735f 7867 626f  conf_params_xgbo
+00000c80: 6f73 742c 2063 6f6e 665f 7472 6169 6e69  ost, conf_traini
+00000c90: 6e67 206f 7220 6578 7065 7269 6d65 6e74  ng or experiment
+00000ca0: 5f74 7261 636b 6572 2069 7320 4e6f 6e65  _tracker is None
+00000cb0: 7a1e 4669 6e69 7368 6564 2068 7970 6572  z.Finished hyper
+00000cc0: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
+00000cd0: 7a20 4669 6e69 7368 6564 2047 7269 6420  z Finished Grid 
+00000ce0: 7365 6172 6368 2066 696e 6520 7475 6e69  search fine tuni
+00000cf0: 6e67 7a1a 5374 6172 7420 6669 6e61 6c20  ngz.Start final 
+00000d00: 6d6f 6465 6c20 7472 6169 6e69 6e67 46a9  model trainingF.
+00000d10: 01da 0e70 7265 6469 6374 6f6e 5f6d 6f64  ...predicton_mod
+00000d20: 657a 7f3a 2055 6e69 6f6e 2074 7261 696e  ez.: Union train
+00000d30: 2061 6e64 2074 6573 7420 6461 7461 2066   and test data f
+00000d40: 6f72 2066 696e 616c 206d 6f64 656c 2074  or final model t
+00000d50: 7261 696e 696e 6720 6261 7365 6420 6f6e  raining based on
+00000d60: 2054 7261 696e 696e 6743 6f6e 6669 670a   TrainingConfig.
+00000d70: 2020 2020 2020 2020 2020 2020 2070 6172               par
+00000d80: 616d 2027 7573 655f 6675 6c6c 5f64 6174  am 'use_full_dat
+00000d90: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
+00000da0: 6c27 da05 7472 6169 6eda 0474 6573 74da  l'..train..test.
+00000db0: 0573 7465 7073 e92c 0100 00e9 0100 0000  .steps.,........
+00000dc0: a904 da0f 6e75 6d5f 626f 6f73 745f 726f  ....num_boost_ro
+00000dd0: 756e 64da 1565 6172 6c79 5f73 746f 7070  und..early_stopp
+00000de0: 696e 675f 726f 756e 6473 da05 6576 616c  ing_rounds..eval
+00000df0: 73da 0c76 6572 626f 7365 5f65 7661 6c7a  s..verbose_evalz
+00000e00: 1146 696e 6973 6865 6420 7472 6169 6e69  .Finished traini
+00000e10: 6e67 2922 7211 0000 0072 0300 0000 7226  ng)"r....r....r&
+00000e20: 0000 0072 2800 0000 7219 0000 0072 1700  ...r(...r....r..
+00000e30: 0000 721a 0000 00da 0a56 616c 7565 4572  ..r......ValueEr
+00000e40: 726f 72da 1973 686f 775f 6465 7461 696c  ror..show_detail
+00000e50: 6564 5f74 756e 696e 675f 6c6f 6773 da06  ed_tuning_logs..
+00000e60: 6f70 7475 6e61 da07 6c6f 6767 696e 67da  optuna..logging.
+00000e70: 0d73 6574 5f76 6572 626f 7369 7479 da07  .set_verbosity..
+00000e80: 5741 524e 494e 47da 0e61 7574 6f74 756e  WARNING..autotun
+00000e90: 655f 6d6f 6465 6cda 0861 7574 6f74 756e  e_model..autotun
+00000ea0: 65da 0570 7269 6e74 da1e 656e 6162 6c65  e..print..enable
+00000eb0: 5f67 7269 645f 7365 6172 6368 5f66 696e  _grid_search_fin
+00000ec0: 655f 7475 6e69 6e67 da09 6669 6e65 5f74  e_tuning..fine_t
+00000ed0: 756e 6572 1b00 0000 da0d 6669 745f 7472  uner......fit_tr
+00000ee0: 616e 7366 6f72 6dda 0974 7261 6e73 666f  ansform..transfo
+00000ef0: 726d da1d 7573 655f 6675 6c6c 5f64 6174  rm..use_full_dat
+00000f00: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
+00000f10: 6cda 0270 64da 0663 6f6e 6361 74da 1163  l..pd..concat..c
+00000f20: 7265 6174 655f 645f 6d61 7472 6963 6573  reate_d_matrices
+00000f30: da06 7061 7261 6d73 da03 706f 70da 1468  ..params..pop..h
+00000f40: 7970 6572 7475 6e69 6e67 5f63 765f 666f  ypertuning_cv_fo
+00000f50: 6c64 7372 1800 0000 da03 7867 6272 3100  ldsr......xgbr1.
+00000f60: 0000 7238 0000 00da 2576 6572 626f 7369  ..r8....%verbosi
+00000f70: 7479 5f64 7572 696e 675f 6669 6e61 6c5f  ty_during_final_
+00000f80: 6d6f 6465 6c5f 7472 6169 6e69 6e67 721c  model_trainingr.
+00000f90: 0000 0029 0972 2200 0000 7229 0000 0072  ...).r"...r)...r
+00000fa0: 2a00 0000 722b 0000 0072 2c00 0000 da07  *...r+...r,.....
+00000fb0: 645f 7472 6169 6eda 0664 5f74 6573 74da  d_train..d_test.
+00000fc0: 0865 7661 6c5f 7365 7472 3300 0000 7223  .eval_setr3...r#
+00000fd0: 0000 0072 2300 0000 7224 0000 00da 0366  ...r#...r$.....f
+00000fe0: 6974 4d00 0000 7370 0000 0012 0808 0104  itM...sp........
+00000ff0: 0302 ff04 0202 fe04 0302 fd02 0502 0104  ................
+00001000: ff08 0410 0108 0210 0108 0108 0210 0108  ................
+00001010: 0108 0206 0106 0104 0108 ff06 0306 010a  ................
+00001020: ff08 0402 010c 0104 ff0e 040e 0114 0210  ................
+00001030: 0110 0212 0204 0106 0102 0102 0106 0102  ................
+00001040: 0106 010a fa06 0804 0106 0102 0102 0106  ................
+00001050: 0102 0106 0108 fa08 0806 017a 1a58 6762  ...........z.Xgb
+00001060: 6f6f 7374 4d6f 6465 6c52 6567 7265 7373  oostModelRegress
+00001070: 696f 6e2e 6669 7463 0500 0000 0000 0000  ion.fitc........
+00001080: 0000 0000 0d00 0000 0e00 0000 0300 0000  ................
+00001090: 7300 0200 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
+000010a0: 019d 0283 0101 0088 006a 0372 1288 006a  .........j.r...j
+000010b0: 0472 1288 006a 0573 1674 0664 0283 0182  .r...j.s.t.d....
+000010c0: 0174 0783 0089 0188 00a0 08a1 0001 0088  .t..............
+000010d0: 006a 0372 2988 006a 0472 2988 006a 0972  .j.r)..j.r)..j.r
+000010e0: 2988 006a 0573 2d74 0664 0383 0182 0188  )..j.s-t.d......
+000010f0: 006a 046a 0a72 6574 0b74 0c88 036a 0d83  .j.j.ret.t...j..
+00001100: 0188 006a 046a 0e64 048d 027d 0574 0b74  ...j.j.d...}.t.t
+00001110: 0c88 026a 0d83 0188 006a 046a 0e64 048d  ...j.....j.j.d..
+00001120: 027d 0688 036a 0f7c 0588 006a 046a 1064  .}...j.|...j.j.d
+00001130: 058d 0289 0388 056a 1188 036a 0d19 0089  .......j...j....
+00001140: 0588 026a 0f7c 0688 006a 046a 1064 058d  ...j.|...j.j.d..
+00001150: 0289 0288 046a 1188 026a 0d19 0089 0487  .....j...j......
+00001160: 0087 0187 0287 0387 0487 0566 0664 0664  ...........f.d.d
+00001170: 0784 087d 0764 087d 0874 126a 136a 1464  ...}.d.}.t.j.j.d
+00001180: 0988 006a 046a 1088 006a 046a 1564 0a8d  ...j.j...j.j.d..
+00001190: 037d 0974 126a 1664 0b7c 097c 089b 0064  .}.t.j.d.|.|...d
+000011a0: 0c9d 0264 0d8d 037d 0a7c 0a6a 177c 0788  ...d...}.|.j.|..
+000011b0: 006a 046a 1888 006a 046a 1964 0964 0964  .j.j...j.j.d.d.d
+000011c0: 0e8d 0501 007a 1674 126a 1aa0 1b7c 0aa1  .....z.t.j...|..
+000011d0: 017d 0b7c 0ba0 1ca1 0001 0074 126a 1aa0  .}.|.......t.j..
+000011e0: 1d7c 0aa1 017d 0b7c 0ba0 1ca1 0001 0057  .|...}.|.......W
+000011f0: 006e 0c04 0074 1e74 1f74 0666 0379 ba01  .n...t.t.t.f.y..
+00001200: 0001 0001 0059 006e 0177 007c 0a6a 206a  .....Y.n.w.|.j j
+00001210: 217d 0c88 006a 096a 2288 006a 096a 2388  !}...j.j"..j.j#.
+00001220: 006a 096a 247c 0c64 0f19 007c 0c64 1019  .j.j$|.d...|.d..
+00001230: 007c 0c64 1119 007c 0c64 1219 007c 0c64  .|.d...|.d...|.d
+00001240: 1319 007c 0c64 1419 007c 0c64 1519 007c  ...|.d...|.d...|
+00001250: 0c64 1619 007c 0c64 1719 007c 0c64 1819  .d...|.d...|.d..
+00001260: 0064 199c 0d88 006a 035f 2169 0088 006a  .d.....j._!i...j
+00001270: 036a 21a5 0188 01a5 0188 006a 035f 2174  .j!........j._!t
+00001280: 0064 1a88 006a 036a 219b 009d 0283 0101  .d...j.j!.......
+00001290: 0064 1b53 0029 1c7a 7b54 756e 6520 6879  .d.S.).z{Tune hy
+000012a0: 7065 7270 6172 616d 6574 6572 732e 0a0a  perparameters...
+000012b0: 2020 2020 2020 2020 416e 2061 6c74 6572          An alter
+000012c0: 6e61 7469 7665 2063 6f6e 6669 6720 6361  native config ca
+000012d0: 6e20 6265 2070 726f 7669 6465 6420 746f  n be provided to
+000012e0: 206f 7665 7277 7269 7465 2074 6865 2068   overwrite the h
+000012f0: 7970 6572 7061 7261 6d65 7465 7220 7365  yperparameter se
+00001300: 6172 6368 2073 7061 6365 2e0a 2020 2020  arch space..    
+00001310: 2020 2020 7a2f 3a20 5374 6172 7420 6879      z/: Start hy
+00001320: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
+00001330: 696e 6720 6f66 2058 6762 6f6f 7374 206d  ing of Xgboost m
+00001340: 6f64 656c 2e72 2e00 0000 fa4f 4174 206c  odel.r.....OAt l
+00001350: 6561 7374 206f 6e65 206f 6620 7468 6520  east one of the 
+00001360: 636f 6e66 6967 7320 6f72 2065 7870 6572  configs or exper
+00001370: 696d 656e 745f 7472 6163 6b65 7220 6973  iment_tracker is
+00001380: 204e 6f6e 652c 2077 6869 6368 2069 7320   None, which is 
+00001390: 6e6f 7420 616c 6c6f 7765 6429 01da 0561  not allowed)...a
+000013a0: 6c70 6861 2901 da0c 7261 6e64 6f6d 5f73  lpha)...random_s
+000013b0: 7461 7465 6301 0000 0000 0000 0000 0000  tatec...........
+000013c0: 0009 0000 0012 0000 0013 0000 0073 0c02  .............s..
+000013d0: 0000 8800 6a00 6a01 8800 6a00 6a02 8800  ....j.j...j.j...
+000013e0: 6a00 6a03 7c00 6a04 6401 8800 6a00 6a05  j.j.|.j.d...j.j.
+000013f0: 8800 6a00 6a06 6402 6403 8d04 7c00 6a07  ..j.j.d.d...|.j.
+00001400: 6404 8800 6a00 6a08 8800 6a00 6a09 6402  d...j.j...j.j.d.
+00001410: 6403 8d04 7c00 6a04 6405 8800 6a00 6a0a  d...|.j.d...j.j.
+00001420: 8800 6a00 6a0b 6402 6403 8d04 7c00 6a04  ..j.j.d.d...|.j.
+00001430: 6406 8800 6a00 6a0c 8800 6a00 6a0d 6402  d...j.j...j.j.d.
+00001440: 6403 8d04 7c00 6a04 6407 8800 6a00 6a0c  d...|.j.d...j.j.
+00001450: 8800 6a00 6a0d 6402 6403 8d04 7c00 a007  ..j.j.d.d...|...
+00001460: 6408 8800 6a00 6a0e 8800 6a00 6a0f a103  d...j.j...j.j...
+00001470: 7c00 a004 6409 8800 6a00 6a10 8800 6a00  |...d...j.j...j.
+00001480: 6a11 a103 7c00 a004 640a 8800 6a00 6a12  j...|...d...j.j.
+00001490: 8800 6a00 6a13 a103 7c00 a004 640b 8800  ..j.j...|...d...
+000014a0: 6a00 6a14 8800 6a00 6a15 a103 7c00 6a07  j.j...j.j...|.j.
+000014b0: 640c 8800 6a00 6a16 8800 6a00 6a17 6402  d...j.j...j.j.d.
+000014c0: 6403 8d04 640d 9c0d 7d01 6900 7c01 a501  d...d...}.i.|...
+000014d0: 8801 a501 7d01 7418 6a19 8803 8805 8800  ....}.t.j.......
+000014e0: 6a1a 6a1b 640e 8d03 7d02 7418 6a19 8802  j.j.d...}.t.j...
+000014f0: 8804 8800 6a1a 6a1b 640e 8d03 7d03 741c  ....j.j.d...}.t.
+00001500: 6a1d a01e 7c00 640f a102 7d04 7c01 a01f  j...|.d...}.|...
+00001510: 640c 6410 a102 7d05 8800 6a1a 6a20 6411  d.d...}...j.j d.
+00001520: 6b02 72b3 8800 a021 7c02 7c03 8804 7c01  k.r....!|.|...|.
+00001530: 7c05 7c04 a106 5300 8800 6a1a 6a20 6411  |.|...S...j.j d.
+00001540: 6b04 72c6 8800 6a1a 6a22 72c6 8800 a023  k.r...j.j"r....#
+00001550: 7c01 8803 8805 8802 8804 a105 5300 7418  |...........S.t.
+00001560: 6a24 7c01 7c02 7c05 8800 6a1a 6a25 8800  j$|.|.|...j.j%..
+00001570: 6a1a 6a20 6402 8800 6a1a 6a26 7c04 6701  j.j d...j.j&|.g.
+00001580: 8800 6a1a 6a27 6412 8d09 7d06 7c06 6413  ..j.j'd...}.|.d.
+00001590: 1900 a028 a100 7d07 7429 8800 6a2a 6a2b  ...(..}.t)..j*j+
+000015a0: 8301 6414 6b02 72ee 6414 7d08 6e08 8800  ..d.k.r.d.}.n...
+000015b0: 6a2a 6a2b 6415 1900 6411 1700 7d08 8800  j*j+d...d...}...
+000015c0: 6a2a 6a2c 7c08 6416 8800 6a1a 7c01 7c07  j*j,|.d...j.|.|.
+000015d0: 6417 6418 6419 8d07 0100 7c07 5300 291a  d.d.d.....|.S.).
+000015e0: 4eda 0365 7461 54a9 01da 036c 6f67 da09  N..etaT....log..
+000015f0: 6d61 785f 6465 7074 6872 5600 0000 da06  max_depthrV.....
+00001600: 6c61 6d62 6461 da05 6761 6d6d 61da 106d  lambda..gamma..m
+00001610: 696e 5f63 6869 6c64 5f77 6569 6768 74da  in_child_weight.
+00001620: 0973 7562 7361 6d70 6c65 da10 636f 6c73  .subsample..cols
+00001630: 616d 706c 655f 6279 7472 6565 da11 636f  ample_bytree..co
+00001640: 6c73 616d 706c 655f 6279 6c65 7665 6c72  lsample_bylevelr
+00001650: 3300 0000 290d da09 6f62 6a65 6374 6976  3...)...objectiv
+00001660: 65da 0762 6f6f 7374 6572 da0b 6576 616c  e..booster..eval
+00001670: 5f6d 6574 7269 6372 5800 0000 725b 0000  _metricrX...r[..
+00001680: 0072 5600 0000 725c 0000 0072 5d00 0000  .rV...r\...r]...
+00001690: 725e 0000 0072 5f00 0000 7260 0000 0072  r^...r_...r`...r
+000016a0: 6100 0000 7233 0000 00a9 02da 056c 6162  a...r3.......lab
+000016b0: 656c da12 656e 6162 6c65 5f63 6174 6567  el..enable_categ
+000016c0: 6f72 6963 616c fa09 7465 7374 2d72 6d73  orical..test-rms
+000016d0: 6572 3400 0000 7235 0000 00a9 0972 4c00  er4...r5.....rL.
+000016e0: 0000 da06 6474 7261 696e 7237 0000 0072  ....dtrainr7...r
+000016f0: 3800 0000 da05 6e66 6f6c 64da 0961 735f  8.....nfold..as_
+00001700: 7061 6e64 6173 da04 7365 6564 da09 6361  pandas..seed..ca
+00001710: 6c6c 6261 636b 73da 0773 6875 6666 6c65  llbacks..shuffle
+00001720: fa0e 7465 7374 2d72 6d73 652d 6d65 616e  ..test-rmse-mean
+00001730: 7201 0000 00e9 ffff ffff da08 6376 5f73  r...........cv_s
+00001740: 636f 7265 7a0d 6164 6a75 7374 6564 2072  corez.adjusted r
+00001750: 6d73 6546 a907 da0d 6578 7065 7269 6d65  mseF....experime
+00001760: 6e74 5f69 64da 0e73 636f 7265 5f63 6174  nt_id..score_cat
+00001770: 6567 6f72 79da 0f74 7261 696e 696e 675f  egory..training_
+00001780: 636f 6e66 6967 da10 6d6f 6465 6c5f 7061  config..model_pa
+00001790: 7261 6d65 7465 7273 da0b 6576 616c 5f73  rameters..eval_s
+000017a0: 636f 7265 73da 0b6d 6574 7269 635f 7573  cores..metric_us
+000017b0: 6564 da17 6d65 7472 6963 5f68 6967 6865  ed..metric_highe
+000017c0: 725f 6973 5f62 6574 7465 7229 2d72 1800  r_is_better)-r..
+000017d0: 0000 da11 7867 626f 6f73 745f 6f62 6a65  ....xgboost_obje
+000017e0: 6374 6976 6572 6300 0000 da13 7867 626f  ctiverc.....xgbo
+000017f0: 6f73 745f 6576 616c 5f6d 6574 7269 63da  ost_eval_metric.
+00001800: 0d73 7567 6765 7374 5f66 6c6f 6174 da07  .suggest_float..
+00001810: 6574 615f 6d69 6eda 0765 7461 5f6d 6178  eta_min..eta_max
+00001820: da0b 7375 6767 6573 745f 696e 74da 0d6d  ..suggest_int..m
+00001830: 6178 5f64 6570 7468 5f6d 696e da0d 6d61  ax_depth_min..ma
+00001840: 785f 6465 7074 685f 6d61 78da 0961 6c70  x_depth_max..alp
+00001850: 6861 5f6d 696e da09 616c 7068 615f 6d61  ha_min..alpha_ma
+00001860: 78da 0a6c 616d 6264 615f 6d69 6eda 0a6c  x..lambda_min..l
+00001870: 616d 6264 615f 6d61 78da 146d 696e 5f63  ambda_max..min_c
+00001880: 6869 6c64 5f77 6569 6768 745f 6d69 6eda  hild_weight_min.
+00001890: 146d 696e 5f63 6869 6c64 5f77 6569 6768  .min_child_weigh
+000018a0: 745f 6d61 78da 0e73 7562 5f73 616d 706c  t_max..sub_sampl
+000018b0: 655f 6d69 6eda 0e73 7562 5f73 616d 706c  e_min..sub_sampl
+000018c0: 655f 6d61 78da 1663 6f6c 5f73 616d 706c  e_max..col_sampl
+000018d0: 655f 6279 5f74 7265 655f 6d69 6eda 1663  e_by_tree_min..c
+000018e0: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
+000018f0: 655f 6d61 78da 1763 6f6c 5f73 616d 706c  e_max..col_sampl
+00001900: 655f 6279 5f6c 6576 656c 5f6d 696e da17  e_by_level_min..
+00001910: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
+00001920: 7665 6c5f 6d61 78da 0973 7465 7073 5f6d  vel_max..steps_m
+00001930: 696e da09 7374 6570 735f 6d61 7872 4f00  in..steps_maxrO.
+00001940: 0000 da07 444d 6174 7269 7872 1700 0000  ....DMatrixr....
+00001950: da1d 6361 745f 656e 636f 6469 6e67 5f76  ..cat_encoding_v
+00001960: 6961 5f6d 6c5f 616c 676f 7269 7468 6d72  ia_ml_algorithmr
+00001970: 3d00 0000 da0b 696e 7465 6772 6174 696f  =.....integratio
+00001980: 6eda 1658 4742 6f6f 7374 5072 756e 696e  n..XGBoostPrunin
+00001990: 6743 616c 6c62 6163 6b72 4d00 0000 724e  gCallbackrM...rN
+000019a0: 0000 00da 1774 7261 696e 5f73 696e 676c  .....train_singl
+000019b0: 655f 666f 6c64 5f6d 6f64 656c da11 7072  e_fold_model..pr
+000019c0: 6563 6973 655f 6376 5f74 756e 696e 67da  ecise_cv_tuning.
+000019d0: 125f 6669 6e65 5f74 756e 655f 7072 6563  ._fine_tune_prec
+000019e0: 6973 65da 0263 7672 3800 0000 7220 0000  ise..cvr8...r ..
+000019f0: 00da 1773 6875 6666 6c65 5f64 7572 696e  ...shuffle_durin
+00001a00: 675f 7472 6169 6e69 6e67 da04 6d65 616e  g_training..mean
+00001a10: da03 6c65 6e72 1a00 0000 7274 0000 00da  ..lenr....rt....
+00001a20: 0b61 6464 5f72 6573 756c 7473 2909 da05  .add_results)...
+00001a30: 7472 6961 6cda 0570 6172 616d 7251 0000  trial..paramrQ..
+00001a40: 0072 5200 0000 da10 7072 756e 696e 675f  .rR.....pruning_
+00001a50: 6361 6c6c 6261 636b 7233 0000 00da 0672  callbackr3.....r
+00001a60: 6573 756c 74da 0e61 646a 7573 7465 645f  esult..adjusted_
+00001a70: 7363 6f72 65da 066e 6577 5f69 64a9 0672  score..new_id..r
+00001a80: 2200 0000 da08 7472 6169 6e5f 6f6e 722a  ".....train_onr*
+00001a90: 0000 0072 2900 0000 722c 0000 0072 2b00  ...r)...r,...r+.
+00001aa0: 0000 7223 0000 0072 2400 0000 7262 0000  ..r#...r$...rb..
+00001ab0: 00cd 0000 0073 d800 0000 0602 0601 0601  .....s..........
+00001ac0: 0401 0201 0601 0601 0201 04fc 0406 0201  ................
+00001ad0: 0601 0601 0201 04fc 0406 0201 0601 0601  ................
+00001ae0: 0201 04fc 0406 0201 0601 0601 0201 04fc  ................
+00001af0: 0406 0201 0601 0601 0201 04fc 0406 0201  ................
+00001b00: 0601 0601 02fd 0405 0201 0601 0601 02fd  ................
+00001b10: 0405 0201 0601 0601 02fd 0405 0201 0601  ................
+00001b20: 0601 02fd 0405 0201 0601 0601 0201 04fc  ................
+00001b30: 06ca 0c3d 0401 0201 0201 0601 06fd 0406  ...=............
+00001b40: 0201 0201 0601 06fd 0606 0401 04ff 0c04  ................
+00001b50: 0c02 0401 0c01 04ff 0c04 0601 02ff 1204  ................
+00001b60: 0402 0201 0201 0201 0601 0601 0201 0601  ................
+00001b70: 0401 0601 06f7 0c0c 1003 0601 1002 0601  ................
+00001b80: 0201 0201 0401 0201 0201 0201 0201 06f9  ................
+00001b90: 040a 7a32 5867 626f 6f73 744d 6f64 656c  ..z2XgboostModel
+00001ba0: 5265 6772 6573 7369 6f6e 2e61 7574 6f74  Regression.autot
+00001bb0: 756e 652e 3c6c 6f63 616c 733e 2e6f 626a  une.<locals>.obj
+00001bc0: 6563 7469 7665 da07 7867 626f 6f73 7454  ective..xgboostT
+00001bd0: 2903 da0c 6d75 6c74 6976 6172 6961 7465  )...multivariate
+00001be0: 726d 0000 00da 106e 5f73 7461 7274 7570  rm.....n_startup
+00001bf0: 5f74 7269 616c 73da 086d 696e 696d 697a  _trials..minimiz
+00001c00: 657a 0720 7475 6e69 6e67 2903 da09 6469  ez. tuning)...di
+00001c10: 7265 6374 696f 6eda 0773 616d 706c 6572  rection..sampler
+00001c20: da0a 7374 7564 795f 6e61 6d65 a904 da08  ..study_name....
+00001c30: 6e5f 7472 6961 6c73 da07 7469 6d65 6f75  n_trials..timeou
+00001c40: 74da 0e67 635f 6166 7465 725f 7472 6961  t..gc_after_tria
+00001c50: 6cda 1173 686f 775f 7072 6f67 7265 7373  l..show_progress
+00001c60: 5f62 6172 725b 0000 0072 5600 0000 725c  _barr[...rV...r\
+00001c70: 0000 0072 5d00 0000 725e 0000 0072 5f00  ...r]...r^...r_.
+00001c80: 0000 7260 0000 0072 6100 0000 7258 0000  ..r`...ra...rX..
+00001c90: 0072 3300 0000 290d 7262 0000 0072 6300  .r3...).rb...rc.
+00001ca0: 0000 7264 0000 0072 5b00 0000 7256 0000  ..rd...r[...rV..
+00001cb0: 0072 5c00 0000 725d 0000 0072 5e00 0000  .r\...r]...r^...
+00001cc0: 725f 0000 0072 6000 0000 7261 0000 0072  r_...r`...ra...r
+00001cd0: 5800 0000 7233 0000 00fa 0d42 6573 7420  X...r3.....Best 
+00001ce0: 7061 7261 6d73 3a20 4e29 2572 1100 0000  params: N)%r....
+00001cf0: 7203 0000 0072 2600 0000 7219 0000 0072  r....r&...r....r
+00001d00: 1700 0000 721a 0000 0072 3b00 0000 720f  ....r....r;...r.
+00001d10: 0000 0072 2800 0000 7218 0000 00da 1973  ...r(...r......s
+00001d20: 616d 706c 655f 6461 7461 5f64 7572 696e  ample_data_durin
+00001d30: 675f 7475 6e69 6e67 7210 0000 0072 9b00  g_tuningr....r..
+00001d40: 0000 da05 696e 6465 78da 1f73 616d 706c  ....index..sampl
+00001d50: 655f 6461 7461 5f64 7572 696e 675f 7475  e_data_during_tu
+00001d60: 6e69 6e67 5f61 6c70 6861 da06 7361 6d70  ning_alpha..samp
+00001d70: 6c65 7220 0000 00da 036c 6f63 723d 0000  ler .....locr=..
+00001d80: 00da 0873 616d 706c 6572 73da 0a54 5045  ...samplers..TPE
+00001d90: 5361 6d70 6c65 72da 1f6f 7074 756e 615f  Sampler..optuna_
+00001da0: 7361 6d70 6c65 725f 6e5f 7374 6172 7475  sampler_n_startu
+00001db0: 705f 7472 6961 6c73 da0c 6372 6561 7465  p_trials..create
+00001dc0: 5f73 7475 6479 da08 6f70 7469 6d69 7a65  _study..optimize
+00001dd0: da1c 6879 7065 7270 6172 616d 6574 6572  ..hyperparameter
+00001de0: 5f74 756e 696e 675f 726f 756e 6473 da26  _tuning_rounds.&
+00001df0: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
+00001e00: 756e 696e 675f 6d61 785f 7275 6e74 696d  uning_max_runtim
+00001e10: 655f 7365 6373 da0d 7669 7375 616c 697a  e_secs..visualiz
+00001e20: 6174 696f 6eda 1970 6c6f 745f 6f70 7469  ation..plot_opti
+00001e30: 6d69 7a61 7469 6f6e 5f68 6973 746f 7279  mization_history
+00001e40: da04 7368 6f77 da16 706c 6f74 5f70 6172  ..show..plot_par
+00001e50: 616d 5f69 6d70 6f72 7461 6e63 6573 da11  am_importances..
+00001e60: 5a65 726f 4469 7669 7369 6f6e 4572 726f  ZeroDivisionErro
+00001e70: 72da 0c52 756e 7469 6d65 4572 726f 72da  r..RuntimeError.
+00001e80: 0a62 6573 745f 7472 6961 6c72 4c00 0000  .best_trialrL...
+00001e90: 727b 0000 0072 6300 0000 727c 0000 0029  r{...rc...r|...)
+00001ea0: 0d72 2200 0000 7229 0000 0072 2a00 0000  .r"...r)...r*...
+00001eb0: 722b 0000 0072 2c00 0000 da10 6e62 5f73  r+...r,.....nb_s
+00001ec0: 616d 706c 6573 5f74 7261 696e da0f 6e62  amples_train..nb
+00001ed0: 5f73 616d 706c 6573 5f74 6573 7472 6200  _samples_testrb.
+00001ee0: 0000 da09 616c 676f 7269 7468 6d72 aa00  ....algorithmr..
+00001ef0: 0000 da05 7374 7564 79da 0366 6967 da12  ....study..fig..
+00001f00: 7867 626f 6f73 745f 6265 7374 5f70 6172  xgboost_best_par
+00001f10: 616d 7223 0000 0072 a300 0000 7224 0000  amr#...r....r$..
+00001f20: 0072 4200 0000 9700 0000 73b8 0000 0012  .rB.......s.....
+00001f30: 0b04 0202 ff04 0202 fe04 0302 fd02 0502  ................
+00001f40: 0104 ff06 0408 0204 0302 ff04 0202 fe04  ................
+00001f50: 0302 fd04 0402 fc02 0602 0104 ff08 0402  ................
+00001f60: 0108 0106 0106 fe02 0408 0106 0106 fe04  ................
+00001f70: 0508 0106 ff0c 0304 0108 0106 ff0c 0316  ................
+00001f80: 0204 7b06 0102 0106 0106 0106 fd04 0502  ..{.............
+00001f90: 0102 0108 0106 fd04 0602 0106 0106 0102  ................
+00001fa0: 0102 0106 fb02 070c 0108 0106 0102 0104  ................
+00001fb0: ff0c 0312 0104 0102 ff08 0306 0306 0106  ................
+00001fc0: 0102 0102 0102 ff06 0306 0106 0106 0106  ................
+00001fd0: 0106 0106 0106 0106 010a f102 1106 0102  ................
+00001fe0: ff02 0208 fe16 047a 1f58 6762 6f6f 7374  .......z.Xgboost
+00001ff0: 4d6f 6465 6c52 6567 7265 7373 696f 6e2e  ModelRegression.
+00002000: 6175 746f 7475 6e65 6301 0000 0000 0000  autotunec.......
+00002010: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00002020: 0073 5e00 0000 7c00 6a00 6a01 7217 7c00  .s^...|.j.j.r.|.
+00002030: 6a00 6a02 6401 6b02 730e 7c00 6a00 6a03  j.j.d.k.s.|.j.j.
+00002040: 7217 7c00 6a04 6a05 6402 6403 8d01 7d01  r.|.j.j.d.d...}.
+00002050: 7c01 5300 7c00 6a00 6a01 722a 7c00 6a00  |.S.|.j.j.r*|.j.
+00002060: 6a02 6401 6b04 722a 7c00 6a04 6a05 6402  j.d.k.r*|.j.j.d.
+00002070: 6403 8d01 7d01 7c01 5300 7406 6a07 7d01  d...}.|.S.t.j.}.
+00002080: 7c01 5300 2904 4e72 3500 0000 da17 726f  |.S.).Nr5.....ro
+00002090: 6f74 5f6d 6561 6e5f 7371 7561 7265 645f  ot_mean_squared_
+000020a0: 6572 726f 7229 01da 0d74 6172 6765 745f  error)...target_
+000020b0: 6d65 7472 6963 2908 7217 0000 0072 4100  metric).r....rA.
+000020c0: 0000 724e 0000 0072 9600 0000 721a 0000  ..rN...r....r...
+000020d0: 00da 0e67 6574 5f62 6573 745f 7363 6f72  ...get_best_scor
+000020e0: 6572 1d00 0000 da03 696e 6629 0272 2200  er......inf).r".
+000020f0: 0000 da12 6265 7374 5f73 636f 7265 5f63  ....best_score_c
+00002100: 765f 6772 6964 7223 0000 0072 2300 0000  v_gridr#...r#...
+00002110: 7224 0000 0072 cd00 0000 7e01 0000 7322  r$...r....~...s"
+00002120: 0000 0008 010c 0106 0102 ff06 0302 0106  ................
+00002130: ff04 0c06 f802 ff0c 0206 0202 0106 ff04  ................
+00002140: 0506 ff04 017a 2558 6762 6f6f 7374 4d6f  .....z%XgboostMo
+00002150: 6465 6c52 6567 7265 7373 696f 6e2e 6765  delRegression.ge
+00002160: 745f 6265 7374 5f73 636f 7265 6305 0000  t_best_scorec...
+00002170: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00002180: 0043 0000 0073 3000 0000 7400 6a01 7c01  .C...s0...t.j.|.
+00002190: 7c02 7c00 6a02 6a03 6401 8d03 7d05 7400  |.|.j.j.d...}.t.
+000021a0: 6a01 7c03 7c04 7c00 6a02 6a03 6401 8d03  j.|.|.|.j.j.d...
+000021b0: 7d06 7c05 7c06 6602 5300 2902 4e72 6500  }.|.|.f.S.).Nre.
+000021c0: 0000 2904 724f 0000 0072 9100 0000 7217  ..).rO...r....r.
+000021d0: 0000 0072 9200 0000 2907 7222 0000 0072  ...r....).r"...r
+000021e0: 2900 0000 722b 0000 0072 2a00 0000 722c  )...r+...r*...r,
+000021f0: 0000 0072 5100 0000 7252 0000 0072 2300  ...rQ...rR...r#.
+00002200: 0000 7223 0000 0072 2400 0000 724b 0000  ..r#...r$...rK..
+00002210: 0091 0100 0073 1600 0000 0401 0201 0201  .....s..........
+00002220: 0601 06fd 0405 0201 0201 0601 06fd 0805  ................
+00002230: 7a28 5867 626f 6f73 744d 6f64 656c 5265  z(XgboostModelRe
+00002240: 6772 6573 7369 6f6e 2e63 7265 6174 655f  gression.create_
+00002250: 645f 6d61 7472 6963 6573 6307 0000 0000  d_matricesc.....
+00002260: 0000 0000 0000 000c 0000 0009 0000 0043  ...............C
+00002270: 0000 0073 9000 0000 7c01 6401 6602 7c02  ...s....|.d.f.|.
+00002280: 6402 6602 6702 7d07 7400 6a01 7c04 7c01  d.f.g.}.t.j.|.|.
+00002290: 7c05 7c00 6a02 6a03 7c07 7c06 6701 7c00  |.|.j.j.|.|.g.|.
+000022a0: 6a04 6a05 6403 8d07 7d08 7c08 a006 7c02  j.j.d...}.|...|.
+000022b0: a101 7d09 7407 7c03 7c09 6404 6405 8d03  ..}.t.|.|.d.d...
+000022c0: 7d0a 7408 7c00 6a09 6a0a 8301 6406 6b02  }.t.|.j.j...d.k.
+000022d0: 7230 6406 7d0b 6e08 7c00 6a09 6a0a 6407  r0d.}.n.|.j.j.d.
+000022e0: 1900 6408 1700 7d0b 7c00 6a09 6a0b 7c0b  ..d...}.|.j.j.|.
+000022f0: 6409 7c00 6a02 7c04 7c0a 640a 6404 640b  d.|.j.|.|.d.d.d.
+00002300: 8d07 0100 7c0a 5300 290c 4e72 3100 0000  ....|.S.).Nr1...
+00002310: 7232 0000 0029 0572 3700 0000 7238 0000  r2...).r7...r8..
+00002320: 0072 3900 0000 726e 0000 0072 3a00 0000  .r9...rn...r:...
+00002330: 46a9 01da 0773 7175 6172 6564 7201 0000  F....squaredr...
+00002340: 0072 7100 0000 7235 0000 00da 1773 696d  .rq...r5.....sim
+00002350: 706c 655f 7472 6169 6e5f 7465 7374 5f73  ple_train_test_s
+00002360: 636f 7265 72cb 0000 0072 7300 0000 290c  corer....rs...).
+00002370: 724f 0000 0072 3100 0000 7217 0000 0072  rO...r1...r....r
+00002380: 3800 0000 7218 0000 00da 2676 6572 626f  8...r.....&verbo
+00002390: 7369 7479 5f64 7572 696e 675f 6879 7065  sity_during_hype
+000023a0: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
+000023b0: 67da 0770 7265 6469 6374 7209 0000 0072  g..predictr....r
+000023c0: 9b00 0000 721a 0000 0072 7400 0000 729c  ....r....rt...r.
+000023d0: 0000 0029 0c72 2200 0000 7251 0000 0072  ...).r"...rQ...r
+000023e0: 5200 0000 722c 0000 0072 9e00 0000 7233  R...r,...r....r3
+000023f0: 0000 0072 9f00 0000 7253 0000 0072 1c00  ...r....rS...r..
+00002400: 0000 da05 7072 6564 73da 036d 7365 72a2  ....preds..mser.
+00002410: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00002420: 0000 7295 0000 009e 0100 0073 3200 0000  ..r........s2...
+00002430: 1003 0401 0201 0201 0201 0601 0201 0401  ................
+00002440: 0601 06f9 0a09 0e01 1003 0601 1002 0601  ................
+00002450: 0201 0201 0401 0201 0201 0201 0201 06f9  ................
+00002460: 0409 7a2e 5867 626f 6f73 744d 6f64 656c  ..z.XgboostModel
+00002470: 5265 6772 6573 7369 6f6e 2e74 7261 696e  Regression.train
+00002480: 5f73 696e 676c 655f 666f 6c64 5f6d 6f64  _single_fold_mod
+00002490: 656c e964 0000 00da 0765 7661 6c5f 6466  el.d.....eval_df
+000024a0: da06 795f 7472 7565 da0a 6974 6572 6174  ..y_true..iterat
+000024b0: 696f 6e73 6305 0000 0000 0000 0000 0000  ionsc...........
+000024c0: 0010 0000 0007 0000 0043 0000 0073 9a00  .........C...s..
+000024d0: 0000 6700 7d05 7400 7c04 8301 4400 5d44  ..g.}.t.|...D.]D
+000024e0: 7d06 6401 6402 7c06 1400 0202 7d07 7d08  }.d.d.|.....}.}.
+000024f0: 7c02 6a01 5c02 7d09 7d0a 7c00 6a02 a003  |.j.\.}.}.|.j...
+00002500: 7c07 7c08 7c09 7c0a 6702 a103 7d0b 7c02  |.|.|.|.g...}.|.
+00002510: 7c0b 1700 7d0c 7c00 6a04 7230 7405 6a06  |...}.|.j.r0t.j.
+00002520: 7c0c 7c03 7c00 6a04 6a07 6403 8d03 7d0d  |.|.|.j.j.d...}.
+00002530: 6e04 7408 6404 8301 8201 7c01 a009 7c0d  n.t.d.....|...|.
+00002540: a101 7d0e 740a 7c03 6a0b a00c a100 7c0e  ..}.t.|.j.....|.
+00002550: a00c a100 6405 6406 8d03 7d0f 7c05 a00d  ....d.d...}.|...
+00002560: 7c0f a101 0100 7106 7c05 5300 2907 619f  |.....q.|.S.).a.
+00002570: 0100 0046 756e 6374 696f 6e20 746f 2061  ...Function to a
+00002580: 6464 2069 6e63 7265 6173 696e 6720 6e6f  dd increasing no
+00002590: 6973 6520 616e 6420 6576 616c 7561 7465  ise and evaluate
+000025a0: 2069 742e 0a0a 2020 2020 2020 2020 5468   it...        Th
+000025b0: 6520 6675 6e63 7469 6f6e 2065 7870 6563  e function expec
+000025c0: 7473 2061 2074 7261 696e 6564 206d 6f64  ts a trained mod
+000025d0: 656c 2061 6e64 2061 2064 6174 6166 7261  el and a datafra
+000025e0: 6d65 2077 6974 6820 7468 6520 7361 6d65  me with the same
+000025f0: 2063 6f6c 756d 6e73 2061 7320 7468 6520   columns as the 
+00002600: 7472 6169 6e69 6e67 2064 6174 612e 0a20  training data.. 
+00002610: 2020 2020 2020 2054 6865 2074 7261 696e         The train
+00002620: 696e 6720 6461 7461 2073 686f 756c 6420  ing data should 
+00002630: 6265 206e 6f72 6d61 6c6c 7920 6469 7374  be normally dist
+00002640: 7269 6275 7465 6420 2863 6f6e 7369 6465  ributed (conside
+00002650: 7220 7573 696e 6720 6120 706f 7765 7220  r using a power 
+00002660: 7472 616e 7366 6f72 6d65 7220 7769 7468  transformer with
+00002670: 2079 656f 2d6a 6f68 6e73 6f6e 292e 0a0a   yeo-johnson)...
+00002680: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
+00002690: 7469 6f6e 2077 696c 6c20 6170 706c 7920  tion will apply 
+000026a0: 696e 6372 6561 7369 6e67 6c79 206e 6f69  increasingly noi
+000026b0: 7365 2074 6f20 7468 6520 6576 616c 2064  se to the eval d
+000026c0: 6174 6166 7261 6d65 2061 6e64 2065 7661  ataframe and eva
+000026d0: 6c75 6174 6520 7468 6520 6d6f 6465 6c20  luate the model 
+000026e0: 6f6e 2069 742e 0a0a 2020 2020 2020 2020  on it...        
+000026f0: 5265 7475 726e 7320 6120 6c69 7374 206f  Returns a list o
+00002700: 6620 6c6f 7373 6573 2e0a 2020 2020 2020  f losses..      
+00002710: 2020 7201 0000 0067 9a99 9999 9999 c93f    r....g.......?
+00002720: 7265 0000 007a 214e 6f20 7472 6169 6e69  re...z!No traini
+00002730: 6e67 5f63 6f6e 6669 6720 636f 756c 6420  ng_config could 
+00002740: 6265 2066 6f75 6e64 4672 d000 0000 290e  be foundFr....).
+00002750: da05 7261 6e67 65da 0573 6861 7065 7221  ..range..shaper!
+00002760: 0000 00da 066e 6f72 6d61 6c72 1700 0000  .....normalr....
+00002770: 724f 0000 0072 9100 0000 7292 0000 0072  rO...r....r....r
+00002780: 3b00 0000 72d4 0000 0072 0900 0000 da06  ;...r....r......
+00002790: 7661 6c75 6573 da06 746f 6c69 7374 da06  values..tolist..
+000027a0: 6170 7065 6e64 2910 7222 0000 00da 086d  append).r".....m
+000027b0: 6c5f 6d6f 6465 6c72 d800 0000 72d9 0000  l_modelr....r...
+000027c0: 0072 da00 0000 da06 6c6f 7373 6573 da01  .r......losses..
+000027d0: 69da 026d 75da 0573 6967 6d61 da01 4eda  i..mu..sigma..N.
+000027e0: 0144 da05 6e6f 6973 65da 0b65 7661 6c5f  .D..noise..eval_
+000027f0: 6466 5f6d 6f64 da06 645f 6576 616c 72d5  df_mod..d_evalr.
+00002800: 0000 00da 046c 6f73 7372 2300 0000 7223  .....lossr#...r#
+00002810: 0000 0072 2400 0000 da1a 696e 6372 6561  ...r$.....increa
+00002820: 7369 6e67 5f6e 6f69 7365 5f65 7661 6c75  sing_noise_evalu
+00002830: 6174 6f72 be01 0000 7326 0000 0004 0d0c  ator....s&......
+00002840: 010e 010a 0114 0108 0106 0104 0102 0102  ................
+00002850: 0106 0108 fd08 060a 0102 0210 0106 ff0c  ................
+00002860: 0304 027a 3158 6762 6f6f 7374 4d6f 6465  ...z1XgboostMode
+00002870: 6c52 6567 7265 7373 696f 6e2e 696e 6372  lRegression.incr
+00002880: 6561 7369 6e67 5f6e 6f69 7365 5f65 7661  easing_noise_eva
+00002890: 6c75 6174 6f72 72e2 0000 0063 0200 0000  luatorr....c....
+000028a0: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+000028b0: 4300 0000 738c 0000 0064 017d 0274 0074  C...s....d.}.t.t
+000028c0: 017c 0183 0183 0144 005d 1c7d 037c 0364  .|.....D.].}.|.d
+000028d0: 0217 0074 017c 0183 0164 0218 006b 0472  ...t.|...d...k.r
+000028e0: 1601 006e 0f7c 017c 0319 007c 017c 0364  ...n.|.|...|.|.d
+000028f0: 0217 0019 006b 0472 247c 0264 0237 007d  .....k.r$|.d.7.}
+00002900: 0271 087c 0264 016b 0272 2d64 037d 047c  .q.|.d.k.r-d.}.|
+00002910: 0453 0074 017c 0183 017d 057c 0164 0119  .S.t.|...}.|.d..
+00002920: 0074 02a0 037c 0164 047c 0285 0219 00a1  .t...|.d.|......
+00002930: 017c 057c 057c 0218 001b 0013 0018 007d  .|.|.|.........}
+00002940: 047c 0453 0029 0561 4201 0000 4361 6c63  .|.S.).aB...Calc
+00002950: 756c 6174 6520 6120 7765 6967 6874 6564  ulate a weighted
+00002960: 206c 6f73 7320 6261 7365 6420 6f6e 2074   loss based on t
+00002970: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
+00002980: 6573 2074 6865 206c 6f73 7320 6465 6372  es the loss decr
+00002990: 6561 7365 642e 0a0a 2020 2020 2020 2020  eased...        
+000029a0: 4578 7065 6374 7320 6120 6c69 7374 206f  Expects a list o
+000029b0: 6620 6c6f 7373 6573 2063 6f6d 696e 6720  f losses coming 
+000029c0: 6672 6f6d 2069 6e63 7265 6173 696e 675f  from increasing_
+000029d0: 6e6f 6973 655f 6576 616c 7561 746f 722e  noise_evaluator.
+000029e0: 2043 6865 636b 7320 686f 7720 6d61 6e79   Checks how many
+000029f0: 2074 696d 6573 2074 6865 206c 6f73 7320   times the loss 
+00002a00: 6465 6372 6561 7365 6420 616e 640a 2020  decreased and.  
+00002a10: 2020 2020 2020 6361 6c63 756c 6174 6573        calculates
+00002a20: 2061 2077 6569 6768 7465 6420 6c6f 7373   a weighted loss
+00002a30: 2062 6173 6564 206f 6e20 7468 6520 6e75   based on the nu
+00002a40: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
+00002a50: 6520 6c6f 7373 2064 6563 7265 6173 6564  e loss decreased
+00002a60: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00002a70: 6e73 2074 6865 2077 6569 6768 7465 6420  ns the weighted 
+00002a80: 6c6f 7373 2e0a 2020 2020 2020 2020 7201  loss..        r.
+00002a90: 0000 0072 3500 0000 69e7 0300 004e 2904  ...r5...i....N).
+00002aa0: 72db 0000 0072 9b00 0000 721d 0000 00da  r....r....r.....
+00002ab0: 0373 7464 2906 7222 0000 0072 e200 0000  .std).r"...r....
+00002ac0: da11 6e62 5f6c 6f73 735f 6465 6372 6561  ..nb_loss_decrea
+00002ad0: 7365 64da 0369 6478 da0d 7765 6967 6874  sed..idx..weight
+00002ae0: 6564 5f6c 6f73 73da 096e 625f 6c6f 7373  ed_loss..nb_loss
+00002af0: 6573 7223 0000 0072 2300 0000 7224 0000  esr#...r#...r$..
+00002b00: 00da 2063 6f6e 7374 616e 745f 6c6f 7373  .. constant_loss
+00002b10: 5f64 6567 7265 6761 7469 6f6e 5f66 6163  _degregation_fac
+00002b20: 746f 72e2 0100 0073 1e00 0000 0408 1001  tor....s........
+00002b30: 1401 0401 1401 0801 0280 0803 0401 040a  ................
+00002b40: 08f8 1601 0a01 06ff 0407 7a37 5867 626f  ..........z7Xgbo
+00002b50: 6f73 744d 6f64 656c 5265 6772 6573 7369  ostModelRegressi
+00002b60: 6f6e 2e63 6f6e 7374 616e 745f 6c6f 7373  on.constant_loss
+00002b70: 5f64 6567 7265 6761 7469 6f6e 5f66 6163  _degregation_fac
+00002b80: 746f 72da 0c74 756e 6564 5f70 6172 616d  tor..tuned_param
+00002b90: 7363 0600 0000 0000 0000 0000 0000 1a00  sc..............
+00002ba0: 0000 0900 0000 4300 0000 73ee 0100 007c  ......C...s....|
+00002bb0: 01a0 0064 0164 02a1 027d 067c 006a 0173  ...d.d...}.|.j.s
+00002bc0: 1174 0283 007c 005f 0174 0364 0383 0101  .t...|._.t.d....
+00002bd0: 0074 047c 006a 016a 0564 047c 006a 016a  .t.|.j.j.d.|.j.j
+00002be0: 0664 058d 037d 0767 007d 0874 077c 07a0  .d...}.g.}.t.|..
+00002bf0: 087c 027c 03a0 0974 0aa1 01a1 0283 0144  .|.|...t.......D
+00002c00: 005d 9c5c 027d 095c 027d 0a7d 0b7c 026a  .].\.}.\.}.}.|.j
+00002c10: 0b7c 0a19 007c 026a 0b7c 0b19 0002 027d  .|...|.j.|.....}
+00002c20: 0c7d 0d7c 036a 0b7c 0a19 007c 036a 0b7c  .}.|.j.|...|.j.|
+00002c30: 0b19 0002 027d 0e7d 0f7c 006a 0c72 667c  .....}.}.|.j.rf|
+00002c40: 006a 0ca0 0d7c 0c7c 0ea1 025c 027d 0c7d  .j...|.|...\.}.}
+00002c50: 0e7c 006a 0ca0 0e7c 047c 05a1 025c 027d  .|.j...|.|...\.}
+00002c60: 107d 117c 006a 0c6a 0e7c 0d7c 0f64 0664  .}.|.j.j.|.|.d.d
+00002c70: 078d 035c 027d 0d7d 0f6e 057c 047c 0502  ...\.}.}.n.|.|..
+00002c80: 027d 107d 1174 0f6a 107c 0d7c 0f7c 006a  .}.}.t.j.|.|.|.j
+00002c90: 016a 1164 088d 037d 127c 006a 1273 8074  .j.d...}.|.j.s.t
+00002ca0: 1383 007c 005f 1274 0364 0983 0101 0074  ...|._.t.d.....t
+00002cb0: 0f6a 107c 0c7c 0e7c 006a 016a 1164 088d  .j.|.|.|.j.j.d..
+00002cc0: 037d 137c 1364 0a66 027c 1264 0b66 0267  .}.|.d.f.|.d.f.g
+00002cd0: 027d 147c 006a 1473 9d74 1583 007c 005f  .}.|.j.s.t...|._
+00002ce0: 1474 0364 0c83 0101 0074 0f6a 167c 017c  .t.d.....t.j.|.|
+00002cf0: 137c 067c 006a 016a 177c 147c 006a 146a  .|.|.j.j.|.|.j.j
+00002d00: 1864 0d8d 067d 1574 0f6a 107c 107c 117c  .d...}.t.j.|.|.|
+00002d10: 006a 016a 1164 088d 037d 167c 15a0 197c  .j.j.d...}.|...|
+00002d20: 16a1 017d 177c 08a0 1a74 1b7c 117c 1764  ...}.|...t.|.|.d
+00002d30: 0664 0e8d 03a1 0101 0071 2974 1ca0 1d74  .d.......q)t...t
+00002d40: 1ca0 1e7c 08a1 01a1 017d 187c 006a 1f72  ...|.....}.|.j.r
+00002d50: f57c 006a 0172 f574 207c 006a 1f6a 2183  .|.j.r.t |.j.j!.
+00002d60: 0164 0f6b 0272 df64 0f7d 196e 087c 006a  .d.k.r.d.}.n.|.j
+00002d70: 1f6a 2164 1019 0064 1117 007d 197c 006a  .j!d...d...}.|.j
+00002d80: 1f6a 227c 1964 127c 006a 017c 017c 1864  .j"|.d.|.j.|.|.d
+00002d90: 1364 0664 148d 0701 007c 1853 0029 154e  .d.d.....|.S.).N
+00002da0: 7233 0000 0072 3400 0000 7a3e 436f 756c  r3...r4...z>Coul
+00002db0: 6420 6e6f 7420 6669 6e64 2054 7261 696e  d not find Train
+00002dc0: 696e 6720 636f 6e66 6967 2e20 4661 6c6c  ing config. Fall
+00002dd0: 696e 6720 6261 636b 2074 6f20 6465 6661  ing back to defa
+00002de0: 756c 7420 7661 6c75 6573 5429 03da 086e  ult valuesT)...n
+00002df0: 5f73 706c 6974 7372 6f00 0000 7257 0000  _splitsro...rW..
+00002e00: 0046 722f 0000 0072 6500 0000 7a49 436f  .Fr/...re...zICo
+00002e10: 756c 6420 6e6f 7420 6669 6e64 2058 6762  uld not find Xgb
+00002e20: 6f6f 7374 4669 6e61 6c50 6172 616d 436f  oostFinalParamCo
+00002e30: 6e66 6967 2e20 4661 6c6c 696e 6720 6261  nfig. Falling ba
+00002e40: 636b 2074 6f20 6465 6661 756c 7420 7365  ck to default se
+00002e50: 7474 696e 6773 2e72 3100 0000 7232 0000  ttings.r1...r2..
+00002e60: 007a 4143 6f75 6c64 206e 6f74 2066 696e  .zACould not fin
+00002e70: 6420 5867 626f 6f73 7454 756e 6550 6172  d XgboostTunePar
+00002e80: 616d 7343 6f6e 6669 672e 2046 616c 6c69  amsConfig. Falli
+00002e90: 6e67 2062 6163 6b20 746f 2064 6566 6175  ng back to defau
+00002ea0: 6c74 732e 7236 0000 0072 d000 0000 7201  lts.r6...r....r.
+00002eb0: 0000 0072 7100 0000 7235 0000 00da 096f  ...rq...r5.....o
+00002ec0: 6f66 5f73 636f 7265 72cb 0000 0072 7300  of_scorer....rs.
+00002ed0: 0000 2923 724d 0000 0072 1700 0000 720b  ..)#rM...r....r.
+00002ee0: 0000 0072 1100 0000 720a 0000 0072 4e00  ...r....r....rN.
+00002ef0: 0000 7220 0000 00da 0965 6e75 6d65 7261  ..r .....enumera
+00002f00: 7465 da05 7370 6c69 74da 0661 7374 7970  te..split..astyp
+00002f10: 65da 0369 6e74 da04 696c 6f63 721b 0000  e..int..ilocr...
+00002f20: 0072 4600 0000 7247 0000 0072 4f00 0000  .rF...rG...rO...
+00002f30: 7291 0000 0072 9200 0000 7219 0000 0072  r....r....r....r
+00002f40: 0c00 0000 7218 0000 0072 2700 0000 7231  ....r....r'...r1
+00002f50: 0000 0072 3800 0000 72d3 0000 0072 d400  ...r8...r....r..
+00002f60: 0000 72e0 0000 0072 0900 0000 721d 0000  ..r....r....r...
+00002f70: 0072 9a00 0000 da07 6173 6172 7261 7972  .r......asarrayr
+00002f80: 1a00 0000 729b 0000 0072 7400 0000 729c  ....r....rt...r.
+00002f90: 0000 0029 1a72 2200 0000 72f3 0000 0072  ...).r"...r....r
+00002fa0: 2900 0000 722b 0000 0072 2a00 0000 722c  )...r+...r*...r,
+00002fb0: 0000 0072 3300 0000 da0a 7374 7261 7469  ...r3.....strati
+00002fc0: 6669 6572 da0b 666f 6c64 5f6c 6f73 7365  fier..fold_losse
+00002fd0: 73da 035f 666e da07 7472 6e5f 6964 78da  s.._fn..trn_idx.
+00002fe0: 0776 616c 5f69 6478 da0c 585f 7472 6169  .val_idx..X_trai
+00002ff0: 6e5f 666f 6c64 da0a 585f 7661 6c5f 666f  n_fold..X_val_fo
+00003000: 6c64 da0c 795f 7472 6169 6e5f 666f 6c64  ld..y_train_fold
+00003010: da0a 795f 7661 6c5f 666f 6c64 da0b 585f  ..y_val_fold..X_
+00003020: 7465 7374 5f66 6f6c 64da 0b79 5f74 6573  test_fold..y_tes
+00003030: 745f 666f 6c64 7252 0000 0072 5100 0000  t_foldrR...rQ...
+00003040: 7253 0000 0072 1c00 0000 72ea 0000 0072  rS...r....r....r
+00003050: d500 0000 5a08 6d73 655f 6d65 616e 72a2  ....Z.mse_meanr.
+00003060: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00003070: 0000 7297 0000 00ff 0100 0073 b000 0000  ..r........s....
+00003080: 0c08 0602 0801 0801 0202 0601 0201 0601  ................
+00003090: 06fd 0406 0201 1001 10ff 0804 0801 06fe  ................
+000030a0: 0805 0801 06fe 0604 0604 0401 02ff 02fd  ................
+000030b0: 0201 0201 0c07 02fd 0201 0201 0605 0601  ................
+000030c0: 04ff 02fd 0201 0401 0a05 0402 0201 0201  ................
+000030d0: 0601 06fd 0606 0801 0201 0201 04ff 0404  ................
+000030e0: 0201 0201 0601 06fd 1005 0602 0801 0201  ................
+000030f0: 0201 04ff 0403 0201 0201 0201 0601 0201  ................
+00003100: 0601 06fa 0408 0201 0201 0601 06fd 0a05  ................
+00003110: 1601 1002 0c02 1002 0601 1002 0601 0201  ................
+00003120: 0201 0401 0201 0201 0201 0201 06f9 0409  ................
+00003130: 7a29 5867 626f 6f73 744d 6f64 656c 5265  z)XgboostModelRe
+00003140: 6772 6573 7369 6f6e 2e5f 6669 6e65 5f74  gression._fine_t
+00003150: 756e 655f 7072 6563 6973 6563 0500 0000  une_precisec....
+00003160: 0000 0000 0000 0000 0c00 0000 0a00 0000  ................
+00003170: 0300 0000 7388 0200 0074 0074 01a0 02a1  ....s....t.t....
+00003180: 009b 0064 019d 0283 0101 0088 006a 0372  ...d.........j.r
+00003190: 1588 006a 0472 1588 006a 0572 1588 006a  ...j.r...j.r...j
+000031a0: 0673 1974 0764 0283 0182 0187 0087 0187  .s.t.d..........
+000031b0: 0287 0387 0466 0564 0364 0484 087d 0588  .....f.d.d...}..
+000031c0: 00a0 08a1 0001 0074 0988 006a 036a 0a64  .......t...j.j.d
+000031d0: 0519 0074 0b83 0272 a774 0988 006a 036a  ...t...r.t...j.j
+000031e0: 0a64 0619 0074 0b83 0272 a774 0988 006a  .d...t...r.t...j
+000031f0: 036a 0a64 0719 0074 0b83 0272 a774 0988  .j.d...t...r.t..
+00003200: 006a 036a 0a64 0819 0074 0b83 0272 a774  .j.j.d...t...r.t
+00003210: 0c6a 0d88 006a 036a 0a64 0519 0064 0914  .j...j.j.d...d..
+00003220: 0088 006a 036a 0a64 0519 0064 0a14 0088  ...j.j.d...d....
+00003230: 006a 046a 0e74 0b64 0b8d 0474 0c6a 0d88  .j.j.t.d...t.j..
+00003240: 006a 036a 0a64 0619 0064 0914 0088 006a  .j.j.d...d.....j
+00003250: 036a 0a64 0619 0064 0a14 0088 006a 046a  .j.d...d.....j.j
+00003260: 0e74 0b64 0b8d 0474 0c6a 0d88 006a 036a  .t.d...t.j...j.j
+00003270: 0a64 0719 0064 0914 0088 006a 036a 0a64  .d...d.....j.j.d
+00003280: 0719 0064 0a14 0088 006a 046a 0e74 0b64  ...d.....j.j.t.d
+00003290: 0b8d 0474 0c6a 0d88 006a 036a 0a64 0819  ...t.j...j.j.d..
+000032a0: 0064 0914 0088 006a 036a 0a64 0819 0064  .d.....j.j.d...d
+000032b0: 0a14 0088 006a 046a 0e74 0b64 0b8d 0464  .....j.j.t.d...d
+000032c0: 0c9c 047d 066e 0474 0764 0d83 0101 0088  ...}.n.t.d......
+000032d0: 00a0 0fa1 007d 0774 106a 1164 0e74 106a  .....}.t.j.d.t.j
+000032e0: 12a0 137c 06a1 0164 0f8d 027d 087c 086a  ...|...d...}.|.j
+000032f0: 147c 0588 006a 046a 0e74 157c 06a0 16a1  .|...j.j.t.|....
+00003300: 0083 0113 0088 006a 046a 1764 1064 1064  .......j.j.d.d.d
+00003310: 118d 0501 007a 1674 106a 18a0 197c 08a1  .....z.t.j...|..
+00003320: 017d 097c 09a0 1aa1 0001 0074 106a 18a0  .}.|.......t.j..
+00003330: 1b7c 08a1 017d 097c 09a0 1aa1 0001 0057  .|...}.|.......W
+00003340: 006e 0c04 0074 1c74 1d74 0766 0379 f001  .n...t.t.t.f.y..
+00003350: 0001 0001 0059 006e 0177 0088 00a0 0fa1  .....Y.n.w......
+00003360: 007d 0a7c 0a7c 076b 0073 fe88 006a 046a  .}.|.|.k.s...j.j
+00003370: 1e90 0173 387c 086a 1f6a 0a7d 0b7c 0b64  ...s8|.j.j.}.|.d
+00003380: 0519 0088 006a 036a 0a64 053c 007c 0b64  .....j.j.d.<.|.d
+00003390: 0619 0088 006a 036a 0a64 063c 007c 0b64  .....j.j.d.<.|.d
+000033a0: 0719 0088 006a 036a 0a64 073c 007c 0b64  .....j.j.d.<.|.d
+000033b0: 0819 0088 006a 036a 0a64 083c 0074 0064  .....j.j.d.<.t.d
+000033c0: 127c 079b 0064 137c 0a9b 0064 149d 0583  .|...d.|...d....
+000033d0: 0101 0074 0064 1588 006a 036a 0a9b 009d  ...t.d...j.j....
+000033e0: 0283 0101 0064 0053 0074 0064 167c 079b  .....d.S.t.d.|..
+000033f0: 0064 177c 0a9b 009d 0483 0101 0064 0053  .d.|.........d.S
+00003400: 0029 184e 7a31 3a20 5374 6172 7420 6772  .).Nz1: Start gr
+00003410: 6964 2073 6561 7263 6820 6669 6e65 2074  id search fine t
+00003420: 756e 696e 6720 6f66 2058 6762 6f6f 7374  uning of Xgboost
+00003430: 206d 6f64 656c 2e72 5500 0000 6301 0000   model.rU...c...
+00003440: 0000 0000 0000 0000 000d 0000 000b 0000  ................
+00003450: 0013 0000 0073 c801 0000 8800 a000 8802  .....s..........
+00003460: 8804 8801 8803 a104 5c02 7d01 7d02 7401  ........\.}.}.t.
+00003470: 6a02 a003 7c00 6401 a102 7d03 7404 8800  j...|.d...}.t...
+00003480: 6a05 6a06 8301 7d04 7c00 6a07 6402 8800  j.j...}.|.j.d...
+00003490: 6a05 6a06 6402 1900 6403 1400 8800 6a05  j.j.d...d.....j.
+000034a0: 6a06 6402 1900 6404 1400 6405 6406 8d04  j.d...d...d.d...
+000034b0: 7d05 7c00 6a07 6407 8800 6a05 6a06 6407  }.|.j.d...j.j.d.
+000034c0: 1900 6403 1400 8800 6a05 6a06 6407 1900  ..d.....j.j.d...
+000034d0: 6404 1400 6405 6406 8d04 7d06 7c00 6a07  d...d.d...}.|.j.
+000034e0: 6408 8800 6a05 6a06 6408 1900 6403 1400  d...j.j.d...d...
+000034f0: 8800 6a05 6a06 6408 1900 6404 1400 6405  ..j.j.d...d...d.
+00003500: 6406 8d04 7d07 7c00 6a07 6409 8800 6a05  d...}.|.j.d...j.
+00003510: 6a06 6409 1900 6403 1400 8800 6a05 6a06  j.d...d.....j.j.
+00003520: 6409 1900 6404 1400 6405 6406 8d04 7d08  d...d...d.d...}.
+00003530: 7c05 7c04 6402 3c00 7c06 7c04 6407 3c00  |.|.d.<.|.|.d.<.
+00003540: 7c07 7c04 6408 3c00 7c08 7c04 6409 3c00  |.|.d.<.|.|.d.<.
+00003550: 7c04 a008 640a 640b a102 7d09 8800 6a09  |...d.d...}...j.
+00003560: 6a0a 640c 6b02 7291 8800 a00b 7c01 7c02  j.d.k.r.....|.|.
+00003570: 8803 7c04 7c09 7c03 a106 5300 8800 6a09  ..|.|.|...S...j.
+00003580: 6a0a 640c 6b04 72a4 8800 6a09 6a0c 72a4  j.d.k.r...j.j.r.
+00003590: 8800 a00d 7c04 8802 8804 8801 8803 a105  ....|...........
+000035a0: 5300 740e 6a0f 7c04 7c01 7c09 8800 6a09  S.t.j.|.|.|...j.
+000035b0: 6a10 8800 6a09 6a0a 640d 8800 6a09 6a11  j...j.j.d...j.j.
+000035c0: 7c03 6701 8800 6a09 6a12 640e 8d09 7d0a  |.g...j.j.d...}.
+000035d0: 7c0a 640f 1900 a013 a100 7d0b 7414 8800  |.d.......}.t...
+000035e0: 6a15 6a16 8301 6410 6b02 72cc 6410 7d0c  j.j...d.k.r.d.}.
+000035f0: 6e08 8800 6a15 6a16 6411 1900 640c 1700  n...j.j.d...d...
+00003600: 7d0c 8800 6a15 6a17 7c0c 6412 8800 6a09  }...j.j.|.d...j.
+00003610: 7c04 7c0b 6413 6405 6414 8d07 0100 7c0b  |.|.d.d.d.....|.
+00003620: 5300 2915 4e72 6800 0000 7256 0000 00e7  S.).Nrh...rV....
+00003630: cdcc cccc cccc ec3f e79a 9999 9999 99f1  .......?........
+00003640: 3f46 7259 0000 0072 5c00 0000 725d 0000  ?FrY...r\...r]..
+00003650: 0072 5800 0000 7233 0000 0072 3400 0000  .rX...r3...r4...
+00003660: 7235 0000 0054 7269 0000 0072 7000 0000  r5...Tri...rp...
+00003670: 7201 0000 0072 7100 0000 7272 0000 0072  r....rq...rr...r
+00003680: cb00 0000 7273 0000 0029 1872 4b00 0000  ....rs...).rK...
+00003690: 723d 0000 0072 9300 0000 7294 0000 0072  r=...r....r....r
+000036a0: 0200 0000 7219 0000 0072 4c00 0000 727d  ....r....rL...r}
+000036b0: 0000 0072 4d00 0000 7217 0000 0072 4e00  ...rM...r....rN.
+000036c0: 0000 7295 0000 0072 9600 0000 7297 0000  ..r....r....r...
+000036d0: 0072 4f00 0000 7298 0000 0072 3800 0000  .rO...r....r8...
+000036e0: 7220 0000 0072 9900 0000 729a 0000 0072  r ...r....r....r
+000036f0: 9b00 0000 721a 0000 0072 7400 0000 729c  ....r....rt...r.
+00003700: 0000 0029 0d72 9d00 0000 7251 0000 0072  ...).r....rQ...r
+00003710: 5200 0000 729f 0000 0072 f300 0000 da0b  R...r....r......
+00003720: 616c 7068 615f 7370 6163 65da 0c6c 616d  alpha_space..lam
+00003730: 6264 615f 7370 6163 65da 0b67 616d 6d61  bda_space..gamma
+00003740: 5f73 7061 6365 da09 6574 615f 7370 6163  _space..eta_spac
+00003750: 6572 3300 0000 72a0 0000 0072 a100 0000  er3...r....r....
+00003760: 72a2 0000 00a9 0572 2200 0000 722a 0000  r......r"...r*..
+00003770: 0072 2900 0000 722c 0000 0072 2b00 0000  .r)...r,...r+...
+00003780: 7223 0000 0072 2400 0000 7262 0000 0080  r#...r$...rb....
+00003790: 0200 0073 9200 0000 1401 0602 0401 04ff  ...s............
+000037a0: 0c04 0401 0201 0e01 0e01 0201 06fc 0406  ................
+000037b0: 0201 0e01 0e01 0201 06fc 0406 0201 0e01  ................
+000037c0: 0e01 0201 06fc 0406 0201 0e01 0e01 0201  ................
+000037d0: 06fc 0807 0801 0801 0801 0c02 0c02 0401  ................
+000037e0: 0c01 04ff 0c04 0601 02ff 0403 0201 0201  ................
+000037f0: 0201 0201 0201 04fb 0408 0201 0201 0201  ................
+00003800: 0601 0601 0201 0601 0401 0601 06f7 0c0c  ................
+00003810: 1003 0601 1002 0601 0201 0201 0401 0201  ................
+00003820: 0201 0201 0201 06f9 040a 7a33 5867 626f  ..........z3Xgbo
+00003830: 6f73 744d 6f64 656c 5265 6772 6573 7369  ostModelRegressi
+00003840: 6f6e 2e66 696e 655f 7475 6e65 2e3c 6c6f  on.fine_tune.<lo
+00003850: 6361 6c73 3e2e 6f62 6a65 6374 6976 6572  cals>.objectiver
+00003860: 5600 0000 725c 0000 0072 5d00 0000 7258  V...r\...r]...rX
+00003870: 0000 0072 0701 0000 7208 0100 0029 01da  ...r....r....)..
+00003880: 0564 7479 7065 2904 7256 0000 0072 5c00  .dtype).rV...r\.
+00003890: 0000 725d 0000 0072 5800 0000 7a29 536f  ..r]...rX...z)So
+000038a0: 6d65 2070 6172 616d 6574 6572 7320 6172  me parameters ar
+000038b0: 6520 6e6f 7420 666c 6f61 7473 206f 7220  e not floats or 
+000038c0: 7374 7269 6e67 7372 a800 0000 2902 72a9  stringsr....).r.
+000038d0: 0000 0072 aa00 0000 5472 ac00 0000 7a26  ...r....Tr....z&
+000038e0: 4772 6964 2073 6561 7263 6820 696d 7072  Grid search impr
+000038f0: 6f76 6564 2065 7661 6c20 6d65 7472 6963  oved eval metric
+00003900: 2066 726f 6d20 7a04 2074 6f20 da01 2e72   from z. to ...r
+00003910: b100 0000 7a2d 4772 6964 2073 6561 7263  ....z-Grid searc
+00003920: 6820 636f 756c 6420 6e6f 7420 696d 7072  h could not impr
+00003930: 6f76 6520 6576 616c 206d 6574 7269 6320  ove eval metric 
+00003940: 6f66 207a 192e 2042 6573 7420 7363 6f72  of z.. Best scor
+00003950: 6520 7265 6163 6865 6420 7761 7320 2920  e reached was ) 
+00003960: 7211 0000 0072 0300 0000 7226 0000 0072  r....r....r&...r
+00003970: 1900 0000 7217 0000 0072 1800 0000 721a  ....r....r....r.
+00003980: 0000 0072 3b00 0000 7228 0000 00da 0a69  ...r;...r(.....i
+00003990: 7369 6e73 7461 6e63 6572 4c00 0000 da05  sinstancerL.....
+000039a0: 666c 6f61 7472 1d00 0000 da08 6c69 6e73  floatr......lins
+000039b0: 7061 6365 da21 6772 6964 7365 6172 6368  pace.!gridsearch
+000039c0: 5f6e 625f 7061 7261 6d65 7465 7273 5f70  _nb_parameters_p
+000039d0: 6572 5f67 7269 6472 cd00 0000 723d 0000  er_gridr....r=..
+000039e0: 0072 ba00 0000 72b7 0000 00da 0b47 7269  .r....r......Gri
+000039f0: 6453 616d 706c 6572 72bb 0000 0072 9b00  dSamplerr....r..
+00003a00: 0000 da04 6b65 7973 da22 6772 6964 7365  ....keys."gridse
+00003a10: 6172 6368 5f74 756e 696e 675f 6d61 785f  arch_tuning_max_
+00003a20: 7275 6e74 696d 655f 7365 6373 72be 0000  runtime_secsr...
+00003a30: 0072 bf00 0000 72c0 0000 0072 c100 0000  .r....r....r....
+00003a40: 72c2 0000 0072 c300 0000 7241 0000 0072  r....r....rA...r
+00003a50: c400 0000 290c 7222 0000 0072 2900 0000  ....).r"...r)...
+00003a60: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00003a70: 6200 0000 da0c 7365 6172 6368 5f73 7061  b.....search_spa
+00003a80: 6365 da0d 6265 7374 5f73 636f 7265 5f63  ce..best_score_c
+00003a90: 7672 c800 0000 72c9 0000 0072 cf00 0000  vr....r....r....
+00003aa0: da17 7867 626f 6f73 745f 6772 6964 5f62  ..xgboost_grid_b
+00003ab0: 6573 745f 7061 7261 6d72 2300 0000 720d  est_paramr#...r.
+00003ac0: 0100 0072 2400 0000 7245 0000 006e 0200  ...r$...rE...n..
+00003ad0: 0073 ae00 0000 1207 0402 02ff 0402 02fe  .s..............
+00003ae0: 0403 02fd 0404 02fc 0206 0201 04ff 1404  ................
+00003af0: 0857 1002 02ff 1002 02fe 1003 02fd 1004  .W..............
+00003b00: 02fc 0407 0a01 0201 02ff 0e02 0601 0201  ................
+00003b10: 04fb 0407 0e01 0e01 0601 0201 04fc 0406  ................
+00003b20: 0e01 0e01 0601 0201 04fc 0406 0e01 0e01  ................
+00003b30: 0601 0201 04fc 08ec 081c 0802 0402 0c01  ................
+00003b40: 06ff 0403 0201 0601 0a01 02ff 0602 0201  ................
+00003b50: 0201 06fa 0209 0c01 0801 0c01 0c01 1201  ................
+00003b60: 0401 02ff 0803 1202 0801 1001 0201 0201  ................
+00003b70: 0cff 1003 1001 0201 1001 04ff 1603 0202  ................
+00003b80: 0e01 08ff 7a20 5867 626f 6f73 744d 6f64  ....z XgboostMod
+00003b90: 656c 5265 6772 6573 7369 6f6e 2e66 696e  elRegression.fin
+00003ba0: 655f 7475 6e65 da02 6466 6302 0000 0000  e_tune..dfc.....
+00003bb0: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+00003bc0: 0000 0073 8800 0000 7400 7401 a002 a100  ...s....t.t.....
+00003bd0: 9b00 6401 9d02 8301 0100 7c00 6a03 720f  ..d.......|.j.r.
+00003be0: 7c00 6a04 7313 7405 6402 8301 8201 7c00  |.j.s.t.d.....|.
+00003bf0: 6a06 7221 7c00 6a06 6a07 7c01 6403 6404  j.r!|.j.j.|.d.d.
+00003c00: 6405 8d03 5c02 7d01 7d02 7408 6a09 7c01  d...\.}.}.t.j.|.
+00003c10: 7c00 6a04 6a0a 6406 8d02 7d03 7c00 6a0b  |.j.j.d...}.|.j.
+00003c20: 7331 740c 6407 8301 8201 7c00 6a0d 7338  s1t.d.....|.j.s8
+00003c30: 740c 6408 8301 8201 7c00 6a0b a00e 7c03  t.d.....|.j...|.
+00003c40: a101 7d04 7400 6409 8301 0100 7c04 5300  ..}.t.d.....|.S.
+00003c50: 290a 7a17 5072 6564 6963 7420 6f6e 2075  ).z.Predict on u
+00003c60: 6e73 6565 6e20 6461 7461 2e7a 333a 2053  nseen data.z3: S
+00003c70: 7461 7274 2070 7265 6469 6374 696e 6720  tart predicting 
+00003c80: 6f6e 206e 6577 2064 6174 6120 7573 696e  on new data usin
+00003c90: 6720 5867 626f 6f73 7420 6d6f 6465 6c2e  g Xgboost model.
+00003ca0: 7a2c 636f 6e66 5f70 6172 616d 735f 7867  z,conf_params_xg
+00003cb0: 626f 6f73 7420 6f72 2063 6f6e 665f 7472  boost or conf_tr
+00003cc0: 6169 6e69 6e67 2069 7320 4e6f 6e65 4e54  aining is NoneNT
+00003cd0: 722f 0000 0029 0172 6700 0000 7a20 4e6f  r/...).rg...z No
+00003ce0: 2074 7261 696e 6564 206d 6f64 656c 2068   trained model h
+00003cf0: 6173 2062 6565 6e20 666f 756e 642e 7a2b  as been found.z+
+00003d00: 4e6f 206d 6f64 656c 2063 6f6e 6669 6775  No model configu
+00003d10: 7261 7469 6f6e 2066 696c 6520 6861 7320  ration file has 
+00003d20: 6265 656e 2066 6f75 6e64 2e7a 1346 696e  been found.z.Fin
+00003d30: 6973 6865 6420 7072 6564 6963 7469 6e67  ished predicting
+00003d40: 290f 7211 0000 0072 0300 0000 7226 0000  ).r....r....r&..
+00003d50: 0072 1800 0000 7217 0000 0072 3b00 0000  .r....r....r;...
+00003d60: 721b 0000 0072 4700 0000 724f 0000 0072  r....rG...rO...r
+00003d70: 9100 0000 7292 0000 0072 1c00 0000 da09  ....r....r......
+00003d80: 4578 6365 7074 696f 6e72 1900 0000 72d4  Exceptionr....r.
+00003d90: 0000 0029 0572 2200 0000 721a 0100 00da  ...).r"...r.....
+00003da0: 015f 7252 0000 0072 d500 0000 7223 0000  ._rR...r....r#..
+00003db0: 0072 2300 0000 7224 0000 0072 d400 0000  .r#...r$...r....
+00003dc0: 2503 0000 7328 0000 0002 020c 0104 ff0c  %...s(..........
+00003dd0: 0308 0106 0206 0106 010a ff04 0402 0106  ................
+00003de0: 0106 fe06 0508 0106 0208 010c 0208 0104  ................
+00003df0: 017a 1e58 6762 6f6f 7374 4d6f 6465 6c52  .z.XgboostModelR
+00003e00: 6567 7265 7373 696f 6e2e 7072 6564 6963  egression.predic
+00003e10: 7429 054e 4e4e 4e4e 2901 72d7 0000 0029  t).NNNNN).r....)
+00003e20: 24da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  $..__name__..__m
+00003e30: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00003e40: 616d 655f 5fda 075f 5f64 6f63 5f5f 7207  ame__..__doc__r.
+00003e50: 0000 0072 0800 0000 720b 0000 0072 2700  ...r....r....r'.
+00003e60: 0000 720c 0000 0072 0e00 0000 7213 0000  ..r....r....r...
+00003e70: 0072 2500 0000 7228 0000 0072 4900 0000  .r%...r(...rI...
+00003e80: da09 4461 7461 4672 616d 65da 0653 6572  ..DataFrame..Ser
+00003e90: 6965 7372 4f00 0000 da07 426f 6f73 7465  iesrO.....Booste
+00003ea0: 7272 5400 0000 7242 0000 0072 cd00 0000  rrT...rB...r....
+00003eb0: 724b 0000 0072 9500 0000 72f9 0000 0072  rK...r....r....r
+00003ec0: ec00 0000 7206 0000 0072 1101 0000 72f2  ....r....r....r.
+00003ed0: 0000 0072 0500 0000 da03 7374 7272 0400  ...r......strr..
+00003ee0: 0000 7297 0000 0072 4500 0000 721d 0000  ..r....rE...r...
+00003ef0: 00da 076e 6461 7272 6179 72d4 0000 0072  ...ndarrayr....r
+00003f00: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
+00003f10: 0000 0072 1400 0000 1d00 0000 73a0 0000  ...r........s...
+00003f20: 0008 0004 0102 0502 0102 0102 0102 0104  ................
+00003f30: f906 0202 fe06 0302 fd06 0402 fc06 0502  ................
+00003f40: fb06 0602 fa06 070a f908 1802 1504 0202  ................
+00003f50: fe04 0302 fd04 0402 fc04 0502 fb04 060a  ................
+00003f60: fa02 4a04 0202 fe04 0302 fd04 0402 fc04  ..J.............
+00003f70: 0502 fb02 060a fa00 7f08 6808 1308 0d02  ..........h.....
+00003f80: 2104 ff04 0102 ff04 0102 ff02 010a ff16  !...............
+00003f90: 2402 1d0a 0202 fe04 0302 fd04 0402 fc04  $...............
+00003fa0: 0502 fb04 060a fa02 6f04 0202 fe04 0302  ........o.......
+00003fb0: fd04 0402 fc04 0502 fb02 060a fa00 7f1a  ................
+00003fc0: 3872 1400 0000 2925 7220 0100 00da 0463  8r....)%r .....c
+00003fd0: 6f70 7972 0200 0000 7203 0000 00da 0674  opyr....r......t
+00003fe0: 7970 696e 6772 0400 0000 7205 0000 0072  ypingr....r....r
+00003ff0: 0600 0000 7207 0000 0072 0800 0000 da05  ....r....r......
+00004000: 6e75 6d70 7972 1d00 0000 723d 0000 00da  numpyr....r=....
+00004010: 0670 616e 6461 7372 4900 0000 72a5 0000  .pandasrI...r...
+00004020: 0072 4f00 0000 da0f 736b 6c65 6172 6e2e  .rO.....sklearn.
+00004030: 6d65 7472 6963 7372 0900 0000 da17 736b  metricsr......sk
+00004040: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
+00004050: 6374 696f 6e72 0a00 0000 da1f 626c 7565  ctionr......blue
+00004060: 6361 7374 2e63 6f6e 6669 672e 7472 6169  cast.config.trai
+00004070: 6e69 6e67 5f63 6f6e 6669 6772 0b00 0000  ning_configr....
+00004080: 720c 0000 0072 0d00 0000 7227 0000 00da  r....r....r'....
+00004090: 2162 6c75 6563 6173 742e 6578 7065 7269  !bluecast.experi
+000040a0: 6d65 6e74 6174 696f 6e2e 7472 6163 6b69  mentation.tracki
+000040b0: 6e67 720e 0000 00da 2462 6c75 6563 6173  ngr.....$bluecas
+000040c0: 742e 6765 6e65 7261 6c5f 7574 696c 732e  t.general_utils.
+000040d0: 6765 6e65 7261 6c5f 7574 696c 7372 0f00  general_utilsr..
+000040e0: 0000 7210 0000 0072 1100 0000 da22 626c  ..r....r....."bl
+000040f0: 7565 6361 7374 2e6d 6c5f 6d6f 6465 6c6c  uecast.ml_modell
+00004100: 696e 672e 6261 7365 5f63 6c61 7373 6573  ing.base_classes
+00004110: 7212 0000 00da 1d62 6c75 6563 6173 742e  r......bluecast.
+00004120: 7072 6570 726f 6365 7373 696e 672e 6375  preprocessing.cu
+00004130: 7374 6f6d 7213 0000 0072 1400 0000 7223  stomr....r....r#
+00004140: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00004150: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00004160: 7322 0000 0004 000c 070c 011c 0108 0208  s"..............
+00004170: 0108 0108 010c 010c 0110 020c 010c 0314  ................
+00004180: 010c 010c 0114 03                        .......
```

### Comparing `bluecast-1.1/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-38.pyc` & `bluecast-1.2.4/bluecast/ml_modelling/__pycache__/xgboost_regression.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/ml_modelling/base_classes.py` & `bluecast-1.2.4/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/ml_modelling/xgboost.py` & `bluecast-1.2.4/bluecast/ml_modelling/xgboost.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from bluecast.config.training_config import (
     TrainingConfig,
     XgboostFinalParamConfig,
     XgboostTuneParamsConfig,
 )
 from bluecast.experimentation.tracking import ExperimentTracker
-from bluecast.general_utils.general_utils import check_gpu_support, logger
+from bluecast.general_utils.general_utils import check_gpu_support, log_sampling, logger
 from bluecast.ml_modelling.base_classes import BaseClassMlModel
 from bluecast.preprocessing.custom import CustomPreprocessing
 
 
 class XgboostModel(BaseClassMlModel):
     """Train and/or tune Xgboost classification model."""
 
@@ -187,14 +187,33 @@
             or not self.conf_xgboost
             or not self.experiment_tracker
         ):
             raise ValueError(
                 "At least one of the configs or experiment_tracker is None, which is not allowed"
             )
 
+        if self.conf_training.sample_data_during_tuning:
+            nb_samples_train = log_sampling(
+                len(x_train.index),
+                alpha=self.conf_training.sample_data_during_tuning_alpha,
+            )
+            nb_samples_test = log_sampling(
+                len(x_test.index),
+                alpha=self.conf_training.sample_data_during_tuning_alpha,
+            )
+
+            x_train = x_train.sample(
+                nb_samples_train, random_state=self.conf_training.global_random_state
+            )
+            y_train = y_train.loc[x_train.index]
+            x_test = x_test.sample(
+                nb_samples_test, random_state=self.conf_training.global_random_state
+            )
+            y_test = y_test.loc[x_test.index]
+
         def objective(trial):
             param = {
                 "objective": self.conf_xgboost.xgboost_objective,
                 "booster": self.conf_xgboost.booster,
                 "eval_metric": self.conf_xgboost.xgboost_eval_metric,
                 "num_class": y_train.nunique(),
                 "eta": trial.suggest_float(
@@ -223,18 +242,18 @@
                 ),
                 "gamma": trial.suggest_float(
                     "gamma",
                     self.conf_xgboost.gamma_min,
                     self.conf_xgboost.gamma_max,
                     log=True,
                 ),
-                "max_leaves": trial.suggest_int(
-                    "max_leaves",
-                    self.conf_xgboost.max_leaves_min,
-                    self.conf_xgboost.max_leaves_max,
+                "min_child_weight": trial.suggest_int(
+                    "min_child_weight",
+                    self.conf_xgboost.min_child_weight_min,
+                    self.conf_xgboost.min_child_weight_max,
                 ),
                 "subsample": trial.suggest_float(
                     "subsample",
                     self.conf_xgboost.sub_sample_min,
                     self.conf_xgboost.sub_sample_max,
                 ),
                 "colsample_bytree": trial.suggest_float(
@@ -252,14 +271,15 @@
                     self.conf_xgboost.steps_min,
                     self.conf_xgboost.steps_max,
                     log=True,
                 ),
             }
             param = {**param, **train_on}
             sample_weight = trial.suggest_categorical("sample_weight", [True, False])
+
             if sample_weight:
                 classes_weights = self.calculate_class_weights(y_train)
                 d_train = xgb.DMatrix(
                     x_train,
                     label=y_train,
                     weight=classes_weights,
                     enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
@@ -302,17 +322,15 @@
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
-                adjusted_score = result["test-mlogloss-mean"].mean() + (
-                    result["test-mlogloss-mean"].std() ** 0.7
-                )
+                adjusted_score = result["test-mlogloss-mean"].mean()
 
                 # track results
                 if len(self.experiment_tracker.experiment_id) == 0:
                     new_id = 0
                 else:
                     new_id = self.experiment_tracker.experiment_id[-1] + 1
                 self.experiment_tracker.add_results(
@@ -365,15 +383,15 @@
             "num_class": y_train.nunique(),
             "max_depth": xgboost_best_param[
                 "max_depth"
             ],  # maximum depth of the decision trees being trained
             "alpha": xgboost_best_param["alpha"],
             "lambda": xgboost_best_param["lambda"],
             "gamma": xgboost_best_param["gamma"],
-            "max_leaves": xgboost_best_param["max_leaves"],
+            "min_child_weight": xgboost_best_param["min_child_weight"],
             "subsample": xgboost_best_param["subsample"],
             "colsample_bytree": xgboost_best_param["colsample_bytree"],
             "colsample_bylevel": xgboost_best_param["colsample_bylevel"],
             "eta": xgboost_best_param["eta"],
             "steps": xgboost_best_param["steps"],
         }
         self.conf_params_xgboost.params = {
@@ -729,17 +747,15 @@
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
-                adjusted_score = result["test-mlogloss-mean"].mean() + (
-                    result["test-mlogloss-mean"].std() ** 0.7
-                )
+                adjusted_score = result["test-mlogloss-mean"].mean()
 
                 # track results
                 if len(self.experiment_tracker.experiment_id) == 0:
                     new_id = 0
                 else:
                     new_id = self.experiment_tracker.experiment_id[-1] + 1
                 self.experiment_tracker.add_results(
```

### Comparing `bluecast-1.1/bluecast/ml_modelling/xgboost_regression.py` & `bluecast-1.2.4/bluecast/ml_modelling/xgboost_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from sklearn.model_selection import KFold
 
 from bluecast.config.training_config import TrainingConfig, XgboostFinalParamConfig
 from bluecast.config.training_config import (
     XgboostTuneParamsRegressionConfig as XgboostTuneParamsConfig,
 )
 from bluecast.experimentation.tracking import ExperimentTracker
-from bluecast.general_utils.general_utils import check_gpu_support, logger
+from bluecast.general_utils.general_utils import check_gpu_support, log_sampling, logger
 from bluecast.ml_modelling.base_classes import BaseClassMlRegressionModel
 from bluecast.preprocessing.custom import CustomPreprocessing
 
 
 class XgboostModelRegression(BaseClassMlRegressionModel):
     """Train and/or tune Xgboost regression model."""
 
@@ -179,14 +179,33 @@
             or not self.conf_xgboost
             or not self.experiment_tracker
         ):
             raise ValueError(
                 "At least one of the configs or experiment_tracker is None, which is not allowed"
             )
 
+        if self.conf_training.sample_data_during_tuning:
+            nb_samples_train = log_sampling(
+                len(x_train.index),
+                alpha=self.conf_training.sample_data_during_tuning_alpha,
+            )
+            nb_samples_test = log_sampling(
+                len(x_test.index),
+                alpha=self.conf_training.sample_data_during_tuning_alpha,
+            )
+
+            x_train = x_train.sample(
+                nb_samples_train, random_state=self.conf_training.global_random_state
+            )
+            y_train = y_train.loc[x_train.index]
+            x_test = x_test.sample(
+                nb_samples_test, random_state=self.conf_training.global_random_state
+            )
+            y_test = y_test.loc[x_test.index]
+
         def objective(trial):
             param = {
                 "objective": self.conf_xgboost.xgboost_objective,
                 "booster": self.conf_xgboost.booster,
                 "eval_metric": self.conf_xgboost.xgboost_eval_metric,
                 "eta": trial.suggest_float(
                     "eta",
@@ -214,18 +233,18 @@
                 ),
                 "gamma": trial.suggest_float(
                     "gamma",
                     self.conf_xgboost.lambda_min,
                     self.conf_xgboost.lambda_max,
                     log=True,
                 ),
-                "max_leaves": trial.suggest_int(
-                    "max_leaves",
-                    self.conf_xgboost.max_leaves_min,
-                    self.conf_xgboost.max_leaves_max,
+                "min_child_weight": trial.suggest_int(
+                    "min_child_weight",
+                    self.conf_xgboost.min_child_weight_min,
+                    self.conf_xgboost.min_child_weight_max,
                 ),
                 "subsample": trial.suggest_float(
                     "subsample",
                     self.conf_xgboost.sub_sample_min,
                     self.conf_xgboost.sub_sample_max,
                 ),
                 "colsample_bytree": trial.suggest_float(
@@ -283,17 +302,15 @@
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
-                adjusted_score = result["test-rmse-mean"].mean() + (
-                    result["test-rmse-mean"].std() ** 0.7
-                )
+                adjusted_score = result["test-rmse-mean"].mean()
 
                 # track results
                 if len(self.experiment_tracker.experiment_id) == 0:
                     new_id = 0
                 else:
                     new_id = self.experiment_tracker.experiment_id[-1] + 1
                 self.experiment_tracker.add_results(
@@ -345,15 +362,15 @@
             "eval_metric": self.conf_xgboost.xgboost_eval_metric,
             "max_depth": xgboost_best_param[
                 "max_depth"
             ],  # maximum depth of the decision trees being trained
             "alpha": xgboost_best_param["alpha"],
             "lambda": xgboost_best_param["lambda"],
             "gamma": xgboost_best_param["gamma"],
-            "max_leaves": xgboost_best_param["max_leaves"],
+            "min_child_weight": xgboost_best_param["min_child_weight"],
             "subsample": xgboost_best_param["subsample"],
             "colsample_bytree": xgboost_best_param["colsample_bytree"],
             "colsample_bylevel": xgboost_best_param["colsample_bylevel"],
             "eta": xgboost_best_param["eta"],
             "steps": xgboost_best_param["steps"],
         }
         self.conf_params_xgboost.params = {
@@ -684,17 +701,15 @@
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
-                adjusted_score = result["test-rmse-mean"].mean() + (
-                    result["test-rmse-mean"].std() ** 0.7
-                )
+                adjusted_score = result["test-rmse-mean"].mean()
 
                 # track results
                 if len(self.experiment_tracker.experiment_id) == 0:
                     new_id = 0
                 else:
                     new_id = self.experiment_tracker.experiment_id[-1] + 1
                 self.experiment_tracker.add_results(
```

### Comparing `bluecast-1.1/bluecast/monitoring/__pycache__/data_monitoring.cpython-310.pyc` & `bluecast-1.2.4/bluecast/monitoring/__pycache__/data_monitoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/monitoring/data_monitoring.py` & `bluecast-1.2.4/bluecast/monitoring/data_monitoring.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/category_encoder_orchestration.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/category_encoder_orchestration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/onehot_encoding.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/onehot_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-1.2.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/category_encoder_orchestration.py` & `bluecast-1.2.4/bluecast/preprocessing/category_encoder_orchestration.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/custom.py` & `bluecast-1.2.4/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/datetime_features.py` & `bluecast-1.2.4/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/encode_target_labels.py` & `bluecast-1.2.4/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/feature_selection.py` & `bluecast-1.2.4/bluecast/preprocessing/feature_selection.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/feature_types.py` & `bluecast-1.2.4/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-1.2.4/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/onehot_encoding.py` & `bluecast-1.2.4/bluecast/preprocessing/onehot_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/schema_checks.py` & `bluecast-1.2.4/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/target_encoding.py` & `bluecast-1.2.4/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/preprocessing/train_test_split.py` & `bluecast-1.2.4/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_cast_cv_regression.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_cv_regression.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_cast_regression.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_cast_regression.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_category_encoder_orchestrator.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_category_encoder_orchestrator.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_conformal_prediction.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_conformal_prediction.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_conformal_prediction_regression.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_conformal_prediction_regression.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_data_leakage_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_data_leakage_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_data_monitoring.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_data_monitoring.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_experiment_tracker.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_experiment_tracker.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_fine_tune.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_fine_tune.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_nonconformity_measures.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_nonconformity_measures.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_onehot_encoding.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_onehot_encoding.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-1.2.4/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-1.2.4/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/make_data/create_data.py` & `bluecast-1.2.4/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_analyse.py` & `bluecast-1.2.4/bluecast/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast.py` & `bluecast-1.2.4/bluecast/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast_binary_conformal_prediction.py` & `bluecast-1.2.4/bluecast/tests/test_cast_binary_conformal_prediction.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast_cv.py` & `bluecast-1.2.4/bluecast/tests/test_cast_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     df_val = synthetic_train_test_data[1]
     df_calibration = synthetic_calibration_data
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.max_depth_max = 3
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
+    train_config.sample_data_during_tuning = True
 
     nb_models = 3
 
     skf = StratifiedKFold(
         n_splits=nb_models,
         shuffle=True,
         random_state=5,
```

### Comparing `bluecast-1.1/bluecast/tests/test_cast_cv_binary_conformal_prediction.py` & `bluecast-1.2.4/bluecast/tests/test_cast_cv_binary_conformal_prediction.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast_cv_multiclass.py` & `bluecast-1.2.4/bluecast/tests/test_cast_cv_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast_cv_multiclass_conformal_prediction.py` & `bluecast-1.2.4/bluecast/tests/test_cast_cv_multiclass_conformal_prediction.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_cast_cv_regression.py` & `bluecast-1.2.4/bluecast/tests/test_cast_cv_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     df_val = synthetic_train_test_data[1]
     df_calibration = synthetic_calibration_data
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.max_depth_max = 3
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
+    train_config.sample_data_during_tuning = True
 
     nb_models = 3
 
     skf = KFold(
         n_splits=nb_models,
         shuffle=True,
         random_state=5,
@@ -65,16 +66,31 @@
     assert (
         len(automl_cv.experiment_tracker.experiment_id)
         <= train_config.hyperparameter_tuning_rounds * nb_models
         + nb_models * 7  # 7 metrics stored in fit_eval
     )
     assert automl_cv.experiment_tracker.experiment_id[-1] < 50
     print("Autotuning successful.")
-    preds = automl_cv.predict(df_val.drop("target", axis=1))
+    preds = automl_cv.predict(df_val.drop("target", axis=1), mean_type="arithmetic")
     print("Predicting successful.")
+
+    preds_geom = automl_cv.predict(df_val.drop("target", axis=1), mean_type="geometric")
+    assert isinstance(preds_geom, pd.Series)
+
+    preds_harm = automl_cv.predict(df_val.drop("target", axis=1), mean_type="harmonic")
+    assert isinstance(preds_harm, pd.Series)
+
+    preds_median = automl_cv.predict(df_val.drop("target", axis=1), mean_type="median")
+    assert isinstance(preds_median, pd.Series)
+
+    preds_wrong_val = automl_cv.predict(
+        df_val.drop("target", axis=1), mean_type="wrong_value"
+    )
+    assert isinstance(preds_wrong_val, pd.Series)
+
     assert len(preds) == len(df_val.index)
     preds = automl_cv.predict(
         df_val.drop("target", axis=1), return_sub_models_preds=True
     )
     assert isinstance(preds, pd.DataFrame)
 
     # Assert that the bluecast_models attribute is updated
```

### Comparing `bluecast-1.1/bluecast/tests/test_cast_regression.py` & `bluecast-1.2.4/bluecast/tests/test_cast_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_category_encoder_orchestrator.py` & `bluecast-1.2.4/bluecast/tests/test_category_encoder_orchestrator.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_check_gpu_support.py` & `bluecast-1.2.4/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_conformal_prediction.py` & `bluecast-1.2.4/bluecast/tests/test_conformal_prediction.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_conformal_prediction_evaluation.py` & `bluecast-1.2.4/bluecast/tests/test_conformal_prediction_evaluation.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_conformal_prediction_regression.py` & `bluecast-1.2.4/bluecast/tests/test_conformal_prediction_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-1.2.4/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_data_leakage_checks.py` & `bluecast-1.2.4/bluecast/tests/test_data_leakage_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_data_monitoring.py` & `bluecast-1.2.4/bluecast/tests/test_data_monitoring.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_datetime_features.py` & `bluecast-1.2.4/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_effectiveness_nonconformity_measures.py` & `bluecast-1.2.4/bluecast/tests/test_effectiveness_nonconformity_measures.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_encode_target_labels.py` & `bluecast-1.2.4/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_experiment_tracker.py` & `bluecast-1.2.4/bluecast/tests/test_experiment_tracker.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_feature_type_detector.py` & `bluecast-1.2.4/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_fine_tune.py` & `bluecast-1.2.4/bluecast/tests/test_fine_tune.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_load_for_production.py` & `bluecast-1.2.4/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_nonconformity_measures.py` & `bluecast-1.2.4/bluecast/tests/test_nonconformity_measures.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_nonconformity_measures_regression.py` & `bluecast-1.2.4/bluecast/tests/test_nonconformity_measures_regression.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_nulls_and_infs.py` & `bluecast-1.2.4/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_onehot_encoding.py` & `bluecast-1.2.4/bluecast/tests/test_onehot_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_save_to_production.py` & `bluecast-1.2.4/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_schema_checks.py` & `bluecast-1.2.4/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_shap_explanations.py` & `bluecast-1.2.4/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_target_encoding_binary.py` & `bluecast-1.2.4/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-1.2.4/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/bluecast/tests/test_train_test_split.py` & `bluecast-1.2.4/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-1.1/pyproject.toml` & `bluecast-1.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "1.1"
+version = "1.2.4"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `bluecast-1.1/PKG-INFO` & `bluecast-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 1.1
+Version: 1.2.4
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -187,15 +187,15 @@
 Documentation is provided via [Read the Docs](https://bluecast.readthedocs.io/en/latest/)
 On GitHub we offer multiple ReadMes to cover all aspects of working
 with BlueCast, covering:
 
 * [Installation](docs/source/Installation.md)
 * [EDA](docs/source/EDA.md)
 * [Basic usage](docs/source/Basic%20usage.md)
-* [Advanced usage](docs/source/Advanced%20usage.md)
+* [Customize training settings](docs/source/Customize%20training%20settings.md)
 * [Customizing configurations and objects](docs/source/Customizing%20configurations%20and%20objects.md)
 * [Model evaluation](docs/source/Model%20evaluation.md)
 * [Model explainability (XAI)](docs/source/Model%20explainability%20(XAI).md)
 * [Uncertainty quantification](docs/source/Uncertainty%20quantification.md)
 * [Monitoring](docs/source/Monitoring.md)
 
 ### How to contribute
```

