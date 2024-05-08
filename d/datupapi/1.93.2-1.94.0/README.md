# Comparing `tmp/datupapi-1.93.2.tar.gz` & `tmp/datupapi-1.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datupapi-1.93.2.tar", last modified: Fri Apr 26 16:49:13 2024, max compression
+gzip compressed data, was "datupapi-1.94.0.tar", last modified: Wed May  8 16:08:34 2024, max compression
```

## Comparing `datupapi-1.93.2.tar` & `datupapi-1.94.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.792054 datupapi-1.93.2/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-26 16:49:13.791054 datupapi-1.93.2/PKG-INFO
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.776054 datupapi-1.93.2/datupapi/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.777054 datupapi-1.93.2/datupapi/configure/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/configure/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/configure/config.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.774054 datupapi-1.93.2/datupapi/distribution/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/distribution/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.2/datupapi/distribution/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.774054 datupapi-1.93.2/datupapi/distribution/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.778054 datupapi-1.93.2/datupapi/evaluate/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/evaluate/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.93.2/datupapi/evaluate/errors.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.779054 datupapi-1.93.2/datupapi/extract/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/extract/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.93.2/datupapi/extract/io.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.93.2/datupapi/extract/io_citrix.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.780054 datupapi-1.93.2/datupapi/feateng/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/relation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/feateng/scale.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.781054 datupapi-1.93.2/datupapi/inventory/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/inventory/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.775054 datupapi-1.93.2/datupapi/inventory/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/DailyUsage/daily_usage.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.782054 datupapi-1.93.2/datupapi/inventory/src/Format/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Format/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.93.2/datupapi/inventory/src/Format/inventory_format.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.783054 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.784054 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/define_periods.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/extract_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.785054 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.785054 datupapi-1.93.2/datupapi/inventory/src/Transformation/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Transformation/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.93.2/datupapi/inventory/src/Transformation/inventory_transformation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/inventory/stocks.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.786054 datupapi-1.93.2/datupapi/predict/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/predict/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/predict/forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.787054 datupapi-1.93.2/datupapi/prepare/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/cleanse.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20602 2023-10-25 22:17:02.000000 datupapi-1.93.2/datupapi/prepare/format.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/prepare/format_dask.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.789054 datupapi-1.93.2/datupapi/training/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/attup.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/training/deepar.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22291 2024-04-26 16:48:36.000000 datupapi-1.93.2/datupapi/training/tft.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.790054 datupapi-1.93.2/datupapi/transform/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/backtesting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    52714 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/forecasting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/transform/ranking.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.790054 datupapi-1.93.2/datupapi/utils/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/utils/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.93.2/datupapi/utils/utils.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-04-26 16:49:13.791054 datupapi-1.93.2/datupapi.egg-info/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/PKG-INFO
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/SOURCES.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/dependency_links.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/requires.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-04-26 16:49:13.000000 datupapi-1.93.2/datupapi.egg-info/top_level.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.93.2/pyproject.toml
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-04-26 16:49:13.792054 datupapi-1.93.2/setup.cfg
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-04-26 16:48:48.000000 datupapi-1.93.2/setup.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.318084 datupapi-1.94.0/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-08 16:08:34.317084 datupapi-1.94.0/PKG-INFO
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.303084 datupapi-1.94.0/datupapi/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.304084 datupapi-1.94.0/datupapi/configure/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/configure/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/configure/config.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.301084 datupapi-1.94.0/datupapi/distribution/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.304084 datupapi-1.94.0/datupapi/distribution/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.94.0/datupapi/distribution/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.301084 datupapi-1.94.0/datupapi/distribution/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.304084 datupapi-1.94.0/datupapi/distribution/src/DistributionFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.94.0/datupapi/distribution/src/DistributionFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.94.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.305084 datupapi-1.94.0/datupapi/evaluate/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/evaluate/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.94.0/datupapi/evaluate/errors.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.306084 datupapi-1.94.0/datupapi/extract/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/extract/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    66939 2024-02-22 19:20:36.000000 datupapi-1.94.0/datupapi/extract/io.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.94.0/datupapi/extract/io_citrix.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.307084 datupapi-1.94.0/datupapi/feateng/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/feateng/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/feateng/relation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/feateng/scale.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.307084 datupapi-1.94.0/datupapi/inventory/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/inventory/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.308084 datupapi-1.94.0/datupapi/inventory/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.302084 datupapi-1.94.0/datupapi/inventory/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.308084 datupapi-1.94.0/datupapi/inventory/src/DailyUsage/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/DailyUsage/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/DailyUsage/daily_usage.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.308084 datupapi-1.94.0/datupapi/inventory/src/Format/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/Format/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5433 2024-02-26 21:37:34.000000 datupapi-1.94.0/datupapi/inventory/src/Format/inventory_format.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.309084 datupapi-1.94.0/datupapi/inventory/src/InventoryFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/InventoryFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.94.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.310084 datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/define_periods.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.310084 datupapi-1.94.0/datupapi/inventory/src/SuggestedForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/SuggestedForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.310084 datupapi-1.94.0/datupapi/inventory/src/Transformation/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/Transformation/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.94.0/datupapi/inventory/src/Transformation/inventory_transformation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/inventory/stocks.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.311084 datupapi-1.94.0/datupapi/predict/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/predict/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/predict/forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.312084 datupapi-1.94.0/datupapi/prepare/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/prepare/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/prepare/cleanse.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20737 2024-05-08 16:06:10.000000 datupapi-1.94.0/datupapi/prepare/format.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/prepare/format_dask.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.313084 datupapi-1.94.0/datupapi/training/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/training/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/training/attup.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/training/deepar.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22819 2024-05-08 16:06:10.000000 datupapi-1.94.0/datupapi/training/tft.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.314084 datupapi-1.94.0/datupapi/transform/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/transform/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/transform/backtesting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    56492 2024-05-08 16:06:10.000000 datupapi-1.94.0/datupapi/transform/forecasting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/transform/ranking.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.314084 datupapi-1.94.0/datupapi/utils/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/utils/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.94.0/datupapi/utils/utils.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-08 16:08:34.316084 datupapi-1.94.0/datupapi.egg-info/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-08 16:08:34.000000 datupapi-1.94.0/datupapi.egg-info/PKG-INFO
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-05-08 16:08:34.000000 datupapi-1.94.0/datupapi.egg-info/SOURCES.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-05-08 16:08:34.000000 datupapi-1.94.0/datupapi.egg-info/dependency_links.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-05-08 16:08:34.000000 datupapi-1.94.0/datupapi.egg-info/requires.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-05-08 16:08:34.000000 datupapi-1.94.0/datupapi.egg-info/top_level.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.94.0/pyproject.toml
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-05-08 16:08:34.318084 datupapi-1.94.0/setup.cfg
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-05-08 16:06:23.000000 datupapi-1.94.0/setup.py
```

### Comparing `datupapi-1.93.2/PKG-INFO` & `datupapi-1.94.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.93.2
+Version: 1.94.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.93.2/datupapi/configure/config.py` & `datupapi-1.94.0/datupapi/configure/config.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/distribution/src/DistributionFunctions/functions_distribution.py` & `datupapi-1.94.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/evaluate/errors.py` & `datupapi-1.94.0/datupapi/evaluate/errors.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/extract/io.py` & `datupapi-1.94.0/datupapi/extract/io.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/extract/io_citrix.py` & `datupapi-1.94.0/datupapi/extract/io_citrix.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/feateng/relation.py` & `datupapi-1.94.0/datupapi/feateng/relation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/feateng/scale.py` & `datupapi-1.94.0/datupapi/feateng/scale.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/DailyUsage/daily_usage.py` & `datupapi-1.94.0/datupapi/inventory/src/DailyUsage/daily_usage.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/Format/inventory_format.py` & `datupapi-1.94.0/datupapi/inventory/src/Format/inventory_format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/InventoryFunctions/functions_inventory.py` & `datupapi-1.94.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/define_periods.py` & `datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/define_periods.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/ProcessForecast/extract_forecast.py` & `datupapi-1.94.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py` & `datupapi-1.94.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/src/Transformation/inventory_transformation.py` & `datupapi-1.94.0/datupapi/inventory/src/Transformation/inventory_transformation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/inventory/stocks.py` & `datupapi-1.94.0/datupapi/inventory/stocks.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/predict/forecast.py` & `datupapi-1.94.0/datupapi/predict/forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/prepare/cleanse.py` & `datupapi-1.94.0/datupapi/prepare/cleanse.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/prepare/format.py` & `datupapi-1.94.0/datupapi/prepare/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
                     8: "-AUG",
                     9: "-SEP",
                     10: "-OCT",
                     11: "-NOV",
                     12: "-DIC"
                 }
                 suffix = suffix + months[month]
