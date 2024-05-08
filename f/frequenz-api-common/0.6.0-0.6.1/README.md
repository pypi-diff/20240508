# Comparing `tmp/frequenz-api-common-0.6.0.tar.gz` & `tmp/frequenz-api-common-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-common-0.6.0.tar", last modified: Mon Mar 25 12:51:58 2024, max compression
+gzip compressed data, was "frequenz-api-common-0.6.1.tar", last modified: Wed May  8 15:37:07 2024, max compression
```

## Comparing `frequenz-api-common-0.6.0.tar` & `frequenz-api-common-0.6.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/grid/delivery_duration.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/market/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/market/energy.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/market/price.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/pagination/pagination_params.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/types/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/types/decimal.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/py/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.787675 frequenz-api-common-0.6.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/py/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/py/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.791675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/market/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/market/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/microgrid/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/pagination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/py/frequenz/api/common/v1/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-25 12:51:58.000000 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-25 12:51:58.000000 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:51:58.000000 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-25 12:51:58.000000 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 12:51:58.000000 frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-25 12:51:47.000000 frequenz-api-common-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:51:58.795675 frequenz-api-common-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.393878 frequenz-api-common-0.6.1/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.393878 frequenz-api-common-0.6.1/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.393878 frequenz-api-common-0.6.1/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.397878 frequenz-api-common-0.6.1/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.397878 frequenz-api-common-0.6.1/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/types/decimal.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.397878 frequenz-api-common-0.6.1/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.397878 frequenz-api-common-0.6.1/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.401878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/market/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/microgrid/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/pagination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/py/frequenz/api/common/v1/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-08 15:37:07.000000 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-08 15:37:07.000000 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:37:07.000000 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-08 15:37:07.000000 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 15:37:07.000000 frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-08 15:36:57.000000 frequenz-api-common-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:37:07.405878 frequenz-api-common-0.6.1/setup.cfg
```

### Comparing `frequenz-api-common-0.6.0/LICENSE` & `frequenz-api-common-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/PKG-INFO` & `frequenz-api-common-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.6.0
+Version: 0.6.1
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.6.0/README.md` & `frequenz-api-common-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/components.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/location.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/metrics.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/grid/delivery_duration.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/grid/delivery_duration.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/location.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/market/energy.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/market/energy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/market/price.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/market/price.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
   // A voltage transformer.
   // Voltage transformers are used to step up or step down the voltage, keeping
   // the power somewhat constant by increasing or decreasing the current.
   // If voltage is stepped up, current is stepped down, and vice versa.
   // Note that voltage transformers have efficiency losses, so the output power
   // is always less than the input power.
   COMPONENT_CATEGORY_VOLTAGE_TRANSFORMER = 14;
+
+  // An HVAC (Heating, Ventilation, and Air Conditioning) system.
+  COMPONENT_CATEGORY_HVAC = 15;
 }
 
 // Metadata specific to a microgrid component.
 message ComponentCategoryMetadataVariant {
   oneof metadata {
     frequenz.api.common.v1.microgrid.components.Battery battery = 1;
     frequenz.api.common.v1.microgrid.components.EvCharger ev_charger = 2;
```

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/proto/frequenz/api/common/v1/types/decimal.proto` & `frequenz-api-common-0.6.1/proto/frequenz/api/common/v1/types/decimal.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/PKG-INFO` & `frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.6.0
+Version: 0.6.1
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/SOURCES.txt` & `frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.6.0/py/frequenz_api_common.egg-info/requires.txt` & `frequenz-api-common-0.6.1/py/frequenz_api_common.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 grpcio<2,>=1.51.1
-protobuf<5,>=4.25.3
+protobuf<6,>=4.25.3
 
 [dev]
 frequenz-api-common[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==24.2.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
 mike==1.1.2
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
-mkdocs-material==9.5.13
-mkdocstrings[python]==0.24.1
-frequenz-repo-config[api]==0.9.1
+mkdocs-material==9.5.21
+mkdocstrings[python]==0.25.1
+frequenz-repo-config[api]==0.9.2
 
 [dev-mypy]
-mypy==1.9.0
+mypy==1.10.0
 grpc-stubs==1.53.0.5
 frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2024.3.2
-frequenz-repo-config[api]==0.9.1
+nox==2024.4.15
+frequenz-repo-config[api]==0.9.2
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==8.1.1
-frequenz-repo-config[extra-lint-examples]==0.9.1
+pytest==8.2.0
+frequenz-repo-config[extra-lint-examples]==0.9.2
```

### Comparing `frequenz-api-common-0.6.0/pyproject.toml` & `frequenz-api-common-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 68.1.0",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[api] == 0.9.1",
+  "frequenz-repo-config[api] == 0.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-api-common"
 description = "Frequenz common gRPC API and bindings"
 readme = "README.md"
@@ -21,53 +21,53 @@
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
-dependencies = ["grpcio >= 1.51.1, < 2", "protobuf >= 4.25.3, < 5"]
+dependencies = ["grpcio >= 1.51.1, < 2", "protobuf >= 4.25.3, < 6"]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 24.2.0", "isort == 5.13.2"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
-  "mkdocs-material == 9.5.13",
-  "mkdocstrings[python] == 0.24.1",
-  "frequenz-repo-config[api] == 0.9.1",
+  "mkdocs-material == 9.5.21",
+  "mkdocstrings[python] == 0.25.1",
+  "frequenz-repo-config[api] == 0.9.2",
 ]
 dev-mypy = [
-  "mypy == 1.9.0",
+  "mypy == 1.10.0",
   "grpc-stubs == 1.53.0.5",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2024.3.2", "frequenz-repo-config[api] == 0.9.1"]
+dev-noxfile = ["nox == 2024.4.15", "frequenz-repo-config[api] == 0.9.2"]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 8.1.1",
-  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
+  "pytest == 8.2.0",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.2",
 ]
 dev = [
   "frequenz-api-common[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-api-common/releases"
```

