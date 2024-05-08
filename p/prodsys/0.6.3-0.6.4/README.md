# Comparing `tmp/prodsys-0.6.3.tar.gz` & `tmp/prodsys-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.6.3.tar", max compression
+gzip compressed data, was "prodsys-0.6.4.tar", max compression
```

## Comparing `prodsys-0.6.3.tar` & `prodsys-0.6.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.3/LICENSE
--rw-r--r--   0        0        0      405 2024-05-08 06:22:41.161244 prodsys-0.6.3/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.3/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    56359 2024-05-05 08:37:15.084888 prodsys-0.6.3/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8854 2024-05-04 15:39:44.446374 prodsys-0.6.3/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.3/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.3/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.3/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.3/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9030 2024-05-04 15:39:44.446374 prodsys-0.6.3/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.3/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2307 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.3/prodsys/express/core.py
--rw-r--r--   0        0        0     1589 2024-05-04 15:39:44.446374 prodsys-0.6.3/prodsys/express/node.py
--rw-r--r--   0        0        0    11649 2024-05-04 15:39:44.446374 prodsys-0.6.3/prodsys/express/process.py
--rw-r--r--   0        0        0     2477 2024-05-04 15:39:44.457893 prodsys-0.6.3/prodsys/express/product.py
--rw-r--r--   0        0        0     7129 2024-05-04 15:39:44.457893 prodsys-0.6.3/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8295 2024-05-04 15:39:44.457893 prodsys-0.6.3/prodsys/express/resources.py
--rw-r--r--   0        0        0     2573 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/express/sink.py
--rw-r--r--   0        0        0     3413 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.3/prodsys/express/state.py
--rw-r--r--   0        0        0     9374 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.3/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3382 2024-05-08 06:17:55.371995 prodsys-0.6.3/prodsys/factories/link_transport_process_updater.py
--rw-r--r--   0        0        0     1745 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/factories/node_factory.py
--rw-r--r--   0        0        0     3752 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.3/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.3/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    11157 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.3/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.3/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.3/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2024-05-06 07:18:41.418213 prodsys-0.6.3/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1583 2024-05-04 15:39:44.464082 prodsys-0.6.3/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.3/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     1233 2024-05-04 15:39:44.473598 prodsys-0.6.3/prodsys/models/node_data.py
--rw-r--r--   0        0        0     3963 2024-05-05 08:37:15.084888 prodsys-0.6.3/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.3/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0    14397 2024-05-04 15:39:44.476967 prodsys-0.6.3/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.3/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.3/prodsys/models/queue_data.py
--rw-r--r--   0        0        0    12335 2024-05-04 15:39:44.476967 prodsys-0.6.3/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10745 2024-05-05 05:55:40.858758 prodsys-0.6.3/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.3/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.3/prodsys/models/source_data.py
--rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.3/prodsys/models/state_data.py
--rw-r--r--   0        0        0    13285 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.3/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12423 2024-05-05 08:37:15.084888 prodsys-0.6.3/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28142 2024-05-05 08:37:15.084888 prodsys-0.6.3/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.3/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46203 2024-05-04 15:39:44.483548 prodsys-0.6.3/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9523 2024-05-05 08:37:15.091916 prodsys-0.6.3/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11829 2024-05-05 08:37:15.091916 prodsys-0.6.3/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.3/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    31006 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.3/prodsys/simulation/logger.py
--rw-r--r--   0        0        0      459 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/node.py
--rw-r--r--   0        0        0     3765 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9599 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0    11900 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/process.py
--rw-r--r--   0        0        0    10255 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/product.py
--rw-r--r--   0        0        0     5716 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/request.py
--rw-r--r--   0        0        0    18086 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/resources.py
--rw-r--r--   0        0        0     9958 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/simulation/route_finder.py
--rw-r--r--   0        0        0    15942 2024-05-04 15:39:44.489571 prodsys-0.6.3/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3202 2024-05-05 08:37:15.091916 prodsys-0.6.3/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.3/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     4139 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29728 2024-05-04 15:39:44.505331 prodsys-0.6.3/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.3/prodsys/simulation/store.py
--rw-r--r--   0        0        0    14403 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.3/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.3/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.3/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12939 2024-05-06 07:36:03.343941 prodsys-0.6.3/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.3/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4390 2024-05-04 15:39:44.505331 prodsys-0.6.3/prodsys/util/util.py
--rw-r--r--   0        0        0     1633 2024-05-08 06:22:40.088634 prodsys-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     7237 2024-05-05 08:37:14.995920 prodsys-0.6.3/README.md
--rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 prodsys-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.4/LICENSE
+-rw-r--r--   0        0        0      405 2024-05-08 06:48:01.321630 prodsys-0.6.4/prodsys/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.4/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    56359 2024-05-05 08:37:15.084888 prodsys-0.6.4/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8854 2024-05-04 15:39:44.446374 prodsys-0.6.4/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.4/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.4/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.4/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.4/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9030 2024-05-04 15:39:44.446374 prodsys-0.6.4/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.4/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2307 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.4/prodsys/express/core.py
+-rw-r--r--   0        0        0     1589 2024-05-04 15:39:44.446374 prodsys-0.6.4/prodsys/express/node.py
+-rw-r--r--   0        0        0    11649 2024-05-04 15:39:44.446374 prodsys-0.6.4/prodsys/express/process.py
+-rw-r--r--   0        0        0     2477 2024-05-04 15:39:44.457893 prodsys-0.6.4/prodsys/express/product.py
+-rw-r--r--   0        0        0     7129 2024-05-04 15:39:44.457893 prodsys-0.6.4/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8295 2024-05-04 15:39:44.457893 prodsys-0.6.4/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2573 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3413 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.4/prodsys/express/state.py
+-rw-r--r--   0        0        0     9374 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.4/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3382 2024-05-08 06:17:55.371995 prodsys-0.6.4/prodsys/factories/link_transport_process_updater.py
+-rw-r--r--   0        0        0     1745 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/factories/node_factory.py
+-rw-r--r--   0        0        0     3752 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.4/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.4/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    11157 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.4/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.4/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.4/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2024-05-06 07:18:41.418213 prodsys-0.6.4/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1583 2024-05-04 15:39:44.464082 prodsys-0.6.4/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.4/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     1233 2024-05-04 15:39:44.473598 prodsys-0.6.4/prodsys/models/node_data.py
+-rw-r--r--   0        0        0     3963 2024-05-05 08:37:15.084888 prodsys-0.6.4/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.4/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    14397 2024-05-04 15:39:44.476967 prodsys-0.6.4/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.4/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.4/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12335 2024-05-04 15:39:44.476967 prodsys-0.6.4/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10745 2024-05-05 05:55:40.858758 prodsys-0.6.4/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.4/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.4/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.4/prodsys/models/state_data.py
+-rw-r--r--   0        0        0    13285 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.4/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12423 2024-05-05 08:37:15.084888 prodsys-0.6.4/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28142 2024-05-05 08:37:15.084888 prodsys-0.6.4/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.4/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46203 2024-05-04 15:39:44.483548 prodsys-0.6.4/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9523 2024-05-05 08:37:15.091916 prodsys-0.6.4/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11829 2024-05-05 08:37:15.091916 prodsys-0.6.4/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.4/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    31006 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.4/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0      459 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/node.py
+-rw-r--r--   0        0        0     3765 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9599 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0    11900 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    10255 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     5716 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    18086 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0     9958 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/simulation/route_finder.py
+-rw-r--r--   0        0        0    15942 2024-05-04 15:39:44.489571 prodsys-0.6.4/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3202 2024-05-05 08:37:15.091916 prodsys-0.6.4/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.4/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     4139 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29728 2024-05-04 15:39:44.505331 prodsys-0.6.4/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.4/prodsys/simulation/store.py
+-rw-r--r--   0        0        0    14403 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.4/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.4/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.4/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12939 2024-05-06 07:36:03.343941 prodsys-0.6.4/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.4/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4390 2024-05-04 15:39:44.505331 prodsys-0.6.4/prodsys/util/util.py
+-rw-r--r--   0        0        0     1657 2024-05-08 06:47:59.694862 prodsys-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7237 2024-05-05 08:37:14.995920 prodsys-0.6.4/README.md
+-rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 prodsys-0.6.4/PKG-INFO
```

### Comparing `prodsys-0.6.3/LICENSE` & `prodsys-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/adapters/__init__.py` & `prodsys-0.6.4/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/adapters/adapter.py` & `prodsys-0.6.4/prodsys/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/adapters/json_adapter.py` & `prodsys-0.6.4/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/conf/logging.ini` & `prodsys-0.6.4/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/conf/logging_config.py` & `prodsys-0.6.4/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/control/routing_control_env.py` & `prodsys-0.6.4/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/control/sequencing_control_env.py` & `prodsys-0.6.4/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/__init__.py` & `prodsys-0.6.4/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/core.py` & `prodsys-0.6.4/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/node.py` & `prodsys-0.6.4/prodsys/express/node.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/process.py` & `prodsys-0.6.4/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/product.py` & `prodsys-0.6.4/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/production_system.py` & `prodsys-0.6.4/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/resources.py` & `prodsys-0.6.4/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/sink.py` & `prodsys-0.6.4/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/source.py` & `prodsys-0.6.4/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/state.py` & `prodsys-0.6.4/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/express/time_model.py` & `prodsys-0.6.4/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/__init__.py` & `prodsys-0.6.4/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/link_transport_process_updater.py` & `prodsys-0.6.4/prodsys/factories/link_transport_process_updater.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/node_factory.py` & `prodsys-0.6.4/prodsys/factories/node_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/process_factory.py` & `prodsys-0.6.4/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/product_factory.py` & `prodsys-0.6.4/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/queue_factory.py` & `prodsys-0.6.4/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/resource_factory.py` & `prodsys-0.6.4/prodsys/factories/resource_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/sink_factory.py` & `prodsys-0.6.4/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/source_factory.py` & `prodsys-0.6.4/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/state_factory.py` & `prodsys-0.6.4/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/factories/time_model_factory.py` & `prodsys-0.6.4/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/__init__.py` & `prodsys-0.6.4/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/core_asset.py` & `prodsys-0.6.4/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/node_data.py` & `prodsys-0.6.4/prodsys/models/node_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/performance_data.py` & `prodsys-0.6.4/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/performance_indicators.py` & `prodsys-0.6.4/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/processes_data.py` & `prodsys-0.6.4/prodsys/models/processes_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/product_data.py` & `prodsys-0.6.4/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/queue_data.py` & `prodsys-0.6.4/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/resource_data.py` & `prodsys-0.6.4/prodsys/models/resource_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/scenario_data.py` & `prodsys-0.6.4/prodsys/models/scenario_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/sink_data.py` & `prodsys-0.6.4/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/source_data.py` & `prodsys-0.6.4/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/state_data.py` & `prodsys-0.6.4/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/models/time_model_data.py` & `prodsys-0.6.4/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/__init__.py` & `prodsys-0.6.4/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.6.4/prodsys/optimization/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/math_opt.py` & `prodsys-0.6.4/prodsys/optimization/math_opt.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/optimization_analysis.py` & `prodsys-0.6.4/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/optimization_util.py` & `prodsys-0.6.4/prodsys/optimization/optimization_util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/simulated_annealing.py` & `prodsys-0.6.4/prodsys/optimization/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/optimization/tabu_search.py` & `prodsys-0.6.4/prodsys/optimization/tabu_search.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/__init__.py` & `prodsys-0.6.4/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/control.py` & `prodsys-0.6.4/prodsys/simulation/control.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/logger.py` & `prodsys-0.6.4/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/observer.py` & `prodsys-0.6.4/prodsys/simulation/observer.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/proces_models.py` & `prodsys-0.6.4/prodsys/simulation/proces_models.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/process.py` & `prodsys-0.6.4/prodsys/simulation/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/product.py` & `prodsys-0.6.4/prodsys/simulation/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/request.py` & `prodsys-0.6.4/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/resources.py` & `prodsys-0.6.4/prodsys/simulation/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/route_finder.py` & `prodsys-0.6.4/prodsys/simulation/route_finder.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/router.py` & `prodsys-0.6.4/prodsys/simulation/router.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/sim.py` & `prodsys-0.6.4/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/sink.py` & `prodsys-0.6.4/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/source.py` & `prodsys-0.6.4/prodsys/simulation/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/state.py` & `prodsys-0.6.4/prodsys/simulation/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/store.py` & `prodsys-0.6.4/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/simulation/time_model.py` & `prodsys-0.6.4/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/util/kpi_visualization.py` & `prodsys-0.6.4/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/util/post_processing.py` & `prodsys-0.6.4/prodsys/util/post_processing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/util/runner.py` & `prodsys-0.6.4/prodsys/util/runner.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/util/statistical_functions.py` & `prodsys-0.6.4/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/prodsys/util/util.py` & `prodsys-0.6.4/prodsys/util/util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/pyproject.toml` & `prodsys-0.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.6.3"
+version = "0.6.4"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
@@ -18,14 +18,15 @@
 hydra-core = "^1.3.2"
 pandas = "^2.0.0"
 openpyxl = "^3.1.2"
 plotly = "^5.14.1"
 scipy = "^1.11.1"
 tqdm = "^4.65"
 email-validator = "^2.1.1"
+pathfinding = "^1.0.9"
 
 [tool.poetry.extras]
 ai = ["torch", "torchvision", "torchaudio", "tensorboard", "gymnasium", "stable-baselines3"]
 
 
 [tool.poetry.group.ai]
 optional = true
```

### Comparing `prodsys-0.6.3/README.md` & `prodsys-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.3/PKG-INFO` & `prodsys-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.6.3
+Version: 0.6.4
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: deap (>=1.3.3,<2.0.0)
 Requires-Dist: email-validator (>=2.1.1,<3.0.0)
 Requires-Dist: fastapi (==0.99.1)
 Requires-Dist: gurobipy (>=10.0.1,<11.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pathfinding (>=1.0.9,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: simanneal (>=0.5.0,<0.6.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: tqdm (>=4.65,<5.0)
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0)
```