-        elif frequency == "W":
+        elif frequency == "W" or frequency == "3W": ## KT ##
             day = Qprep["timestamp"].min().day_name()
             days = {
                 "Monday": "-MON",
                 "Tuesday": "-TUE",
                 "Wednesday": "-WED",
                 "Thursday": "-THU",
                 "Friday": "-FRI",
@@ -447,14 +447,16 @@
             df_aux = df_aux.fillna(0)
             df_aux.index = pd.to_datetime(df_aux.index)
 
             if self.dataset_frequency == 'M':
                 frequency = 12
             elif self.dataset_frequency == 'W':
                 frequency = 52
+            elif self.dataset_frequency == '3W': ## KT ##
+                frequency = 17                
             elif self.dataset_frequency == '2M':
                 frequency = 6
             elif self.dataset_frequency == 'Q':
                 frequency = 4
             decompose_result_mult = sm.tsa.STL(df_aux.demand.values, period=frequency, robust=robust).fit()
             #decompose_result_mult = sm.tsa.seasonal_decompose(df_aux.demand.values, model='additive', period=frequency, extrapolate_trend='freq')
             trend = decompose_result_mult.trend
```

### Comparing `datupapi-1.93.2/datupapi/prepare/format_dask.py` & `datupapi-1.94.0/datupapi/prepare/format_dask.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/training/attup.py` & `datupapi-1.94.0/datupapi/training/attup.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/training/deepar.py` & `datupapi-1.94.0/datupapi/training/deepar.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/training/tft.py` & `datupapi-1.94.0/datupapi/training/tft.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                     8: "-AUG",
                     9: "-SEP",
                     10: "-OCT",
                     11: "-NOV",
                     12: "-DIC"
                 }
                 suffix = suffix + months[month]
