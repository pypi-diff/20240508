# Comparing `tmp/forecastout-0.1.0.tar.gz` & `tmp/forecastout-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.1.0.tar", max compression
+gzip compressed data, was "forecastout-0.2.8.tar", max compression
```

## Comparing `forecastout-0.1.0.tar` & `forecastout-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,46 @@
--rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.1.0/README.md
--rw-r--r--   0        0        0      336 2024-03-12 14:38:44.842875 forecastout-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 15:09:40.924641 forecastout-0.1.0/src/forecastout/__init__.py
--rw-r--r--   0        0        0       86 2024-03-12 14:32:00.299108 forecastout-0.1.0/src/forecastout/function_test.py
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.2.8/README.md
+-rw-r--r--   0        0        0       68 2024-05-07 14:07:25.242092 forecastout-0.2.8/forecastout/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-08 10:37:53.539734 forecastout-0.2.8/forecastout/a_data_engine/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-07 13:09:08.224000 forecastout-0.2.8/forecastout/a_data_engine/data_handler.py
+-rw-r--r--   0        0        0     1358 2024-05-07 13:09:08.225000 forecastout-0.2.8/forecastout/a_data_engine/train_test_split.py
+-rw-r--r--   0        0        0      445 2024-05-08 10:37:53.542174 forecastout-0.2.8/forecastout/b_forecast_engine/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-07 13:09:08.227000 forecastout-0.2.8/forecastout/b_forecast_engine/anomaly_detector.py
+-rw-r--r--   0        0        0     2461 2024-05-07 13:50:24.522141 forecastout-0.2.8/forecastout/b_forecast_engine/anomaly_fixer.py
+-rw-r--r--   0        0        0     2780 2024-05-07 13:50:24.334676 forecastout-0.2.8/forecastout/b_forecast_engine/backtester.py
+-rw-r--r--   0        0        0      776 2024-05-07 13:09:08.231000 forecastout-0.2.8/forecastout/b_forecast_engine/decompose_time_series.py
+-rw-r--r--   0        0        0      780 2024-05-07 13:50:24.492189 forecastout-0.2.8/forecastout/b_forecast_engine/ensemble_models.py
+-rw-r--r--   0        0        0     2219 2024-05-07 13:09:08.234000 forecastout-0.2.8/forecastout/b_forecast_engine/ensembler.py
+-rw-r--r--   0        0        0     1294 2024-05-07 13:50:24.370831 forecastout-0.2.8/forecastout/b_forecast_engine/forecast_model_factory.py
+-rw-r--r--   0        0        0      806 2024-05-07 13:09:08.235000 forecastout-0.2.8/forecastout/b_forecast_engine/model_predictor.py
+-rw-r--r--   0        0        0     1048 2024-05-07 13:50:24.344533 forecastout-0.2.8/forecastout/b_forecast_engine/model_trainer.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:37:53.542587 forecastout-0.2.8/forecastout/c_forecast_models/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-07 13:09:08.237000 forecastout-0.2.8/forecastout/c_forecast_models/abstract_model.py
+-rw-r--r--   0        0        0     1499 2024-05-07 13:50:24.391425 forecastout-0.2.8/forecastout/c_forecast_models/autoarima_model.py
+-rw-r--r--   0        0        0     3745 2024-05-07 13:50:24.413897 forecastout-0.2.8/forecastout/c_forecast_models/holtwinters_model.py
+-rw-r--r--   0        0        0     2298 2024-05-07 13:50:24.583771 forecastout-0.2.8/forecastout/c_forecast_models/naive_seasonal.py
+-rw-r--r--   0        0        0     1723 2024-05-07 13:50:24.339749 forecastout-0.2.8/forecastout/c_forecast_models/prophet_model.py
+-rw-r--r--   0        0        0     1064 2024-05-07 13:09:08.247000 forecastout-0.2.8/forecastout/config.yaml
+-rw-r--r--   0        0        0     7573 2024-05-08 10:37:53.545475 forecastout-0.2.8/forecastout/core.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:37:53.545659 forecastout-0.2.8/forecastout/d_disaggregation_features/__init__.py
+-rw-r--r--   0        0        0     1336 2024-05-07 13:50:24.396345 forecastout-0.2.8/forecastout/d_disaggregation_features/add_features.py
+-rw-r--r--   0        0        0     3092 2024-04-15 09:42:13.028000 forecastout-0.2.8/forecastout/d_disaggregation_features/feature_creator.py
+-rw-r--r--   0        0        0      612 2024-05-07 13:09:08.249000 forecastout-0.2.8/forecastout/d_disaggregation_features/feature_encoding.py
+-rw-r--r--   0        0        0      561 2024-05-07 13:09:08.251000 forecastout-0.2.8/forecastout/d_disaggregation_features/feature_normalizer.py
+-rw-r--r--   0        0        0      586 2024-05-08 10:37:53.547856 forecastout-0.2.8/forecastout/e_disaggregation_engine/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-07 13:09:08.253000 forecastout-0.2.8/forecastout/e_disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
+-rw-r--r--   0        0        0      556 2024-05-07 13:50:24.375781 forecastout-0.2.8/forecastout/e_disaggregation_engine/disaggregation_model_factory.py
+-rw-r--r--   0        0        0     1680 2024-05-07 13:50:24.324360 forecastout-0.2.8/forecastout/e_disaggregation_engine/disaggregation_model_predictor.py
+-rw-r--r--   0        0        0      945 2024-05-07 13:50:24.360961 forecastout-0.2.8/forecastout/e_disaggregation_engine/disaggregation_model_trainer.py
+-rw-r--r--   0        0        0     1035 2024-05-07 13:09:08.260000 forecastout-0.2.8/forecastout/e_disaggregation_engine/get_daily_shares.py
+-rw-r--r--   0        0        0     1537 2024-05-07 13:09:08.261000 forecastout-0.2.8/forecastout/e_disaggregation_engine/remake_monthly_forecast_current_month.py
+-rw-r--r--   0        0        0      567 2024-05-07 13:09:08.263000 forecastout-0.2.8/forecastout/f_disaggregation_models/abstract_model.py
+-rw-r--r--   0        0        0     2415 2024-05-07 13:50:24.511339 forecastout-0.2.8/forecastout/f_disaggregation_models/random_forest_model.py
+-rw-r--r--   0        0        0      864 2024-05-08 10:06:52.637332 forecastout-0.2.8/forecastout/main.py
+-rw-r--r--   0        0        0      118 2024-05-07 13:50:24.385366 forecastout-0.2.8/forecastout/y_utils/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-07 13:50:24.547551 forecastout-0.2.8/forecastout/y_utils/input_checker.py
+-rw-r--r--   0        0        0      819 2024-05-07 13:09:08.270000 forecastout-0.2.8/forecastout/y_utils/update_config.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:26:39.480000 forecastout-0.2.8/forecastout/z_data_test/__init__.py
+-rw-r--r--   0        0        0      870 2024-03-28 08:26:39.481000 forecastout-0.2.8/forecastout/z_data_test/data_test1.csv
+-rw-r--r--   0        0        0    25910 2024-05-07 13:09:08.272000 forecastout-0.2.8/forecastout/z_data_test/data_test2.csv
+-rw-r--r--   0        0        0      454 2024-05-08 12:39:29.613222 forecastout-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.2.8/PKG-INFO
```