-        elif frequency == "W":
+        elif frequency == "W" or frequency == "3W": #ADDED KT
             day = data1["timestamp"].min().day_name()
             days = {
                 "Monday": "-MON",
                 "Tuesday": "-TUE",
                 "Wednesday": "-WED",
                 "Thursday": "-THU",
                 "Friday": "-FRI",
@@ -197,17 +197,26 @@
         test_data = test_data.assign(demand=0)
         data1 = pd.concat([data1, test_data], axis=0)
 
         #add holidays
         io.datalake = "unimilitar-datalake"
         holidays = io.download_object_csv(datalake_path="as-is/opendata/Holidays.csv").loc[:, :"holidays_Colombia"]
         holidays.Date = pd.to_datetime(holidays.Date)
-        holidays = holidays.set_index("Date").resample(frequency + suffix).sum().reset_index()
-        holidays = holidays.rename(columns={"Date": "timestamp", "holidays_Colombia": "holidays_col"})
-        data1 = data1.merge(holidays, on="timestamp")
+        #ADDED KT
+        if frequency=='3W':
+            date_start = data1.timestamp.min()
+            holidays = holidays[(holidays['Date']>=date_start)]
+            holidays = holidays.set_index("Date").resample(frequency + suffix).sum().reset_index()
+            holidays = holidays.rename(columns={"Date": "timestamp", "holidays_Colombia": "holidays_col"})
+            data1 = data1.merge(holidays, on="timestamp")
+        else:
+            holidays = holidays.set_index("Date").resample(frequency + suffix).sum().reset_index()
+            holidays = holidays.rename(columns={"Date": "timestamp", "holidays_Colombia": "holidays_col"})
+            data1 = data1.merge(holidays, on="timestamp")
+
         io = IO(config_file=DOCKER_CONFIG_PATH, logfile='data_training', log_path='output/logs')
 
         #Add time related features
         timestamp = data1[["timestamp"]]
         ts_column = 'timestamp'
         data1["Mes"] = pd.to_datetime(data1[ts_column]).dt.month
         #data1["timestamp_weekofyear"] = data1[ts_column].dt.weekofyear
@@ -286,15 +295,15 @@
         #    known.remove('timestamp_dayofmonth')
 
         return data1, scalers, suffix, known, unknown, group_ids, test_data, n_features, item_location, categorical
 
     def add_dates(self, data1, predict, suffix, scalers):
         data_range = pd.date_range(
             start=data1.timestamp.min(), periods=data1.timestamp.nunique() + self.forecast_horizon, freq=self.dataset_frequency +
-            suffix) if self.dataset_frequency == "M" or self.dataset_frequency == "Q" or self.dataset_frequency == "2M" else pd.date_range(
+            suffix) if self.dataset_frequency == "M" or self.dataset_frequency == "Q" or self.dataset_frequency == "2M" or self.dataset_frequency == "3W" else pd.date_range(      #ADDED KT
                 start=data1.timestamp.min(),
                 end=data1.timestamp.max().date() + relativedelta(weeks=self.forecast_horizon),
                 freq=self.dataset_frequency + suffix)
         predict[0]["date"] = predict[0].apply(lambda row: data_range[int(row["time_idx"])], axis=1)
         column_names = ["item_id", "location", "date", "p5", "p20", "p40", "p50", "p60", "p80", "p95"
                        ] if self.use_location else ["item_id", "date", "p5", "p20", "p40", "p50", "p60", "p80", "p95"]
         predict[0] = predict[0].reindex(columns=column_names)
```

### Comparing `datupapi-1.93.2/datupapi/transform/backtesting.py` & `datupapi-1.94.0/datupapi/transform/backtesting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/transform/forecasting.py` & `datupapi-1.94.0/datupapi/transform/forecasting.py`

 * *Files 3% similar despite different names*

```diff
@@ -563,14 +563,16 @@
                         var1    var2    var3
                 idx0     1       2       3
         """
         if self.dataset_frequency == 'D':
             df_forecast = df_forecast.loc[df_forecast['Date'] >= df_forecast['Date'].max() - DateOffset(days=self.forecast_horizon)]
         elif self.dataset_frequency == 'W':
             df_forecast = df_forecast.loc[df_forecast['Date'] >= df_forecast['Date'].max() - DateOffset(weeks=self.forecast_horizon)]
+        elif self.dataset_frequency == '3W':
+            df_forecast = df_forecast.loc[df_forecast['Date'] >= df_forecast['Date'].max() - DateOffset(weeks=3*(self.forecast_horizon))]              
         elif self.dataset_frequency == 'M':
             df_forecast = df_forecast.loc[df_forecast['Date'] >= df_forecast['Date'].max() - DateOffset(months=self.forecast_horizon)]
         elif self.dataset_frequency == 'Y':
             df_forecast = df_forecast.loc[df_forecast['Date'] >= df_forecast['Date'].max() - DateOffset(years=self.forecast_horizon)]
         else:
             self.logger.debug(f'No valid dataset frequency. Please check config parameters in config.yml')
         try:
@@ -592,14 +594,15 @@
             df_strategy['WMAPE'] = df_strategy['WMAPE'].apply(lambda x: round(x, 2))
             df_strategy['MASE'] = df_strategy['MASE'].apply(lambda x: round(x, 2))
         except KeyError as err:
             self.logger.exception(f'Invalid column name. Please check dataframe metadata: {err}')
             raise
         return df_strategy
 
+
     def concat_forecast_horizons(self, model_type=None, forecast_horizons=None):
         """
         Return a dataframe contatenating short-, mid- and long-term forecasts.
 
         :param model_type: Deep learning model type. Either deepar or attup
         :param forecast_horizons: List of integers of short-, mid- and long-term forecast horizons. Frequency is autotaken from config file
         :return dataframe: Dataframe containing short-, mid- and long-term forecasts
@@ -607,14 +610,55 @@
         >>> df = concat_forecast_horizons(model_type='deepar', forecast_horizons=[1, 3, 6])
         >>> df =
                         var1    var2    var3
                 idx0     1       2       3
         """
 
         try:
+          if self.io.dataset_frequency == '3W': ##
+            df_fcst_s = self.io.download_csv(q_name='Qfcst', datalake_path=os.path.join(self.multiforecast_path,
+                                                                            model_type + str(forecast_horizons[0]) +'p-'+ self.dataset_frequency.lower(), 'output'), date_cols=['Date'])
+            df_fcst_s.Item = df_fcst_s.Item.astype(str)
+            if len(forecast_horizons) == 2:
+                df_fcst_m = self.io.download_csv(q_name='Qfcst', datalake_path=os.path.join(self.multiforecast_path,
+                                                                            model_type + str(forecast_horizons[1]) +'p-'+ self.dataset_frequency.lower(), 'output'), date_cols=['Date'])
+                df_fcst_m.Item = df_fcst_m.Item.astype(str)
+            elif len(forecast_horizons) == 3:
+                df_fcst_m = self.io.download_csv(q_name='Qfcst', datalake_path=os.path.join(self.multiforecast_path,
+                                                                            model_type + str(forecast_horizons[1]) +'p-'+ self.dataset_frequency.lower(), 'output'), date_cols=['Date'])
+                df_fcst_m.Item = df_fcst_m.Item.astype(str)
+                df_fcst_l = self.io.download_csv(q_name='Qfcst', datalake_path=os.path.join(self.multiforecast_path,
+                                                                            model_type + str(forecast_horizons[2]) +'p-'+ self.dataset_frequency.lower(), 'output'), date_cols=['Date'])
+                df_fcst_l.Item = df_fcst_l.Item.astype(str)
+            else:
+                self.logger.debug(f'No valid number of forecasts. It should minimum 1 and maximum 3.')
+
+            if len(forecast_horizons) == 2:      
+                df_bckt_s = df_fcst_s[df_fcst_s['Date'] <= df_fcst_s['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[0])]
+                df_bckt_m = df_fcst_m[df_fcst_m['Date'] < df_bckt_s['Date'].min()]
+                df_fcst_s = df_fcst_s[df_fcst_s['Date'] > df_fcst_s['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[0])]
+                df_fcst_m = df_fcst_m[df_fcst_m['Date'] > df_fcst_m['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[1] - 3*forecast_horizons[0])]
+            
+                df_fcst = pd.concat([df_fcst_m, df_fcst_s, df_bckt_s, df_bckt_m], axis='rows') \
+                            .sort_values(['Date', 'Item'], ascending=False)
+
+            elif len(forecast_horizons) == 3:
+                df_bckt_s = df_fcst_s[df_fcst_s['Date'] <= df_fcst_s['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[0])]
+                df_bckt_m = df_fcst_m[df_fcst_m['Date'] < df_bckt_s['Date'].min()]
+                df_bckt_l = df_fcst_l[df_fcst_l['Date'] < df_bckt_m['Date'].min()]
+                df_fcst_s = df_fcst_s[df_fcst_s['Date'] > df_fcst_s['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[0])]
+                df_fcst_m = df_fcst_m[df_fcst_m['Date'] > df_fcst_m['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[1] - 3*forecast_horizons[0])]
+                df_fcst_l = df_fcst_l[df_fcst_l['Date'] > df_fcst_l['Date'].max() - pd.DateOffset(weeks=3*forecast_horizons[2] - 3*forecast_horizons[1])]
+
+                df_fcst = pd.concat([df_fcst_l, df_fcst_m, df_fcst_s, df_bckt_s, df_bckt_m, df_bckt_l], axis='rows') \
+                            .sort_values(['Date', 'Item'], ascending=False)
+            else:
+                self.logger.debug(f'No valid number of forecasts. It should minimum 1 and maximum 3.') ##
+                          
+          else:  
             df_fcst_s = self.io.download_csv(q_name='Qfcst',
                                              datalake_path=os.path.join(self.multiforecast_path,
                                                                         model_type + str(forecast_horizons[0]) + self.dataset_frequency.lower(),
                                                                         'output'),
                                              date_cols=['Date'])
             df_fcst_s.Item = df_fcst_s.Item.astype(str)
             if len(forecast_horizons) == 2:
```

### Comparing `datupapi-1.93.2/datupapi/transform/ranking.py` & `datupapi-1.94.0/datupapi/transform/ranking.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi/utils/utils.py` & `datupapi-1.94.0/datupapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi.egg-info/PKG-INFO` & `datupapi-1.94.0/datupapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.93.2
+Version: 1.94.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.93.2/datupapi.egg-info/SOURCES.txt` & `datupapi-1.94.0/datupapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/datupapi.egg-info/requires.txt` & `datupapi-1.94.0/datupapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.93.2/setup.py` & `datupapi-1.94.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='datupapi',
-      version='1.93.2',
+      version='1.94.0',
       description='Utility library to support Datup AI MLOps processes',
       long_description_content_type="text/markdown",
       long_description="foo bar baz",
       author='Datup AI',
       author_email='ramiro@datup.ai',
       packages=[
           'datupapi',
```

