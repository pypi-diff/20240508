# Comparing `tmp/deepcave-1.1.3.tar.gz` & `tmp/deepcave-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcave-1.1.3.tar", last modified: Wed Nov  8 09:12:09 2023, max compression
+gzip compressed data, was "deepcave-1.2.tar", last modified: Wed May  8 13:04:41 2024, max compression
```

## Comparing `deepcave-1.1.3.tar` & `deepcave-1.2.tar`

### file list

```diff
@@ -1,141 +1,146 @@
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.011938 deepcave-1.1.3/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11357 2022-12-07 09:26:39.000000 deepcave-1.1.3/LICENSE.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      332 2022-12-20 11:52:29.000000 deepcave-1.1.3/MANIFEST.in
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5728 2023-11-08 09:12:09.011938 deepcave-1.1.3/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4633 2023-06-28 11:50:11.000000 deepcave-1.1.3/README.md
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4005 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/assets/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1466 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/assets/custom.css
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1546 2022-12-20 12:05:38.000000 deepcave-1.1.3/deepcave/cli.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3063 2023-10-25 12:07:23.000000 deepcave-1.1.3/deepcave/config.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      241 2022-12-20 11:55:20.000000 deepcave-1.1.3/deepcave/constants.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5968 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/custom_queue.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/docs/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      180 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/api.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1481 2023-09-08 09:21:42.000000 deepcave-1.1.3/deepcave/docs/converters.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      542 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/faq.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1564 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/getting_started.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      894 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/glossary.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2369 2022-12-20 12:06:27.000000 deepcave-1.1.3/deepcave/docs/index.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2364 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/installation.rst
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/docs/plugins/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2804 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/budget_correlation.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1993 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/configuration_cube.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3781 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/configuration_footprint.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1738 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/configurations.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1944 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/cost_over_time.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      377 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/importances.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3136 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/index.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3264 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/overview.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3092 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/parallel_coordinates.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      956 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/pareto_front.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      392 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/plugins/partial_dependencies.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1030 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/docs/redis.rst
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/evaluators/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/evaluators/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/evaluators/epm/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/evaluators/epm/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7208 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/evaluators/epm/fanova_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    15605 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/evaluators/epm/random_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      767 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/evaluators/epm/random_forest_surrogate.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4297 2023-09-08 09:21:42.000000 deepcave-1.1.3/deepcave/evaluators/epm/utils.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10283 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/evaluators/fanova.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    18022 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/evaluators/footprint.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    12829 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/evaluators/lpi.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/layouts/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      512 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/layouts/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14750 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/layouts/general.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2147 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/layouts/header.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3544 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/layouts/main.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      432 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/layouts/not_found.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1137 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/layouts/notification.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7143 2023-06-28 15:22:01.000000 deepcave-1.1.3/deepcave/layouts/sidebar.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      433 2022-12-20 12:05:38.000000 deepcave-1.1.3/deepcave/open.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/plugins/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    45914 2023-06-28 15:22:01.000000 deepcave-1.1.3/deepcave/plugins/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/plugins/budget/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/plugins/budget/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7298 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/budget/budget_correlation.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2345 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/dynamic.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/plugins/hyperparameter/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/plugins/hyperparameter/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    12386 2023-10-27 13:14:45.000000 deepcave-1.1.3/deepcave/plugins/hyperparameter/importances.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    12423 2023-10-25 12:07:23.000000 deepcave-1.1.3/deepcave/plugins/hyperparameter/pdp.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/plugins/objective/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/plugins/objective/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9894 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/objective/configuration_cube.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8294 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/objective/cost_over_time.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10331 2023-09-08 08:31:50.000000 deepcave-1.1.3/deepcave/plugins/objective/parallel_coordinates.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13051 2023-06-28 15:22:01.000000 deepcave-1.1.3/deepcave/plugins/objective/pareto_front.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11552 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/static.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave/plugins/summary/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/plugins/summary/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11263 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/summary/configurations.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11931 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/plugins/summary/footprint.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13438 2023-06-28 15:22:01.000000 deepcave-1.1.3/deepcave/plugins/summary/overview.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/py.typed
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.011938 deepcave-1.1.3/deepcave/runs/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    31917 2023-09-08 09:21:42.000000 deepcave-1.1.3/deepcave/runs/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.011938 deepcave-1.1.3/deepcave/runs/converters/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/runs/converters/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2921 2023-06-28 15:22:01.000000 deepcave-1.1.3/deepcave/runs/converters/bohb.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      628 2023-09-08 08:27:43.000000 deepcave-1.1.3/deepcave/runs/converters/deepcave.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4385 2023-09-08 09:21:42.000000 deepcave-1.1.3/deepcave/runs/converters/smac3v1.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4087 2023-10-25 09:19:57.000000 deepcave-1.1.3/deepcave/runs/converters/smac3v2.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      198 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/runs/exceptions.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6411 2023-09-08 09:21:42.000000 deepcave-1.1.3/deepcave/runs/group.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11755 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/runs/handler.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3244 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/runs/objective.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4446 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/runs/recorder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11260 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/runs/run.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      236 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/runs/status.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      899 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/runs/trial.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      297 2022-12-20 11:59:17.000000 deepcave-1.1.3/deepcave/server.py
--rwxrwxr-x   0 skrebs    (1000) skrebs    (1000)     1801 2022-12-20 12:05:38.000000 deepcave-1.1.3/deepcave/start.sh
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.011938 deepcave-1.1.3/deepcave/utils/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3726 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/cache.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      120 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/cast.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1063 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/compression.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1701 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/configs.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3988 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/configspace.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      388 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/dash.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      442 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/data_structures.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1555 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/docs.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      248 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/files.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      370 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/hash.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2831 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/layout.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      482 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/logging.yml
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      379 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/logs.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      612 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/notification.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4688 2023-06-28 09:53:09.000000 deepcave-1.1.3/deepcave/utils/run_caches.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4747 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/utils/styled_plot.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14252 2023-11-08 09:00:44.000000 deepcave-1.1.3/deepcave/utils/styled_plotty.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      527 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/url.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1587 2022-12-07 09:26:39.000000 deepcave-1.1.3/deepcave/utils/util.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      282 2023-09-08 08:47:47.000000 deepcave-1.1.3/deepcave/worker.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/deepcave.egg-info/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5728 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3656 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/SOURCES.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/dependency_links.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       47 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/entry_points.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      474 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/requires.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        9 2023-11-08 09:12:08.000000 deepcave-1.1.3/deepcave.egg-info/top_level.txt
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.007938 deepcave-1.1.3/docs/
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-11-08 09:12:09.011938 deepcave-1.1.3/docs/plugins/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2804 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/budget_correlation.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1993 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/configuration_cube.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3781 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/configuration_footprint.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1738 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/configurations.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1944 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/cost_over_time.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      377 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/importances.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3136 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/index.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3264 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/overview.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3092 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/parallel_coordinates.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      956 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/pareto_front.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      392 2022-12-07 09:26:39.000000 deepcave-1.1.3/docs/plugins/partial_dependencies.rst
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2869 2023-06-28 09:53:09.000000 deepcave-1.1.3/pyproject.toml
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      548 2023-11-08 09:00:44.000000 deepcave-1.1.3/requirements.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2023-11-08 09:12:09.011938 deepcave-1.1.3/setup.cfg
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2123 2022-12-07 09:26:39.000000 deepcave-1.1.3/setup.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.808397 deepcave-1.2/
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)    11357 2022-12-07 09:26:39.000000 deepcave-1.2/LICENSE.txt
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)      332 2022-12-20 11:52:29.000000 deepcave-1.2/MANIFEST.in
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5953 2024-05-08 13:04:41.808397 deepcave-1.2/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4808 2024-05-08 11:47:33.000000 deepcave-1.2/README.md
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.776396 deepcave-1.2/deepcave/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5278 2024-05-08 13:02:51.000000 deepcave-1.2/deepcave/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.780397 deepcave-1.2/deepcave/assets/
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1466 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/assets/custom.css
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1853 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/cli.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4475 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/config.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      566 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/constants.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11037 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/custom_queue.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.780397 deepcave-1.2/deepcave/docs/
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)      180 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/api.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1481 2023-09-08 09:21:42.000000 deepcave-1.2/deepcave/docs/converters.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)      542 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/faq.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1761 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/getting_started.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)      894 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/glossary.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3210 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/how_to_contribute.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2458 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/index.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     2364 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/installation.rst
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.784397 deepcave-1.2/deepcave/docs/plugins/
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     2804 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/plugins/budget_correlation.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1993 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/plugins/configuration_cube.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3974 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/configuration_footprint.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1749 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/configurations.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2231 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/cost_over_time.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      664 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/importances.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3202 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/index.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3420 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/overview.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3093 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/parallel_coordinates.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      958 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/pareto_front.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2352 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/partial_dependencies.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1015 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/docs/plugins/symbolic_explanations.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1030 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/docs/redis.rst
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.788396 deepcave-1.2/deepcave/evaluators/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      330 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.788396 deepcave-1.2/deepcave/evaluators/epm/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      416 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/epm/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9032 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/epm/fanova_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17444 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/epm/random_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1616 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/epm/random_forest_surrogate.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4997 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/epm/utils.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11181 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/fanova.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19847 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/footprint.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    15131 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/evaluators/lpi.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.792397 deepcave-1.2/deepcave/layouts/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      765 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    18369 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/general.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4827 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/header.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4745 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/main.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      769 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/not_found.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1892 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/notification.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8092 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/layouts/sidebar.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      557 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/open.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.792397 deepcave-1.2/deepcave/plugins/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    50719 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.792397 deepcave-1.2/deepcave/plugins/budget/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      142 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/budget/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11367 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/budget/budget_correlation.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4033 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/dynamic.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.792397 deepcave-1.2/deepcave/plugins/hyperparameter/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      331 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/hyperparameter/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19269 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/hyperparameter/importances.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17825 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/hyperparameter/pdp.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    22366 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/hyperparameter/symbolic_explanations.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.796397 deepcave-1.2/deepcave/plugins/objective/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      444 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/objective/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14197 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/objective/configuration_cube.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14214 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/objective/cost_over_time.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14375 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/objective/parallel_coordinates.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    22800 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/objective/pareto_front.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14013 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/static.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.796397 deepcave-1.2/deepcave/plugins/summary/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      349 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/summary/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17546 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/summary/configurations.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17298 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/summary/footprint.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    15754 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/plugins/summary/overview.py
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)        0 2022-12-07 09:26:39.000000 deepcave-1.2/deepcave/py.typed
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.800397 deepcave-1.2/deepcave/runs/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    48543 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.800397 deepcave-1.2/deepcave/runs/converters/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      509 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/converters/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4283 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/converters/bohb.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1683 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/converters/deepcave.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5443 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/converters/smac3v1.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5455 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/converters/smac3v2.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      760 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/exceptions.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11001 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/group.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    15118 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/handler.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5723 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/objective.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8946 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/recorder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13419 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/run.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1023 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/status.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2356 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/runs/trial.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      361 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/server.py
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1801 2022-12-20 12:05:38.000000 deepcave-1.2/deepcave/start.sh
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.804397 deepcave-1.2/deepcave/utils/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1572 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5562 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/cache.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      516 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/cast.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2197 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/compression.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1823 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/configs.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4081 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/configspace.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      938 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/dash.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      568 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/data_structures.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1946 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/docs.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      622 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/files.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      869 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/hash.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7565 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/layout.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      510 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/logging.yml
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      717 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/logs.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1513 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/notification.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5252 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/run_caches.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8578 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/styled_plot.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17338 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/styled_plotty.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5031 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/symbolic_regression.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1240 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/url.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2445 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/utils/util.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      347 2024-05-08 11:47:33.000000 deepcave-1.2/deepcave/worker.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.780397 deepcave-1.2/deepcave.egg-info/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5953 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3874 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/SOURCES.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/dependency_links.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       47 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/entry_points.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      651 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/requires.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        9 2024-05-08 13:04:41.000000 deepcave-1.2/deepcave.egg-info/top_level.txt
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.772396 deepcave-1.2/docs/
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2024-05-08 13:04:41.808397 deepcave-1.2/docs/plugins/
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     2804 2022-12-07 09:26:39.000000 deepcave-1.2/docs/plugins/budget_correlation.rst
+-rwxr-xr-x   0 skrebs    (1000) skrebs    (1000)     1993 2022-12-07 09:26:39.000000 deepcave-1.2/docs/plugins/configuration_cube.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3974 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/configuration_footprint.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1749 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/configurations.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2231 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/cost_over_time.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      664 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/importances.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3202 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/index.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3420 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/overview.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3093 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/parallel_coordinates.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      958 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/pareto_front.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2352 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/partial_dependencies.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1015 2024-05-08 11:47:33.000000 deepcave-1.2/docs/plugins/symbolic_explanations.rst
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2219 2024-05-08 11:47:33.000000 deepcave-1.2/pyproject.toml
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      789 2024-05-08 12:44:03.000000 deepcave-1.2/requirements.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2024-05-08 13:04:41.808397 deepcave-1.2/setup.cfg
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2257 2024-05-08 11:47:33.000000 deepcave-1.2/setup.py
```

### Comparing `deepcave-1.1.3/LICENSE.txt` & `deepcave-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/PKG-INFO` & `deepcave-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: deepcave
-Version: 1.1.3
+Version: 1.2
 Summary: An interactive framework to visualize and analyze your AutoML process in real-time.
 Home-page: https://www.automl.org
-Author-email: sass@tnt.uni-hannover.de
+Author-email: s.segel@ai.uni-hannover.de
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/automl/deepcave
 Project-URL: Source Code, https://github.com/automl/deepcave
 Platform: Linux
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Python: >=3.9, <3.10
+Requires-Python: >=3.9, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: examples
 License-File: LICENSE.txt
 
+<img src="docs/images/DeepCAVE_Logo_wide.png" alt="Logo"/> 
+
 # DeepCAVE
 
 DeepCAVE is a visualization and analysis tool for AutoML (especially for the sub-problem
 hyperparameter optimization) runs. The framework is programmed on top of Dash and therefore
 entirely interactive. Multiple and diverse plugins make it possible to efficiently generate insights
 and bring the human back in the loop. Moreover, the powerful run interface and the modularized
 plugin structure allow extending the tool at any time effortlessly.
@@ -38,15 +41,15 @@
 
 Following features are provided:
 - Interactive Dashboard (completely written in Python) to self-analyze optimization runs/processes.
 - Analyzing while optimizing (run changes are automatically detected).
 - A large collection of plugins to explore multiple areas like performance, hyperparameter and
 budget analysis.
 - Save your runs using DeepCAVE's native recorder.
-- Support for many optimizers using converter (e.g., DeepCAVE, SMAC and BOHB).
+- Support for many optimizers using converters (e.g., DeepCAVE, SMAC and BOHB).
 - Select runs directly from a working directory in the interface.
 - Select groups of runs for combined analysis.
 - Modularized plugin structure with access to selected runs/groups to provide maximal flexibility.
 - Asynchronous execution of expensive plugins and caching of their results.
 - Help buttons and integrated documentation in the interface helps you to understand the plugins.
 - Use the matplotlib mode to customize and save the plots for your publication.
 - The API mode gives you full access to the code, while you do not have to interact with the 
@@ -65,20 +68,26 @@
 conda install -c anaconda swig
 pip install DeepCAVE
 ```
 
 If you want to contribute to DeepCAVE use the following steps instead:
 ```bash
 git clone https://github.com/automl/DeepCAVE.git
+cd DeepCAVE
 conda create -n DeepCAVE python=3.9
 conda activate DeepCAVE
 conda install -c anaconda swig
 make install-dev
 ```
 
+If you want to use the given examples, run this after installing:
+```bash
+make install-examples
+```
+
 Please visit the [documentation](https://automl.github.io/DeepCAVE/main/installation.html) to get
 further help (e.g. if you can not install redis server or you are on a mac).
 
 
 ## Recording
 
 A minimal example is given to show the simplicity yet powerful API to record runs.
@@ -140,8 +149,7 @@
     publisher = {arXiv},
     year = {2022},
     copyright = {arXiv.org perpetual, non-exclusive license}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org/).
-
```

### Comparing `deepcave-1.1.3/README.md` & `deepcave-1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<img src="docs/images/DeepCAVE_Logo_wide.png" alt="Logo"/> 
+
 # DeepCAVE
 
 DeepCAVE is a visualization and analysis tool for AutoML (especially for the sub-problem
 hyperparameter optimization) runs. The framework is programmed on top of Dash and therefore
 entirely interactive. Multiple and diverse plugins make it possible to efficiently generate insights
 and bring the human back in the loop. Moreover, the powerful run interface and the modularized
 plugin structure allow extending the tool at any time effortlessly.
@@ -10,15 +12,15 @@
 
 Following features are provided:
 - Interactive Dashboard (completely written in Python) to self-analyze optimization runs/processes.
 - Analyzing while optimizing (run changes are automatically detected).
 - A large collection of plugins to explore multiple areas like performance, hyperparameter and
 budget analysis.
 - Save your runs using DeepCAVE's native recorder.
-- Support for many optimizers using converter (e.g., DeepCAVE, SMAC and BOHB).
+- Support for many optimizers using converters (e.g., DeepCAVE, SMAC and BOHB).
 - Select runs directly from a working directory in the interface.
 - Select groups of runs for combined analysis.
 - Modularized plugin structure with access to selected runs/groups to provide maximal flexibility.
 - Asynchronous execution of expensive plugins and caching of their results.
 - Help buttons and integrated documentation in the interface helps you to understand the plugins.
 - Use the matplotlib mode to customize and save the plots for your publication.
 - The API mode gives you full access to the code, while you do not have to interact with the 
@@ -37,20 +39,26 @@
 conda install -c anaconda swig
 pip install DeepCAVE
 ```
 
 If you want to contribute to DeepCAVE use the following steps instead:
 ```bash
 git clone https://github.com/automl/DeepCAVE.git
+cd DeepCAVE
 conda create -n DeepCAVE python=3.9
 conda activate DeepCAVE
 conda install -c anaconda swig
 make install-dev
 ```
 
+If you want to use the given examples, run this after installing:
+```bash
+make install-examples
+```
+
 Please visit the [documentation](https://automl.github.io/DeepCAVE/main/installation.html) to get
 further help (e.g. if you can not install redis server or you are on a mac).
 
 
 ## Recording
 
 A minimal example is given to show the simplicity yet powerful API to record runs.
```

### Comparing `deepcave-1.1.3/deepcave/__init__.py` & `deepcave-1.2/deepcave/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,57 @@
+#  noqa: D400
+"""
+# DeepCAVE
+
+This module is used to initialize and set up the configuration for the DeepCAVE framework.
+
+The Dash application gets created.
+"""
+
 from typing import Any, Callable, TypeVar, cast
 
 import datetime
 import os
 import sys
 from functools import wraps
 from pathlib import Path
 
 name = "DeepCAVE"
 package_name = "deepcave"
 author = "R. Sass and E. Bergman and A. Biedenkapp and F. Hutter and M. Lindauer"
-author_email = "sass@tnt.uni-hannover.de"
+author_email = "s.segel@ai.uni-hannover.de"
 description = "An interactive framework to visualize and analyze your AutoML process in real-time."
 url = "automl.org"
 project_urls = {
     "Documentation": "https://automl.github.io/DeepCAVE/main",
     "Source Code": "https://github.com/automl/deepcave",
 }
 copyright = f"Copyright {datetime.date.today().strftime('%Y')}, {author}"
-version = "1.1.3"
+version = "1.2"
 
 _exec_file = sys.argv[0]
 _exec_files = ["server.py", "worker.py", "sphinx-build"]
 
 ROOT_DIR = Path(__file__).parent
 
 
-def get_app(title: str):
+def get_app(title: str) -> Any:
+    """
+    Get the Dash Proxy.
+
+    Parameters
+    ----------
+    title : str
+        The title of the application.
+
+    Returns
+    -------
+    DashProxy
+        The dash proxy.
+    """
     import dash_bootstrap_components as dbc
     from dash_extensions.enrich import (
         DashProxy,
         MultiplexerTransform,
         NoOutputTransform,
         TriggerTransform,
     )
@@ -57,16 +79,16 @@
     )
     return app
 
 
 if any(file in _exec_file for file in _exec_files):
     from deepcave.custom_queue import Queue
     from deepcave.runs.handler import RunHandler
-    from deepcave.runs.objective import Objective  # noqa
-    from deepcave.runs.recorder import Recorder  # noqa
+    from deepcave.runs.objective import Objective
+    from deepcave.runs.recorder import Recorder
     from deepcave.utils.cache import Cache
     from deepcave.utils.configs import parse_config
     from deepcave.utils.notification import Notification
     from deepcave.utils.run_caches import RunCaches
 
     # Get config
     config_name = None
@@ -111,29 +133,67 @@
         "Recorder",
         "Objective",
     ]
 else:
     try:
         from deepcave.runs.objective import Objective  # noqa
         from deepcave.runs.recorder import Recorder  # noqa
+        from deepcave.utils.configs import parse_config
+        from deepcave.utils.notification import Notification
 
-        __all__ = ["version", "Recorder", "Objective"]
+        config_name = None
+        if "--config" in sys.argv:
+            config_name = sys.argv[sys.argv.index("--config") + 1]
+        config = parse_config(config_name)
+
+        # Notifications
+        notification = Notification()
+
+        __all__ = ["version", "Recorder", "Objective", "notification", "config"]
     except ModuleNotFoundError:
         __all__ = ["version"]
 
 
 _api_mode = False if "app" in globals() else True
 
-
 # This TypeVar is necessary to ensure that the decorator works with arbitrary signatures.
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def interactive(func: F) -> F:
+    """
+    Define the interactive decorator.
+
+    Parameters
+    ----------
+    func : F
+        The function to be decorated.
+
+    Returns
+    -------
+    F
+        The decorated function.
+    """
+
     @wraps(func)
     def inner(*args: Any, **kwargs: Any) -> Any:
+        """
+        Inner function of the decorator.
+
+        Parameters
+        ----------
+        *args : Any
+            Arguments to be passed to the wrap function.
+        **kwargs : Any
+            Keyword arguments to be passed to the wrap function.
+
+        Returns
+        -------
+        Any
+            The result of the function.
+        """
         if _api_mode:
             return
 
         return func(*args, **kwargs)
 
     return cast(F, inner)
```

### Comparing `deepcave-1.1.3/deepcave/assets/custom.css` & `deepcave-1.2/deepcave/assets/custom.css`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/cli.py` & `deepcave-1.2/deepcave/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-from typing import Any, List
+#  noqa: D400
+"""
+# CLI
+
+This module defines command-line options using flags.
+
+This includes the entry point for the programs execution.
+"""
+
+from typing import Any
 
 import multiprocessing
 import subprocess
 from pathlib import Path
 
 from absl import app, flags
 
@@ -19,15 +28,16 @@
 flags.DEFINE_boolean("docker", False, "Uses docker image to start DeepCAVE. Not supported yet.")
 flags.DEFINE_string("config", None, "Filename to a user-specific config.")
 flags.DEFINE_string(
     "get_config_value", None, "Prints the value of a given config key. Useful for bash scripts."
 )
 
 
-def execute(_) -> None:
+def execute(_: Any) -> None:
+    """Entry point for the programs execution."""
     if (config_key := FLAGS.get_config_value) is not None:
         config = FLAGS.config
         if config is not None:
             config = str(FLAGS.config)
         config = parse_config(config)
         print(getattr(config, config_key))
         return
@@ -45,8 +55,12 @@
         if FLAGS.config is not None:
             subprocess.call([start, open, n_workers, str(FLAGS.config)])
         else:
             subprocess.call([start, open, n_workers])
 
 
 def main() -> None:
-    app.run(execute)
+    """Call the execute function."""
+    try:
+        app.run(execute)
+    except KeyboardInterrupt:
+        exit("KeyboardInterrupt.")
```

### Comparing `deepcave-1.1.3/deepcave/docs/converters.rst` & `deepcave-1.2/deepcave/docs/converters.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/faq.rst` & `deepcave-1.2/deepcave/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/getting_started.rst` & `deepcave-1.2/deepcave/docs/getting_started.rst`

 * *Files 9% similar despite different names*

```diff
@@ -35,11 +35,14 @@
 can select the runs you want to analyze. Please have a look at the following image
 to see the dashboard in action:
 
 
 .. image:: images/plugins/general.png
 
 
+Displaying the data is done via plugins. You can select the plugins you want to use in the menu on the left.
+This is further explained in the :ref:`plugins<Displaying Data with Plugins>` section.
+
 DeepCAVE uses runs to interprete data. A run is a collection of trials
 (a configuration with associated costs). Once valid runs (see :ref:`converter<Converters>`) are
 found, you can select them to analyze them further. After selecting runs, you can also add them to
 groups to analyze combined runs easily.
```

### Comparing `deepcave-1.1.3/deepcave/docs/glossary.rst` & `deepcave-1.2/deepcave/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/index.rst` & `deepcave-1.2/deepcave/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+.. image:: ./images/DeepCAVE_Logo_wide.png
+   :alt: DeepCAVE Logo
+|
+
 Home
 ====
 
 .. toctree::
    :hidden:
    :maxdepth: 2
 
    installation
    getting_started
    examples/index
    plugins/index
    converters
+   how_to_contribute
    api
    glossary
    faq
 
-
 DeepCAVE is a visualization and analysis tool for AutoML (especially for the sub-problem
 hyperparameter optimization) runs. The framework is programmed on top of Dash and therefore
 entirely interactive. Multiple and diverse plugins make it possible to efficiently generate insights
 and bring the human back in the loop. Moreover, the powerful run interface and the modularized
 plugin structure allow extending the tool at any time effortlessly.
```

### Comparing `deepcave-1.1.3/deepcave/docs/installation.rst` & `deepcave-1.2/deepcave/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/budget_correlation.rst` & `deepcave-1.2/deepcave/docs/plugins/budget_correlation.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/configuration_cube.rst` & `deepcave-1.2/deepcave/docs/plugins/configuration_cube.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/configuration_footprint.rst` & `deepcave-1.2/deepcave/docs/plugins/configuration_footprint.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 grasp on your configuration footprint.
 
 
 Performance plot
 ----------------
 Perhaps the most useful plot of the two is to see how much we know about which configuration will
 achieve which **objective** score. To view this, mousing over the **Incumbent** will tell you the
-best configuration found for the given *objective* and *budget*. The **Evaluated Configuration**
+best configuration found for the given *objective* and *budget*. For non-deterministic runs (i.e.
+multiple seeds evaluated per configuration), only configurations evaluated on the maximum number of
+seeds are considered to choose the best configuration from. The **Evaluated Configuration**
 points will have a true objective score, all be it possibly noisy if the objective is noisy.
 Using these two kind of points, we can try to infer what the performance for the rest of the
 configuration space will be.
 
 It's important to note that the background colour, represnting the objective is a best estimate
 given what we already know and does not indicate the true objective value in regions where there
 are no configurations evaluated. We can increase the resolution using the *Details* option, which
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/configurations.rst` & `deepcave-1.2/deepcave/docs/plugins/configurations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Configuration
 * Code
 
 Since configurations are used throughout the application, you might find links associated to this
 plugin. This plugin is capable of answering following questions:
 
 * Where is the configuration coming from?
-* How are the objective values wrt the budgets?
+* How are the objective values with respect to the budgets?
 * How is the status of a trial associated with the selected configuration?
 * Which values have been used for a certain configuration?
 * How can I access the configuration in python?
 
 
 Overview
 --------
@@ -39,11 +39,11 @@
 In the configuration section, you see how the hyperparameters were selected in the end. While the
 graph view gives you a nice overview, the table displays the concrete values.
 
 
 Code
 ----
 Often a configuration is selected for deployment, which makes it crucial to access it somehow.
-The code block provides you the code to access the configuration code-wise. 
+The code block provides you the code to access the configuration code-wise.
 
 
 .. image:: ../images/plugins/configurations.png
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/cost_over_time.rst` & `deepcave-1.2/deepcave/docs/plugins/cost_over_time.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 how the objectives change over time. To see the change based on the time or number of
 configurations, this plugin visualize it for you.
 
 Since multiple runs are supported, you directly see which run performs best to which time.
 If you decide to display groups (which are combined runs), you will see the mean and standard
 deviation too.
 
-.. note:: 
-    The configuration spaces of the selected runs have to be equal. Otherwise, a good comparison
-    is not possible.
+.. note::
+    The configuration spaces of the selected runs should be equal. Otherwise, a good comparison
+    is not possible. They can, however, still be displayed in the same graph.
+
+.. note::
+    For non-deterministic runs (i.e. multiple seeds evaluated per configuration), only
+    configurations evaluated on the maximum number of seeds are considered to choose the best
+    configuration at a given time from.
 
 This plugin is capable of answering following questions:
 
 * Does the optimizer converge?
 * How performs optimizer A in comparison to optimizer B? Is optimizer A better than optimizer B?
 * How long does the optimizer need to reach a certain objective value?
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/index.rst` & `deepcave-1.2/deepcave/docs/plugins/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Plugins
-=======
+Displaying Data with Plugins
+============================
 
 .. toctree::
    :hidden:
    :maxdepth: 2
 
    overview
    configurations
@@ -11,14 +11,15 @@
    cost_over_time
    configuration_cube
    pareto_front
    parallel_coordinates
    budget_correlation
    importances
    partial_dependencies
+   symbolic_explanations
 
 
 Plugins are used to display data in a specific way. There are plugins to analyse the performance,
 the hyperparameters and the budgets. Since AutoML runs are multi-dimensional, the plugins
 provide a way to look into specific aspects in more detail.
 
 The goal of the plugins are to provide a way to visualize the data in a way that is easy to
@@ -74,10 +75,10 @@
 Custom Plugin
 -------------
 
 DeepCAVE was designed so that the plugins require minimal design. We recommend using any of our
 provided plugins as a starting point and change it to your needs.
 
 After you have created your plugin, you need to register it in your config file. If you work
-on the branch directly, you can adapt ``deepcave/config.py`` to your needs. 
+on the branch directly, you can adapt ``deepcave/config.py`` to your needs.
 We would be very happy to receive pull-requests!
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/overview.rst` & `deepcave-1.2/deepcave/docs/plugins/overview.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,56 +19,58 @@
 * When was the latest change of the optimizer's data?
 * What is the best configuration?
 * Are the meta data as expected?
 * Are the objectives as expected?
 * Is the configuration space as expected?
 * How many trials have been successful/unsuccessful?
 * Why did certain trials crash?
-* On which budgets were the configurations evaluated?
+* On which multi-fidelity budgets were the configurations evaluated?
 
 
 Quick Information
 -----------------
 
 In the **Quick Information** box you'll information regarding summary statistics about your run or
 group of runs. Notably information on the optimizer used, how many configurations were tried, when
 the runs were last updated and a handy quick link to the best **Configuration**.
 
 Meta
 ----
 Next we show some meta information regarding your runs. Notably, you can see information such as the
-possible **budget** allocations that were considered during the run.
+possible **budget** allocations that were considered during the run. The **budget** is the amount of
+resources that were allocated to a configuration as it was being evaluated using a multi-fidelity
+approach.
 
 
 Objectives
 ----------
 In this section, we see the objectives that were considered during the optimization run. Here we get
 information about it's name and the bounds they were in.
 
 
 Statuses
 --------
 To get a nice overview of the optimization run, we provide a barplot that details how the end status
-of the many trials that occured. You can also view these as a heatmap or get more information from
+of the many trials that occurred. You can also view these as a heatmap or get more information from
 the **Details** tab.
 
-The barplot shows which trial recieved which status and under which budget allocation. These are
+The barplot shows which trial received which status and under which budget allocation. These are
 grouped according to the status and coloured based on the status it exited with.
 
 To see details on how these configurations faired as they progressed in budget, you can refer to
 the **Heatmap** tab. Here you'll see the budget allocation along the x-axis with the configuration
 ID stacked on the y-axis. In an ideal scenario, you would see mostly **Success** bars spanning
 across the entire plot, with some **NOT_EVALUATED** lines indicating there is further configurations
 to try. However if you faced many crashes at high budgets for example, you'll see **CRASHED** bars
 from the highest budget onwards. In general, you can use this to understand how often your optimizer
 balances out between low budget evaluations and full budget evaluations.
 
-In the **Details** tab, you'll recieve an overview of configurations that were not successful.
-Here you'll get some breif information about the config id number, the budget it was evaluated under
-and the status it recieved. If there is an associated error we can provide, such as when it recieved
+In the **Details** tab, you'll receive an overview of configurations that were not successful.
+Here you'll get some brief information about the config id number, the budget it was evaluated under
+and the status it received. If there is an associated error we can provide, such as when it received
 the **CRASHED** status, we will display it in the error column.
 
 
 Configuration Space
 -------------------
 
 Lastly you can find information on the configuration space that was being optimized over.
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/parallel_coordinates.rst` & `deepcave-1.2/deepcave/docs/plugins/parallel_coordinates.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Parallel Coordinates
 ====================
 
-With parallel coordinates, you can see configurations plotted as a line through their hyperparamter
+With parallel coordinates, you can see configurations plotted as a line through their hyperparameter
 values and to which final score they reach.
 You can use this to identify trends in hyperparamter value ranges that achieve certain scores.
 For example, you may find that high performing configurations may all share the same value for a
 certain categorical hyperparamter, as indicated by many high scoring lines passing through this
 value. These lines will be ordered according to their importance in determining the final score from
 left to right with the default to show the top 10 important ones.
 Lastly, you can place visual filters along these spines to really home-in on hyperparamters
```

### Comparing `deepcave-1.1.3/deepcave/docs/plugins/pareto_front.rst` & `deepcave-1.2/deepcave/docs/plugins/pareto_front.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 configuration can be chosen due to multiple important objectives which should be considered.
 For example, I want to find a configuration for my problem which has both a good performance
 and low computational cost. To select a suitable configuration, the pareto front shows you the best
 configurations for two given objectives.
 
 .. note::
     You can enable or disable specific runs if you click on the name right to the plot.
-    If you click on a configuration you a redirected to the configuration plugin to see 
+    If you click on a configuration you are redirected to the configuration plugin to see 
     the configuration in detail.
 
 This plugin is capable of answering following questions:
 
 * Which configuration should I choose if I prefer objective A slightly over objective B?
 * How performs optimizer A in comparison to optimizer B? Is optimizer A better than optimizer B?
```

### Comparing `deepcave-1.1.3/deepcave/docs/redis.rst` & `deepcave-1.2/deepcave/docs/redis.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/evaluators/epm/fanova_forest.py` & `deepcave-1.2/deepcave/evaluators/epm/fanova_forest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,61 @@
-from typing import List, Optional, Tuple
+# noqa: D400
+"""
+# FanovaForest
+
+The module provides utilities for creating a fANOVA forest.
+
+It includes a FanovaForest wrapper for pyrfr.
+fANOVA can be used for analyzing the importances of Hyperparameters.
+
+## Classes
+    - FanovaForest: A fANOVA forest wrapper for pyrfr.
+"""
+
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import itertools as it
 
 import numpy as np
 import pyrfr
 import pyrfr.regression as regression
 import pyrfr.util
 from ConfigSpace import ConfigurationSpace
 
 from deepcave.evaluators.epm.random_forest import RandomForest
 
 
 class FanovaForest(RandomForest):
     """
-    A fanova forest wrapper for pyrfr.
+    A fANOVA forest wrapper for pyrfr.
+
+    Properties
+    ----------
+    cutoffs : Tuple[float, float]
+        The cutoffs of the model.
+    percentiles : NDArray[floating]
+        The percentiles of the data points Y.
+    all_midpoints : List
+        All midpoints tree wise for the whole forest.
+    all_sizes : List
+        All interval sizes tree wise for the whole forest.
+    bounds : List[Tuple[float, float]
+        Stores feature bounds.
+    trees_total_variances : List
+        The total variances of the trees.
+    trees_total_variance : Any
+        The total variance of a tree.
+    trees_variance_fractions : Dict
+        The variance fractions of the trees.
+    V_U_total : Dict[Tuple[int, ...], List[Any]]
+        Store variance-related information across all trees.
+    V_U_individual : Dict[Tuple[int, ...], List[Any]]
+        Store variance-related information for individual subsets.
+    n_params : int
+        The number of Hyperparameters to sample.
     """
 
     def __init__(
         self,
         configspace: ConfigurationSpace,
         n_trees: int = 10,
         ratio_features: float = 1.0,
@@ -48,48 +86,48 @@
             seed=seed,
         )
 
         self.cutoffs = cutoffs
 
     def _get_model(self) -> regression.base_tree:
         """
-        Returns the internal model.
+        Return the internal model.
 
         Returns
         -------
         model : regression.base_tree
             Model which is used internally.
         """
         return regression.fanova_forest()
 
     def _train(self, X: np.ndarray, Y: np.ndarray) -> None:
         """
-        Trains the random forest on X and Y.
+        Train the Random Forest on X and Y.
 
         Parameters
         ----------
         X : np.ndarray
             Input data points.
         Y : np.ndarray
             Target values.
         """
         super()._train(X, Y)
         self.percentiles = np.percentile(Y, range(0, 100))
 
-        # all midpoints and interval sizes treewise for the whole forest
+        # all midpoints and interval sizes tree wise for the whole forest
         self.all_midpoints = []
         self.all_sizes = []
 
         # getting split values
         forest_split_values = self._model.all_split_values()
 
         # compute midpoints and interval sizes for variables in each tree
         for tree_split_values in forest_split_values:
-            sizes = []
-            midpoints = []
+            sizes: List = []
+            midpoints: List = []
             for i, split_vals in enumerate(tree_split_values):
                 if np.isnan(self.bounds[i][1]):  # categorical parameter
                     # check if the tree actually splits on this parameter
                     if len(split_vals) > 0:
                         midpoints.append(split_vals)
                         sizes.append(np.ones(len(split_vals)))
                     # if not, simply append 0 as the value with the number of categories as the
@@ -104,39 +142,52 @@
                     midpoints.append((1 / 2) * (sv[1:] + sv[:-1]))
                     sizes.append(sv[1:] - sv[:-1])
 
             self.all_midpoints.append(midpoints)
             self.all_sizes.append(sizes)
 
         # capital V in the paper
-        self.trees_total_variances = []
+        self.trees_total_variances: list = []
 
         # dict of lists where the keys are tuples of the dimensions
         # and the value list contains \hat{f}_U for the individual trees
         # reset all the variance fractions computed
-        self.trees_variance_fractions = {}
-        self.V_U_total = {}
-        self.V_U_individual = {}
+        self.trees_variance_fractions: dict = {}
+        self.V_U_total: Dict[Tuple[int, ...], List[Any]] = {}
+        self.V_U_individual: Dict[Tuple[int, ...], List[Any]] = {}
 
         # Set cut-off
         self._model.set_cutoffs(self.cutoffs[0], self.cutoffs[1])
 
         # recompute the trees' total variance
         self.trees_total_variance = self._model.get_trees_total_variances()
 
-    def compute_marginals(self, hp_ids: List[int], depth=1):
+    def compute_marginals(
+        self, hp_ids: Union[List[int], Tuple[int, ...]], depth: int = 1
+    ) -> Tuple[Dict[Tuple[int, ...], List[Any]], Dict[Tuple[int, ...], List[Any]],]:
         """
-        Returns the marginal of selected parameters.
+        Return the marginal of selected Hyperparameters.
 
         Parameters
         ----------
-        hp_ids: List[int]
-            Contains the indices of the configspace for the selected parameters (starts with 0).
+        hp_ids: Union[List[int], Tuple[int, ...]]
+            Contains the indices of the configspace for the selected Hyperparameters
+            (starts with 0).
+        depth: int
+            The depth of the marginalization.
+            Default value is 1.
+
+        Returns
+        -------
+        Tuple[Dict[Tuple[int, ...], List[Any]],
+        Dict[Tuple[int, ...], List[Any]],
+            The marginal of selected Hyperparameters.
         """
-        hp_ids = tuple(hp_ids)
+        if not isinstance(hp_ids, tuple):
+            hp_ids = tuple(hp_ids)
 
         # check if values has been previously computed
         if hp_ids in self.V_U_individual:
             return self.V_U_individual, self.V_U_total
 
         # otherwise make sure all lower order marginals have been
         # computed, if not compute them
@@ -160,29 +211,29 @@
             midpoints = [self.all_midpoints[tree_idx][hp_id] for hp_id in hp_ids]
             sizes = [self.all_sizes[tree_idx][hp_id] for hp_id in hp_ids]
             stat = pyrfr.util.weighted_running_stats()
 
             prod_midpoints = it.product(*midpoints)
             prod_sizes = it.product(*sizes)
 
-            sample = np.full(self.n_params, np.nan, dtype=float)
+            sample: np.ndarray = np.full(self.n_params, np.nan, dtype=float)
 
             # make prediction for all midpoints and weigh them by the corresponding size
             for i, (m, s) in enumerate(zip(prod_midpoints, prod_sizes)):
                 sample[list(hp_ids)] = list(m)
 
                 ls = self._model.marginal_prediction_stat_of_tree(tree_idx, sample.tolist())
                 # self.logger.debug("%s, %s", (sample, ls.mean()))
                 if not np.isnan(ls.mean()):
                     stat.push(ls.mean(), np.prod(np.array(s)) * ls.sum_of_weights())
 
             # line 10 in algorithm 2
             # note that V_U^2 can be computed by var(\hat a)^2 - \sum_{subU} var(f_subU)^2
             # which is why, \hat{f} is never computed in the code, but
-            # appears in the pseudocode
+            # appears in the pseudo code
             V_U_total = np.nan
             V_U_individual = np.nan
 
             if stat.sum_of_weights() > 0:
                 V_U_total = stat.variance_population()
                 V_U_individual = stat.variance_population()
                 for k in range(1, len(hp_ids)):
```

### Comparing `deepcave-1.1.3/deepcave/evaluators/epm/random_forest.py` & `deepcave-1.2/deepcave/evaluators/epm/random_forest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,27 @@
-from typing import Dict, Optional, Tuple
+# noqa: D400
+"""
+# RandomForest
+
+This module can be used for training and using a Random Forest Regression model.
+
+A pyrfr wrapper is used for simplification.
+
+## Classes
+    - RandomForest: A random forest wrapper for pyrfr.
+
+## Constants
+    VERY_SMALL_NUMBER : float
+    PYRFR_MAPPING : Dict[str, str]
+"""
+
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import functools
 import warnings
-from random import random
 
 import numpy as np
 import pyrfr.regression as regression
 from ConfigSpace import ConfigurationSpace
 from ConfigSpace.hyperparameters import (
     CategoricalHyperparameter,
     Constant,
@@ -30,20 +45,47 @@
     "eps_purity": "tree_opts.epsilon_purity",
     "max_nodes": "tree_opts.max_num_nodes",
 }
 
 
 class RandomForest:
     """
-    A random forest wrapper for pyrfr. This is handy because we only need to pass the configspace
+    A random forest wrapper for pyrfr.
+
+    This is handy because only the configuration space needs to be passed.
     and have a working version without specifying e.g. types and bounds.
 
     Note
     ----
     This wrapper also supports instances.
+
+    Properties
+    ----------
+    cs : ConfigurationSpace
+        The configuration space.
+    log_y : bool
+        Whether y should be treated as a logarithmic transformation.
+    seed : int
+        The seed. If not provided, it is random.
+    types : List[int]
+        The types of the Hyperparameters.
+    bounds : List[Tuple[float, float]]
+        The bounds of the Hyperparameters.
+    n_params : int
+        The number of Hyperparameters in the configuration space.
+    n_features : int
+        The number of features.
+    pca_components : int
+        The number of components to keep for the principal component analysis (PCA).
+    pca : PCA
+        The principal component analysis (PCA) object.
+    scaler : MinMaxScaler
+        A MinMaxScaler to scale the features.
+    instance_features : ndarray
+        The instance features.
     """
 
     def __init__(
         self,
         configspace: ConfigurationSpace,
         n_trees: int = 16,
         ratio_features: float = 5.0 / 6.0,
@@ -52,22 +94,23 @@
         max_depth: int = 2**20,
         max_nodes: int = 2**20,
         eps_purity: float = 1e-8,
         bootstrapping: bool = True,
         instance_features: Optional[np.ndarray] = None,
         pca_components: Optional[int] = 2,
         log_y: bool = False,
-        seed: int = 0,
+        seed: Optional[int] = 0,
     ):
         self.cs = configspace
         self.log_y = log_y
         self.seed = seed
 
         # Set types and bounds automatically
-        self.types, self.bounds = get_types(configspace, instance_features)
+        types, self.bounds = get_types(configspace, instance_features)
+        self.types = np.array(types)
 
         # Prepare everything for PCA
         self.n_params = len(configspace.get_hyperparameters())
         self.n_features = 0
         if instance_features is not None:
             self.n_features = instance_features.shape[1]
 
@@ -91,73 +134,81 @@
             max_nodes=max_nodes,
             eps_purity=eps_purity,
             bootstrapping=bootstrapping,
         )
 
     def _get_model(self) -> regression.base_tree:
         """
-        Returns the internal model.
+        Return the internal model.
 
         Returns
         -------
         model : regression.base_tree
             Model which is used internally.
         """
         return regression.binary_rss_forest()
 
-    def _get_model_options(self, **kwargs) -> regression.forest_opts:
+    def _get_model_options(self, **kwargs: Union[int, float, bool]) -> regression.forest_opts:
         """
-        Get model options from kwargs. The mapping `PYRFR_MAPPING` is used in combination with
+        Get model options from kwargs.
+
+        The mapping `PYRFR_MAPPING` is used in combination with
         a recursive attribute setter to set the options for the pyrfr model.
 
+        Parameters
+        ----------
+        **kwargs : Dict[str, Any]
+            The key word arguments for the model options.
+
         Returns
         -------
         options : regression.forest_opts
             Random forest options.
         """
-        # Now we set the options
+        # Now the options are set
         options = regression.forest_opts()
 
-        def rgetattr(obj, attr, *args):
-            def _getattr(obj, attr):
+        def rgetattr(obj: object, attr: str, *args: Any) -> Any:
+            def _getattr(obj: object, attr: object) -> Any:
+                attr = str(attr)
                 return getattr(obj, attr, *args)
 
             return functools.reduce(_getattr, [obj] + attr.split("."))
 
-        def rsetattr(obj, attr, val):
+        def rsetattr(obj: object, attr: str, val: Any) -> None:
             pre, _, post = attr.rpartition(".")
             return setattr(rgetattr(obj, pre) if pre else obj, post, val)
 
         for k, v in kwargs.items():
             new_k = PYRFR_MAPPING[k]
             rsetattr(options, new_k, v)
 
         return options
 
     def _impute_inactive(self, X: np.ndarray) -> np.ndarray:
         """
-        Imputs inactive values in X.
+        Impute inactive values in X.
 
         Parameters
         ----------
         X : np.ndarray
             Data points.
 
         Returns
         -------
         np.ndarray
             Imputed data points.
 
         Raises
         ------
         ValueError
-            If hyperparameter is not supported.
+            If Hyperparameter is not supported.
         """
-        conditional = {}  # type: Dict[int, bool]
-        impute_values = {}  # type: Dict[int, float]
+        conditional: Dict[int, bool] = {}
+        impute_values: Dict[int, float] = {}
 
         X = X.copy()
         for idx, hp in enumerate(self.cs.get_hyperparameters()):
             if idx not in conditional:
                 parents = self.cs.get_parents_of(hp.name)
                 if len(parents) == 0:
                     conditional[idx] = False
@@ -176,15 +227,15 @@
                 nonfinite_mask = ~np.isfinite(X[:, idx])
                 X[nonfinite_mask, idx] = impute_values[idx]
 
         return X
 
     def _check_dimensions(self, X: np.ndarray, Y: Optional[np.ndarray] = None) -> None:
         """
-        Checks if the dimensions of X and Y are correct wrt features.
+        Check if the dimensions of X and Y are correct with respect to features.
 
         Parameters
         ----------
         X : np.ndarray
             Input data points.
         Y : Optional[np.ndarray], optional
             Target values. By default None.
@@ -206,30 +257,30 @@
             if X.shape[0] != Y.shape[0]:
                 raise ValueError(f"X.shape[0] ({X.shape[0]}) != y.shape[0] ({Y.shape[0]})")
 
     def _get_data_container(
         self, X: np.ndarray, y: np.ndarray
     ) -> regression.default_data_container:
         """
-        Fills a pyrfr default data container s.t. the forest knows
-        categoricals and bounds for continuous data.
+        Fill a pyrfr default data container.
+
+        The goal here is, that the forest knows categoricals and bounds for continuous data.
 
         Parameters
         ----------
         X : np.ndarray [n_samples, n_features]
             Input data points.
         y : np.ndarray [n_samples, ]
             Target values.
 
         Returns
         -------
         data : regression.default_data_container
-            The filled data container that pyrfr can interpret
+            The filled data container that pyrfr can interpret.
         """
-
         # retrieve the types and the bounds from the ConfigSpace
         data = regression.default_data_container(X.shape[1])
 
         for i, (mn, mx) in enumerate(self.bounds):
             if np.isnan(mx):
                 data.set_type_of_feature(i, mn)
             else:
@@ -238,15 +289,17 @@
         for row_X, row_y in zip(X, y):
             data.add_data_point(row_X, row_y)
 
         return data
 
     def train(self, X: np.ndarray, Y: np.ndarray) -> None:
         """
-        Trains the random forest on X and Y. Transforms X if PCA is applied.
+        Train the random forest on X and Y.
+
+        Transform X if principal component analysis (PCA) is applied.
         Afterwards, `_train` is called.
 
         Parameters
         ----------
         X : np.ndarray [n_samples, n_features (config + instance features)]
             Input data points.
         Y : np.ndarray [n_samples, n_objectives]
@@ -279,15 +332,15 @@
             )
             self._pca_applied = True
 
         self._train(X, Y)
 
     def _train(self, X: np.ndarray, Y: np.ndarray) -> None:
         """
-        Trains the random forest on X and Y.
+        Train the random forest on X and Y.
 
         Parameters
         ----------
         X : np.ndarray
             Input data points.
         Y : np.ndarray
             Target values.
@@ -298,28 +351,28 @@
 
         rng = regression.default_random_engine(seed)
 
         # Set more specific model options and finally fit it
         self._model.options.num_data_points_per_tree = X.shape[0]
         self._model.fit(data, rng=rng)
 
-    def predict(self, X: np.ndarray) -> Tuple[np.ndarray, Optional[np.ndarray]]:
+    def predict(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Predict means and variances for a given X.
 
         Parameters
         ----------
         X : np.ndarray [n_samples, n_features (config + instance features)]
             Training samples.
 
         Returns
         -------
         means : np.ndarray [n_samples, n_objectives]
             Predictive mean.
-        vars : Optional[np.ndarray] [n_samples, n_objectives] or [n_samples, n_samples]
+        vars : np.ndarray [n_samples, n_objectives] or [n_samples, n_samples]
             Predictive variance or standard deviation.
         """
         self._check_dimensions(X)
 
         if self._pca_applied:
             try:
                 X_features = X[:, -self.n_features :]
@@ -339,48 +392,49 @@
             mean = mean.reshape((-1, 1))
 
         if var is not None and len(var.shape) == 1:
             var = var.reshape((-1, 1))
 
         return mean, var
 
-    def _predict(self, X: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+    def _predict(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Predict means and variances for a given X.
 
         Parameters
         ----------
-        X : np.ndarray [n_samples, n_features (config + instance features)]
+        X : np.ndarray
+            [n_samples, n_features (config + instance features)]
 
         Returns
         -------
         means : np.ndarray [n_samples, 1]
             Predictive mean.
         vars : np.ndarray [n_samples, 1]
             Predictive variance.
         """
-
         self._check_dimensions(X)
         X = self._impute_inactive(X)
 
         if self.log_y:
             all_preds = []
             third_dimension = 0
 
-            # Gather data in a list of 2d arrays and get statistics about the required size of the 3d array
+            # Gather data in a list of 2d arrays and get statistics about the required size of the
+            # 3d array
             for row_X in X:
                 preds_per_tree = self._model.all_leaf_values(row_X)
                 all_preds.append(preds_per_tree)
                 max_num_leaf_data = max(map(len, preds_per_tree))
                 third_dimension = max(max_num_leaf_data, third_dimension)
 
             # Transform list of 2d arrays into a 3d array
-            preds_as_array = (
-                np.zeros((X.shape[0], self._model_options.num_trees, third_dimension)) * np.NaN
-            )
+            num_trees = self._model.options.num_trees
+            shape = (X.shape[0], num_trees, third_dimension)
+            preds_as_array = np.zeros(shape) * np.NaN
             for i, preds_per_tree in enumerate(all_preds):
                 for j, pred in enumerate(preds_per_tree):
                     preds_as_array[i, j, : len(pred)] = pred
 
             # Do all necessary computation with vectorized functions
             preds_as_array = np.log(np.nanmean(np.exp(preds_as_array), axis=2) + VERY_SMALL_NUMBER)
 
@@ -398,15 +452,16 @@
         vars_ = np.array(vars_)
 
         return means.reshape((-1, 1)), vars_.reshape((-1, 1))
 
     def predict_marginalized(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Predict mean and variance marginalized over all instances.
-        Returns the predictive mean and variance marginalised over all
+
+        Return the predictive mean and variance marginalized over all
         instances for a set of configurations.
 
         Parameters
         ----------
         X : np.ndarray
             [n_samples, n_features (config)]
 
@@ -426,34 +481,32 @@
             var[var < VERY_SMALL_NUMBER] = VERY_SMALL_NUMBER
             var[np.isnan(var)] = VERY_SMALL_NUMBER
             return mean_, var
 
         X = self._impute_inactive(X)
 
         # marginalized predictions for each tree
-        dat_ = np.zeros((X.shape[0], self._model_options.num_trees))
+        dat_ = np.zeros((X.shape[0], self._model.options.num_trees))
         for i, x in enumerate(X):
-
             # marginalize over instances
             # 1. get all leaf values for each tree
-            # type: list[list[float]]
-            preds_trees = [[] for i in range(self._model_options.num_trees)]
+            preds_trees: List[List[float]] = [[] for i in range(self._model.options.num_trees)]
 
             for feat in self.instance_features:
                 x_ = np.concatenate([x, feat])
                 preds_per_tree = self._model.all_leaf_values(x_)
                 for tree_id, preds in enumerate(preds_per_tree):
                     preds_trees[tree_id] += preds
 
             # 2. average in each tree
             if self.log_y:
-                for tree_id in range(self._model_options.num_trees):
+                for tree_id in range(self._model.options.num_trees):
                     dat_[i, tree_id] = np.log(np.exp(np.array(preds_trees[tree_id])).mean())
             else:
-                for tree_id in range(self._model_options.num_trees):
+                for tree_id in range(self._model.options.num_trees):
                     dat_[i, tree_id] = np.array(preds_trees[tree_id]).mean()
 
         # 3. compute statistics across trees
         mean_ = dat_.mean(axis=1)
         var = dat_.var(axis=1)
 
         var[var < VERY_SMALL_NUMBER] = VERY_SMALL_NUMBER
@@ -461,9 +514,22 @@
         if len(mean_.shape) == 1:
             mean_ = mean_.reshape((-1, 1))
         if len(var.shape) == 1:
             var = var.reshape((-1, 1))
 
         return mean_, var
 
-    def get_leaf_values(self, x: np.ndarray):
+    def get_leaf_values(self, x: np.ndarray) -> regression.binary_rss_forest:
+        """
+        Get the leaf values of the model.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            Input data array.
+
+        Returns
+        -------
+        regression.binary_rss_forest
+            The leaf values of the model.
+        """
         return self._model.all_leaf_values(x)
```

### Comparing `deepcave-1.1.3/deepcave/evaluators/epm/utils.py` & `deepcave-1.2/deepcave/evaluators/epm/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+#  noqa: D400
+"""
+# Utils
+
+This module provides a utility to get the types
+as well as the bounds of the Hyperparameters.
+"""
+
 import typing
 
 import numpy as np
 from ConfigSpace import ConfigurationSpace
 from ConfigSpace.hyperparameters import (
     BetaFloatHyperparameter,
     BetaIntegerHyperparameter,
@@ -15,16 +23,38 @@
 )
 
 
 def get_types(
     config_space: ConfigurationSpace,
     instance_features: typing.Optional[np.ndarray] = None,
 ) -> typing.Tuple[typing.List[int], typing.List[typing.Tuple[float, float]]]:
-    """Return the types of the hyperparameters and the bounds of the
-    hyperparameters and instance features.
+    """
+    Return the types of the Hyperparameters.
+
+    Also return the bounds of the Hyperparameters and instance features.
+
+    Parameters
+    ----------
+    config_space : ConfigurationSpace
+        The configuration space.
+    instance_features : Optional[np.ndarray], optional
+        The instance features.
+        Default is None.
+
+    Returns
+    -------
+    Tuple[typing.List[int], List[Tuple[float, float]]]
+        The types of the Hyperparameters, as well as the bounds and instance features.
+
+    Raises
+    ------
+    ValueError
+        Inactive parameters not supported for Beta and Normal Hyperparameters.
+    TypeError
+        If the Hyperparameter Type is unknown.
     """
     # Extract types vector for rf from config space and the bounds
     types = [0] * len(config_space.get_hyperparameters())
     bounds = [(np.nan, np.nan)] * len(types)
 
     for i, param in enumerate(config_space.get_hyperparameters()):
         parents = config_space.get_parents_of(param.name)
@@ -43,23 +73,23 @@
             n_cats = len(param.sequence)
             types[i] = 0
             if can_be_inactive:
                 bounds[i] = (0, int(n_cats))
             else:
                 bounds[i] = (0, int(n_cats) - 1)
         elif isinstance(param, Constant):
-            # for constants we simply set types to 0 which makes it a numerical
+            # for constants types are simply set to 0 which makes it a numerical
             # parameter
             if can_be_inactive:
                 bounds[i] = (2, np.nan)
                 types[i] = 2
             else:
                 bounds[i] = (0, np.nan)
                 types[i] = 0
-            # and we leave the bounds to be 0 for now
+            # and the bounds are left to be 0 for now
         elif isinstance(param, UniformFloatHyperparameter):
             # Are sampled on the unit hypercube thus the bounds
             # are always 0.0, 1.0
             if can_be_inactive:
                 bounds[i] = (-1.0, 1.0)
             else:
                 bounds[i] = (0, 1.0)
```

### Comparing `deepcave-1.1.3/deepcave/evaluators/fanova.py` & `deepcave-1.2/deepcave/evaluators/fanova.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,49 @@
-from typing import Dict, List, Optional, Tuple, Union
+#  noqa: D400
+"""
+# fANOVA
+
+This module provides a tool for assessing the importance of an algorithms Hyperparameters.
+
+Utilities provide calculation of the data wrt the budget and train the forest on the encoded data.
+
+## Classes
+    - fANOVA: Calculate and provide midpoints and sizes.
+"""
+
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import itertools as it
 
 import numpy as np
 
 from deepcave.constants import COMBINED_COST_NAME
 from deepcave.evaluators.epm.fanova_forest import FanovaForest
 from deepcave.runs import AbstractRun
 from deepcave.runs.objective import Objective
 
 
 class fANOVA:
     """
-    Calculate and provide midpoints and sizes from the forest's
-    split values in order to get the marginals.
+    Calculate and provide midpoints and sizes.
+
+    They are generated from the forest's split values in order to get the marginals.
+
+    Properties
+    ----------
+    run : AbstractRun
+        The Abstract Run used for the calculation.
+    cs : ConfigurationSpace
+        The configuration space of the run.
+    hps : List[Hyperparameters]
+        The Hyperparameters of the configuration space.
+    hp_names : List[str]
+        The corresponding names of the Hyperparameters.
+    n_trees : int
+        The number of trees.
     """
 
     def __init__(self, run: AbstractRun):
         if run.configspace is None:
             raise RuntimeError("The run needs to be initialized.")
 
         self.run = run
@@ -29,36 +55,36 @@
         self,
         objectives: Optional[Union[Objective, List[Objective]]] = None,
         budget: Optional[Union[int, float]] = None,
         n_trees: int = 16,
         seed: int = 0,
     ) -> None:
         """
-        Get the data wrt budget and trains the forest on the encoded data.
+        Get the data with respect to budget and train the forest on the encoded data.
 
         Note
         ----
         Right now, only `n_trees` is used. It can be further specified if needed.
 
         Parameters
         ----------
         objectives : Optional[Union[Objective, List[Objective]]], optional
-            Considerd objectives. By default None. If None, all objectives are considered.
+            Considered objectives. By default None. If None, all objectives are considered.
         budget : Optional[Union[int, float]], optional
             Considered budget. By default None. If None, the highest budget is chosen.
         n_trees : int, optional
             How many trees should be used. By default 16.
         seed : int
             Random seed. By default 0.
         """
         if objectives is None:
             objectives = self.run.get_objectives()
 
         if budget is None:
-            budget = self.get_highest_budget()
+            budget = self.run.get_highest_budget()
 
         self.n_trees = n_trees
 
         # Get data
         df = self.run.get_encoded_data(
             objectives, budget, specific=True, include_combined_cost=True
         )
@@ -70,34 +96,34 @@
         self._model = FanovaForest(self.cs, n_trees=n_trees, seed=seed)
         self._model.train(X, Y)
 
     def get_importances(
         self, hp_names: Optional[List[str]] = None, depth: int = 1, sort: bool = True
     ) -> Dict[Union[str, Tuple[str, ...]], Tuple[float, float, float, float]]:
         """
-        Returns the importance scores from the passed hyperparameter names.
+        Return the importance scores from the passed Hyperparameter names.
 
         Warning
         -------
         Using a depth higher than 1 might take much longer.
 
         Parameters
         ----------
         hp_names : Optional[List[str]]
-            Selected hyperparameter names to get the importance scores from. If None, all
-            hyperparameters of the configspace are used.
+            Selected Hyperparameter names to get the importance scores from. If None, all
+            Hyperparameters of the configuration space are used.
         depth : int, optional
             How often dimensions should be combined. By default 1.
         sort : bool, optional
-            Whether the hyperparameters should be sorted by importance. By default True.
+            Whether the Hyperparameters should be sorted by importance. By default True.
 
         Returns
         -------
         Dict[Union[str, Tuple[str, ...]], Tuple[float, float, float, float]]
-            Dictionary with hyperparameter names and the corresbonding importance scores.
+            Dictionary with Hyperparameter names and the corresponding importance scores.
             The values are tuples of the form (mean individual, var individual, mean total,
             var total). Note that individual and total are the same if depth is 1.
 
         Raises
         ------
         RuntimeError
             If there is zero total variance in all trees.
@@ -108,22 +134,21 @@
         hp_ids = []
         for hp_name in hp_names:
             hp_ids.append(self.cs.get_idx_by_hyperparameter_name(hp_name))
 
         # Calculate the marginals
         vu_individual, vu_total = self._model.compute_marginals(hp_ids, depth)
 
-        importances = {}
+        importances: Dict[Tuple[Any, ...], Tuple[float, float, float, float]] = {}
         for k in range(1, len(hp_ids) + 1):
             if k > depth:
                 break
 
             for sub_hp_ids in it.combinations(hp_ids, k):
                 sub_hp_ids = tuple(sub_hp_ids)
-                importances[sub_hp_ids] = {}
 
                 # clean here to catch zero variance in a trees
                 non_zero_idx = np.nonzero(
                     [self._model.trees_total_variance[t] for t in range(self.n_trees)]
                 )
 
                 if len(non_zero_idx[0]) == 0:
@@ -151,31 +176,32 @@
 
         # Sort by total mean fraction
         if sort:
             importances = {
                 k: v for k, v in sorted(importances.items(), key=lambda item: item[1][2])
             }
 
-        # We want to replace the ids with hyperparameter names again
+        # The ids get replaced with hyperparameter names again
         all_hp_names = self.cs.get_hyperparameter_names()
-        importances_ = {}
-        for hp_ids, values in importances.items():
-            hp_names = [all_hp_names[hp_id] for hp_id in hp_ids]
+        importances_: Dict[Union[str, Tuple[str, ...]], Tuple[float, float, float, float]] = {}
+        for hp_ids_importances, values in importances.items():
+            hp_names = [all_hp_names[hp_id] for hp_id in hp_ids_importances]
+            hp_names_key: Union[Tuple[str, ...], str]
             if len(hp_names) == 1:
-                hp_names = hp_names[0]
+                hp_names_key = hp_names[0]
             else:
-                hp_names = tuple(hp_names)
-            importances_[hp_names] = values
+                hp_names_key = tuple(hp_names)
+            importances_[hp_names_key] = values
 
         return importances_
 
     '''
     def marginal_mean_variance_for_values(self, dimlist, values_to_predict):
         """
-        Returns the marginal of selected parameters for specific values
+        Return the marginal of selected parameters for specific values
 
         Parameters
         ----------
         dimlist: list
                 Contains the indices of ConfigSpace for the selected parameters
                 (starts with 0)
         values_to_predict: list
@@ -190,15 +216,15 @@
         for i in range(len(dimlist)):
             sample[dimlist[i]] = values_to_predict[i]
 
         return self._model.forest.marginal_mean_variance_prediction(sample)
 
     def get_most_important_pairwise_marginals(self, params=None, n=10):
         """
-        Returns the n most important pairwise marginals from the whole ConfigSpace.
+        Return the n most important pairwise marginals from the whole ConfigSpace.
 
         Parameters
         ----------
         params: list of strings or ints
             If specified, limit analysis to those parameters. If ints, interpreting as indices from
             ConfigurationSpace
         n: int
@@ -237,15 +263,15 @@
         for marginal, p1, p2 in pairwise_marginal_performance[:n]:
             self.tot_imp_dict[(p1, p2)] = marginal
 
         return self.tot_imp_dict
 
     def get_triple_marginals(self, params=None):
         """
-        Returns the n most important pairwise marginals from the whole ConfigSpace
+        Return the n most important pairwise marginals from the whole ConfigSpace
 
         Parameters
         ----------
         params: list
              The parameters
 
         Returns
```

### Comparing `deepcave-1.1.3/deepcave/evaluators/footprint.py` & `deepcave-1.2/deepcave/evaluators/footprint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#  noqa: D400
+"""
+# Footprint
+
+This module provides utilities for creating a footprint of a run.
+It uses multidimensional scaling (MDS).
+It also provides utilities to get the surface and the points of the plot.
+
+
+## Classes
+    - Footprint: Can train and create a footprint of a run.
+"""
+
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from ConfigSpace.hyperparameters import (
     CategoricalHyperparameter,
     Constant,
     Hyperparameter,
@@ -16,14 +29,28 @@
 from deepcave.utils.configspace import sample_border_config, sample_random_config
 from deepcave.utils.logs import get_logger
 
 logger = get_logger(__name__)
 
 
 class Footprint:
+    """
+    Can train and create a footprint of a run.
+
+    It uses multidimensional scaling (MDS).
+    Provides utilities to get the surface and the points of the plot.
+
+    Properties
+    ----------
+    run : AbstractRun
+        The AbstractRun used for the calculation of the footprint.
+    cs : ConfigurationSpace
+        The configuration space of the run.
+    """
+
     def __init__(self, run: AbstractRun):
         if run.configspace is None:
             raise RuntimeError("The run needs to be initialized.")
 
         self.run = run
         self.cs = run.configspace
 
@@ -32,23 +59,24 @@
         for hp in self.cs.get_hyperparameters():
             if isinstance(hp, CategoricalHyperparameter):
                 is_categorical.append(True)
             else:
                 is_categorical.append(False)
             depth.append(self._get_depth(hp))
 
-        self._is_categorical = np.array(is_categorical)  # type: ignore
-        self._depth = np.array(depth)  # type: ignore
+        self._is_categorical = np.array(is_categorical)
+        self._depth = np.array(depth)
 
         # Global variables
-        self._distances = None
+        self._distances: Optional[np.ndarray] = None
         self._trained = False
         self._reset()
 
     def _reset(self) -> None:
+        """Reset the footprint."""
         self._objective_model: Optional[RandomForestRegressor] = None
         self._area_model: Optional[RandomForestRegressor] = None
         self._config_ids: Optional[List[int]] = None
         self._incumbent_id: Optional[int] = None
 
         # Those are used to fit the MDS (consists of random and border configs).
         self._X: Optional[np.ndarray] = None
@@ -61,33 +89,38 @@
         budget: Union[int, float],
         support_discretization: Optional[int] = 10,
         rejection_rate: float = 0.01,
         retries: int = 3,
         exclude_configs: bool = False,
     ) -> None:
         """
-        Calculates the distances and trains the model.
+        Calculate the distances and train the model.
 
         Parameters
         ----------
         objective : Objective
-            Objective and colour to show.
+            Objective and color to show.
         budget : Union[int, float]
             All configurations with this budget are considered.
         support_discretization : Optional[int], optional
-            Discretization steps for integer and float hyperparameter values.
+            Discretization steps for integer and float hyperparameter (HP) values.
+            Default is set to 10.
         rejection_rate : float, optional
             Rejection rate whether a configuration should be rejected or not. Internally,
             the max distance is calculated and if a configuration has a distance smaller than
             max distance * rejection_rate, the configuration is rejected.
+            Default is set to 0.01.
         retries : int, optional
             How many times to retry adding a new configuration.
+            Default is set to 3.
         exclude_configs : bool, optional
-            Whether the configurations from the run should be excluded in the MDS scaling.
-            This is particullary interseting if only the search space should be plotted.
+            Whether the configurations from the run should be excluded
+            in the multidimensional scaling (MDS).
+            This is particularly interesting if only the search space should be plotted.
+            Default is set to False.
         """
         # Reset everything
         self._reset()
         self.cs.seed(0)
 
         # Get config rejection threshold
         # If the distance between two configs is smaller than the threshold, the config
@@ -99,30 +132,31 @@
             objective, budget, statuses=Status.SUCCESS, specific=False, include_config_ids=True
         )
         hp_names = self.run.configspace.get_hyperparameter_names()
 
         # Make numpy arrays
         X = data[hp_names].to_numpy()
         Y = data[objective.name].to_numpy()
-        config_ids = data["config_id"].values.tolist()  # type: ignore
+        config_ids = data["config_id"].values.tolist()
 
         # Get the incumbent
         incumbent_config, _ = self.run.get_incumbent(objective, budget)
         self._incumbent_id = self.run.get_config_id(incumbent_config)
 
         # Reshape Y to 2D
         Y = Y.reshape(-1, 1)
 
         # Init distances
         self._init_distances(X, config_ids, exclude_configs=exclude_configs)
+        assert self._distances is not None
 
         border_generator = sample_border_config(self.cs)
         random_generator = sample_random_config(self.cs, d=support_discretization)
 
-        # Now we add the border and random configs
+        # Now the border and random configs are added
         count_border = 0
         count_random = 0
         tries = 0
         logger.info("Starting to calculate distances and add border and random configurations...")
         while True:
             _configs = []
             _config_ids = []
@@ -141,89 +175,89 @@
 
             counter = 0
             for config, config_id in zip(_configs, _config_ids):
                 if config is None:
                     continue
 
                 # Encode config
-                config = np.array(self.run.encode_config(config))
-                rejected = self._update_distances(config, config_id, rejection_threshold)
+                config_array = np.array(self.run.encode_config(config))
+                rejected = self._update_distances(config_array, config_id, rejection_threshold)
                 if not rejected:
                     # Count
                     if config_id == BORDER_CONFIG_ID:
                         count_border += 1
 
                     if config_id == RANDOM_CONFIG_ID:
                         count_random += 1
 
                     counter += 1
 
             # Abort criteria
-            # If we don't get new configs
+            # If there are no new configs
             if counter == 0:
                 tries += 1
             else:
                 tries = 0
 
             if tries >= retries:
                 break
 
-            # Or if we reach more than 4000 (otherwise it takes too long)
-            assert self._distances is not None
-
+            # Or if reach more than 4000 are reached (otherwise it takes too long)
             if self._distances.shape[0] % 100 == 0:
                 logger.info(f"Found {self._distances.shape[0]} configurations...")
 
             if self._distances.shape[0] > 4000:
                 break
 
-        assert self._distances is not None
         logger.info(f"Added {count_border} border configs and {count_random} random configs.")
         logger.info(f"Total configurations: {self._distances.shape[0]}.")
         logger.info("Getting MDS data...")
 
         # Calculate MDS now to get 2D coordinates and set those points to reach them later.
         MDS_X = self._get_mds()
         self._MDS_X = MDS_X
 
         # But here's the catch: Get rid of border and random configs because
-        # we don't have the y values for them.
-        # However, it makes no sense to train the RF if we exclude the configs
+        # the y values for them are not known.
+        # However, it makes no sense to train the RF if the configs are excluded
         # which were evaluated.
         if not exclude_configs:
             self._train_on_objective(MDS_X[: len(X)], Y.ravel())
             self._trained = True
         else:
             self._trained = False
 
         # Train on areas can be done anytime.
         self._train_on_areas()
 
     def get_surface(
         self, details: float = 0.5, performance: bool = True
     ) -> Tuple[List, List, List]:
         """
-        Get surface of the MDS plot.
+        Get surface of the multidimensional scaling (MDS) plot.
 
         Parameters
         ----------
         details : float, optional
             Steps to create the meshgrid. By default 0.5.
         performance : bool, optional
             Whether to get the surface from the performance or the valid areas.
+            Default is set to True (i.e. from performance).
 
         Returns
         -------
         Tuple[List, List, List]
             x (1D), y (1D) and z (2D) arrays for heatmap.
 
         Raises
         ------
         RuntimeError
             If `calculate` was not called before.
+        RuntimeError
+            If evaluated configs weren't included.
         """
         X = self._MDS_X
         if X is None:
             raise RuntimeError("You need to call `calculate` first.")
 
         if performance and not self._trained:
             raise RuntimeError(
@@ -251,15 +285,15 @@
         z = model.predict(conc)
         z = z.reshape(x_mesh.shape)
 
         return x.tolist(), y.tolist(), z.tolist()
 
     def get_points(self, category: str = "configs") -> Tuple[List[float], List[float], List[int]]:
         """
-        Returns the points of the MDS plot.
+        Return the points of the multidimensional scaling (MDS) plot.
 
         Parameters
         ----------
         category : str, optional
             Points of a specific category. Chose between `configs`, `borders`, `supports`
             or `incumbents`. By default `configs`.
 
@@ -268,14 +302,16 @@
         Tuple[List[float], List[float], List[int]]
             X, Y and config_ids as lists.
 
         Raises
         ------
         RuntimeError
             If category is not supported.
+        RuntimeError
+            If calculated wasn't called before.
         """
         if category not in ["configs", "borders", "supports", "incumbents"]:
             raise RuntimeError("Unknown category.")
 
         if self._MDS_X is None or self._config_ids is None:
             raise RuntimeError("You need to call `calculate` first.")
 
@@ -285,94 +321,113 @@
         for x, config_id in zip(self._MDS_X, self._config_ids):
             if (
                 (category == "configs" and config_id >= 0)
                 or (category == "borders" and config_id == BORDER_CONFIG_ID)
                 or (category == "incumbents" and config_id == self._incumbent_id)
                 or (category == "supports" and config_id == RANDOM_CONFIG_ID)
             ):
-                x = x.tolist()  # type: ignore
+                x = x.tolist()
                 X += [x[0]]
                 Y += [x[1]]
                 config_ids += [config_id]
 
         return X, Y, config_ids
 
     def _get_max_distance(self) -> float:
         """
         Calculate the maximum distance between all configs.
-        Basically, we just count the number of hps.
+
+        Basically, the number of Hyperparameters are just counted.
 
         Returns
         -------
         float
             Maximal distance between two configurations.
         """
-        # We just count the number of hps
-        # Since X is normalized, we can just sum 1
+        # The number of hps is just counted
+        # Since X is normalized, 1 can just be added
         max_distance = 0
         for hp in self.cs.get_hyperparameters():
             if isinstance(hp, CategoricalHyperparameter) or isinstance(hp, Constant):
                 continue
 
             max_distance += 1
 
         return max_distance
 
     def _get_distance(self, x: np.ndarray, y: np.ndarray) -> float:
         """
-        Calculates distance between x and y. Both arrays must have the same length.
+        Calculate distance between x and y. Both arrays must have the same length.
 
         Parameters
         ----------
         x : np.ndarray
             Configuration 1.
         y : np.ndarray
             Configuration 2.
 
         Returns
         -------
         float
             Distance from configuration 1 and configuration 2.
+
+        Raises
+        ------
+        RuntimeError
+            If calculate wasn't called first.
         """
         if self._depth is None or self._is_categorical is None:
             raise RuntimeError("You need to call `calculate` first.")
 
         d = np.abs(x - y)
         d[np.isnan(d)] = 1
         d[np.logical_and(self._is_categorical, d != 0)] = 1
         d = np.sum(d / self._depth)
 
         return d
 
     def _get_distances(self, X: np.ndarray) -> np.ndarray:
+        """
+        Get the distances between the configurations.
+
+        Parameters
+        ----------
+        X : np.ndarray
+            The configurations.
+
+        Returns
+        -------
+        np.ndarray
+            The calculated distances.
+        """
         n_configs = X.shape[0]
 
-        # We initiate the distances
+        # The distances are initiated
         distances = np.zeros((n_configs, n_configs))
 
         for i in tqdm(range(n_configs)):
             for j in range(i + 1, n_configs):
                 d = self._get_distance(X[i, :], X[j, :])
                 distances[i, j] = d
                 distances[j, i] = d
 
         return distances
 
     def _init_distances(
         self, X: np.ndarray, config_ids: List[int], exclude_configs: bool = False
     ) -> None:
         """
-        Initializes the distances.
+        Initialize the distances.
 
         Parameters
         ----------
         X : np.ndarray
             Encoded data.
         config_ids : List[int]
-            Corresponding config_ids.
+            Corresponding configuration ids.
         exclude_configs : bool, optional
             Whether the passed X should be used or not. By default False.
         """
         if not exclude_configs:
             self._X = X.copy()
             self._config_ids = config_ids
             self._distances = self._get_distances(X)
@@ -385,32 +440,34 @@
     def _update_distances(
         self,
         config: np.ndarray,
         config_id: int,
         rejection_threshold: Optional[float] = 0.0,
     ) -> bool:
         """
-        Updates the internal distance if the passed config is not rejectded.
+        Update the internal distance if the passed configuration is not rejected.
 
         Parameters
         ----------
         config : np.ndarray
-            Config, which is tried to be added.
+            Configuration, which is tried to be added.
         config_id : int
-            Corresponding config id. This is important for later identification as the config might
-            be a border or random configuration.
+            Corresponding configuration id. This is important for later identification
+            as the configuration might be a border or random configuration.
         rejection_threshold : Optional[float], optional
-            Threshold for rejecting the config. By default 0.0.
+            Threshold for rejecting the configuration. By default 0.0.
 
         Returns
         -------
         rejected : bool
-            Whether the config was rejected or not.
+            Whether the configuration was rejected or not.
         """
         X = self._X
+
+        assert self._distances is not None
         distances = self._distances
 
         if X is None:
             X = np.array([[]])
             n_configs = 0
         else:
             n_configs = X.shape[0]
@@ -439,31 +496,34 @@
             # Add to X here
             if X.shape[1] == 0:
                 X = np.array([config])
             else:
                 X = np.concatenate((X, np.array([config])), axis=0)
 
             self._X = X
-            self._config_ids += [config_id]
+            # There is no += to a None, an Issue has already been created
+            if self._config_ids is not None:
+                self._config_ids += [config_id]
             self._distances = new_distances
 
         return rejected
 
     def _get_depth(self, hp: Hyperparameter) -> int:
         """
-        Get depth (generations above) in configuration space of a given hyperparameter.
+        Get depth (generations above) in configuration space of a given hyperparameter (HP).
 
         Parameters
         ----------
-        param: str
-            name of parameter to inspect
+        hp: Hyperparameter
+            name of Hyperparameter to inspect
 
         Returns
+        -------
         int
-            Depth of the hyperparameter.
+            Depth of the Hyperparameter.
         """
         parents = self.cs.get_parents_of(hp)
         if not parents:
             return 1
 
         new_parents = parents
         d = 1
@@ -478,58 +538,63 @@
                 else:
                     return d
 
         return d
 
     def _get_mds(self) -> np.ndarray:
         """
-        Perform MDS on the internal distances.
-
-        Parameters
-        ----------
-        distances : np.ndarray
-            Numpy array with distances between configurations.
+        Perform multidimensional scaling (MDS) on the internal distances.
 
         Returns
         -------
         np.ndarray
-            Numpy array with MDS coordinates in 2D.
+            Numpy array with multidimensional scaling (MDS) coordinates in 2D.
+
+        Raises
+        ------
+        RuntimeError
+            When calculated wasn't called first.
         """
         if self._distances is None:
             raise RuntimeError("You need to call `calculate` first.")
 
         mds = MDS(n_components=2, dissimilarity="precomputed", random_state=0)
         return mds.fit_transform(self._distances)
 
     def _train_on_objective(self, X: np.ndarray, Y: np.ndarray) -> None:
         """
-        Trains the random forest on the performance.
+        Train the random forest on the performance.
 
         Parameters
         ----------
         X : np.ndarray
-            Numpy array with MDS coordinates in 2D.
+            Numpy array with multidimensional scaling (MDS) coordinates in 2D.
         Y : np.ndarray
             Numpy array with costs.
         """
         logger.info("Training on objective...")
         self._objective_model = RandomForestRegressor(random_state=0)
         self._objective_model.fit(X, Y)
 
     def _train_on_areas(self) -> None:
         """
-        Trains the random forest on the "valid" areas.
+        Train the random forest on the "valid" areas.
+
+        Raises
+        ------
+        RuntimeError
+            If calculated wasn't called first.
         """
         if self._MDS_X is None:
             raise RuntimeError("You need to call `calculate` first.")
 
         logger.info("Training on area...")
         MDS_X = self._MDS_X
 
-        # We basically have to create a grid here
+        # Basically, a grid has to be created here
         x_min, x_max = MDS_X[:, 0].min() - 1, MDS_X[:, 0].max() + 1
         y_min, y_max = MDS_X[:, 1].min() - 1, MDS_X[:, 1].max() + 1
 
         x = np.linspace(x_min, x_max, 20)
         y = np.linspace(y_min, y_max, 20)
 
         X = []
@@ -544,13 +609,13 @@
                     if a >= x1 and a <= x2 and b >= y1 and b <= y2:
                         value = 1
                         break
 
                 X.append(center)
                 Y.append(value)
 
-        X = np.array(X)  # type: ignore
-        Y = np.array(Y)  # type: ignore
+        X_array = np.array(X)
+        Y_array = np.array(Y)
 
         # Train the model
         self._area_model = RandomForestRegressor(random_state=0)
-        self._area_model.fit(X, Y)
+        self._area_model.fit(X_array, Y_array)
```

### Comparing `deepcave-1.1.3/deepcave/evaluators/lpi.py` & `deepcave-1.2/deepcave/evaluators/lpi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-from typing import Dict, List, Optional, Tuple, Union
+#  noqa: D400
+"""
+# LPI
 
-from random import random
+This module provides utilities to calculate the local parameter importance (LPI).
+
+## Classes
+    - LPI: This class calculates the local parameter importance (LPI).
+"""
+
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from ConfigSpace import Configuration
 from ConfigSpace.c_util import change_hp_value, check_forbidden
 from ConfigSpace.exceptions import ForbiddenValueError
 from ConfigSpace.hyperparameters import CategoricalHyperparameter
 from ConfigSpace.util import impute_inactive_values
@@ -13,84 +21,121 @@
 from deepcave.evaluators.epm.fanova_forest import FanovaForest
 from deepcave.runs import AbstractRun
 from deepcave.runs.objective import Objective
 
 
 # https://github.com/automl/ParameterImportance/blob/f4950593ee627093fc30c0847acc5d8bf63ef84b/pimp/evaluator/local_parameter_importance.py#L27
 class LPI:
+    """
+    Calculate the local parameter importance (LPI).
+
+    Properties
+    ----------
+    run : AbstractRun
+        The AbstractRun to get the importance from.
+    cs : ConfigurationSpace
+        The configuration space of the run.
+    hp_names : List[str]
+        The names of the Hyperparameters.
+    variances : Dict[Any, list]
+        The overall variances per tree.
+    importances : dict
+        The importances of the Hyperparameters.
+    continuous_neighbors : int
+        The number of neighbors chosen for continuous Hyperparameters.
+    incumbent : Configuration
+        The incumbent of the run.
+    default : Configuration
+        A configuration containing Hyperparameters with default values.
+    incumbent_array : numpy.ndarray
+        The internal vector representation of the incumbent.
+    seed : int
+        The seed. If not provided it will be random.
+    rs : RandomState
+        A random state with a given seed value.
+    """
+
     def __init__(self, run: AbstractRun):
         self.run = run
         self.cs = run.configspace
         self.hp_names = self.cs.get_hyperparameter_names()
-        self.variances = None
-        self.importances = None
+        self.variances: Optional[Dict[Any, List[Any]]] = None
+        self.importances: Optional[Dict[Any, Any]] = None
 
     def calculate(
         self,
         objectives: Optional[Union[Objective, List[Objective]]] = None,
         budget: Optional[Union[int, float]] = None,
         continous_neighbors: int = 500,
         n_trees: int = 10,
         seed: int = 0,
     ) -> None:
         """
-        Prepares the data and trains a RandomForest model.
+        Prepare the data and train a RandomForest model.
 
         Parameters
         ----------
         objectives : Optional[Union[Objective, List[Objective]]], optional
-            Considerd objectives. By default None. If None, all objectives are considered.
+            Considered objectives. By default, None. If None, all objectives are considered.
         budget : Optional[Union[int, float]], optional
-            Considered budget. By default None. If None, the highest budget is chosen.
-        continous_neighbors : int, optional
-            How many neighbors should be chosen for continous hyperparameters. By default 500.
+            Considered budget. By default, None. If None, the highest budget is chosen.
+        continuous_neighbors : int, optional
+            How many neighbors should be chosen for continuous hyperparameters (HPs).
+            By default, 500.
+        n_trees : int, optional
+            The number of trees for the fanova forest.
+            Default is 10.
+        seed : Optional[int], optional
+            The seed. By default None. If None, a random seed is chosen.
         """
         if objectives is None:
             objectives = self.run.get_objectives()
 
         if budget is None:
-            budget = self.get_highest_budget()
+            budget = self.run.get_highest_budget()
 
         # Set variables
         self.continous_neighbors = continous_neighbors
         self.incumbent, _ = self.run.get_incumbent(budget=budget)
         self.default = self.cs.get_default_configuration()
         self.incumbent_array = self.incumbent.get_array()
 
         self.seed = seed
         self.rs = np.random.RandomState(seed)
 
         # Get data
-        df = self.run.get_encoded_data(budget=budget, specific=True, include_combined_cost=True)
+        df = self.run.get_encoded_data(
+            objectives=objectives, budget=budget, specific=True, include_combined_cost=True
+        )
         X = df[self.hp_names].to_numpy()
         Y = df[COMBINED_COST_NAME].to_numpy()
 
         # Get model and train it
         # Use same forest as for fanova
         self._model = FanovaForest(self.cs, n_trees=n_trees, seed=seed)
         self._model.train(X, Y)
 
         # Get neighborhood sampled on an unit-hypercube.
         neighborhood = self._get_neighborhood()
 
-        # We need the delta performance from the default configuration and the incumbent
+        # The delta performance is needed from the default configuration and the incumbent
         def_perf, def_var = self._predict_mean_var(self.default)
         inc_perf, inc_var = self._predict_mean_var(self.incumbent)
         delta = def_perf - inc_perf
 
         # These are used for plotting and hold the predictions for each neighbor of each parameter.
         # That means performances holds the mean, variances the variance of the forest.
-        performances = {}
-        variances = {}
-        # This are used for importance and hold the corresponding importance/variance over
+        performances: Dict[str, List[np.ndarray]] = {}
+        variances: Dict[str, List[np.ndarray]] = {}
+        # These are used for importance and hold the corresponding importance/variance over
         # neighbors. Only import if NOT quantifying importance via performance-variance across
-        # neighbours.
+        # neighbors.
         importances = {}
         # Nested list of values per tree in random forest.
-        predictions = {}
+        predictions: Dict[str, List[List[np.ndarray]]] = {}
 
         # Iterate over parameters
         for hp_idx, hp_name in enumerate(self.incumbent.keys()):
             if hp_name not in neighborhood:
                 continue
 
             performances[hp_name] = []
@@ -174,37 +219,40 @@
         ]
 
         # Normalize
         overall_var_per_tree = {
             p: [t / sum_var_per_tree[idx] for idx, t in enumerate(trees)]
             for p, trees in overall_var_per_tree.items()
         }
-
         self.variances = overall_var_per_tree
         self.importances = importances
 
     def get_importances(self, hp_names: List[str]) -> Dict[str, Tuple[float, float]]:
         """
-        Returns the importances.
+        Return the importances.
 
         Parameters
         ----------
         hp_names : List[str]
-            Selected hyperparameter names to get the importance scores from.
+            Selected Hyperparameter names to get the importance scores from.
 
         Returns
         -------
         importances : Dict[str, Tuple[float, float]]
             Hyperparameter name and mean+var importance.
-        """
 
+        Raises
+        ------
+        RuntimeError
+            If the important scores are not calculated.
+        """
         if self.importances is None or self.variances is None:
             raise RuntimeError("Importance scores must be calculated first.")
 
-        importances = {}
+        importances: Dict[str, Tuple[float, float]] = {}
         for hp_name in hp_names:
             mean = 0
             std = 0
 
             if hp_name in self.importances:
                 mean = self.importances[hp_name][0]
                 std = np.var(self.variances[hp_name])
@@ -218,23 +266,29 @@
                 mean = 0
                 std = 0
 
             importances[hp_name] = (mean, std)
 
         return importances
 
-    def _get_neighborhood(self):
+    def _get_neighborhood(self) -> Dict[str, List[Union[np.ndarray, List[np.ndarray]]]]:
         """
-        Slight modification of ConfigSpace's get_one_exchange neighborhood. This orders the
-        parameter values and samples more neighbors in one go. Further we need to rigorously
-        check each and every neighbor if it is forbidden or not.
+        Slight modification of ConfigSpace's get_one_exchange neighborhood.
+
+        This orders the parameter values and samples more neighbors in one go.
+        Further each and every neighbor needs to be rigorously checked if it is forbidden or not.
+
+        Returns
+        -------
+        neighborhood : Dict[str, List[Union[np.ndarray, List[np.ndarray]]]]
+            The neighborhood.
         """
         hp_names = self.cs.get_hyperparameter_names()
 
-        neighborhood = {}
+        neighborhood: Dict[str, List[Union[np.ndarray, List[np.ndarray]]]] = {}
         for hp_idx, hp_name in enumerate(hp_names):
             # Check if hyperparameter is active
             if not np.isfinite(self.incumbent_array[hp_idx]):
                 continue
 
             hp_neighborhood = []
             checked_neighbors = []  # On unit cube
@@ -245,24 +299,24 @@
             if num_neighbors == 0:
                 continue
             elif np.isinf(num_neighbors):
                 if hp.log:
                     base = np.e
                     log_lower = np.log(hp.lower) / np.log(base)
                     log_upper = np.log(hp.upper) / np.log(base)
-                    neighbors = np.logspace(
+                    neighbors_range = np.logspace(
                         start=log_lower,
                         stop=log_upper,
                         num=self.continous_neighbors,
                         endpoint=True,
                         base=base,
                     )
                 else:
-                    neighbors = np.linspace(hp.lower, hp.upper, self.continous_neighbors)
-                neighbors = list(map(lambda x: hp._inverse_transform(x), neighbors))
+                    neighbors_range = np.linspace(hp.lower, hp.upper, self.continous_neighbors)
+                neighbors = list(map(lambda x: hp._inverse_transform(x), neighbors_range))
             else:
                 neighbors = hp.get_neighbors(self.incumbent_array[hp_idx], self.rs)
 
             for neighbor in neighbors:
                 if neighbor in checked_neighbors:
                     continue
 
@@ -280,46 +334,48 @@
                 except (ForbiddenValueError, ValueError):
                     pass
 
             sort_idx = list(
                 map(lambda x: x[0], sorted(enumerate(checked_neighbors), key=lambda y: y[1]))
             )
             if isinstance(self.cs.get_hyperparameter(hp_name), CategoricalHyperparameter):
-                checked_neighbors_non_unit_cube = list(
+                checked_neighbors_non_unit_cube_categorical = list(
                     np.array(checked_neighbors_non_unit_cube)[sort_idx]
                 )
+                neighborhood[hp_name] = [
+                    np.array(checked_neighbors)[sort_idx],
+                    checked_neighbors_non_unit_cube_categorical,
+                ]
             else:
-                checked_neighbors_non_unit_cube = np.array(checked_neighbors_non_unit_cube)[
-                    sort_idx
+                checked_neighbors_non_unit_cube_non_categorical = np.array(
+                    checked_neighbors_non_unit_cube
+                )[sort_idx]
+                neighborhood[hp_name] = [
+                    np.array(checked_neighbors)[sort_idx],
+                    checked_neighbors_non_unit_cube_non_categorical,
                 ]
 
-            neighborhood[hp_name] = [
-                np.array(checked_neighbors)[sort_idx],
-                checked_neighbors_non_unit_cube,
-            ]
-
         return neighborhood
 
-    def _predict_mean_var(self, config):
+    def _predict_mean_var(self, config: Configuration) -> Tuple[np.ndarray, np.ndarray]:
         """
         Small wrapper to predict marginalized over instances.
 
         Parameter
         ---------
         config:Configuration
-            The self.incumbent of wich the performance across the whole instance set is to be
+            The self.incumbent of which the performance across the whole instance set is to be
             estimated.
 
         Returns
         -------
-        mean
+        mean: np.ndarray
             The mean performance over the instance set.
-        var
+        var: np.ndarray
             The variance over the instance set. If logged values are used, the variance might not
             be able to be used.
         """
-
         config = impute_inactive_values(config)
         array = np.array([config.get_array()])
         mean, var = self._model.predict_marginalized(array)
 
         return mean.squeeze(), var.squeeze()
```

### Comparing `deepcave-1.1.3/deepcave/layouts/general.py` & `deepcave-1.2/deepcave/layouts/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+#  noqa: D400
+"""
+# GeneralLayout
+
+This module provides the General Layout.
+
+It handles different callbacks of the layout.
+
+## Classes
+    - GeneralLayout: Provide different utilities to handle callbacks for the layout.
+"""
+
 from typing import Dict, List, Optional, Type
 
 from pathlib import Path
 
 import dash_bootstrap_components as dbc
 from dash import dcc, html
 from dash.dependencies import ALL, Input, Output, State
@@ -13,24 +25,35 @@
 from deepcave.runs import NotMergeableError
 from deepcave.runs.run import Run
 from deepcave.utils.layout import help_button
 from deepcave.utils.util import short_string
 
 
 class GeneralLayout(Layout):
+    """
+    Provide different utilities to handle callbacks for the general layout.
+
+    Properties
+    ----------
+    logger : Logger
+        A logger used for debug information of the groups.
+    """
+
     def register_callbacks(self) -> None:
+        """Register if there were any callbacks."""
         self._callback_working_directory_changed()
         self._callback_display_available_runs()
         self._callback_display_selected_runs()
         self._callback_manage_run()
         self._callback_display_groups()
         self._callback_manage_groups()
         self._callback_clear_cache()
 
     def _callback_working_directory_changed(self) -> None:
+        """Check for change in working directory."""
         inputs = [
             Input("on-page-load", "href"),
             Input("general-working-directory-input", "value"),
             # Those inputs are for changing working directory quickly
             # (if someone is pressing on a directory)
             # Only works with "ALL"
             Input({"type": "general-dynamic-change-directory", "index": ALL}, "n_clicks"),
@@ -43,20 +66,32 @@
             # Converter text
             Output("general-converter-label", "children"),
             Output("general-available-runs", "data"),
         ]
 
         # Register updates from inputs
         @app.callback(outputs, inputs)  # type: ignore
-        def callback(  # type: ignore
+        def callback(
             _,
             working_dir: str,
             dynamic_n_clicks: List[Optional[int]],
             dynamic_working_dirs: List[str],
         ):
+            """
+            Register updates from inputs.
+
+            Parameters
+            ----------
+            working_dir : str
+                The working directory.
+            dynamic_n_clicks : List[Optional[int]]
+                The number of clicks.
+            dynamic_working_dirs : List[str]
+                The working directories.
+            """
             # `working_dir` is only none on page load
             if working_dir is None:
                 # Handler working directory
                 working_dir = run_handler.get_working_directory()
                 converter = run_handler.available_run_classes
             else:
                 for dir, n_clicks in zip(dynamic_working_dirs, dynamic_n_clicks):
@@ -70,19 +105,28 @@
             return (
                 str(working_dir),
                 self.get_converter_text(converter),
                 run_handler.get_available_run_paths(),
             )
 
     def _callback_display_available_runs(self) -> None:
+        """Display available runs."""
         output = Output("general-available-runs-container", "children")
         input = Input("general-available-runs", "data")
 
         @app.callback(output, input)  # type: ignore
-        def callback(run_paths: List[str]):  # type: ignore
+        def callback(run_paths: List[str]):
+            """
+            Display the available runs.
+
+            Parameters
+            ----------
+            run_paths : List[str]
+                The run paths.
+            """
             children = []
 
             # Add text to go to parent directory
             new_element = html.Div(
                 [
                     dbc.Button(
                         "+", id={"type": "general-dynamic-add-run", "index": -1}, disabled=True
@@ -122,19 +166,28 @@
 
             if len(children) == 0:
                 return html.Div("No runs found.")
 
             return children
 
     def _callback_display_selected_runs(self) -> None:
+        """Display the selected runs."""
         output = Output("general-selected-runs-container", "children")
         input = Input("general-selected-runs", "data")
 
         @app.callback(output, input)  # type: ignore
-        def callback(run_paths: List[str]):  # type: ignore
+        def callback(run_paths: List[str]):
+            """
+            Display the selected runs.
+
+            Parameters
+            ----------
+            run_paths : List[str]
+                The run paths.
+            """
             children = []
 
             for i, run_path in enumerate(run_paths):
                 run_name = run_handler.get_run_name(run_path)
 
                 shortened_run_path = short_string(run_path, 30, mode="prefix")
 
@@ -167,14 +220,15 @@
 
             if len(children) == 0:
                 return html.Div("No runs selected.")
 
             return children
 
     def _callback_manage_run(self) -> None:
+        """Manage runs, including adding and removing them."""
         outputs = [
             Output({"type": "general-dynamic-add-run", "index": ALL}, "n_clicks"),
             Output({"type": "general-dynamic-remove-run", "index": ALL}, "n_clicks"),
             Output("general-selected-runs", "data"),
         ]
 
         inputs = [
@@ -184,17 +238,16 @@
 
         states = [
             State({"type": "general-dynamic-available-run-path", "index": ALL}, "data"),
             State({"type": "general-dynamic-selected-run-path", "index": ALL}, "data"),
         ]
 
         @app.callback(outputs, inputs, states)  # type: ignore
-        def callback(  # type: ignore
-            add_n_clicks, remove_n_clicks, available_run_paths, selected_run_paths
-        ):
+        def callback(add_n_clicks, remove_n_clicks, available_run_paths, selected_run_paths):
+            """Add and remove runs."""
             # Add run path
             for n_click, run_path in zip(add_n_clicks, available_run_paths):
                 if n_click is not None:
                     success = run_handler.add_run(run_path)
                     if not success:
                         notification.update("The run could not be added.")
 
@@ -209,34 +262,56 @@
 
             # Remove last inputs
             c.set("last_inputs", value={})
 
             return add_n_clicks, remove_n_clicks, run_handler.get_selected_run_paths()
 
     def _callback_display_groups(self) -> None:
+        """Responsible of displaying the groups."""
         outputs = [
             Output("general-group-container", "children"),
             Output("general-add-group", "n_clicks"),
         ]
         inputs = [
             Input("general-add-group", "n_clicks"),
             Input("general-selected-runs-container", "children"),
             Input("general-group-trigger", "data"),
             State("general-group-container", "children"),
         ]
 
         # Let's take care of the groups here
         @app.callback(outputs, inputs)  # type: ignore
-        def callback(n_clicks: int, _trigger1, _trigger2, children):  # type: ignore
+        def callback(n_clicks: int, _trigger1, _trigger2, children):
+            """Display groups."""
+
             def get_layout(
                 index: int,
                 options: Dict[str, str],
                 input_value: str = "",
                 dropdown_value: Optional[List[str]] = None,
             ) -> Component:
+                """
+                Get the layout for the groups.
+
+                Parameters
+                ----------
+                index : int
+                    The index.
+                options : Dict[str, str]
+                    The options.
+                input_value : str, optional
+                    The input value, by default "".
+                dropdown_value : Optional[List[str]], optional
+                    The dropdown value, by default None.
+
+                Returns
+                -------
+                Component
+                    The layout for the groups.
+                """
                 if dropdown_value is None:
                     dropdown_value = []
 
                 return html.Div(
                     [
                         dbc.Input(
                             id={"type": "group-name", "index": index},
@@ -258,106 +333,148 @@
             groups = run_handler.get_selected_groups()
             selected_run_paths = run_handler.get_selected_run_paths()
             selected_runs = {p: run_handler.get_run_name(p) for p in selected_run_paths}
             index = 0
 
             # Load from cache if page is loaded
             children = []
+
             for name, paths in groups.items():
                 if name is None:
                     continue
 
                 children.append(get_layout(index, selected_runs, name, paths))
 
                 index += 1
 
             if n_clicks is not None and len(selected_runs) > 0:
                 children.append(get_layout(index, selected_runs))
 
             return children, None
 
     def _callback_manage_groups(self) -> None:
+        """Manage the groups."""
         outputs = Output("general-group-trigger", "data")
         inputs = [
             Input({"type": "group-name", "index": ALL}, "value"),
             Input({"type": "group-dropdown", "index": ALL}, "value"),
             State("general-group-trigger", "data"),
         ]
 
         @app.callback(outputs, inputs)  # type: ignore
-        def callback(group_names, all_run_paths, i):  # type: ignore
+        def callback(group_names: List[str], all_run_paths, i):
+            """Manage the groups."""
             # Abort on page load
+            self._refresh_groups: bool
             if self._refresh_groups:
                 self._refresh_groups = False
                 raise PreventUpdate()
 
+            # For the default group names, if no name was entered
+            group_counter = 0
+
             groups = {}
             for group_name, run_paths in zip(group_names, all_run_paths):
                 if group_name is None or group_name == "":
-                    continue
+                    # Set the default group name with a counter,
+                    # so the groups dont overwrite themselves
+                    group_name_unavailable = True
+
+                    groups_cache = c.get("groups")
+                    if groups_cache is None:
+                        continue
+
+                    # Check to see that no group name that already exists
+                    # gets picked
+                    while group_name_unavailable:
+                        group_name = f"Group {group_counter}"
+                        assert groups_cache is not None
+                        if group_name not in groups_cache.keys():
+                            group_name_unavailable = False
+                        else:
+                            group_counter += 1
 
                 if run_paths is None or len(run_paths) == 0:
                     continue
 
                 valid_run_paths = []
                 for run_path in run_paths:
                     if run_path in run_handler.get_selected_run_paths():
                         valid_run_paths.append(run_path)
 
                 if len(valid_run_paths) == 0:
                     continue
 
                 groups[group_name] = valid_run_paths
 
+            # Sort the groups alphabetically, so when added
+            # they appear ordered
+            sorted_groups = dict(sorted(groups.items()))
+
             try:
                 # Now save it
-                run_handler.update_groups(groups)
+                run_handler.update_groups(sorted_groups)
             except NotMergeableError:
                 notification.update("The selected runs are not mergeable.")
 
                 # This will automatically trigger the group display s.t. the selection is redo.
                 return i + 1
 
-            self.logger.debug(f"Groups: {groups}")
+            self.logger.debug(f"Groups: {sorted_groups}")
 
             raise PreventUpdate()
 
     def _callback_clear_cache(self) -> None:
+        """Responsible for clearing the cache."""
         output = Output("general-clear-cache-button", "n_clicks")
         input = Input("general-clear-cache-button", "n_clicks")
 
         @app.callback(output, input)  # type: ignore
-        def callback(n_clicks):  # type: ignore
+        def callback(n_clicks):
+            """Clear the cache, stop all running jobs, create new run caches."""
             if n_clicks is not None:
                 rc.clear()
 
                 # Also remove last inputs
                 c.set("last_inputs", value={})
 
-                # Also: We have to stop all running jobs
+                # Also: All the running jobs have to be stopped
                 queue.delete_jobs()
 
-                # We have to call `update_runs` now to create the run caches again
+                # `update_runs` has to be called now to create the run caches again
                 run_handler.update_runs()
                 notification.update("Plugin caches successfully cleared.", "success")
 
             return None
 
     @staticmethod
     def get_converter_text(converters: List[Type[Run]]) -> html.Div:
+        """
+        Get the text for the available run converters.
+
+        Parameters
+        ----------
+        converters : List[Type[Run]]
+            A list of the avaialble run converters.
+
+        Returns
+        -------
+        html.Div
+            The text with all the available converters.
+        """
         converter_text = []
         for converter in converters:
             converter_text += [converter.prefix]
 
         return html.Div(
             html.Span(f"Available run converters: {', '.join(converter_text)}"),
             className="mt-2",
         )
 
-    def __call__(self) -> List[Component]:
+    def __call__(self) -> List[Component]:  # noqa: D102
         self._refresh_groups = True
 
         return [
             html.H1("General"),
             # Working dir
             dbc.Label("Working Directory"),
             help_button("Relative and absolute paths are supported."),
```

### Comparing `deepcave-1.1.3/deepcave/layouts/main.py` & `deepcave-1.2/deepcave/layouts/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-from typing import Dict, List
+#  noqa: D400
+"""
+# MainLayout
+
+This module provides and defines the visualization of the main layout.
+
+Also registers and handles the callbacks.
+
+## Classes
+    - MainLayout: This class defines and provides the main layout.
+"""
+
+from typing import Any, Dict, List
 
 from urllib.parse import urlparse
 
 from dash import dcc, html
 from dash.dependencies import Input, Output
 from dash.development.base_component import Component
 
@@ -14,32 +26,67 @@
 from deepcave.layouts.notification import NotificationLayout
 from deepcave.layouts.sidebar import SidebarLayout
 from deepcave.plugins import Plugin
 from deepcave.utils.dash import alert
 
 
 class MainLayout(Layout):
+    """
+    Define and provide the main layout.
+
+    Handle different callbacks of the layout.
+
+    Properties
+    ----------
+    plugins : Dict[str, Plugin]
+        A dictionary containing the different plugins.
+    sidebar_layout : SidebarLayout
+        A sidebar layout with the categorized plugins.
+    head_layout : HeaderLayout
+        The header layout.
+    general_layout : GeneralLayout
+        The general layout.
+    notification_layout : NotificationLayout
+        The notification layout.
+    not_found_layout : NotFoundLayout
+        The Not Found layout.
+    """
+
     def __init__(self, categorized_plugins: Dict[str, List[Plugin]]):
         super().__init__()
         self.plugins = {}
         self.sidebar_layout = SidebarLayout(categorized_plugins)
         self.header_layout = HeaderLayout()
         self.general_layout = GeneralLayout()
         self.notification_layout = NotificationLayout()
         self.not_found_layout = NotFoundLayout  # Needs to be class here to add url
         for plugins in categorized_plugins.values():
             for plugin in plugins:
                 self.plugins[plugin.id] = plugin
 
     def register_callbacks(self) -> None:
+        """Register and handle the callbacks."""
         output = Output("content", "children")
         input = Input("on-page-load", "pathname")
 
         @app.callback(output, input)  # type: ignore
-        def display_page(pathname: str):  # type: ignore
+        def display_page(pathname: str) -> Any:
+            """
+            Display the page with the given path url, check for plugins.
+
+            Parameters
+            ----------
+            pathname : str
+                Pathname.
+
+            Returns
+            -------
+            Any
+                Either a General Layout, Not Found Layout or an Alert.
+            """
             pathname = urlparse(pathname).path
             paths = pathname.split("/")[1:]
 
             if paths[0] == "":
                 return self.general_layout()
             else:
                 if not queue.ready():
@@ -50,15 +97,15 @@
                     if paths[0] == "plugins":
                         plugin = self.plugins.get(paths[1], None)
                         if plugin is not None:
                             return plugin()
 
             return self.not_found_layout(pathname)()
 
-    def __call__(self) -> Component:
+    def __call__(self) -> Component:  # noqa: D102
         return html.Div(
             children=[
                 dcc.Interval(id="global-update", interval=config.REFRESH_RATE),
                 self.header_layout(),
                 html.Div(
                     id="main-container",
                     className="container-fluid",
```

### Comparing `deepcave-1.1.3/deepcave/layouts/notification.py` & `deepcave-1.2/deepcave/layouts/notification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,67 @@
+# noqa: D400
+"""
+# Notification
+
+This module provides a notification layout.
+
+It utilizes Dash and provides utilities for displaying notifications.
+With a notification from the Notification module an alert component can be updated.
+Callbacks are registered and handled.
+
+## Classes
+    - NotificationLayout: Layout class for displaying notifications.
+"""
+
 from typing import List, Tuple, Union
 
 import dash_bootstrap_components as dbc
 from dash.dependencies import Output
 from dash.development.base_component import Component
 from dash.exceptions import PreventUpdate
 from dash_extensions.enrich import Trigger
 
 from deepcave import app, notification
 from deepcave.layouts import Layout
 
 
 class NotificationLayout(Layout):
+    """
+    Layout class for displaying notifications.
+
+    Provide callback registering methods.
+    """
+
     def __init__(self) -> None:
         super().__init__()
 
     def register_callbacks(self) -> None:
+        """Register callbacks for updating notification alert."""
+
         @app.callback(
             Output("alert", "children"),
             Output("alert", "color"),
             Output("alert", "is_open"),
             Trigger("global-update", "n_intervals"),
-        )
+        )  # type: ignore
         def update_alert() -> Tuple[str, str, bool]:
+            """
+            Update the notification alert.
+
+            Returns
+            -------
+            Tuple[str, str, bool]
+                The message, color and True.
+            """
             if (result := notification.get_latest()) is not None:
                 (message, color) = result
                 return message, color, True
             else:
                 raise PreventUpdate()
 
-    def __call__(self) -> Union[List[Component], Component]:
+    def __call__(self) -> Union[List[Component], Component]:  # noqa: D102
         return dbc.Alert(
             id="alert",
             is_open=False,
             dismissable=True,
             fade=True,
         )
```

### Comparing `deepcave-1.1.3/deepcave/layouts/sidebar.py` & `deepcave-1.2/deepcave/layouts/sidebar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,92 @@
+#  noqa: D400
+"""
+# SidebarLayout
+
+This module defines layout for the sidebar.
+
+Callbacks are registered and handled.
+
+## Classes
+    - SidebarLayout: Customize the Sidebar Layout.
+"""
+
 from typing import Dict, List, Tuple, Union
 
 import dash_bootstrap_components as dbc
 from dash import ALL, html
 from dash.dependencies import Input, Output, State
 from dash.development.base_component import Component
 from dash_extensions.enrich import Trigger
 
 from deepcave import app, queue
 from deepcave.layouts import Layout
 from deepcave.plugins import Plugin
 
 
 class SidebarLayout(Layout):
+    """
+    Customize the Sidebar Layout.
+
+    Callbacks are registered and handled.
+
+    Properties
+    ----------
+    plugins : Dict[str, List[Plugin]]
+        A dictionary of all categorized plugins.
+    nav_points : Dict[str, List[Tuple[str, str, str]]]
+        A dictionary with plugins attributes corresponding to their category.
+    """
+
     def __init__(self, categorized_plugins: Dict[str, List[Plugin]]) -> None:
         super().__init__()
         self.plugins = categorized_plugins
 
         nav_points: Dict[str, List[Tuple[str, str, str]]] = {
             category: [] for category in categorized_plugins
         }
         for category, plugins in categorized_plugins.items():
             for plugin in plugins:
                 nav_points[category].append((plugin.id, plugin.name, plugin.icon))
 
         self.nav_points = nav_points
 
     def register_callbacks(self) -> None:
+        """Register the callbacks for the sidebar layout."""
         # Update navigation items
         output = Output("navigation-items", "children")
         input = Input("on-page-load", "pathname")
 
         @app.callback(output, input)  # type: ignore
-        def update_navigation_items(pathname):  # type: ignore
+        def update_navigation_items(pathname: str) -> List[Component]:
+            """
+            Update the navigation items.
+
+            Parameters
+            ----------
+            pathname : str
+                The pathname.
+
+            Returns
+            -------
+            List[Component]
+                The navigation items.
+            """
             layouts = []
             for category, points in self.nav_points.items():
                 layouts += [
                     html.H6(
                         className="sidebar-heading d-flex justify-content-between "
                         "align-items-center px-3 mt-4 mb-1 text-muted",
                         children=[html.Span(category)],
                     )
                 ]
 
                 point_layouts = []
-                for (id, name, icon) in points:
+                for id, name, icon in points:
                     href = f"/plugins/{id}"
                     point_layouts += [
                         html.Li(
                             className="nav-item",
                             children=[
                                 html.A(
                                     [html.I(className=icon), name],
@@ -56,16 +95,14 @@
                                 )
                             ],
                         )
                     ]
 
                 layouts += [html.Ul(className="nav flex-column", children=point_layouts)]
 
-            icon = {"data-feather": "file-text"}
-
             return html.Div(
                 className="position-sticky pt-3",
                 children=[
                     html.Ul(
                         className="nav flex-column",
                         children=[
                             html.A(
@@ -82,35 +119,36 @@
         # Callback to cancel jobs
         @app.callback(
             # Output('dropdown-container-output', 'children'),
             Input({"type": "cancel-job", "index": ALL}, "n_clicks"),
             State({"type": "cancel-job", "index": ALL}, "name"),
         )
         def delete_job(n_clicks, job_ids):  # type: ignore
+            """Delete the job from the queue."""
             for n_click, job_id in zip(n_clicks, job_ids):
                 if n_click is not None:
                     queue.delete_job(job_id)
 
         # Update queue information panel
         output = Output("queue-info", "children")
 
         @app.callback(output, Trigger("global-update", "n_intervals"))  # type: ignore
         def update_queue_info() -> List[Component]:
+            """Update the information of the queue."""
             try:
                 all_jobs = [
                     queue.get_finished_jobs(),
                     queue.get_running_jobs(),
                     queue.get_pending_jobs(),
                 ]
 
                 job_stati = ["[FINISHED]", "[RUNNING]", "[PENDING]"]
 
                 collect = []
                 for jobs, status in zip(all_jobs, job_stati):
-
                     for job in jobs:
                         name = job.meta["display_name"]
                         job_id = job.id
                         link = job.meta["link"]
 
                         collect += [(name, job_id, status, link)]
 
@@ -165,15 +203,15 @@
                         html.Ul(className="nav flex-column", children=items),
                     ]
 
                 return []
             except Exception:
                 return []
 
-    def __call__(self) -> Union[List[Component], Component]:
+    def __call__(self) -> Union[List[Component], Component]:  # noqa: D102
         return html.Nav(
             className="col-md-3 col-lg-2 d-md-block sidebar collapse",
             id="sidebarMenu",
             children=[
                 html.Div(id="navigation-items"),
                 html.Div(id="queue-info"),
             ],
```

### Comparing `deepcave-1.1.3/deepcave/plugins/__init__.py` & `deepcave-1.2/deepcave/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  noqa: D400
+"""
+# Plugins
+
+This module provides a base class for all the available plugins.
+It provides different utilities to handle the plugins and check for compatibility in the runs.
+
+## Classes
+    - Plugin: Base class for all plugins.
+"""
+
 from abc import ABC
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import copy
 import re
 import webbrowser
 from collections import defaultdict
@@ -27,32 +38,43 @@
 logger = get_logger(__name__)
 
 
 class Plugin(Layout, ABC):
     """
     Base class for all plugins.
 
-    Attributes
+    Provides different utilities to handle the plugins and check for compatibility in the runs.
+
+    Properties
     ----------
-    id : int
-        Unique identifier for the plugin.
-    name : str
-        Name of the plugin. It is shown in the navigation and in the title.
-    description : str, optional
-        Description of the plugin. Displayed below the title.
-    icon : str, optional
-        FontAwesome icon. Shown in the navigation.
-    help : str, optional
-        Path to the help file.
-    button_caption : str, optional
-        Caption of the button. Shown only, if `StaticPlugin` is used.
-    activate_run_selection : bool, optional
+    inputs : List[Tuple[str, str, bool, Any]]
+        The registered inputs.
+    outputs : List[Tuple[str, str, bool]]
+        The registered outputs.
+    previous_inputs : Dict[str, Dict[str, str]]
+        The previous inputs.
+    raw_outputs : Optional[Dict[str, Any]]
+        The raw outputs.
+    activate_run_selection : bool
         Shows a dropdown to select a run in the inputs layout.
         This feature is useful if only one run could be viewed at a time.
         Moreover, it prevents the plugin to calculate results across all runs.
+    id : str
+        The unique identifier for the plugin.
+    runs : List[AbstractRun]
+        A list of the abstract runs.
+    groups : List[Group]
+        A list of the groups.
+    help : str
+        The path to the documentation.
+    name : str
+        The name of the plugin.
+        It is shown in the navigation and title.
+    button_caption : str
+        Caption of the button. Shown only, if `StaticPlugin` is used.
     """
 
     id: str
     name: str
     description: Optional[str] = None
     icon: str = "far fa-file"
     help: Optional[str] = None
@@ -64,15 +86,15 @@
         self.inputs: List[Tuple[str, str, bool, Any]] = []
         self.outputs: List[Tuple[str, str, bool]] = []
 
         # For runtime
         self.previous_inputs: Dict[str, Dict[str, str]] = {}
         self.raw_outputs: Optional[Dict[str, Any]] = None
 
-        # We have to call the output layout one time to register
+        # The output layout has to be called one time to register
         # the values
         # Problem: Inputs/Outputs can't be changed afterwards anymore.
 
         if self.activate_run_selection:
             self.__class__.get_run_input_layout(self.register_input)
 
         self.__class__.get_input_layout(self.register_input)
@@ -82,30 +104,31 @@
 
         super().__init__()
 
     @classmethod
     @interactive
     def get_base_url(cls) -> str:
         """
-        Generates the url for the plugin.
+        Generate the url for the plugin.
 
         Returns
         -------
         str
             Url for the plugin as string.
         """
         from deepcave import config
 
         return f"http://{config.DASH_ADDRESS}:{config.DASH_PORT}/plugins/{cls.id}"
 
     @staticmethod
     def check_run_compatibility(run: AbstractRun) -> bool:
         """
-        Checks if a run is compatible with this plugin. If a plugin is not compatible,
-        you can not select the run.
+        Check if a run is compatible with this plugin.
+
+        If a plugin is not compatible, you can not select the run.
 
         Note
         ----
         This function is only called if `activate_run_selection` is True.
 
         Parameters
         ----------
@@ -117,15 +140,16 @@
         bool
             Returns True if the run is compatible.
         """
         return True
 
     def check_runs_compatibility(self, runs: List[AbstractRun]) -> None:
         """
-        This function is needed if all selected runs need something in common
+        Needed if all selected runs need something in common.
+
         (e.g. budget or objective). Since this function is called before the layout is created,
         it can be also used to set common values for the plugin.
 
         Parameters
         ----------
         runs : List[AbstractRun]
             Selected runs.
@@ -141,24 +165,26 @@
         self,
         id: str,
         attributes: Union[str, List[str]] = "value",
         filter: bool = False,
         type: Any = None,
     ) -> str:
         """
-        Registers an input variable for the plugin. It is important to register the inputs
-        because callbacks have to be defined before the server is started.
+        Register an input variable for the plugin.
+
+        It is important to register the inputs.
+        This is, because callbacks have to be defined before the server is started.
         After registering all inputs, an internal mapping is created.
 
         Parameters
         ----------
         id : str
             Specifies the id of the input.
         attributes : Union[str, List[str]], optional
-            Attributes which should be passed to the (dash) component, by default ("value",)
+            Attributes which should be passed to the (dash) component, by default ("value",).
         filter : bool, optional
             Specifies if the input is a filter. By default False.
         type : Any, optional
             Type to which the *first* attribute should be casted to. By default str.
 
         Returns
         -------
@@ -174,26 +200,26 @@
             if i == 0:
                 type_ = type
 
             key = (id, attribute, filter, type_)
             if key not in self.inputs:
                 self.inputs.append(key)
 
-        # We have to rearrange the inputs because `State`
-        # must follow all `Input`. Since all filters are `Input`, we have to
-        # shift them to the front.
+        # The inputs have to be rearranged, because `State`
+        # must follow all `Input`. Since all filters are `Input`, they have to
+        # be shifted to the front.
         self.inputs.sort(key=lambda x: x[2], reverse=True)
 
         return self.get_internal_input_id(id)
 
     def register_output(
         self, id: str, attributes: Union[str, List[str]] = "value", mpl: bool = False
     ) -> str:
         """
-        Registers an output variable for the plugin.
+        Register an output variable for the plugin.
 
         Parameters
         ----------
         id : str
             Specifies the id of the output.
         attributes : Union[str, List[str]], optional
             Attribute, by default "value"
@@ -215,35 +241,40 @@
             key = (id, attribute, mpl)
             if key not in self.outputs:
                 self.outputs.append(key)
 
         return self.get_internal_output_id(id)
 
     def get_internal_id(self, id: str) -> str:
+        """Get the internal id."""
         return f"{self.id}-{id}"
 
     def get_internal_input_id(self, id: str) -> str:
+        """Get the internal input id."""
         return f"{self.id}-{id}-input"
 
     def get_internal_output_id(self, id: str) -> str:
+        """Get the internal output id."""
         return f"{self.id}-{id}-output"
 
     @interactive
     def register_callbacks(self) -> None:
         """
-        Registers basic callbacks for the plugin. Following callbacks are registered:
+        Register basic callbacks for the plugin.
+
+        Following callbacks are registered:
         - If inputs changes, the changes are pasted back. This is in particular
         interest if input dependencies are used.
         - Raw data dialog to display raw data.
         - Callback to be redirected to the config if clicked on it.
 
         Raises
         ------
         RuntimeError
-            _description_
+            If no run id is found.
         """
         from deepcave import app, c, run_handler
 
         # Handles the initial and the cashed input values
         outputs = []
         inputs = [Input("on-page-load", "href")]
 
@@ -253,15 +284,16 @@
 
         for id, attribute, _, _ in self.inputs:
             outputs.append(Output(self.get_internal_input_id(id), attribute))
 
         if len(outputs) > 0:
 
             @app.callback(outputs, inputs)  # type: ignore
-            def plugin_input_update(pathname: str, *inputs_list: str) -> List[str]:
+            def plugin_input_update(pathname: str, *inputs_list: str) -> List[Optional[str]]:
+                """Update the input of the plugin."""
                 # Simple check if page was loaded for the first time
                 init = all(input is None for input in inputs_list)
 
                 # Reload our inputs
                 if init:
                     inputs = c.get("last_inputs", self.id)
                     passed_inputs = parse_url(pathname)
@@ -269,18 +301,18 @@
                     if passed_inputs is not None:
                         # First get normal inputs
                         inputs = self.load_inputs()
 
                         # Overwrite/set the passed inputs
                         update_dict(inputs, passed_inputs)
 
-                        # Then we have to take care of the run_selection
+                        # Then the run_selection has to be taken care of
                         selected_run: Optional[AbstractRun] = None
                         if self.activate_run_selection:
-                            # If run_selection is active and we don't have an id, then
+                            # If run_selection is active and the id is not known, then
                             # the passed inputs have no use.
                             try:
                                 run_id = passed_inputs["run"]["value"]
                             except Exception:
                                 raise RuntimeError("No run id found.")
                             selected_run = run_handler.get_run(run_id)
 
@@ -310,96 +342,106 @@
                                 self.runs,
                                 self.groups,
                                 self.__class__.check_run_compatibility,
                             )
                             update_dict(inputs, new_inputs)
 
                         # Set not used inputs
-                        for (id, attribute, _, _) in self.inputs:
+                        for id, attribute, _, _ in self.inputs:
                             if id not in inputs:
                                 inputs[id] = {}
 
                             if attribute not in inputs[id]:
                                 inputs[id][attribute] = None
                     elif inputs is not None:
-                        # We have to update the options of the run selection here.
+                        # The options of the run selection have to be updated here.
                         # This is important if the user have added/removed runs.
                         if self.activate_run_selection:
                             run_value = inputs["run"]["value"]
                             new_inputs = self.__class__.load_run_inputs(
                                 self.runs,
                                 self.groups,
                                 self.__class__.check_run_compatibility,
                             )
                             update_dict(inputs, new_inputs)
 
                             # Keep the run value
                             inputs["run"]["value"] = run_value
                 else:
                     # Map the list `inputs` to a dict.
-                    inputs = self._list_to_dict(inputs_list)  # type: ignore
+                    # inputs_list_as_list is necessary as new variable,
+                    # because inputs_list is a tuple and cant be passed to _list_to_dict.
+                    inputs_list_as_list = list(inputs_list)
+                    inputs = self._list_to_dict(inputs_list_as_list)
 
                     if len(self.previous_inputs) == 0:
                         self.previous_inputs = inputs.copy()
 
                     # Only work on copies.
-                    # We don't want the inputs dict to be changed by the user.
+                    # The inputs dict should not be changed by the user.
                     _previous_inputs = self.previous_inputs.copy()
                     _inputs = inputs.copy()
 
                     selected_run = None
                     if self.activate_run_selection:
                         if "run" in _previous_inputs:
                             _previous_run_id = _previous_inputs["run"]["value"]
                         else:
                             _previous_run_id = None
                         _run_id = inputs["run"]["value"]
 
                         # Reset everything if run name changed.
                         if _previous_run_id is not None and _previous_run_id != _run_id:
-                            # We can't use load_inputs here only
+                            # load_inputs cannot be used here, only
                             # because `run` would be removed.
-                            # Also: We want to keep the current run name.
+                            # Also: The current run name does not need to be kept.
                             update_dict(_inputs, self.load_inputs())
+                            # Reset inputs
+                            if "objective_id" in _inputs.keys():
+                                update_dict(_inputs, {"objective_id": {"value": None}})
+                            if "budget_id" in _inputs.keys():
+                                update_dict(_inputs, {"budget_id": {"value": None}})
+                            if "hyperparameter_name_1" in _inputs.keys():
+                                update_dict(_inputs, {"hyperparameter_name_1": {"value": None}})
+                            if "hyperparameter_name_2" in _inputs.keys():
+                                update_dict(_inputs, {"hyperparameter_name_2": {"value": None}})
 
-                            # TODO: Reset only inputs which are not available in another run.
-                            # E.g. if options from budget in run_2 and run_3 are the same
-                            # take the budget from run_2 if changed to run_3. Otherwise,
-                            # reset budgets.
-
-                        selected_run = run_handler.get_run(_run_id)
-
-                    # How to update only parameters which have a dependency?
-                    user_dependencies_inputs = self.load_dependency_inputs(
-                        selected_run, _previous_inputs, _inputs
-                    )
+                        if _run_id:
+                            selected_run = run_handler.get_run(_run_id)
 
-                    # Update dict
-                    # dict.update() remove keys, so we use our own method to do so
-                    update_dict(inputs, user_dependencies_inputs)  # inplace operation
+                    if selected_run is not None:
+                        # How to update only parameters which have a dependency?
+                        user_dependencies_inputs = self.load_dependency_inputs(
+                            selected_run, _previous_inputs, _inputs
+                        )
+
+                        # Update dict
+                        # dict.update() removes keys, so our own method is used to do so
+                        update_dict(inputs, user_dependencies_inputs)  # inplace operation
 
                 # Let's cast the inputs
                 inputs = self._cast_inputs(inputs)
 
                 # From dict to list
-                inputs_list = self._dict_to_list(inputs, input=True)  # type: ignore
+                inputs_list_from_dict = self._dict_to_list(inputs, input=True)
                 self.previous_inputs = inputs
 
-                return list(inputs_list)
+                return inputs_list_from_dict
 
         # Register modal for raw data here
         @app.callback(  # type: ignore
             [
                 Output(self.get_internal_id("raw_data"), "is_open"),
                 Output(self.get_internal_id("raw_data_content"), "value"),
             ],
             Input(self.get_internal_id("show_raw_data"), "n_clicks"),
             State(self.get_internal_id("raw_data"), "is_open"),
         )
         def toggle_raw_data_modal(n: Optional[int], is_open: bool) -> Tuple[bool, str]:
+            """Toggle the raw data modal."""
             code = ""
             if n:
                 if (out := self.raw_outputs) is not None:
                     # Make list
                     code = str(out)
 
                 return not is_open, code
@@ -410,29 +452,30 @@
         @app.callback(  # type: ignore
             [
                 Output(self.get_internal_id("help"), "is_open"),
             ],
             Input(self.get_internal_id("show_help"), "n_clicks"),
             State(self.get_internal_id("help"), "is_open"),
         )
-        def toggle_help_modal(n: Optional[int], is_open: bool) -> Tuple[bool, str]:
+        def toggle_help_modal(n: Optional[int], is_open: bool) -> bool:
+            """Toggle the help modal."""
             if n:
                 return not is_open
-
             return is_open
 
         # Register callback to click on configurations
-        for (id, *_) in self.outputs:
+        for id, *_ in self.outputs:
             internal_id = self.get_internal_output_id(id)
 
             @app.callback(
                 Output(internal_id, "clickData"),
                 Input(internal_id, "clickData"),
-            )
-            def go_to_configuration(click_data):  # type: ignore
+            )  # type: ignore
+            def go_to_configuration(click_data: Any):
+                """Open link from hovertext."""
                 if click_data is not None:
                     # Get hovertext
                     try:
                         hovertext = click_data["points"][0]["hovertext"]
 
                         # Now extract the link from href
                         match = re.search("<a href='(.+?)'", hovertext)
@@ -445,15 +488,15 @@
                 return None
 
     @interactive
     def _inputs_changed(
         self, inputs: Dict[str, Dict[str, str]], last_inputs: Dict[str, Dict[str, str]]
     ) -> Tuple[bool, bool]:
         """
-        Checks if the inputs have changed.
+        Check if the inputs have changed.
 
         Parameters
         ----------
         inputs : Dict[str, Dict[str, str]]
             Current inputs.
         last_inputs : Dict[str, Dict[str, str]]
             Last inputs.
@@ -463,19 +506,18 @@
         Tuple[bool, bool]
             Whether input and filter inputs have changed.
         """
         # Check if last_inputs are the same as the given inputs.
         inputs_changed = False
         filters_changed = False
 
-        # If only filters changed, then we don't need to
+        # If only filters changed, there is no need to
         # calculate the results again.
         if last_inputs is not None:
-            for (id, attribute, filter, _) in self.inputs:
-
+            for id, attribute, filter, _ in self.inputs:
                 if self.activate_run_selection:
                     if id == "run":
                         continue
 
                 if inputs[id][attribute] != last_inputs[id][attribute]:
                     if not filter:
                         inputs_changed = True
@@ -483,52 +525,70 @@
                         filters_changed = True
 
         return inputs_changed, filters_changed
 
     @interactive
     def _process_raw_outputs(
         self, inputs: Dict[str, Dict[str, str]], raw_outputs: Dict[str, Any]
-    ) -> Union[Any, List[Any]]:
+    ) -> Any:
+        """
+        Process the raw outputs and update the layout.
+
+        Parameters
+        ----------
+        inputs : Dict[str, Dict[str, str]]
+            The inputs for the passed runs.
+        raw_outputs : Dict[str, Any]
+            The raw outputs to process.
+
+        Returns
+        -------
+        Any
+            The processed outputs.
+        """
         from deepcave import c, run_handler
 
         # Use raw outputs to update our layout
         mpl_active = c.get("matplotlib-mode")
+        passed_runs: Union[List[AbstractRun], AbstractRun]
 
         if self.activate_run_selection:
             passed_runs = run_handler.get_run(inputs["run"]["value"])
             passed_outputs = raw_outputs[passed_runs.id]
         else:
-            passed_runs = self.all_runs  # type: ignore
+            passed_runs = self.all_runs
             passed_outputs = raw_outputs
 
         # Clean inputs
         cleaned_inputs = self._clean_inputs(inputs)
 
+        # passed runs could be a list, but load mpl outputs and load outputs do not
+        # accept lists, but expect single runs
         if mpl_active:
-            outputs = self.__class__.load_mpl_outputs(passed_runs, cleaned_inputs, passed_outputs)
+            outputs = self.__class__.load_mpl_outputs(passed_runs, cleaned_inputs, passed_outputs)  # type: ignore # noqa: E501
         else:
-            outputs = self.__class__.load_outputs(passed_runs, cleaned_inputs, passed_outputs)
+            outputs = self.__class__.load_outputs(passed_runs, cleaned_inputs, passed_outputs)  # type: ignore # noqa: E501
 
         logger.debug("Raw outputs processed successfully.")
 
         if outputs == PreventUpdate:
             raise PreventUpdate()
 
         # Map outputs here because it may be that the outputs are
         # differently sorted than the values were registered.
         if isinstance(outputs, dict):
             outputs = self._dict_to_list(outputs, input=False)
         else:
             if not isinstance(outputs, list):
                 outputs = [outputs]
 
-        # We have to add no_updates here for the mode we don't want
+        # no_updates has to be added here for the mode that is not wanted
         count_outputs = 0
         count_mpl_outputs = 0
-        for (_, _, mpl_mode) in self.outputs:
+        for _, _, mpl_mode in self.outputs:
             if mpl_mode:
                 count_mpl_outputs += 1
             else:
                 count_outputs += 1
 
         if mpl_active:
             outputs = [no_update for _ in range(count_outputs)] + outputs
@@ -539,33 +599,37 @@
             return outputs[0]
 
         return outputs
 
     @interactive
     def _list_to_dict(self, values: List[str], input: bool = True) -> Dict[str, Dict[str, str]]:
         """
-        Maps the given values to a dict, regarding the sorting from
-        either self.inputs or self.outputs.
+        Map the given values to a dict.
+
+        Regarding the sorting from either self.inputs or self.outputs.
 
         Parameters
         ----------
         values : Iterable[str]
             Values to map.
         input : bool, optional
             Whether the data should be linked to the input or outputs. By default True.
 
         Returns
         -------
         Dict[str, Dict[str, str]]
-            _description_
+            Dictionary containing the mapping information.
         """
+        # This is necessary, because of the conditional type of order
+        order: Union[List[Tuple[str, str, bool]], List[Tuple[str, str, bool, Any]]]
+
         if input:
             order = self.inputs
         else:
-            order = self.outputs  # type: ignore
+            order = self.outputs
 
         mapping: Dict[str, Any] = {}
         for value, (id, attribute, *_) in zip(values, order):
             if id not in mapping:
                 mapping[id] = {}
 
             mapping[id][attribute] = value
@@ -573,16 +637,17 @@
         return mapping
 
     @interactive
     def _dict_to_list(
         self, d: Dict[str, Dict[str, str]], input: bool = False
     ) -> List[Optional[str]]:
         """
-        Maps the given dict to a list, respecting the sorting from either
-        self.inputs or self.outputs.
+        Map the given dict to a list.
+
+        Respecting the sorting from either self.inputs or self.outputs.
 
         Parameters
         ----------
         d : Dict[str, Dict[str, str]]
             Dictionary to transform.
         input : bool, optional
             Whether the data should be linked to the input or outputs. By default False.
@@ -590,21 +655,24 @@
         Returns
         -------
         List[Optional[str]]
             Sorted list from the given dict.
         """
         from deepcave import c
 
+        # This is necessary, because of the conditional type of order
+        order: Union[List[Tuple[str, str, bool]], List[Tuple[str, str, bool, Any]]]
+
         if input:
             order = self.inputs
         else:
-            order = self.outputs  # type: ignore
+            order = self.outputs
 
         result: List[Optional[str]] = []
-        for (id, attribute, instance, *_) in order:
+        for id, attribute, instance, *_ in order:
             if not input:
                 # Instance is mlp_mode in case of outputs
                 # Simply ignore other outputs.
                 if instance != c.get("matplotlib-mode"):
                     continue
 
             try:
@@ -612,148 +680,195 @@
                 result += [value]
             except Exception:
                 result += [None]
 
         return result
 
     @interactive
-    def _dict_as_key(self, d: Dict[str, Any], remove_filters: bool = False) -> Optional[str]:
+    def _dict_as_key(self, d: Dict[str, Any], remove_filters: bool = False) -> str:
         """
-        Converts a dictionary to a key. Only ids from self.inputs are considered.
+        Convert a dictionary to a key. Only ids from self.inputs are considered.
 
         Parameters
         ----------
         d : Dict[str, Any]
             Dictionary to get the key from.
         remove_filters : bool, optional
-            Option wheather the filters should be included or not. By default False.
+            Option whether the filters should be included or not. By default False.
 
         Returns
         -------
         Optional[str]
             Key as string from the given dictionary. Returns none if `d` is not a dictionary.
+
+        Raises
+        ------
+        TypeError
+            If `d` is not a dictionary.
         """
         if not isinstance(d, dict):
-            return None
+            raise TypeError("d must be a dictionary.")
 
         new_d = copy.deepcopy(d)
         if remove_filters:
-            for (id, _, filter, _) in self.inputs:
+            for id, _, filter, _ in self.inputs:
                 if filter:
                     if id in new_d:
                         del new_d[id]
 
         return string_to_hash(str(new_d))
 
     def _cast_inputs(self, inputs: Dict[str, Dict[str, str]]) -> Dict[str, Dict[str, str]]:
         """
-        Casts the inputs based on `self.inputs`. Background is that dash always casts integers/
-        booleans to strings. This method ensured that the correct types are returned.
+        Cast the inputs based on `self.inputs`.
+
+        Background is that dash always casts integers/booleans to strings.
+        This method ensures that the correct types are returned.
 
         Parameters
         ----------
         inputs : Dict[str, Dict[str, str]]
             Inputs, which should be casted.
 
         Returns
         -------
         Dict[str, Dict[str, str]]
             Casted inputs.
         """
         casted_inputs: Dict[str, Dict[str, str]] = defaultdict(dict)
         for id, attributes in inputs.items():
             for attribute in attributes:
-
                 # Find corresponding input
                 type = None
-                for (id_, attribute_, _, type_) in self.inputs:
+                for id_, attribute_, _, type_ in self.inputs:
                     if id == id_ and attribute == attribute_:
                         type = type_
                         break
 
                 value = inputs[id][attribute]
                 if not (type is None or value is None):
                     value = type(value)
 
                 casted_inputs[id][attribute] = value
 
         return casted_inputs
 
     def _clean_inputs(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """
-        Cleans the given inputs s.t. only the first value is used.
-        Also, boolean values are casted to booleans.
+        Clean the given inputs s.t. only the first value is used.
+
+        Also, boolean values are cast to booleans.
 
         Example
         -------
         You register the following input:
         ```
         dbc.Select(id=register("objective_name", ["value", "options"]))
         ```
         However, in the `process` or `load_outputs` method you don't need `options`.
         Instead of writing `inputs["objective_name"]["value"]` you can simply write
         `inputs["objective_name"]`.
 
         Parameters
         ----------
-        inputs (dict): Inputs to clean.
+        inputs : Dict[str, Any]
+            Inputs to clean.
 
-        Returns:
-            dict: Cleaned inputs.
+        Returns
+        -------
+        Dict[str, Any]
+            Cleaned inputs.
         """
         used_ids = []
         cleaned_inputs = {}
-        for (id, attribute, *_) in self.inputs:
-            # Since self.inputs is ordered, we use the first occuring attribute and add
-            # the id so it is not used again.
+        for id, attribute, *_ in self.inputs:
+            # Since self.inputs is ordered, the first occurring attribute is used and
+            # the id is added so it is not used again.
             if id not in used_ids:
                 i = inputs[id][attribute]
 
                 if i == "true":
                     i = True
 
                 if i == "false":
                     i = False
 
                 cleaned_inputs[id] = i
                 used_ids += [id]
 
         return cleaned_inputs
 
-    @property  # type: ignore
+    @property
     @interactive
     def runs(self) -> List[AbstractRun]:
+        """
+        Get the runs as a list.
+
+        Returns
+        -------
+        List[AbstractRun]
+            The list with the runs.
+        """
         from deepcave import run_handler
 
         return run_handler.get_runs()
 
-    @property  # type: ignore
+    @property
     @interactive
     def groups(self) -> List[Group]:
+        """
+        Get the groups as a list.
+
+        Returns
+        -------
+        List[Group]
+            The list with the groups.
+        """
         from deepcave import run_handler
 
         return run_handler.get_groups()
 
-    @property  # type: ignore
+    @property
     @interactive
     def all_runs(self) -> List[AbstractRun]:
+        """
+        Get all runs and include the groups as a list.
+
+        Returns
+        -------
+        List[AbstractRun]
+            The list with all runs and included groups.
+        """
         from deepcave import run_handler
 
         return run_handler.get_runs(include_groups=True)
 
     @interactive
     def __call__(self, render_button: bool = False) -> List[Component]:
         """
-        Returns the components for the plugin. Basically, all blocks and elements of the plugin
-        are stacked-up here
+        Return the components for the plugin.
+
+        Basically, all blocks and elements of the plugin are stacked-up here.
+
+        Parameters
+        ----------
+        render_button : bool, optional
+            Whether to render the button or not. By default False.
 
         Returns
         -------
         List[Component]
             Layout as list of components.
+
+        Raises
+        ------
+        NotMergeableError
+            If runs are not compatible.
+        FileNotFoundError
+            If the help file can not be found.
         """
         from deepcave import c, notification
 
         # Reset runtime variables
         self.previous_inputs = {}
         self.raw_outputs = None
 
@@ -798,15 +913,14 @@
                         ),
                     ]
                 ),
                 modal,
             ]
         else:
             components += [html.H1(self.name)]
-
         try:
             self.check_runs_compatibility(self.all_runs)
         except NotMergeableError as message:
             notification.update(str(message))
             return components
 
         if self.activate_run_selection:
@@ -827,15 +941,15 @@
                 dbc.Button(
                     children=self.button_caption,
                     id=self.get_internal_id("update-button"),
                 ),
             ],
         )
 
-        # We always have to render it because of the button.
+        # It always has to be rendered, because of the button.
         # Button tells us if the page was just loaded.
         components += [
             html.Div(
                 id=f"{self.id}-input",
                 className="shadow-sm p-3 mb-3 bg-white rounded-lg",
                 children=run_input_layout
                 + separator_layout
@@ -843,15 +957,35 @@
                 + [input_control_layout],
                 style={}
                 if render_button or input_layout or run_input_layout
                 else {"display": "none"},
             )
         ]
 
-        def register_in(a, b):  # type: ignore
+        def register_in(a: str, b: Union[List[str], str]) -> str:
+            """
+            Register the given input.
+
+            Note
+            ----
+            For more information, see 'register_input'.
+
+            Parameters
+            ----------
+            a : str
+                Specifies the id of the input.
+            b : Union[List[str], str]
+                Attributes which should be passed to the (dash) component, by default ("value",).
+
+            Returns
+            -------
+            str
+                Unique id for the input and plugin.
+                This is necessary because ids are defined globally.
+            """
             return self.register_input(a, b, filter=True)
 
         filter_layout = self.__class__.get_filter_layout(register_in)
         if len(filter_layout) > 0:
             components += [
                 html.Div(
                     id=f"{self.id}-filter",
@@ -867,15 +1001,35 @@
                     id=f"{self.id}-output",
                     className="shadow-sm p-3 bg-white rounded-lg loading-container",
                     children=output_layout,
                     style={} if not c.get("matplotlib-mode") else {"display": "none"},
                 )
             ]
 
-        def register_out(a, b):  # type: ignore
+        def register_out(a: str, b: Union[List[str], str]) -> str:
+            """
+            Register the output.
+
+            Note
+            ----
+            For more information, see 'register_output'
+
+            Parameters
+            ----------
+            a : str
+                Specifies the id of the output.
+            b : Union[List[str], str]
+                Attribute.
+
+            Returns
+            -------
+            str
+                Unique id for the output and plugin.
+                This is necessary because ids are defined globally.
+            """
             return self.register_output(a, b, mpl=True)
 
         output_layout = self.__class__.get_mpl_output_layout(register_out)
         if output_layout is not None:
             components += [
                 html.Div(
                     id=f"{self.id}-mpl-output",
@@ -928,23 +1082,25 @@
 
         components += [modal]
 
         return components
 
     @staticmethod
     @interactive
-    def get_run_input_layout(register: Callable[[str, Union[str, List[str]]], str]) -> Component:
+    def get_run_input_layout(register: Callable) -> Component:
         """
-        Generates the run selection input.
+        Generate the run selection input.
+
         This is only the case if `activate_run_selection` is True.
 
         Parameters
         ----------
-        register : Callable[[str, Union[str, List[str]]], str]
+        register : Callable
             The register method to register (user) variables.
+            For more information, see 'register_input'.
 
         Returns
         -------
         Component
             The layout of the run selection input.
         """
         return html.Div(
@@ -960,32 +1116,32 @@
     @interactive
     def load_run_inputs(
         runs: List[AbstractRun],
         groups: List[Group],
         check_run_compatibility: Callable[[AbstractRun], bool],
     ) -> Dict[str, Any]:
         """
-        Loads the options for `get_run_input_layout`.
+        Load the options for `get_run_input_layout`.
+
         Both runs and groups are displayed.
 
         Parameters
         ----------
-        runs : Dict[str, Run]
+        runs : List[AbstractRun]
             The runs to display.
-        groups : Dict[str, Group]
+        groups : List[Group]
             The groups to display.
         check_run_compatibility : Callable[[AbstractRun], bool]
             If a single run is compatible. If not, the run is not shown.
 
         Returns
         -------
         Dict[str, Any]
             Both runs and groups, separated by a separator.
         """
-
         labels = []
         values = []
         disabled = []
 
         for run in runs:
             if check_run_compatibility(run):
                 try:
@@ -1014,15 +1170,16 @@
                 "value": None,
             }
         }
 
     @interactive
     def get_selected_runs(self, inputs: Dict[str, Any]) -> List[AbstractRun]:
         """
-        Parses selected runs from inputs.
+        Parse selected runs from inputs.
+
         If self.activate_run_selection is set, return only selected run. Otherwise, return all
         possible runs.
 
         Parameters
         ----------
         inputs : Dict[str, Any]
             The inputs to parse.
@@ -1046,25 +1203,26 @@
                 raise PreventUpdate()
 
             # Update runs
             run = run_handler.get_run(run_id)
 
             # Also:
             # Remove `run` from inputs_key because
-            # we don't want the run names included.
+            # The runs name does not need to be included
             _inputs = inputs.copy()
             del _inputs["run"]
 
             return [run]
         else:
             return self.all_runs
 
     def load_inputs(self) -> Dict[str, Any]:
         """
         Load the content for the defined inputs in `get_input_layout` and `get_filter_layout`.
+
         This method is necessary to pre-load contents for the inputs. So, if the plugin is
         called for the first time or there are no results in the cache, the plugin gets its
         content from this method.
 
         Returns
         -------
         Dict[str, Any]
@@ -1075,24 +1233,26 @@
     def load_dependency_inputs(
         self,
         run: Optional[Union[AbstractRun, List[AbstractRun]]],
         previous_inputs: Dict[str, Any],
         inputs: Dict[str, Any],
     ) -> Dict[str, Any]:
         """
-        Same as `load_inputs` but called after inputs have changed. Provides a lot of flexibility.
+        Load the content as in 'load_inputs' but called after inputs have changed.
+
+        Provides a lot of flexibility.
 
         Note
         ----
         Only the changes have to be returned. The returned dictionary will be merged with the
         inputs.
 
         Parameters
         ----------
-        selected_run : Optional[Union[AbstractRun, List[AbstractRun]]], optional
+        run : Optional[Union[AbstractRun, List[AbstractRun]]], optional
             The selected run from the user. In case of `activate_run_selection`, only one run
             is passed. Defaults to None.
         previous_inputs : Dict[str, Any]
             Previous content of the inputs.
         inputs : Dict[str, Any]
             Current content of the inputs.
 
@@ -1100,98 +1260,100 @@
         -------
         Dict[str, Any]
             Dictionary with the changes.
         """
         return inputs
 
     @staticmethod
-    def get_input_layout(register: Callable[[str, Union[str, List[str]]], str]) -> List[Component]:
+    def get_input_layout(register: Callable) -> List[Component]:
         """
         Layout for the input block.
 
         Parameters
         ----------
-        register : Callable[[str, Union[str, List[str]]], str]
+        register : Callable
             The register method to register (user) variables.
+            For more information, see 'register_input'.
 
         Returns
         -------
         List[Component]
             Layouts for the input block.
         """
         return []
 
     @staticmethod
-    def get_filter_layout(register: Callable[[str, Union[str, List[str]]], str]) -> List[Component]:
+    def get_filter_layout(register: Callable) -> List[Component]:
         """
         Layout for the filter block.
 
         Parameters
         ----------
-        register : Callable[[str, Union[str, List[str]]], str]
+        register : Callable
             The register method to register (user) variables.
+            For more information, see 'register_input'.
 
         Returns
         -------
         List[Component]
             Layouts for the filter block.
         """
         return []
 
     @staticmethod
-    def get_output_layout(
-        register: Callable[[str, Union[str, List[str]]], str]
-    ) -> Optional[Union[Component, List[Component]]]:
+    def get_output_layout(register: Callable) -> Optional[Union[Component, List[Component]]]:
         """
         Layout for the output block.
 
         Parameters
         ----------
-        register : Callable[[str, Union[str, List[str]]], str]
+        register : Callable
             The register method to register outputs.
+            For more information, see 'register_input'.
 
         Returns
         -------
         Union[Component, List[Component]]
             Layouts for the output block.
         """
         return None
 
     @staticmethod
-    def get_mpl_output_layout(
-        register: Callable[[str, Union[str, List[str]]], str]
-    ) -> Optional[Union[Component, List[Component]]]:
+    def get_mpl_output_layout(register: Callable) -> Optional[Union[Component, List[Component]]]:
         """
         Layout for the matplotlib output block.
 
         Parameters
         ----------
-        register : Callable[[str, Union[str, List[str]]], str]
+        register : Callable
             The register method to register outputs.
+            For more information, see 'register_input'.
 
         Returns
         -------
-        Union[Component, List[Component]]
+        Optional[Union[Component, List[Component]]]
             Layout for the matplotlib output block.
         """
         return None
 
     @staticmethod
     def load_outputs(
         runs: Union[AbstractRun, Dict[str, AbstractRun]],
         inputs: Dict[str, Dict[str, str]],
         outputs: Dict[str, Union[str, Dict[str, str]]],
     ) -> Union[Component, List[Component]]:
         """
-        Reads in the raw data and prepares them for the layout.
+        Read in the raw data and prepare them for the layout.
 
         Note
         ----
         The passed `inputs` are cleaned and therefore differs compared to `load_inputs` or
-        `load_dependency_inputs`. Please see `_clean_inputs` for more information.
+        `load_dependency_inputs`.
+        Inputs are cleaned s.t. only the first value is used.
+        Also, boolean values are casted to booleans.
 
         Parameters
         ----------
         runs : Union[AbstractRun, Dict[str, AbstractRun]]
             All selected runs. If `activate_run_selection` is set, only the selected run is
             returned.
         inputs : Dict[str, Dict[str, str]]
@@ -1210,20 +1372,21 @@
     @staticmethod
     def load_mpl_outputs(
         runs: Union[AbstractRun, Dict[str, AbstractRun]],
         inputs: Dict[str, Dict[str, str]],
         outputs: Dict[str, Union[str, Dict[str, str]]],
     ) -> Union[Component, List[Component]]:
         """
-        Reads in the raw data and prepares them for the layout.
+        Read in the raw data and prepare them for the layout.
 
         Note
         ----
         The passed `inputs` are cleaned and therefore differs compared to `load_inputs` or
-        `load_dependency_inputs`. Please see `_clean_inputs` for more information.
+        `load_dependency_inputs`. Inputs are cleaned s.t. only the first value is used.
+        Also, boolean values are casted to booleans.
 
         Parameters
         ----------
         runs : Union[AbstractRun, Dict[str, AbstractRun]]
             All selected runs. If `activate_run_selection` is set, only the selected run is
             returned.
         inputs : Dict[str, Dict[str, str]]
@@ -1238,24 +1401,25 @@
             The components must be in the same position as defined in `get_output_layout`.
         """
         return []
 
     @staticmethod
     def process(run: AbstractRun, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """
-        Returns raw data based on a run and input data.
+        Return raw data based on a run and input data.
 
         Warning
         -------
         The returned data must be JSON serializable.
 
         Note
         ----
         The passed `inputs` are cleaned and therefore differs compared to `load_inputs` or
-        `load_dependency_inputs`. Please see `_clean_inputs` for more information.
+        `load_dependency_inputs`. Inputs are cleaned s.t. only the first value is used.
+        Also, boolean values are casted to booleans.
 
         Parameters
         ----------
         run : AbstractRun
             The run to process.
         inputs : Dict[str, Any]
             Input data.
@@ -1268,15 +1432,16 @@
         return {}
 
     @classmethod
     def generate_outputs(
         cls, runs: Union[AbstractRun, List[AbstractRun]], inputs: Dict[str, Any]
     ) -> Union[Dict[str, Any], Dict[str, Dict[str, Any]]]:
         """
-        Checks whether run selection is active and accepts either one or multiple runs at once.
+        Check whether run selection is active and accepts either one or multiple runs at once.
+
         Calls `process` internally.
 
         Parameters
         ----------
         runs : Union[AbstractRun, List[AbstractRun]]
             Run or runs to process.
         inputs : Dict[str, Any]
@@ -1310,15 +1475,16 @@
             for run in runs:
                 outputs[run.id] = cls.process(run, inputs)
 
             return outputs
 
     def generate_inputs(self, **kwargs: Any) -> Dict[str, Any]:
         """
-        Generates inputs for the `process` and `load_outputs` required for api mode.
+        Generate inputs for the `process` and `load_outputs` required for api mode.
+
         The arguments are validated against the input schema.
 
         Note
         ----
         Arguments are only available at runtime. Therefore, no api can be shown beforehand.
 
         Parameters
@@ -1326,19 +1492,25 @@
         kwargs : Any
             Additional keyword arguments.
 
         Returns
         -------
         Dict[str, Any]
             The inputs for the run.
+
+        Raises
+        ------
+        ValueError
+            If an unknown input is passed.
+            If an input is missing.
         """
         mapping = {}
-        for (id, attribute, *_) in self.inputs:
-            # Since `self.inputs` is ordered, we use the first occuring attribute and add
-            # the id so it is not used again.
+        for id, attribute, *_ in self.inputs:
+            # Since `self.inputs` is ordered, the first occurring attribute is used and
+            # the id is added, so it is not used again.
             if id not in mapping:
                 mapping[id] = attribute
 
         inputs: Dict[str, Dict[str, Any]] = {}
         for k, v in kwargs.items():
             if k in mapping:
                 if k not in inputs:
```

### Comparing `deepcave-1.1.3/deepcave/plugins/hyperparameter/importances.py` & `deepcave-1.2/deepcave/plugins/objective/parallel_coordinates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,428 @@
+#  noqa: D400
+
+"""
+# ParallelCoordinates
+
+This module provides utilities for visualizing the parallel coordinates.
+
+## Classes
+    - ParallelCoordinates : Can be used for visualizing the parallel coordinates.
+"""
+
+from typing import Any, Callable, Dict, List
+
+from collections import defaultdict
+
 import dash_bootstrap_components as dbc
 import numpy as np
+import pandas as pd
 import plotly.graph_objs as go
 from dash import dcc, html
 from dash.exceptions import PreventUpdate
 
 from deepcave import config
-from deepcave.evaluators.fanova import fANOVA as GlobalEvaluator
-from deepcave.evaluators.lpi import LPI as LocalEvaluator
+from deepcave.constants import VALUE_RANGE
+from deepcave.evaluators.fanova import fANOVA
 from deepcave.plugins.static import StaticPlugin
-from deepcave.utils.cast import optional_int
+from deepcave.utils.compression import deserialize, serialize
 from deepcave.utils.layout import get_checklist_options, get_select_options, help_button
-from deepcave.utils.styled_plot import plt
-from deepcave.utils.styled_plotty import get_color, save_image
+from deepcave.utils.logs import get_logger
+from deepcave.utils.styled_plotty import get_hyperparameter_ticks, save_image
+
+logger = get_logger(__name__)
 
 
-class Importances(StaticPlugin):
-    id = "importances"
-    name = "Importances"
-    icon = "far fa-star"
-    help = "docs/plugins/importances.rst"
+class ParallelCoordinates(StaticPlugin):
+    """Can be used for visualizing the parallel coordinates."""
+
+    id = "parallel_coordinates"
+    name = "Parallel Coordinates"
+    icon = "far fa-map"
     activate_run_selection = True
+    help = "docs/plugins/parallel_coordinates.rst"
 
     @staticmethod
-    def get_input_layout(register):
+    def get_input_layout(register: Callable) -> List[Any]:
+        """
+        Get the layout for the input block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to regsiter (user) variables.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[Any]
+            The layouts for the input block.
+        """
         return [
-            html.Div(
-                [
-                    dbc.Label("Objective"),
-                    dbc.Select(
-                        id=register("objective_id", ["value", "options"], type=int),
-                        placeholder="Select objective ...",
-                    ),
-                ],
-                className="mb-3",
-            ),
             dbc.Row(
                 [
                     dbc.Col(
                         [
-                            dbc.Label("Method"),
-                            help_button(
-                                "Local Parameter Importance: Quantify importance by changing the "
-                                "neighborhood of a configuration. Uses default and incumbent "
-                                "configuration as reference. \n\n"
-                                "fANOVA: Quantify importance globally."
-                            ),
+                            dbc.Label("Objective"),
                             dbc.Select(
-                                id=register("method", ["value", "options"]),
-                                placeholder="Select ...",
+                                id=register("objective_id", ["value", "options"], type=int),
+                                placeholder="Select objective ...",
                             ),
                         ],
                         md=6,
                     ),
                     dbc.Col(
                         [
-                            dbc.Label("Trees"),
+                            dbc.Label("Budget"),
                             help_button(
-                                "The number of trees of the internal random forest to estimate the "
-                                "hyperparameter importance. "
-                                "The more trees are used the more accurate the results. "
-                                "However, also it takes longer to compute."
+                                "Budget refers to the multi-fidelity budget. "
+                                "Combined budget means that the trial on the highest evaluated"
+                                " budget is used.  \n "
+                                "Note: Selecting combined budget might be misleading if a time"
+                                " objective is used. Often, higher budget take longer to evaluate,"
+                                " which might negatively influence the results."
+                            ),
+                            dbc.Select(
+                                id=register("budget_id", ["value", "options"], type=int),
+                                placeholder="Select budget ...",
                             ),
-                            dbc.Input(id=register("n_trees", type=optional_int), type="number"),
                         ],
                         md=6,
                     ),
                 ],
+                className="mb-3",
+            ),
+            html.Div(
+                [
+                    dbc.Label("Show Important Hyperparameters"),
+                    help_button(
+                        "Only the most important hyperparameters are shown which are "
+                        "calculated by fANOVA using 10 trees. The more left a "
+                        "hyperparameter stands, the more important it is. However, activating "
+                        "this option might take longer."
+                    ),
+                    dbc.Select(
+                        id=register("show_important_only", ["value", "options"]),
+                        placeholder="Select ...",
+                    ),
+                ]
             ),
         ]
 
     @staticmethod
-    def get_filter_layout(register):
+    def get_filter_layout(register: Callable) -> List[Any]:
+        """
+        Get the layout for the filter block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register (user) variables.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[Any]
+            The layouts for the filter block.
+        """
         return [
-            html.Div(
+            dbc.Row(
                 [
-                    dbc.Label("Hyperparameters"),
-                    dbc.Checklist(
-                        id=register("hyperparameter_names", ["value", "options"]), inline=True
+                    dbc.Col(
+                        [
+                            dbc.Label("Limit Hyperparameters"),
+                            help_button(
+                                "Shows either the n most important hyperparameters (if show "
+                                "important hyperparameters is true) or the first n selected "
+                                "hyperparameters."
+                            ),
+                            dbc.Input(id=register("n_hps", "value"), type="number"),
+                        ],
+                        md=6,
+                    ),
+                    dbc.Col(
+                        [
+                            dbc.Label("Show Unsuccessful Configurations"),
+                            help_button("Whether to show all configurations or only failed ones."),
+                            dbc.Select(
+                                id=register("show_unsuccessful", ["value", "options"]),
+                                placeholder="Select ...",
+                            ),
+                        ],
+                        md=6,
                     ),
                 ],
-                className="mb-3",
             ),
             html.Div(
                 [
-                    dbc.Label("Limit Hyperparameters"),
-                    help_button(
-                        "Shows only the n most important hyperparameters. If an important "
-                        "hyperparameter was de-selected, it is not shown but skipped."
+                    dbc.Label("Hyperparameters"),
+                    dbc.Checklist(
+                        id=register("hyperparameter_names", ["value", "options"]), inline=True
                     ),
-                    dbc.Input(id=register("n_hps", "value"), type="number"),
                 ],
-                className="mb-3",
-            ),
-            html.Div(
-                [
-                    dbc.Label("Budgets"),
-                    help_button("The hyperparameters are sorted by the highest budget."),
-                    dbc.Checklist(id=register("budget_ids", ["value", "options"]), inline=True),
-                ]
+                className="mt-3",
+                id=register("hide_hps", ["hidden"]),
             ),
         ]
 
-    def load_inputs(self):
-        method_labels = ["Local Parameter Importance (local)", "fANOVA (global)"]
-        method_values = ["local", "global"]
-
+    def load_inputs(self) -> Dict[str, Dict[str, Any]]:
+        """
+        Load the content for the defined inputs in 'get_input_layout' and 'get_filter_layout'.
+
+        This method is necessary to pre-load contents for the inputs.
+        So, if the plugin is called for the first time or there are no results in the cache,
+        the plugin gets its content from this method.
+
+        Returns
+        -------
+        Dict[str, Dict[str, Any]]
+            Content to be filled.
+        """
         return {
-            "method": {
-                "options": get_select_options(method_labels, method_values),
-                "value": "local",
-            },
-            "n_trees": {"value": 10},
-            "hyperparameter_names": {"options": get_checklist_options(), "value": []},
+            "show_important_only": {"options": get_select_options(binary=True), "value": "true"},
+            "show_unsuccessful": {"options": get_select_options(binary=True), "value": "false"},
             "n_hps": {"value": 0},
-            "budget_ids": {"options": get_checklist_options(), "value": []},
+            "hyperparameter_names": {"options": get_checklist_options(), "value": []},
+            "hide_hps": {"hidden": True},
         }
 
-    def load_dependency_inputs(self, run, _, inputs):
-        # Prepare objetives
+    def load_dependency_inputs(self, run, _, inputs) -> Dict[str, Any]:  # type: ignore
+        """
+        Work like 'load_inputs' but called after inputs have changed.
+
+        Note
+        ----
+        Only the changes have to be returned.
+        The returned dictionary will be merged with the inputs.
+
+        Parameters
+        ----------
+        run
+            The selected run.
+        inputs
+            Current content of the inputs.
+
+        Returns
+        -------
+        Dict[str, Any]
+            The dictionary with the changes.
+        """
+        # Prepare objectives
         objective_names = run.get_objective_names()
         objective_ids = run.get_objective_ids()
         objective_options = get_select_options(objective_names, objective_ids)
         objective_value = inputs["objective_id"]["value"]
 
         # Prepare budgets
         budgets = run.get_budgets(human=True)
         budget_ids = run.get_budget_ids()
         budget_options = get_checklist_options(budgets, budget_ids)
-        budget_value = inputs["budget_ids"]["value"]
+        budget_value = inputs["budget_id"]["value"]
 
-        hp_names = run.configspace.get_hyperparameter_names()
-        hp_options = get_checklist_options(hp_names)
-        hp_value = inputs["hyperparameter_names"]["value"]
+        # Prepare others
         n_hps = inputs["n_hps"]["value"]
+        hp_names = run.configspace.get_hyperparameter_names()
+
+        if inputs["show_important_only"]["value"] == "true":
+            hp_options = []
+            hp_value = inputs["hyperparameter_names"]["value"]
+            hidden = True
+        else:
+            hp_options = get_select_options(hp_names)
+
+            values = inputs["hyperparameter_names"]["value"]
+            if len(values) == 0:
+                values = hp_names
+
+            hp_value = values
+            hidden = False
 
-        # Pre-set values
         if objective_value is None:
             objective_value = objective_ids[0]
-            n_hps = len(hp_names)
+            budget_value = budget_ids[-1]
+            hp_value = hp_names
 
         if n_hps == 0:
             n_hps = len(hp_names)
 
-        # Pre-selection of the hyperparameters
-        if run is not None:
-            if len(hp_value) == 0:
-                hp_value = hp_names
-            if len(budget_value) == 0:
-                budget_value = [budget_ids[-1]]
-
         return {
             "objective_id": {
                 "options": objective_options,
                 "value": objective_value,
             },
-            "method": {
-                "value": inputs["method"]["value"],
+            "budget_id": {
+                "options": budget_options,
+                "value": budget_value,
             },
             "hyperparameter_names": {
                 "options": hp_options,
                 "value": hp_value,
             },
-            "budget_ids": {
-                "options": budget_options,
-                "value": budget_value,
-            },
             "n_hps": {"value": n_hps},
-            "n_trees": {"value": inputs["n_trees"]["value"]},
+            "hide_hps": {"hidden": hidden},
         }
 
     @staticmethod
-    def process(run, inputs):
+    def process(run, inputs) -> Dict[str, Any]:  # type: ignore
+        """
+        Return raw data based on a run and input data.
+
+        Warning
+        -------
+        The returned data must be JSON serializable.
+
+        Note
+        ----
+        The passed inputs are cleaned and therefore differs compared to 'load_inputs'
+        or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
+
+        Parameters
+        ----------
+        run : AbstractRun
+            The run to process.
+        inputs : Dict[str, Any]
+            The input data.
+
+        Returns
+        -------
+        Dict[str, Any]
+            The serialized dictionary.
+        """
+        budget = run.get_budget(inputs["budget_id"])
         objective = run.get_objective(inputs["objective_id"])
-        method = inputs["method"]
-        n_trees = inputs["n_trees"]
-
-        if n_trees is None:
-            raise RuntimeError("Please specify the number of trees.")
-
-        hp_names = run.configspace.get_hyperparameter_names()
-        budgets = run.get_budgets(include_combined=True)
-
-        if method == "local":
-            # Intiatize the evaluator
-            evaluator = LocalEvaluator(run)
-        elif method == "global":
-            evaluator = GlobalEvaluator(run)
-        else:
-            raise RuntimeError("Method was not found.")
-
-        # Collect data
-        data = {}
-        for budget_id, budget in enumerate(budgets):
-            evaluator.calculate(objective, budget, n_trees=n_trees, seed=0)
-
-            importances = evaluator.get_importances(hp_names)
-            data[budget_id] = importances
+        df = run.get_encoded_data(objective, budget)
+        df = df.groupby(df.columns.drop(objective.name).to_list(), as_index=False).mean()
+        df = serialize(df)
+        result: Dict[str, Any] = {"df": df}
+
+        if inputs["show_important_only"]:
+            # Let's run a quick fANOVA here
+            evaluator = fANOVA(run)
+            evaluator.calculate(objective, budget, n_trees=10, seed=0)
+            importances_dict = evaluator.get_importances()
+            importances = {u: v[0] for u, v in importances_dict.items()}
+            important_hp_names = sorted(
+                importances, key=lambda key: importances[key], reverse=False
+            )
+            result["important_hp_names"] = important_hp_names
 
-        return data
+        return result
 
     @staticmethod
-    def get_output_layout(register):
-        return dcc.Graph(register("graph", "figure"), style={"height": config.FIGURE_HEIGHT})
+    def get_output_layout(register: Callable) -> dcc.Graph:
+        """
+        Get the layout for the output block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register outputs.
+            The register_output function is located in the Plugin superclass.
+
+        Returns
+        -------
+        dcc.Graph
+            The layouts for the output block.
+        """
+        return dcc.Graph(
+            register("graph", "figure"),
+            style={"height": config.FIGURE_HEIGHT},
+            config={"toImageButtonOptions": {"scale": config.FIGURE_DOWNLOAD_SCALE}},
+        )
 
     @staticmethod
-    def load_outputs(run, inputs, outputs):
-        # First selected, should always be shown first
-        selected_hp_names = inputs["hyperparameter_names"]
-        selected_budget_ids = inputs["budget_ids"]
+    def load_outputs(run, inputs, outputs) -> go.Figure:  # type: ignore
+        """
+        Read in the raw data and prepare them for the layout.
+
+        Note
+        ----
+        The passed inputs are cleaned and therefore differs compared to 'load_inputs'
+        or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
+
+        Parameters
+        ----------
+        run
+            The selected run.
+        inputs
+            The inputs and filter values fromt the user.
+        outputs
+            Raw output from the run.
+
+        Returns
+        -------
+        go.Figure
+            The output figure.
+        """
+        objective = run.get_objective(inputs["objective_id"])
+        objective_name = objective.name
+
+        show_important_only = inputs["show_important_only"]
+        show_unsuccessful = inputs["show_unsuccessful"]
         n_hps = inputs["n_hps"]
 
         if n_hps == "" or n_hps is None:
             raise PreventUpdate
         else:
             n_hps = int(n_hps)
 
-        if len(selected_hp_names) == 0 or len(selected_budget_ids) == 0:
-            raise PreventUpdate()
+        if show_important_only:
+            hp_names = outputs["important_hp_names"]
+        else:
+            hp_names = inputs["hyperparameter_names"]
 
-        # Collect data
-        data = {}
-        for budget_id, importances in outputs.items():
-            # Important to cast budget_id here because of json serialization
-            budget_id = int(budget_id)
-            if budget_id not in selected_budget_ids:
-                continue
-
-            x = []
-            y = []
-            error_y = []
-            for hp_name, results in importances.items():
-                if hp_name not in selected_hp_names:
-                    continue
-
-                x += [hp_name]
-                y += [results[0]]
-                error_y += [results[1]]
-
-            data[budget_id] = (np.array(x), np.array(y), np.array(error_y))
-
-        # Sort by last fidelity now
-        selected_budget_id = max(selected_budget_ids)
-        idx = np.argsort(data[selected_budget_id][1], axis=None)[::-1]
-        idx = idx[:n_hps]
-
-        bar_data = []
-        for budget_id, values in data.items():
-            budget = run.get_budget(budget_id, human=True)
-
-            x = values[0][idx]
-            # new_x = []
-            # for string in x:
-            #    string = string.replace("center_optimizer:", "")
-            #    string = string.replace(":__choice__", "")
-            #    string = string.replace("AdamWOptimizer", "AdamW")
-            #    string = string.replace("SGDOptimizer", "SGD")
-            #    new_x += [string]
-            # x = new_x
-
-            bar_data += [
-                go.Bar(
-                    name=budget,
-                    x=x,
-                    y=values[1][idx],
-                    error_y_array=values[2][idx],
-                    marker_color=get_color(budget_id),
-                )
-            ]
-
-        figure = go.Figure(data=bar_data)
-        figure.update_layout(
-            barmode="group",
-            yaxis_title="Importance",
-            legend={"title": "Budget"},
-            margin=config.FIGURE_MARGIN,
-            xaxis=dict(tickangle=-45),
-        )
-        save_image(figure, "importances.pdf")
+        hp_names = hp_names[:n_hps]
 
-        return figure
+        df = outputs["df"]
+        df = deserialize(df, dtype=pd.DataFrame)
+        objective_values = []
+        for value in df[objective_name].values:
+            b = np.isnan(value)
+            if not show_unsuccessful:
+                b = not b
+            if b:
+                objective_values += [value]
+
+        data: defaultdict = defaultdict(dict)
+        for hp_name in hp_names:
+            values = []
+            for hp_v, objective_v in zip(df[hp_name].values, df[objective_name].values):
+                b = np.isnan(objective_v)
+                if not show_unsuccessful:
+                    b = not b
+                if b:
+                    values += [hp_v]
+
+            data[hp_name]["values"] = values
+            data[hp_name]["label"] = hp_name
+            data[hp_name]["range"] = VALUE_RANGE
 
-    @staticmethod
-    def get_mpl_output_layout(register):
-        return html.Img(
-            id=register("graph", "src"),
-            className="img-fluid",
-        )
+            hp = run.configspace.get_hyperparameter(hp_name)
+            tickvals, ticktext = get_hyperparameter_ticks(hp, ticks=4, include_nan=True)
 
-    @staticmethod
-    def load_mpl_outputs(run, inputs, outputs):
-        # First selected, should always be shown first
-        selected_hp_names = inputs["hyperparameter_names"]
-        selected_budget_ids = inputs["budget_ids"]
-        n_hps = inputs["n_hps"]
+            data[hp_name]["tickvals"] = tickvals
+            data[hp_name]["ticktext"] = ticktext
 
-        if n_hps == "" or n_hps is None:
-            raise PreventUpdate()
+        if show_unsuccessful:
+            line = dict()
         else:
-            n_hps = int(n_hps)
-
-        if len(selected_hp_names) == 0 or len(selected_budget_ids) == 0:
-            raise PreventUpdate()
-
-        # Collect data
-        data = {}
-        for budget_id, importances in outputs.items():
-            # Important to cast budget_id here because of json serialization
-            budget_id = int(budget_id)
-            # if budget_id not in selected_budget_ids:
-            #    continue
-
-            x = []
-            y = []
-            error_y = []
-            for hp_name, results in importances.items():
-                if hp_name not in selected_hp_names:
-                    continue
-
-                x += [hp_name]
-                y += [results[0]]
-                error_y += [results[1]]
-
-            data[budget_id] = (np.array(x), np.array(y), np.array(error_y))
-
-        # Sort by last fidelity now
-        selected_budget_id = max(selected_budget_ids)
-        idx = np.argsort(data[selected_budget_id][1], axis=None)[::-1]
-        idx = idx[:n_hps]
-
-        x_labels = []
-        for hp_name in data[selected_budget_id][0][idx]:
-            if len(hp_name) > 18:
-                hp_name = "..." + hp_name[-18:]
-
-            x_labels += [hp_name]
-        x = np.arange(len(x_labels))
-
-        plt.figure()
-        for budget_id, values in data.items():
-            if budget_id not in selected_budget_ids:
-                continue
-
-            y = values[1][idx]
-            y_err = values[2][idx]
-
-            budget = run.get_budget(budget_id, human=True)
-            plt.bar(
-                x,
-                y,
-                yerr=y_err,
-                color=plt.get_color(budget_id),
-                label=budget,
-                error_kw=dict(lw=1, capsize=2, capthick=1),
+            data[objective_name]["values"] = objective_values
+            data[objective_name]["label"] = objective_name
+            line = dict(
+                color=data[objective_name]["values"],
+                showscale=True,
+                colorscale="aggrnyl",
             )
 
-        plt.legend(title="Budgets")
-
-        # Rotate x ticks
-        plt.xticks(x, x_labels, rotation=90)
-        plt.ylabel("Importance")
+        figure = go.Figure(
+            data=go.Parcoords(
+                line=line,
+                dimensions=list([d for d in data.values()]),
+                labelangle=45,
+            ),
+            layout=dict(margin=dict(t=150, b=50, l=100, r=0)),
+        )
+        save_image(figure, "parallel_coordinates.pdf")
 
-        return plt.render()
+        return figure
```

### Comparing `deepcave-1.1.3/deepcave/plugins/hyperparameter/pdp.py` & `deepcave-1.2/deepcave/plugins/objective/configuration_cube.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,73 @@
+#  noqa: D400
+"""
+# ConfigurationCube
+
+This module provides utilities for visualizing and creating a configuration cube.
+
+The configuration cube displays configurations and their score on the objective.
+
+## Classes
+    - ConfigurationCube: A plugin for visualizing a configuration cube.
+"""
+
+from typing import Any, Callable, Dict, List, Tuple
+
 import dash_bootstrap_components as dbc
 import numpy as np
+import pandas as pd
 import plotly.graph_objs as go
 from dash import dcc, html
-from pyPDP.algorithms.pdp import PDP
+from dash.exceptions import PreventUpdate
 
 from deepcave import config
-from deepcave.evaluators.epm.random_forest_surrogate import RandomForestSurrogate
-from deepcave.plugins.static import StaticPlugin
-from deepcave.runs import Status
-from deepcave.utils.layout import get_checklist_options, get_select_options, help_button
-from deepcave.utils.styled_plotty import get_color, get_hyperparameter_ticks, save_image
-
-GRID_POINTS_PER_AXIS = 20
-SAMPLES_PER_HP = 10
-MAX_SAMPLES = 10000
-MAX_SHOWN_SAMPLES = 100
-
-
-class PartialDependencies(StaticPlugin):
-    id = "pdp"
-    name = "Partial Dependencies"
-    icon = "far fa-grip-lines"
-    help = "docs/plugins/partial_dependencies.rst"
+from deepcave.plugins.dynamic import DynamicPlugin
+from deepcave.runs import AbstractRun, Status
+from deepcave.utils.compression import deserialize, serialize
+from deepcave.utils.layout import (
+    get_checklist_options,
+    get_select_options,
+    get_slider_marks,
+    help_button,
+)
+from deepcave.utils.logs import get_logger
+from deepcave.utils.styled_plotty import (
+    get_hovertext_from_config,
+    get_hyperparameter_ticks,
+    save_image,
+)
+
+logger = get_logger(__name__)
+
+
+class ConfigurationCube(DynamicPlugin):
+    """A plugin for visualizing a configuration cube."""
+
+    id = "ccube"
+    name = "Configuration Cube"
+    icon = "fas fa-cube"
     activate_run_selection = True
+    help = "docs/plugins/configuration_cube.rst"
 
     @staticmethod
-    def get_input_layout(register):
+    def get_input_layout(register: Callable) -> List[dbc.Row]:
+        """
+        Get the layout for the input block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register (user) variables.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[dbc.Row]
+            Layouts for the input block.
+        """
         return [
             dbc.Row(
                 [
                     dbc.Col(
                         [
                             dbc.Label("Objective"),
                             dbc.Select(
@@ -39,316 +77,358 @@
                         ],
                         md=6,
                     ),
                     dbc.Col(
                         [
                             dbc.Label("Budget"),
                             help_button(
+                                "Budget refers to the multi-fidelity budget. "
                                 "Combined budget means that the trial on the highest"
-                                " evaluated budget is used.\n\n"
+                                " evaluated budget is used.  \n "
                                 "Note: Selecting combined budget might be misleading if"
                                 " a time objective is used. Often, higher budget take "
                                 " longer to evaluate, which might negatively influence "
                                 " the results."
                             ),
                             dbc.Select(
                                 id=register("budget_id", ["value", "options"], type=int),
                                 placeholder="Select budget ...",
                             ),
                         ],
                         md=6,
                     ),
                 ],
-                className="mb-3",
-            ),
-            dbc.Row(
-                [
-                    dbc.Col(
-                        [
-                            dbc.Label("Hyperparameter #1"),
-                            dbc.Select(
-                                id=register("hyperparameter_name_1", ["value", "options"]),
-                                placeholder="Select hyperparameter ...",
-                            ),
-                        ],
-                        md=6,
-                    ),
-                    dbc.Col(
-                        [
-                            dbc.Label("Hyperparameter #2"),
-                            dbc.Select(
-                                id=register("hyperparameter_name_2", ["value", "options"]),
-                                placeholder="Select hyperparameter ...",
-                            ),
-                        ],
-                        md=6,
-                    ),
-                ],
             ),
         ]
 
     @staticmethod
-    def get_filter_layout(register):
+    def get_filter_layout(register: Callable) -> List[html.Div]:
+        """
+        Get the layout for the filter block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register (user) variables.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[html.Div]
+            Layouts for the filter block.
+        """
         return [
-            dbc.Row(
+            html.Div(
                 [
-                    dbc.Col(
-                        [
-                            html.Div(
-                                [
-                                    dbc.Label("Show confidence"),
-                                    help_button("Displays the confidence bands."),
-                                    dbc.Select(
-                                        id=register("show_confidence", ["value", "options"])
-                                    ),
-                                ]
-                            )
-                        ],
-                        md=6,
+                    dbc.Label("Number of Configurations"),
+                    help_button(
+                        "The number of configurations to show, these are ordered based on"
+                        " the time at which they were evaluated."
                     ),
-                    dbc.Col(
-                        [
-                            html.Div(
-                                [
-                                    dbc.Label("Show ICE curves"),
-                                    help_button(
-                                        "Displays the ICE curves from which the PDP curve is "
-                                        "derivied."
-                                    ),
-                                    dbc.Select(id=register("show_ice", ["value", "options"])),
-                                ]
-                            )
-                        ],
-                        md=6,
+                    dcc.Slider(
+                        id=register("n_configs", ["value", "min", "max", "marks"]), step=None
                     ),
                 ],
+                className="mb-3",
+            ),
+            html.Div(
+                [
+                    dbc.Label("Hyperparameters"),
+                    help_button("Which hyperparameters to show. Maxium 3 active."),
+                    dbc.Checklist(
+                        id=register("hyperparameter_names", ["value", "options"]), inline=True
+                    ),
+                ]
             ),
         ]
 
-    def load_inputs(self):
+    def load_inputs(self) -> Dict[str, Any]:
+        """
+        Load the content for the defined inputs in 'get_input_layout' and 'get_filter_layout'.
+
+        This method is necessary to pre-load contents for the inputs.
+        So, if the plugin is called for the first time or there are no results in the cache,
+        the plugin gets its content from this method.
+
+        Returns
+        -------
+        Dict[str, Any]
+            The content to be filled.
+        """
         return {
-            "show_confidence": {"options": get_select_options(binary=True), "value": "true"},
-            "show_ice": {"options": get_select_options(binary=True), "value": "true"},
+            "n_configs": {"min": 0, "max": 0, "marks": get_slider_marks(), "value": 0},
+            "hyperparameter_names": {"options": get_checklist_options(), "value": []},
         }
 
-    def load_dependency_inputs(self, run, previous_inputs, inputs):
+    def load_dependency_inputs(self, run, _, inputs) -> Dict[str, Any]:  # type: ignore
+        """
+        Work like 'load_inputs' but called after inputs have changed.
+
+        It is restricted to three Hyperparameters.
+
+        Note
+        ----
+        Only the changes have to be returned.
+        The returned dictionary will be merged with the inputs.
+
+        Parameters
+        ----------
+        run
+            The selected run.
+        inputs
+            Current content of the inputs.
+
+        Returns
+        -------
+        Dict[str, Any]
+           The dictionary with the changes.
+        """
+        # Prepare objectives
         objective_names = run.get_objective_names()
         objective_ids = run.get_objective_ids()
         objective_options = get_select_options(objective_names, objective_ids)
+        objective_value = inputs["objective_id"]["value"]
 
+        # Prepare budgets
         budgets = run.get_budgets(human=True)
         budget_ids = run.get_budget_ids()
-        budget_options = get_checklist_options(budgets, budget_ids)
+        budget_options = get_select_options(budgets, budget_ids)
+        budget_value = inputs["budget_id"]["value"]
 
+        # Prepare others
         hp_names = run.configspace.get_hyperparameter_names()
 
         # Get selected values
-        objective_value = inputs["objective_id"]["value"]
-        budget_value = inputs["budget_id"]["value"]
-        hp1_value = inputs["hyperparameter_name_1"]["value"]
+        n_configs_value = inputs["n_configs"]["value"]
 
+        # Pre-set values
         if objective_value is None:
             objective_value = objective_ids[0]
+        if budget_value is None:
             budget_value = budget_ids[-1]
-            hp1_value = hp_names[0]
+        else:
+            budget_value = inputs["budget_id"]["value"]
+
+        budget = run.get_budget(budget_value)
+        configs = run.get_configs(budget=budget)
+        if n_configs_value == 0:
+            n_configs_value = len(configs)
+        else:
+            if n_configs_value > len(configs):
+                n_configs_value = len(configs)
+
+        # Restrict to three hyperparameters
+        selected_hps = inputs["hyperparameter_names"]["value"]
+        n_selected = len(selected_hps)
+        if n_selected > 3:
+            del selected_hps[0]
 
         return {
-            "objective_id": {"options": objective_options, "value": objective_value},
-            "budget_id": {"options": budget_options, "value": budget_value},
-            "hyperparameter_name_1": {
-                "options": get_checklist_options(hp_names),
-                "value": hp1_value,
+            "objective_id": {
+                "options": objective_options,
+                "value": objective_value,
+            },
+            "budget_id": {
+                "options": budget_options,
+                "value": budget_value,
+            },
+            "n_configs": {
+                "min": 0,
+                "max": len(configs),
+                "marks": get_slider_marks(list(range(0, len(configs) + 1))),
+                "value": n_configs_value,
             },
-            "hyperparameter_name_2": {
-                "options": get_checklist_options([None] + hp_names),
+            "hyperparameter_names": {
+                "options": get_select_options(hp_names),
+                "value": selected_hps,
             },
         }
 
     @staticmethod
-    def process(run, inputs):
-        # Surrogate
-        hp_names = run.configspace.get_hyperparameter_names()
-        objective = run.get_objective(inputs["objective_id"])
+    def process(run: AbstractRun, inputs: Dict[str, Any]) -> Dict[str, str]:
+        """
+        Return raw data based on the run and input data.
+
+        Warning
+        -------
+        The returned data must be JSON serializable.
+
+        Note
+        ----
+        The passed inputs are cleaned and therefore differs compared to 'load_inputs'
+        or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
+
+        Parameters
+        ----------
+        run : AbstractRun
+            The selected run.
+        inputs : Dict[str, Any]
+            The input data.
+
+        Returns
+        -------
+        Dict[str, str]
+            The serialized dictionary.
+        """
         budget = run.get_budget(inputs["budget_id"])
-        hp1 = inputs["hyperparameter_name_1"]
-        hp2 = inputs["hyperparameter_name_2"]
-
-        if objective is None:
-            raise RuntimeError("Objective not found.")
+        objective = run.get_objective(inputs["objective_id"])
 
-        # Encode data
         df = run.get_encoded_data(
-            objective,
-            budget,
-            specific=True,
-            statuses=Status.SUCCESS,
-        )
-
-        X = df[hp_names].to_numpy()
-        Y = df[objective.name].to_numpy()
-
-        # Let's initialize the surrogate
-        surrogate_model = RandomForestSurrogate(run.configspace, seed=0)
-        surrogate_model.fit(X, Y)
-
-        # Prepare the hyperparameters
-        selected_hyperparameters = [hp1]
-        if hp2 is not None and hp2 != "":
-            selected_hyperparameters += [hp2]
-
-        num_samples = SAMPLES_PER_HP * len(X)
-        # We limit the samples to max 10k
-        if num_samples > MAX_SAMPLES:
-            num_samples = MAX_SAMPLES
-
-        # And finally call PDP
-        pdp = PDP.from_random_points(
-            surrogate_model,
-            selected_hyperparameter=selected_hyperparameters,
-            seed=0,
-            num_grid_points_per_axis=GRID_POINTS_PER_AXIS,
-            num_samples=num_samples,
+            objectives=objective, budget=budget, statuses=Status.SUCCESS, include_config_ids=True
         )
-
-        x = pdp.x_pdp.tolist()
-        y = pdp.y_pdp.tolist()
-
-        # We have to cut the ICE curves because it's too much data
-        x_ice = pdp._ice.x_ice.tolist()
-        y_ice = pdp._ice.y_ice.tolist()
-
-        if len(x_ice) > MAX_SHOWN_SAMPLES:
-            x_ice = x_ice[:MAX_SHOWN_SAMPLES]
-            y_ice = y_ice[:MAX_SHOWN_SAMPLES]
-
-        return {
-            "x": x,
-            "y": y,
-            "variances": pdp.y_variances.tolist(),
-            "x_ice": x_ice,
-            "y_ice": y_ice,
-        }
+        return {"df": serialize(df)}
 
     @staticmethod
-    def get_output_layout(register):
-        return dcc.Graph(register("graph", "figure"), style={"height": config.FIGURE_HEIGHT})
+    def get_output_layout(register: Callable) -> Tuple[dcc.Graph,]:
+        """
+        Get the layout for the output block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register output.
+            The register_output function is located in the Plugin superclass.
+
+        Returns
+        -------
+        Tuple[dcc.Graph,]
+            Layout for the output block.
+        """
+        return (
+            dcc.Graph(
+                register("graph", "figure"),
+                style={"height": config.FIGURE_HEIGHT},
+                config={"toImageButtonOptions": {"scale": config.FIGURE_DOWNLOAD_SCALE}},
+            ),
+        )
 
     @staticmethod
-    def load_outputs(run, inputs, outputs):
-        # Parse inputs
-        hp1_name = inputs["hyperparameter_name_1"]
-        hp1_idx = run.configspace.get_idx_by_hyperparameter_name(hp1_name)
-        hp1 = run.configspace.get_hyperparameter(hp1_name)
-
-        hp2_name = inputs["hyperparameter_name_2"]
-        hp2_idx = None
-        hp2 = None
-        if hp2_name is not None and hp2_name != "":
-            hp2_idx = run.configspace.get_idx_by_hyperparameter_name(hp2_name)
-            hp2 = run.configspace.get_hyperparameter(hp2_name)
+    def load_outputs(run, inputs, outputs) -> go.Figure:  # type: ignore
+        """
+        Read in the raw data and prepares them for the layout.
+
+        Note
+        ----
+        The passed inputs are cleaned and therefore differs compared to 'load_inputs'
+        or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
+
+        Parameters
+        ----------
+        run
+            The selected run.
+        inputs
+            Input and filter values from the user.
+        outputs
+            Raw output from the run.
+
+        Returns
+        -------
+        go.Figure
+            The output figure.
+        """
+        df = deserialize(outputs["df"], dtype=pd.DataFrame)
+        hp_names = inputs["hyperparameter_names"]
+        n_configs = inputs["n_configs"]
+        objective_id = inputs["objective_id"]
+        objective = run.get_objective(objective_id)
+        budget = run.get_budget(inputs["budget_id"])
+        df = df.groupby(df.columns.drop(objective.name).to_list(), as_index=False).mean()
+        df.index = df.index.astype("str")
 
-        show_confidence = inputs["show_confidence"]
-        show_ice = inputs["show_ice"]
+        # Limit to n_configs
+        idx = [str(i) for i in range(n_configs, len(df))]
+        df = df.drop(idx)
+
+        costs = df[objective.name].values.tolist()
+        config_ids = df["config_id"].values.tolist()
+        data = []
+
+        # Specify layout kwargs
+        layout_kwargs = {}
+        if n_configs > 0 and len(hp_names) > 0:
+            for i, (hp_name, axis_name) in enumerate(zip(hp_names, ["xaxis", "yaxis", "zaxis"])):
+                hp = run.configspace.get_hyperparameter(hp_name)
+                values = df[hp_name].values.tolist()
+
+                tickvals, ticktext = get_hyperparameter_ticks(hp, ticks=4, include_nan=True)
+                layout_kwargs[axis_name] = {
+                    "tickvals": tickvals,
+                    "ticktext": ticktext,
+                    "title": hp_name,
+                }
+                data.append(values)
 
-        objective = run.get_objective(inputs["objective_id"])
-        objective_name = objective.name
+        if len(data) == 0:
+            raise PreventUpdate
 
-        # Parse outputs
-        x = np.asarray(outputs["x"])
-        y = np.asarray(outputs["y"])
-        sigmas = np.sqrt(np.asarray(outputs["variances"]))
-
-        x_ice = np.asarray(outputs["x_ice"])
-        y_ice = np.asarray(outputs["y_ice"])
-
-        traces = []
-        if hp2_idx is None:  # 1D
-            # Add ICE curves
-            if show_ice:
-                for x_, y_ in zip(x_ice, y_ice):
-                    traces += [
-                        go.Scatter(
-                            x=x_[:, hp1_idx],
-                            y=y_,
-                            line=dict(color=get_color(1, 0.1)),
-                            hoverinfo="skip",
-                            showlegend=False,
-                        )
-                    ]
-
-            if show_confidence:
-                traces += [
-                    go.Scatter(
-                        x=x[:, hp1_idx],
-                        y=y + sigmas,
-                        line=dict(color=get_color(0, 0.1)),
-                        hoverinfo="skip",
-                        showlegend=False,
-                    )
-                ]
+        # Transforms data to values
+        values = np.transpose(np.array(data)).tolist()
 
-                traces += [
-                    go.Scatter(
-                        x=x[:, hp1_idx],
-                        y=y - sigmas,
-                        fill="tonexty",
-                        fillcolor=get_color(0, 0.2),
-                        line=dict(color=get_color(0, 0.1)),
-                        hoverinfo="skip",
-                        showlegend=False,
-                    )
-                ]
+        # Now the duplicates are filtered
+        filtered_data: Dict[Tuple[int, float], Tuple] = {}
+        for config_id, cost, v in zip(config_ids, costs, values):
+            v = tuple(v)  # Make hashable
+            key = (config_id, cost)
+
+            if v in filtered_data.values():
+                old_key = list(filtered_data.keys())[list(filtered_data.values()).index(v)]
+                old_cost = old_key[1]
+
+                if objective.optimize == "lower":
+                    if old_cost < cost:
+                        continue
+
+                if objective.optimize == "upper":
+                    if old_cost > cost:
+                        continue
+
+                # Otherwise it is replaced
+                del filtered_data[old_key]
+
+            filtered_data[key] = v
+
+        # Replace data
+        config_ids = [k[0] for k in filtered_data.keys()]
+        costs = [k[1] for k in filtered_data.keys()]
+
+        # Specify scatter kwargs
+        scatter_kwargs = {
+            "mode": "markers",
+            "marker": {
+                "size": 5,
+                "color": costs,
+                "colorbar": {"thickness": 30, "title": objective.name},
+            },
+            "hovertext": [
+                get_hovertext_from_config(run, config_id, budget) for config_id in config_ids
+            ],
+            "meta": {"colorbar": costs},
+            "hoverinfo": "text",
+        }
 
-            traces += [
-                go.Scatter(
-                    x=x[:, hp1_idx],
-                    y=y,
-                    line=dict(color=get_color(0, 1)),
-                    hoverinfo="skip",
-                    showlegend=False,
-                )
-            ]
-
-            tickvals, ticktext = get_hyperparameter_ticks(hp1)
-            layout = go.Layout(
-                {
-                    "xaxis": {
-                        "tickvals": tickvals,
-                        "ticktext": ticktext,
-                        "title": hp1_name,
-                    },
-                    "yaxis": {
-                        "title": objective_name,
-                    },
-                }
-            )
+        if len(data) >= 1:
+            x = [v[0] for v in filtered_data.values()]
+        if len(data) >= 2:
+            y = [v[1] for v in filtered_data.values()]
+        if len(data) >= 3:
+            z = [v[2] for v in filtered_data.values()]
+
+        if len(data) == 3:
+            trace = go.Scatter3d(x=x, y=y, z=z, **scatter_kwargs)
+            layout = go.Layout({"scene": {**layout_kwargs}})
         else:
-            z = y
-            if show_confidence:
-                z = sigmas
-            traces += [
-                go.Contour(
-                    z=z,
-                    x=x[:, hp1_idx],
-                    y=x[:, hp2_idx],
-                    colorbar=dict(
-                        title=objective_name if not show_confidence else "Confidence (1-Sigma)",
-                    ),
-                    hoverinfo="skip",
-                )
-            ]
-
-            x_tickvals, x_ticktext = get_hyperparameter_ticks(hp1)
-            y_tickvals, y_ticktext = get_hyperparameter_ticks(hp2)
-
-            layout = go.Layout(
-                dict(
-                    xaxis=dict(tickvals=x_tickvals, ticktext=x_ticktext, title=hp1_name),
-                    yaxis=dict(tickvals=y_tickvals, ticktext=y_ticktext, title=hp2_name),
-                    margin=config.FIGURE_MARGIN,
-                )
-            )
-
-        figure = go.Figure(data=traces, layout=layout)
-        save_image(figure, "pdp.pdf")
+            if len(data) == 1:
+                y = [0 for _ in x]
+                trace = go.Scatter(x=x, y=y, **scatter_kwargs)
+            elif len(data) == 2:
+                trace = go.Scatter(x=x, y=y, **scatter_kwargs)
+            else:
+                trace = go.Scatter(x=[], y=[])
+            layout = go.Layout(**layout_kwargs)
+
+        figure = go.Figure(data=trace, layout=layout)
+        figure.update_layout(dict(margin=config.FIGURE_MARGIN))
+        save_image(figure, "configuration_cube.pdf")
 
         return figure
```

### Comparing `deepcave-1.1.3/deepcave/plugins/static.py` & `deepcave-1.2/deepcave/plugins/static.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+#  noqa: D400
+"""
+# Static
+
+This module provides a plugin class for a static plugin.
+
+It provides an Enum used for the plugin state.
+
+## Classes
+    - PluginState: An Enum to define the state of the Plugin.
+    - StaticPlugin: This class provides a static plugin object.
+"""
+
 from abc import ABC
-from typing import Any, Callable, Dict, List
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import traceback
 from enum import Enum
 
 import dash_bootstrap_components as dbc
 from dash import dcc, html
 from dash.dash import no_update
@@ -14,56 +27,102 @@
 from deepcave import interactive
 from deepcave.plugins import Plugin
 from deepcave.runs import AbstractRun
 from deepcave.utils.url import create_url
 
 
 class PluginState(Enum):
+    """An Enum to define the state of the Plugin."""
+
     UNSET = -1
     READY = 0
     NEEDS_PROCESSING = 1
     PROCESSING = 2
     FAILED = 3
 
 
 def _process(
     process: Callable[[AbstractRun, Any], None], run: AbstractRun, inputs: Dict[str, Any]
-) -> Any:
+) -> None:
+    """
+    Process the run with the input data if possible.
+
+    Return raw data based on a run and input data.
+
+    Parameters
+    ----------
+    process : Callable[[AbstractRun, Any], None]
+        The process function.
+    run : AbstractRun
+        The run.
+    inputs : Dict[str, Any]
+        The inputs as a dictionary.
+
+    Raises
+    ------
+    Exception
+        If the process function fails.
+    """
     try:
         return process(run, inputs)
     except Exception:
         traceback.print_exc()
         raise
 
 
 class StaticPlugin(Plugin, ABC):
     """
+    Provide a static plugin object.
+
     Calculation with queue. Made for time-consuming tasks.
+    Register and handle callbacks.
+
+    Properties
+    ----------
+    outputs : List[Tuple[str, str, bool]]
+        The plugin specific outputs.
+    inputs : List[Tuple[str, str, bool, Any]]
+        The plugin specific inputs.
+    id : str
+        The plugin id.
+    raw_outputs : dict[str, Any]
+        The raw outputs of a run.
+    logger : Logger
+        The logger for the plugin.
+    name : str
+        The name of the plugin.
+    process : Callable
+        Return raw data based on a run and input data.
+    button_caption : str
+        The caption for the button.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._setup()
 
     def _setup(self) -> None:
+        """Set up the plugin."""
         self._state = PluginState.UNSET  # Set in the main loop to track what's going on right now
-        self._previous_state = None  # Used for updating status
+        self._previous_state: Optional[PluginState] = None  # Used for updating status
         self._refresh_required = True
         self._reset_button = False
         self._blocked = False
 
     @interactive
     def register_callbacks(self) -> None:
+        """Register different callbacks."""
         super().register_callbacks()
         self._callback_inputs_changed()
         self._callback_loop_update_status_label()
         self._callback_loop_trigger_main_loop()
 
     @interactive
     def _callback_inputs_changed(self) -> None:
+        """Handle callback if the inputs changed."""
         from deepcave import app, c, queue, rc, run_handler
 
         # Plugin specific outputs
         outputs = []
         for id, attribute, _ in self.outputs:
             outputs.append(Output(self.get_internal_output_id(id), attribute))
 
@@ -73,21 +132,21 @@
         ]
 
         # Get other plugin specific inputs that might change
         for id, attribute, _, _ in self.inputs:
             inputs.append(Input(self.get_internal_input_id(id), attribute))
 
         # Register updates from inputs
-        @app.callback(outputs, inputs)
-        def plugin_process(n_clicks, _, *inputs_list):  # type: ignore
+        @app.callback(outputs, inputs)  # type: ignore
+        def plugin_process(n_clicks: int, _: Any, *inputs_list: str) -> Optional[Any]:
+            """Register updates from inputs."""
             self._blocked = True
-
             # Map the list `inputs_list` to a dict s.t.
             # it's easier to access them.
-            inputs = self._list_to_dict(inputs_list, input=True)
+            inputs = self._list_to_dict(list(inputs_list), input=True)
             inputs_key = self._dict_as_key(inputs, remove_filters=True)
             cleaned_inputs = self._clean_inputs(inputs)
             last_inputs = c.get("last_inputs", self.id)
 
             link = create_url(self.get_base_url(), inputs)
             runs = self.get_selected_runs(inputs)
 
@@ -121,19 +180,19 @@
             else:
                 # Load from process
                 self._state = PluginState.NEEDS_PROCESSING
 
                 if button_pressed and self._state != PluginState.PROCESSING:
                     self.logger.debug("Button pressed.")
 
-                    # Check if we need to process
+                    # Check if processing is needed
                     for run in runs:
                         job_id = self._get_job_id(run.id, inputs_key)
 
-                        # We already got our results or it was already processed
+                        # Results are already achieved or it was already processed
                         if raw_outputs[run.id] is not None or queue.is_processed(job_id):
                             continue
 
                         job_meta = {
                             "display_name": self.name,
                             "run_name": run.name,
                             "run_id": run.id,
@@ -166,14 +225,15 @@
                             job_run_id = job_meta["run_id"]
                             job_plugin_id = job_meta["plugin_id"]
 
                             self.logger.debug(f"Job {job_id} for run_id {job_meta['run_id']}.")
                             run = run_handler.get_run(job_run_id)
 
                             # Save results in cache
+                            # Same optional string problem
                             rc.set(run, job_plugin_id, job_inputs_key, job_run_outputs)
                             self.logger.debug(f"Job {job_id} cached.")
 
                             queue.delete_job(job_id)
                             self.logger.debug(f"Job {job_id} deleted.")
                         except Exception as e:
                             self.logger.error(f"Job {job_id} failed with exception {e}.")
@@ -217,16 +277,24 @@
             Input(self.get_internal_id("update-interval"), "n_intervals"),
             State(self.get_internal_id("update-interval-output"), "data"),
         ]
 
         # Interval should not always run the main callback the whole time
         # Especially not if it's blocked because PreventUpdate
         # prevent output updates from previous callback calls.
-        @app.callback(output, inputs)
-        def plugin_check_blocked(_, data):  # type: ignore
+        @app.callback(output, inputs)  # type: ignore
+        def plugin_check_blocked(_: Any, data: Any) -> Any:
+            """
+            Check if blocked.
+
+            Raises
+            ------
+            PreventUpdate
+                If '_blocked' is True.
+            """
             if self._blocked:
                 raise PreventUpdate
 
             # This will trigger the main loop
             return data + 1
 
     @interactive
@@ -238,35 +306,36 @@
             Output(self.get_internal_id("update-button"), "n_clicks"),
             Output(self.get_internal_id("update-button"), "disabled"),
         ]
         input = Input(self.get_internal_id("update-interval"), "n_intervals")
 
         # Update status label
         # Register updates from inputs
-        @app.callback(output, input)
-        def plugin_update_status(_):  # type: ignore
+        @app.callback(output, input)  # type: ignore
+        def plugin_update_status(_: Any) -> Tuple[List[Any], Optional[Any], bool]:
+            """Update the status of the plugin."""
             button_text = [html.Span(self.button_caption)]
 
             if self._state == PluginState.UNSET:
                 # Disable and reset button
                 return button_text, None, True
 
-            # Important so we don't update the button every time (would result in an ugly spinner)
+            # Important so the button is not updated every time (would result in an ugly spinner)
             if self._previous_state == self._state:
                 raise PreventUpdate
 
             # This is a special case where the main loop goes into "needs processing"
             # although the result is already there. This is because the queue needs a second
             # to be updated.
             if (
                 self._previous_state == PluginState.PROCESSING
                 and self._state == PluginState.NEEDS_PROCESSING
             ):
-                # However: We have to unset the previous state so if we really change the inputs
-                # the visualizes will be updated.
+                # However: The previous state has to be unset, so if the inputs are really changed
+                # the visualizer will be updated.
                 self._previous_state = PluginState.UNSET
                 raise PreventUpdate
 
             if self._state == PluginState.FAILED:
                 notification.update(
                     "The job failed. Check the logs or make sure the worker is still running. "
                     "Most of the times, a simple restart might help."
@@ -287,18 +356,43 @@
 
             # Update the previous state
             self._previous_state = self._state
 
             return button_text, button, disabled
 
     def _get_job_id(self, run_name: str, inputs_key: str) -> str:
+        """
+        Get the job id.
+
+        Parameters
+        ----------
+        run_name : str
+            The name of the run.
+        inputs_key : str
+            The inputs key.
+
+        Returns
+        -------
+        str
+            The job id.
+        """
         return f"{run_name}-{inputs_key}"
 
     @interactive
     def __call__(self) -> List[Component]:  # type: ignore
+        """
+        Return the components for the plugin.
+
+        Basically, all blocks and elements of the plugin are stacked-up here.
+
+        Returns
+        -------
+        List[Component]
+            Layout as list of components.
+        """
         from deepcave import config
 
         self._setup()
 
         components = [
             dcc.Interval(id=self.get_internal_id("update-interval"), interval=config.REFRESH_RATE),
             dcc.Store(id=self.get_internal_id("update-interval-output"), data=0),
```

### Comparing `deepcave-1.1.3/deepcave/plugins/summary/configurations.py` & `deepcave-1.2/deepcave/plugins/budget/budget_correlation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,334 +1,353 @@
+#  noqa: D400
+"""
+# BudgetCorrelation
+
+This module provides utilities to visualize budget correlations.
+
+Provided utilities include getting input and output layout, processing the data
+and loading the outputs.
+
+## Classes
+    - BudgetCorrelation: Can be used for visualizing the correlation of budgets.
+"""
+from typing import Any, Callable, DefaultDict, Dict, List
+
 from collections import defaultdict
 
 import dash_bootstrap_components as dbc
-import pandas as pd
 import plotly.graph_objs as go
 from dash import dcc, html
+from scipy import stats
 
-from deepcave import config
-from deepcave.constants import VALUE_RANGE
+from deepcave import config, notification
 from deepcave.plugins.dynamic import DynamicPlugin
 from deepcave.runs import AbstractRun, Status
-from deepcave.utils.compression import deserialize, serialize
-from deepcave.utils.layout import create_table, get_slider_marks
-from deepcave.utils.styled_plotty import (
-    generate_config_code,
-    get_color,
-    get_hyperparameter_ticks,
-    save_image,
-)
-from deepcave.utils.url import create_url
-
-
-class Configurations(DynamicPlugin):
-    id = "configurations"
-    name = "Configurations"
-    icon = "fas fa-sliders-h"
-    help = "docs/plugins/configurations.rst"
+from deepcave.utils.layout import create_table, get_select_options
+from deepcave.utils.logs import get_logger
+from deepcave.utils.styled_plotty import get_color, save_image
+
+logger = get_logger(__name__)
+
+
+class BudgetCorrelation(DynamicPlugin):
+    """
+    Used for visualizing the correlation of budgets.
+
+    Provided utilities include getting input/output layout, data processing
+    and loading outputs.
+    """
+
+    id = "budget_correlation"
+    name = "Budget Correlation"
+    icon = "fas fa-coins"
+    help = "docs/plugins/budget_correlation.rst"
     activate_run_selection = True
-    use_cache = False
 
     @staticmethod
-    def get_link(run: AbstractRun, config_id: int) -> str:
+    def check_run_compatibility(run: AbstractRun) -> bool:
         """
-        Creates a link to a specific configuration.
+        Check if the run has more than one budget and is compatible.
 
         Parameters
         ----------
         run : AbstractRun
-            Selected run.
-        config_id : int
-            Configuration, which should be visited.
+            The run to be checked.
 
         Returns
         -------
-        str
-            Link to the configuration.
+        bool
+            True if the run is compatible, otherwise False.
         """
-        # Create "fake" inputs to overwrite the selection.
-        # Everything else will be taken from `load_inputs` and `load_dependency_inputs`.
-        inputs = {
-            "run": dict(value=run.id),
-            "config_id": dict(value=config_id),
-        }
-        url = Configurations.get_base_url()
+        if len(run.get_budgets()) == 1:
+            notification.update(f"{run.name} can not be selected because it has only one budget.")
+            return False
 
-        return create_url(url, inputs)
+        return True
 
     @staticmethod
-    def get_input_layout(register):
+    def get_input_layout(register: Callable) -> List[html.Div]:
+        """
+        Get the layout for the input block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register (user) variables.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[html.Div]
+            Layouts for the input block.
+        """
         return [
             html.Div(
                 [
-                    dbc.Label("Configuration ID"),
-                    dcc.Slider(id=register("config_id", ["value", "min", "max", "marks"])),
+                    dbc.Label("Objective"),
+                    dbc.Select(
+                        id=register("objective_id", ["value", "options"], type=int),
+                        placeholder="Select objective ...",
+                    ),
                 ],
             ),
         ]
 
-    def load_inputs(self):
-        return {
-            "config_id": {"min": 0, "max": 0, "marks": get_slider_marks(), "value": 0},
-        }
+    def load_dependency_inputs(self, run, _, inputs) -> Dict[str, Dict[str, Any]]:  # type: ignore
+        """
+        Work like 'load_inputs' but called after inputs have changed.
 
-    def load_dependency_inputs(self, run, previous_inputs, inputs):
-        # Get selected values
-        config_id_value = inputs["config_id"]["value"]
-        configs = run.get_configs()
-        if config_id_value > len(configs) - 1:
-            config_id_value = len(configs) - 1
+        Note
+        ----
+        Only the changes are returned, they will be later merged with the inputs.
+
+        Parameters
+        ----------
+        run
+            The run to get the objective from.
+        inputs
+            The inputs containing the objective id and a value.
+
+        Returns
+        -------
+        Dict[str, Dict[str, Any]]
+            A dictionary with the changes.
+        """
+        objective_names = run.get_objective_names()
+        objective_ids = run.get_objective_ids()
+        objective_options = get_select_options(objective_names, objective_ids)
+
+        value = inputs["objective_id"]["value"]
+        if value is None:
+            value = objective_ids[0]
 
         return {
-            "config_id": {
-                "min": 0,
-                "max": len(configs) - 1,
-                "marks": get_slider_marks(list(configs.keys()), access_all=True),
-                "value": config_id_value,
+            "objective_id": {
+                "options": objective_options,
+                "value": value,
             },
         }
 
     @staticmethod
-    def process(run, inputs):
-        selected_config_id = int(inputs["config_id"])
-        origin = run.get_origin(selected_config_id)
-        objectives = run.get_objectives()
-        budgets = run.get_budgets(include_combined=False)
-
-        overview_table_data = {
-            "Key": ["Selected Configuration", "Origin"],
-            "Value": [selected_config_id, origin],
-        }
-
-        if run.prefix == "group":
-            original_run = run.get_original_run(selected_config_id)
-            original_config_id = run.get_original_config_id(selected_config_id)
-            overview_table_data["Key"] += ["Derived from"]
-            overview_table_data["Value"] += [
-                str(original_run.path) + f" (Configuration ID: {original_config_id})"
-            ]
-
-        performances = {}
-        performances_table_data = {"Budget": []}
-        for objective_id, objective in enumerate(objectives):
-            if objective.name not in performances:
-                performances[objective.name] = {}
-                performances_table_data[objective.name] = []
-
-            for budget in budgets:
-                # Budget might not be evaluated
-                try:
-                    costs = run.get_costs(selected_config_id, budget)
-                except Exception:
-                    costs = [None for _ in range(len(objectives))]
-
-                performances[objective.name][budget] = costs[objective_id]
-
-                # And add table data
-                if budget not in performances_table_data["Budget"]:
-                    performances_table_data["Budget"] += [budget]
-
-                status = run.get_status(selected_config_id, budget)
-                if status == Status.SUCCESS:
-                    performances_table_data[objective.name] += [costs[objective_id]]
-                else:
-                    performances_table_data[objective.name] += [status.to_text()]
+    def process(run: AbstractRun, inputs: Dict[str, int]) -> Dict[str, Any]:
+        """
+        Return raw data based on a run and the input data.
 
-        # Let's start with the configspace
-        X = []
-        cs_table_data = {"Hyperparameter": [], "Value": []}
-        for config_id, config in run.get_configs().items():
-            x = run.encode_config(config)
+        Warning
+        -------
+        The returned data must be JSON serializable.
 
-            highlight = 0
-            if config_id == selected_config_id:
-                highlight = 1
+        Note
+        ----
+        The passed inputs are cleaned and therefore differ
+        compared to 'load_inputs' or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
 
-                for k, v in config.items():
-                    # Add accurate data for our table here
-                    cs_table_data["Hyperparameter"] += [k]
-                    cs_table_data["Value"] += [v]
+        Parameters
+        ----------
+        run : AbstractRun
+            The run to process.
+        inputs : Dict[str, int]
+            The input to get the objective id from.
 
-            # We simply add highlight as a new column
-            x += [highlight]
+        Returns
+        -------
+        Dict[str, Any]
+            Serialized dictionary with the correlations
+            as well as the correlations symmetric.
+        """
+        objective_id = inputs["objective_id"]
+        budget_ids = run.get_budget_ids(include_combined=False)
 
-            # And add it to the lists
-            X.append(x)
+        # Add symmetric correlations; table ready
+        correlations_symmetric: DefaultDict[str, Dict[str, float]] = defaultdict(dict)
 
-        columns = run.configspace.get_hyperparameter_names()
-        columns += ["highlighted"]
+        correlations: DefaultDict[str, Dict[str, float]] = defaultdict(dict)
+        for budget1_id in budget_ids:
+            budget1 = run.get_budget(budget1_id)
+            budget1_readable = run.get_budget(budget1_id, human=True)
+
+            for budget2_id in budget_ids:
+                budget2 = run.get_budget(budget2_id)
+                budget2_readable = run.get_budget(budget2_id, human=True)
+
+                config_ids1 = run.get_configs(budget1, statuses=[Status.SUCCESS]).keys()
+                config_ids2 = run.get_configs(budget2, statuses=[Status.SUCCESS]).keys()
+
+                # Combine config ids
+                # So it is guaranteed that there is the same number of configs for each budget
+                config_ids = set(config_ids1) & set(config_ids2)
+
+                c1, c2 = [], []
+                for config_id in config_ids:
+                    c1 += [
+                        run.get_avg_costs(config_id, budget1, statuses=[Status.SUCCESS])[0][
+                            objective_id
+                        ]
+                    ]
+                    c2 += [
+                        run.get_avg_costs(config_id, budget2, statuses=[Status.SUCCESS])[0][
+                            objective_id
+                        ]
+                    ]
+
+                correlation = round(stats.spearmanr(c1, c2).correlation, 2)
+                correlations_symmetric["Budget"][budget2_readable] = budget2_readable  # type: ignore # noqa: E501
+                correlations_symmetric[budget1_readable][budget2_readable] = correlation  # type: ignore # noqa: E501
+
+                # Exclude if budget2 is higher than budget1
+                if budget2 > budget1:
+                    continue
 
-        cs_df = pd.DataFrame(data=X, columns=columns)
+                correlations[budget1_readable][budget2_readable] = correlation  # type: ignore
 
         return {
-            "overview_table_data": overview_table_data,
-            "performances": performances,
-            "performances_table_data": performances_table_data,
-            "cs_df": serialize(cs_df),
-            "cs_table_data": cs_table_data,
+            "correlations": correlations,
+            "correlations_symmetric": correlations_symmetric,
         }
 
     @staticmethod
-    def get_output_layout(register):
+    def get_output_layout(register: Callable) -> List[Any]:
+        """
+        Get the layout for the output block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register outputs.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[Any]
+            Layout for the output block.
+        """
         return [
-            html.Div(id=register("overview_table", "children"), className="mb-3"),
-            html.Hr(),
-            html.H3("Objectives"),
-            dbc.Tabs(
-                [
-                    dbc.Tab(
-                        dcc.Graph(
-                            id=register("performance_graph", "figure"),
-                            style={"height": config.FIGURE_HEIGHT},
-                        ),
-                        label="Graph",
-                    ),
-                    dbc.Tab(html.Div(id=register("performance_table", "children")), label="Table"),
-                ]
-            ),
-            html.Hr(),
-            html.H3("Configuration"),
+            html.Div(id=register("text", "children"), className="mb-3"),
             dbc.Tabs(
                 [
                     dbc.Tab(
                         dcc.Graph(
-                            id=register("configspace_graph", "figure"),
+                            id=register("graph", "figure"),
                             style={"height": config.FIGURE_HEIGHT},
+                            config={
+                                "toImageButtonOptions": {"scale": config.FIGURE_DOWNLOAD_SCALE}
+                            },
                         ),
                         label="Graph",
                     ),
-                    dbc.Tab(html.Div(id=register("configspace_table", "children")), label="Table"),
+                    dbc.Tab(html.Div(id=register("table", "children")), label="Table"),
                 ]
             ),
-            html.Hr(),
-            dbc.Accordion(
-                [
-                    dbc.AccordionItem(
-                        html.Output(
-                            generate_config_code(register, variables=["path", "config_dict"])
-                        ),
-                        title="See code",
-                    ),
-                ],
-                start_collapsed=True,
-            ),
         ]
 
     @staticmethod
-    def _get_objective_figure(_, outputs, run):
-        objective_data = []
-        for i, (metric, values) in enumerate(outputs["performances"].items()):
-            trace_kwargs = {
-                "x": list(values.keys()),
-                "y": list(values.values()),
-                "name": metric,
-                "fill": "tozeroy",
-            }
-
-            if i > 0:
-                trace_kwargs.update({"yaxis": f"y{i+1}"})
-
-            trace = go.Scatter(**trace_kwargs)
-            objective_data.append(trace)
-
-        layout_kwargs = {
-            "margin": config.FIGURE_MARGIN,
-            "xaxis": {"title": "Budget", "domain": [0.05 * len(run.get_objectives()), 1]},
-        }
+    def load_outputs(run, _, outputs) -> List[Any]:  # type: ignore
+        """
+        Read the raw data and prepare it for the layout.
 
-        # We create an axis for each objective now
-        for id, objective in enumerate(run.get_objectives()):
-            yaxis = "yaxis"
-            if id > 0:
-                # yaxis, yaxis2, yaxis3, ...
-                yaxis = f"yaxis{id+1}"
-
-            layout_kwargs[yaxis] = {
-                # "title": objective.name,
-                "titlefont": {"color": get_color(id)},
-                "tickfont": {"color": get_color(id)},
-                "range": [objective.lower, objective.upper],
-            }
-
-            if id > 0:
-                layout_kwargs[yaxis].update(
-                    {
-                        "anchor": "free",
-                        "overlaying": "y",
-                        "side": "left",
-                        "position": 0.05 * id,
-                    }
-                )
+        Note
+        ----
+        The passed inputs are cleaned and therefore differ
+        compared to 'load_inputs' or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
 
-        objective_layout = go.Layout(**layout_kwargs)
-        objective_figure = go.Figure(data=objective_data, layout=objective_layout)
-        save_image(objective_figure, "configure.pdf")
+        Parameters
+        ----------
+        run
+            The selected run.
+        outputs
+            Raw output from the run.
 
-        return objective_figure
+        Returns
+        -------
+        List[Any]
+            The text, the figure and the created table.
+        """
+        traces = []
+        categories: defaultdict = defaultdict(list)
+        correlations = outputs["correlations"]
+        correlations_symmetric = outputs["correlations_symmetric"]
+        for idx, (budget1, budgets) in enumerate(correlations.items()):
+            x, y = [], []
+            for budget2, correlation in budgets.items():
+                x += [float(budget2)]
+                y += [correlation]
+
+                category = None
+                if correlation >= 0.7:
+                    category = "very strong"
+                elif correlation >= 0.4:
+                    category = "strong"
+                elif correlation >= 0.3:
+                    category = "moderate"
+                elif correlation >= 0.2:
+                    category = "weak"
+                else:
+                    category = "not given"
 
-    @staticmethod
-    def _get_configspace_figure(inputs, outputs, run):
-        df = outputs["cs_df"]
-        df = deserialize(df, dtype=pd.DataFrame)
-
-        highlighted = df["highlighted"].values
-        hp_names = run.configspace.get_hyperparameter_names()
-
-        # Get highlighted column
-        highlighted_df = df[df["highlighted"] == 1]
-
-        data = defaultdict(dict)
-        for hp_name in hp_names:
-            data[hp_name]["values"] = df[hp_name].values
-            data[hp_name]["label"] = hp_name
-            data[hp_name]["range"] = VALUE_RANGE
-
-            hp = run.configspace.get_hyperparameter(hp_name)
-            tickvals, ticktext = get_hyperparameter_ticks(
-                hp, additional_values=highlighted_df[hp_name].values, ticks=4, include_nan=True
-            )
+                key = (budget1, budget2)
+                key2 = (budget2, budget1)
 
-            data[hp_name]["tickvals"] = tickvals
-            data[hp_name]["ticktext"] = ticktext
+                if budget1 == budget2:
+                    continue
 
-        fig = go.Figure(
-            data=go.Parcoords(
-                line=dict(
-                    color=highlighted,
-                    showscale=False,
-                    colorscale=["rgba(255,255,255,0.1)", "red"],
-                ),
-                dimensions=list([d for d in data.values()]),
-                labelangle=45,
-                labelside="top",
-            ),
-            layout=dict(
-                margin=dict(
-                    t=150,
-                    b=50,
+                if key not in categories[category] and key2 not in categories[category]:
+                    if float(budget1) < float(budget2):
+                        categories[category] += [key]
+                    else:
+                        categories[category] += [key2]
+
+            traces.append(
+                go.Scatter(
+                    x=x,
+                    y=y,
+                    name=budget1,
+                    line=dict(color=get_color(idx)),
                 )
-            ),
+            )
+
+        layout = go.Layout(
+            xaxis=dict(title="Budget"),
+            yaxis=dict(title="Correlation"),
+            margin=config.FIGURE_MARGIN,
+            legend=dict(title="Budgets"),
         )
 
-        return fig
+        figure = go.Figure(data=traces, layout=layout)
+        save_image(figure, "budget_correlation.png")
 
-    @staticmethod
-    def load_outputs(run, inputs, outputs):
-        config_id = inputs["config_id"]
-        config = run.get_config(config_id)
-
-        if run.path is not None:
-            path = run.path / "configspace.json"
-        else:
-            assert run.prefix == "group"
-            original_run = run.get_original_run(config_id)
-            path = original_run.path
+        # Add vertical lines
+        readable_budgets = run.get_budgets(human=True, include_combined=False)
+        for idx, budget in enumerate(readable_budgets):
+            figure.add_vline(
+                x=budget,
+                line=dict(
+                    color=get_color(idx),
+                    width=1,
+                    dash="dot",
+                ),
+            )
 
+        text = "The budget correlation of"
+        n_categories = len(categories)
+        for i, (relation, pairs) in enumerate(categories.items()):
+            if n_categories > 1 and i == n_categories - 1:
+                text += ", and "
+            elif n_categories > 1 and i > 0:
+                text += ", "
+            else:
+                text += " "
+
+            formated_pairs = []
+            for pair in pairs:
+                formated_pairs += [f"({pair[0]}, {pair[1]})"]
+
+            pairs_text = ", ".join(formated_pairs)
+            text += f"{pairs_text} is {relation}"
+            if i == n_categories - 1:
+                text += "."
         return [
-            create_table(outputs["overview_table_data"], head=False, striped=False),
-            Configurations._get_objective_figure(inputs, outputs, run),
-            create_table(outputs["performances_table_data"]),
-            Configurations._get_configspace_figure(inputs, outputs, run),
-            create_table(outputs["cs_table_data"]),
-            str(path),
-            str(config.get_dictionary()),
+            text,
+            figure,
+            create_table(correlations_symmetric, mb=False),
         ]
```

### Comparing `deepcave-1.1.3/deepcave/plugins/summary/overview.py` & `deepcave-1.2/deepcave/plugins/summary/overview.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+# noqa: D400
+"""
+# Overview
+
+This module provides utilities for visualizing an overview of the selected runs.
+
+It holds the most important information, e.g. meta data, objectives and statistics.
+
+The module includes a dynamic plugin for the overview.
+
+## Classes
+    - Overview: Visualize an overall overview of the selected run.
+"""
+
+from typing import Any, Callable, Dict, List
+
+import itertools
+
 import dash_bootstrap_components as dbc
 import numpy as np
 import plotly.graph_objs as go
 from ConfigSpace.hyperparameters import (
     CategoricalHyperparameter,
     Constant,
     NormalFloatHyperparameter,
@@ -19,23 +37,39 @@
 from deepcave.runs.status import Status
 from deepcave.utils.layout import create_table, help_button
 from deepcave.utils.styled_plotty import get_discrete_heatmap, save_image
 from deepcave.utils.util import get_latest_change
 
 
 class Overview(DynamicPlugin):
+    """Visualize an overall overview of the selected run."""
+
     id = "overview"
     name = "Overview"
     icon = "fas fa-search"
     help = "docs/plugins/overview.rst"
     use_cache = False
     activate_run_selection = True
 
     @staticmethod
-    def get_output_layout(register):
+    def get_output_layout(register: Callable) -> List[Any]:
+        """
+        Get the layout for the output block.
+
+        Parameters
+        ----------
+        register : Callable
+            Method to register the outputs.
+            The register_input function is located in the Plugin superclass.
+
+        Returns
+        -------
+        List[Any]
+            The layouts for the output block.
+        """
         return [
             html.Div(
                 id=register("card", "children"),
                 className="mb-3",
             ),
             html.Hr(),
             html.H3("Meta"),
@@ -48,52 +82,71 @@
             html.Div(id=register("status_text", "children"), className="mb-3"),
             dbc.Tabs(
                 [
                     dbc.Tab(
                         dcc.Graph(
                             id=register("status_statistics", "figure"),
                             style={"height": config.FIGURE_HEIGHT},
+                            config={
+                                "toImageButtonOptions": {"scale": config.FIGURE_DOWNLOAD_SCALE}
+                            },
                         ),
                         label="Barplot",
                     ),
                     dbc.Tab(
                         dcc.Graph(
                             id=register("config_statistics", "figure"),
                             style={"height": config.FIGURE_HEIGHT},
+                            config={
+                                "toImageButtonOptions": {"scale": config.FIGURE_DOWNLOAD_SCALE}
+                            },
                         ),
                         label="Heatmap",
                     ),
                     dbc.Tab(html.Div(id=register("status_details", "children")), label="Details"),
                 ]
             ),
             html.Hr(),
             html.H3("Configuration Space"),
             html.Div(id=register("configspace", "children")),
         ]
 
     @staticmethod
-    def load_outputs(run, *_):
+    def load_outputs(run, *_: Any) -> List[Any]:  # type: ignore
+        """
+        Read in the raw data and prepare them for the layout.
+
+        Note
+        ----
+        The passed inputs are cleaned and therefore differs compared to 'load_inputs'
+        or 'load_dependency_inputs'.
+        Please see '_clean_inputs' for more information.
+
+        Parameters
+        ----------
+        run
+            The selected run.
+
+        Returns
+        -------
+        List[Any]
+            A list of the created tables of the overview.
+        """
         # Get best cost across all objectives, highest budget
-        incumbent, _ = run.get_incumbent()
+        incumbent, _ = run.get_incumbent(statuses=[Status.SUCCESS])
         config_id = run.get_config_id(incumbent)
         objective_names = run.get_objective_names()
 
-        best_performance = {}
-        # Budget might not be evaluated
-        try:
-            costs = run.get_costs(config_id)
-        except Exception:
-            costs = [None for _ in range(len(objective_names))]
-
-        for idx, cost in enumerate(costs):
-            best_performance[objective_names[idx]] = cost
+        avg_costs, std_costs = run.get_avg_costs(config_id)
 
         best_performances = []
-        for name, value in best_performance.items():
-            best_performances += [f"{round(value, 2)} ({name})"]
+        for idx in range(len(objective_names)):
+            best_performances += [
+                f"{round(avg_costs[idx], 2)} ± {round(std_costs[idx], 2)} ({objective_names[idx]})"
+            ]
 
         optimizer = run.prefix
         if isinstance(run, Group):
             optimizer = run.get_runs()[0].prefix
 
         # Design card for quick information here
         card = dbc.Card(
@@ -138,87 +191,107 @@
                 ),
             ],
             color="secondary",
             inverse=True,
         )
 
         # Meta
-        meta = {"Attribute": [], "Value": []}
+        meta: Dict[str, List[str]] = {"Attribute": [], "Value": []}
         for k, v in run.get_meta().items():
             if k == "objectives":
                 continue
 
             if isinstance(v, list):
                 v = ", ".join(str(_v) for _v in v)
 
             meta["Attribute"].append(k)
             meta["Value"].append(str(v))
 
         # Objectives
-        objectives = {"Name": [], "Bounds": []}
+        objectives: Dict[str, List[str]] = {"Name": [], "Bounds": []}
         for objective in run.get_objectives():
             objectives["Name"].append(objective.name)
             objectives["Bounds"].append(f"[{objective.lower}, {objective.upper}]")
 
         # Budgets
         budgets = run.get_budgets(include_combined=False)
 
-        # Statistics
-        status_statistics = {}
-        status_details = {"Configuration ID": [], "Budget": [], "Status": [], "Error": []}
+        # Seeds
+        seeds = run.get_seeds(include_combined=False)
+
+        # Budget-seed combinations
+        budget_seed_combinations = list(itertools.product(budgets, seeds))
+
+        # Setup statistics dict for bar plot
+        status_statistics: Dict[float, Dict[Status, int]] = {}
+
         for budget in budgets:
             budget = round(budget, 2)
             if budget not in status_statistics:
                 status_statistics[budget] = {}
 
                 for s in Status:
                     status_statistics[budget][s] = 0
 
-        status_statistics_total = {}
-        status_budget = {}
+        # Setup details dict for to collect information on failed trials
+        status_details: Dict[str, List[Any]] = {
+            "Configuration ID": [],
+            "Budget": [],
+            "Seed": [],
+            "Status": [],
+            "Error": [],
+        }
+
+        status_count = {}
+        budget_count = {}
         len_trials = 0
         for trial in run.get_trials():
             budget = round(trial.budget, 2)
+            seed = trial.seed
 
             len_trials += 1
+
+            # Status count over budget for bar plot
             status_statistics[budget][trial.status] += 1
 
-            # For text information
-            if trial.status not in status_statistics_total:
-                status_statistics_total[trial.status] = 1
+            # Total status count for text information
+            if trial.status not in status_count:
+                status_count[trial.status] = 1
             else:
-                status_statistics_total[trial.status] += 1
+                status_count[trial.status] += 1
 
-            # For text information
-            if budget not in status_budget:
-                status_budget[budget] = 1
+            # Total budget count for text information
+            if budget not in budget_count:
+                budget_count[budget] = 1
             else:
-                status_budget[budget] += 1
+                budget_count[budget] += 1
 
             # Add to table data
             if trial.status != Status.SUCCESS:
                 link = Configurations.get_link(run, trial.config_id)
 
                 status_details["Configuration ID"] += [
                     html.A(trial.config_id, href=link, target="_blank")
                 ]
                 status_details["Budget"] += [budget]
+                status_details["Seed"] += [seed]
                 status_details["Status"] += [trial.status.to_text()]
 
                 if "traceback" in trial.additional:
                     traceback = trial.additional["traceback"]
                     status_details["Error"] += [help_button(traceback)]
                 else:
                     status_details["Error"] += ["No traceback available."]
 
-        successful_trials_rate = status_statistics_total[Status.SUCCESS] / len_trials * 100
+        # Successful / unsuccessful trials rate for text information
+        successful_trials_rate = status_count[Status.SUCCESS] / len_trials * 100
         successful_trials_rate = round(successful_trials_rate, 2)
 
         trials_rates = []
-        for status, count in status_statistics_total.items():
+        for status, count in status_count.items():
             if status == Status.SUCCESS:
                 continue
 
             rate = round(count / len_trials * 100, 2)
             trials_rates += [status.to_text() + f" ({rate}%)"]
 
         # Add an "or" to the last rate
@@ -233,69 +306,69 @@
                 unsuccessful_trials_text += "either "
                 trials_rates[-1] = " or " + trials_rates[-1]
                 unsuccessful_trials_text += ", ".join(trials_rates)
             unsuccessful_trials_text += "."
         else:
             unsuccessful_trials_text = ""
 
-        status_budget_values = [
-            str(round(count / len_trials * 100, 2)) + "%" for count in status_budget.values()
+        # Budget rate for text information
+        budget_rate = [
+            str(round(count / len_trials * 100, 2)) + "%" for count in budget_count.values()
         ]
-        status_budget_values_text = "/".join(status_budget_values)
-        status_budget_keys_text = [str(key) for key in status_budget.keys()]
-        status_budget_keys_text = "/".join(status_budget_keys_text)
+        budget_rate_text = "/".join(budget_rate)
+        budget_keys_text_list = [str(key) for key in budget_count.keys()]
+        budget_keys_text = "/".join(budget_keys_text_list)
 
+        # Text information
         status_text = f"""
         Taking all evaluated trials into account, {successful_trials_rate}% have been successful.
         {unsuccessful_trials_text}
-        Moreover, {status_budget_values_text} of the configurations were evaluated on budget
-        {status_budget_keys_text}, respectively.
+        Moreover, {budget_rate_text} of the trials were evaluated on budget
+        {budget_keys_text}, respectively.
         """
 
-        # Now remove status that are not used
+        # Status statistics for bar plot: remove status that are not used
         for budget in list(status_statistics.keys()):
             for status in list(status_statistics[budget].keys()):
                 if status_statistics[budget][status] == 0:
                     del status_statistics[budget][status]
 
-        # It is interesting to see on which budget a configuration was evaluated
+        # Config statistics for heatmap showing on which budget / seed a configuration was evaluated
         config_statistics = {}
         configs = run.get_configs()
         config_ids = list(configs.keys())
 
-        z_values = np.zeros((len(config_ids), len(budgets))).tolist()
-        z_labels = np.zeros((len(config_ids), len(budgets))).tolist()
+        z_values = np.zeros((len(config_ids), len(budget_seed_combinations))).tolist()
+        z_labels = np.zeros((len(config_ids), len(budget_seed_combinations))).tolist()
 
         for i, config_id in enumerate(configs.keys()):
-            for j, budget in enumerate(budgets):
-                trial_key = run.get_trial_key(config_id, budget)
+            for j, (b, s) in enumerate(budget_seed_combinations):
+                trial_key = run.get_trial_key(config_id, b, s)
                 trial = run.get_trial(trial_key)
 
                 status = Status.NOT_EVALUATED
                 if trial is not None:
                     status = trial.status
-
                 z_values[i][j] = status.value
                 z_labels[i][j] = status.to_text()
 
-        config_statistics["X"] = budgets
+        config_statistics["X"] = budget_seed_combinations
         config_statistics["Y"] = config_ids
         config_statistics["Z_values"] = z_values
         config_statistics["Z_labels"] = z_labels
 
         # Prepare configspace table
-        configspace = {
+        configspace: Dict[str, List] = {
             "Hyperparameter": [],
             "Possible Values": [],
             "Default": [],
             "Log": [],
         }
 
         for hp_name, hp in run.configspace.get_hyperparameters_dict().items():
-
             log = False
             value = None
             if (
                 isinstance(hp, UniformIntegerHyperparameter)
                 or isinstance(hp, NormalIntegerHyperparameter)
                 or isinstance(hp, UniformFloatHyperparameter)
                 or isinstance(hp, NormalFloatHyperparameter)
@@ -306,40 +379,40 @@
                 value = ", ".join([str(i) for i in hp.choices])
             elif isinstance(hp, OrdinalHyperparameter):
                 value = ", ".join([str(i) for i in hp.sequence])
             elif isinstance(hp, Constant):
                 value = str(hp.value)
 
             default = str(hp.default_value)
-            log = str(log)
+            log_str = str(log)
 
             configspace["Hyperparameter"].append(hp_name)
             configspace["Possible Values"].append(value)
             configspace["Default"].append(default)
-            configspace["Log"].append(log)
+            configspace["Log"].append(log_str)
 
         stats_data = []
         for budget, stats in status_statistics.items():
             x = [s.to_text() for s in stats.keys()]
             trace = go.Bar(x=x, y=list(stats.values()), name=budget)
             stats_data.append(trace)
 
         stats_layout = go.Layout(
-            legend={"title": "Budget"},
+            legend={"title": "Budget (Seed)"},
             barmode="group",
             xaxis=dict(title="Status"),
             yaxis=dict(title="Number of configurations"),
             margin=config.FIGURE_MARGIN,
         )
         stats_figure = go.Figure(data=stats_data, layout=stats_layout)
         save_image(stats_figure, "status_bar.pdf")
 
         config_layout = go.Layout(
             legend={"title": "Status"},
-            xaxis=dict(title="Budget"),
+            xaxis=dict(title="Budget (Seed)"),
             yaxis=dict(title="Configuration ID"),
             margin=config.FIGURE_MARGIN,
         )
         config_figure = go.Figure(
             data=get_discrete_heatmap(
                 config_statistics["X"],
                 config_statistics["Y"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepcave-1.1.3/deepcave/runs/__init__.py` & `deepcave-1.2/deepcave/runs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+#  noqa: D400
+"""
+# AbstractRun
+
+This module provides utilities to create and handle an abstract run.
+
+It provides functions to get information of the run, as well as the used objectives.
+
+## Classes
+    - AbstractRun: Create a new run.
+"""
+
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 from pathlib import Path
 
 import ConfigSpace
 import numpy as np
@@ -13,149 +25,293 @@
     UniformFloatHyperparameter,
     UniformIntegerHyperparameter,
 )
 
 from deepcave.constants import (
     COMBINED_BUDGET,
     COMBINED_COST_NAME,
+    COMBINED_SEED,
     CONSTANT_VALUE,
     NAN_VALUE,
 )
-from deepcave.runs.exceptions import NotMergeableError
+from deepcave.runs.exceptions import NotMergeableError, RunInequality
 from deepcave.runs.objective import Objective
 from deepcave.runs.status import Status
 from deepcave.runs.trial import Trial
 from deepcave.utils.logs import get_logger
 
 
 class AbstractRun(ABC):
+    """
+    Create a new run.
+
+    Provide functions to get information of the run, as well as the used objectives.
+
+    Properties
+    ----------
+    name : str
+        The name of the run.
+    path : Optional[Path]
+        The path to the run.
+    logger : Logger
+        The logger for the run.
+    meta: Dict[str, Any]
+        Contains the run's meta information.
+    configspace: ConfigSpace.ConfigurationSpace
+        The configuration space of the run.
+    configs: Dict[int, Configuration]
+        Contains the configurations.
+    origins: Dict[int, str]
+        The origin of the configuration.
+    models: Dict[int, Optional[Union[str, "torch.nn.Module"]]]
+        Contains the modules.
+    history: List[Trial]
+        The history of Trials.
+    trial_keys: Dict[Tuple[str, int], int]
+        Contains config_id, budget and the corresponding trial_id.
+    models_dir : Path
+        The directory of the model.
+    """
+
     prefix: str
 
     def __init__(self, name: str) -> None:
         self.name: str = name
         self.path: Optional[Path] = None
         self.logger = get_logger(self.__class__.__name__)
 
         # objects created by reset
         self.reset()
 
     def reset(self) -> None:
+        """
+        Reset the run to default values / empties.
+
+        Clear the initial data and configurations of the object.
+        """
         self.meta: Dict[str, Any] = {}
         self.configspace: ConfigSpace.ConfigurationSpace
-        self.configs: Dict[int, Configuration] = {}
-        self.origins: Dict[int, str] = {}
-        self.models: Dict[int, Optional[Union[str, "torch.nn.Module"]]] = {}
+        self.configs: Dict[int, Union[Configuration, Dict[Any, Any]]] = {}
+        self.origins: Dict[int, Optional[str]] = {}
+        self.models: Dict[  # type: ignore
+            int, Optional[Union[str, "torch.nn.Module"]]  # noqa: F821
+        ] = {}
 
         self.history: List[Trial] = []
-        self.trial_keys: Dict[Tuple[str, int], int] = {}  # (config_id, budget) -> trial_id
+        self.trial_keys: Dict[
+            Tuple[int, Optional[Union[int, float]], Optional[int]], int
+        ] = {}  # (config_id, budget, seed) -> trial_id
 
         # Cached data
         self._highest_budget: Dict[int, Union[int, float]] = {}  # config_id -> budget
 
     def _update_highest_budget(
         self, config_id: int, budget: Union[int, float], status: Status
     ) -> None:
+        """
+        Update the highest budget.
+
+        Parameters
+        ----------
+        config_id : int
+            The identificator of the configuration.
+        budget : Union[int, float]
+            The new highest budget.
+        status : Status
+            The status of the run.
+        """
         if status == Status.SUCCESS:
             # Update highest budget
             if config_id not in self._highest_budget:
                 self._highest_budget[config_id] = budget
             else:
                 if budget > self._highest_budget[config_id]:
                     self._highest_budget[config_id] = budget
 
     @property
     @abstractmethod
     def hash(self) -> str:
         """
-        Hash of the current run. If hash changes, cache has to be cleared. This ensures that
+        Hash of the current run.
+
+        If hash changes, cache has to be cleared. This ensures that
         the cache always holds the latest results of the run.
 
         Returns
         -------
         hash : str
             Hash of the run.
         """
         pass
 
     @property
     @abstractmethod
     def id(self) -> str:
         """
-        Hash of the file. This is used to identify the file.
+        Hash of the file.
+
+        This is used to identify the file.
         In contrast to `hash`, this hash should not be changed throughout the run.
 
         Returns
         -------
         str
             Hash of the run.
         """
         pass
 
     @property
     def latest_change(self) -> float:
+        """
+        Get the latest change.
+
+        Returns
+        -------
+        float
+            The latest change.
+        """
         return 0
 
     @staticmethod
-    def get_trial_key(config_id: int, budget: Union[int, float]):
-        return (config_id, budget)
+    def get_trial_key(
+        config_id: int, budget: Optional[Union[int, float]], seed: Optional[int]
+    ) -> Tuple[int, Optional[Union[int, float]], Optional[int]]:
+        """
+        Get the trial key.
+
+        It is obtained through the assembly of configuration and budget.
+
+        Parameters
+        ----------
+        config_id : int
+            The identificator of the configuration.
+        budget : Optional[Union[int, float]]
+            The budget of the Trial.
+        seed: Optional[int]
+            The seed used for the Trial.
+
+        Returns
+        -------
+        Tuple[int, Optional[Union[int, float]], Optional[int]]
+            Tuple representing the trial key, consisting of configuration id, budget, and seed.
+        """
+        return (config_id, budget, seed)
 
-    def get_trial(self, trial_key) -> Optional[Trial]:
+    def get_trial(self, trial_key: tuple[int, Union[int, float], int]) -> Optional[Trial]:
+        """
+        Get the trial with the responding key if existing.
+
+        Parameters
+        ----------
+        trial_key : Tuple[int, Union[int, float], int]
+            The key for the desired trial.
+
+        Returns
+        -------
+        Optional[Trial]
+            The trial object.
+        """
         if trial_key not in self.trial_keys:
             return None
 
         return self.history[self.trial_keys[trial_key]]
 
     def get_trials(self) -> Iterator[Trial]:
+        """
+        Get an iterator of all stored trials.
+
+        Returns
+        -------
+        Iterator[Trial]
+            An iterator over all stored trials.
+        """
         yield from self.history
 
     def get_meta(self) -> Dict[str, Any]:
+        """
+        Get a shallow copy of the meta information.
+
+        Returns
+        -------
+        Dict[str, Any]
+            A shallow copy of the meta information dictionary.
+        """
         return self.meta.copy()
 
     def empty(self) -> bool:
+        """
+        Check if the run's history is empty.
+
+        Returns
+        -------
+        bool
+            True if run history is empty, False otherwise.
+        """
         return len(self.history) == 0
 
-    def get_origin(self, config_id: int) -> str:
+    def get_origin(self, config_id: int) -> Optional[str]:
+        """
+        Get the origin, given a config id.
+
+        Parameters
+        ----------
+        config_id : int
+            The identificator of the configuration.
+
+        Returns
+        -------
+        Optional[str]
+            An origin string corresponding to the given configuration id.
+        """
         return self.origins[config_id]
 
     def get_objectives(self) -> List[Objective]:
+        """
+        Get a list of all objectives corresponding to the run.
+
+        Returns
+        -------
+        List[Objective]
+            A list containing all objectives associated with the run.
+        """
         objectives = []
         for d in self.meta["objectives"].copy():
             objective = Objective.from_json(d)
             objectives += [objective]
 
         return objectives
 
     def get_objective(self, id: Union[str, int]) -> Optional[Objective]:
-        """Returns the objective based on the id or the name.
+        """
+        Return the objective based on the id or the name.
 
         Parameters
         ----------
         id : Union[str, int]
             The id or name of the objective.
 
         Returns
         -------
-        Objective
-            The objective object.
+        Optional[Objective]
+            The objective.
         """
-
         objectives = self.get_objectives()
         if type(id) == int:
             return objectives[id]
 
         # Otherwise, iterate till the name is found
         for objective in objectives:
             if objective.name == id:
                 return objective
 
         return None
 
     def get_objective_id(self, objective: Union[Objective, str]) -> int:
         """
-        Returns the id of the objective if it is found.
+        Return the id of the objective if it is found.
 
         Parameters
         ----------
         objective : Union[Objective, str]
             The objective or objective name for which the id is returned.
 
         Returns
@@ -176,173 +332,350 @@
             else:
                 if objective == objective2.name:
                     return id
 
         raise RuntimeError("Objective was not found.")
 
     def get_objective_ids(self) -> List[int]:
+        """
+        Get the ids of the objectives.
+
+        Returns
+        -------
+        List[int]
+            A list of the ids of the objectives.
+        """
         return list(range(len(self.get_objectives())))
 
     def get_objective_name(self, objectives: Optional[List[Objective]] = None) -> str:
         """
         Get the cost name of given objective names.
+
         Returns "Combined Cost" if multiple objective names were involved.
-        """
 
+        Parameters
+        ----------
+        objectives : Optional[List[Objective]]
+            A list of the objectives.
+            By default None.
+
+        Returns
+        -------
+        str
+            The name of the objective.
+            Returns "Combined Cost" if multiple objective names were involved.
+        """
         available_objective_names = self.get_objective_names()
 
         if objectives is None:
             if len(available_objective_names) == 1:
                 return available_objective_names[0]
         else:
             if len(objectives) == 1:
                 return objectives[0].name
 
         return COMBINED_COST_NAME
 
     def get_objective_names(self) -> List[str]:
+        """
+        Get the names of the objectives.
+
+        Returns
+        -------
+        List[str]
+            A list containing the names of the objectives.
+        """
         return [obj.name for obj in self.get_objectives()]
 
-    def get_configs(self, budget: Union[int, float] = None) -> Dict[int, Configuration]:
+    def get_configs(
+        self,
+        budget: Optional[Union[int, float]] = None,
+        seed: Optional[int] = None,
+        statuses: Optional[Union[Status, List[Status]]] = None,
+    ) -> Dict[int, Configuration]:
         """
-        Get configurations of the run. Optionally, only configurations which were evaluated
-        on the passed budget are considered.
+        Get configurations of the run.
+
+        Optionally, only configurations which were evaluated on the passed budget, seed,
+        and stati are considered.
 
         Parameters
         ----------
-        budget : Union[int, float], optional
-            Considered budget. By default None (all configurations are included).
+        budget : Optional[Union[int, float]]
+            Budget to select the configs. If no budget is given, all seeds are considered.
+            By default None.
+        seed: Optional[int]
+            Seed to select the configs. If no seed is given, all seeds are considered.
+            By default None.
+        statuses : Optional[Union[Status, List[Status]]]
+            Only selected stati are considered. If no status is given, all stati are considered.
+            By default None.
+
 
         Returns
         -------
         Dict[int, Configuration]
             Configuration id and the configuration.
         """
-        # Include all configs if we have combined budget
+        # Include all configs if budget is a combined budget
         if budget == COMBINED_BUDGET:
             budget = None
 
+        # Include all configs if we have combined seed
+        if seed == COMBINED_SEED:
+            seed = None
+
         configs = {}
         for trial in self.history:
             if budget is not None:
                 if budget != trial.budget:
                     continue
 
+            if seed is not None:
+                if seed != trial.seed:
+                    continue
+
+            if statuses is not None:
+                if isinstance(statuses, Status):
+                    statuses = [statuses]
+
+                if trial.status not in statuses:
+                    continue
+
             if (config_id := trial.config_id) not in configs:
                 config = self.get_config(config_id)
                 configs[config_id] = config
 
         # Sort dictionary
         configs = dict(sorted(configs.items()))
 
         return configs
 
     def get_config(self, id: int) -> Configuration:
+        """
+        Retrieve the configuration with the corresponding id.
+
+        Parameters
+        ----------
+        id : int
+            The id of the configuration.
+
+        Returns
+        -------
+        Configuration
+            The corresponding Configuration.
+        """
         config = Configuration(self.configspace, self.configs[id])
         return config
 
     def get_config_id(self, config: Union[Configuration, Dict]) -> Optional[int]:
+        """
+        Get the id of the configuration.
+
+        Parameters
+        ----------
+        config : Union[Configuration, Dict]
+            The configuration for which to find the id.
+
+        Returns
+        -------
+        Optional[int]
+            The configuration id.
+        """
         if isinstance(config, Configuration):
             config = config.get_dictionary()
 
         # Find out config id
         for id, c in self.configs.items():
             if c == config:
                 return id
 
         return None
 
-    def get_num_configs(self, budget: Union[int, float] = None) -> int:
-        return len(self.get_configs(budget=budget))
+    def get_num_configs(
+        self, budget: Optional[Union[int, float]] = None, seed: Optional[int] = None
+    ) -> int:
+        """
+        Count the number of configurations stored in this run with a specific budget.
+
+        Parameters
+        ----------
+        budget : Optional[Union[int, float]]
+            The budget for which to count the configurations.
+            If not provided, counts all configurations.
+            Default is None.
+        seed : Optional[int]
+            The seed for which to count the configurations.
+            If not provided, counts all configurations.
+            Default is None.
+
+        Returns
+        -------
+        int
+            The number of all configurations with a given budget.
+            If budget is None, counts all configurations.
+        """
+        return len(self.get_configs(budget=budget, seed=seed))
 
-    def get_budget(self, id: Union[int, str], human=False) -> float:
+    def get_budget(self, id: Union[int, str], human: bool = False) -> Union[int, float]:
         """
-        Gets the budget given an id.
+        Get the budget given an id.
 
         Parameters
         ----------
         id : Union[int, str]
-            Id of the wanted budget. If id is a string, it is converted to an integer.
+            The id of the wanted budget.
+            If id is a string, it is converted to an integer.
+        human : bool, optional
+            Make the output more readable.
+            By default False.
 
         Returns
         -------
-        float
-            Budget.
+        float, int
+            The budget.
+
+        Raises
+        ------
+        TypeError
+            If the budget with this id is invalid.
         """
         budgets = self.get_budgets(human=human)
-        return budgets[int(id)]
+        return budgets[int(id)]  # type: ignore
 
     def get_budget_ids(self, include_combined: bool = True) -> List[int]:
+        """
+        Get the corresponding ids for the budgets.
+
+        Parameters
+        ----------
+        include_combined : bool, optional
+            If False, cut last id of budget ids.
+            By default True.
+
+        Returns
+        -------
+        List[int]
+            A list of the budget ids.
+        """
         budget_ids = list(range(len(self.get_budgets())))
         if not include_combined:
             budget_ids = budget_ids[:-1]
 
         return budget_ids
 
     def get_budgets(
         self, human: bool = False, include_combined: bool = True
-    ) -> List[Union[int, float]]:
+    ) -> List[Union[int, float, str]]:
         """
-        Returns the budgets from the meta data.
+        Return the budgets from the meta data.
 
         Parameters
         ----------
         human : bool, optional
-            Make the output better readable. By default False.
+            Make the output more readable.
+            By default False.
+        include_combined : bool, optional
+            If True, include the combined budget.
+            By default True.
 
         Returns
         -------
-        List[Union[int, float]]
-            List of budgets.
+        List[Union[int, float, str]]
+            List of budgets. In a readable form, if human is True.
         """
         budgets = self.meta["budgets"].copy()
         if include_combined and len(budgets) > 1 and COMBINED_BUDGET not in budgets:
             budgets += [COMBINED_BUDGET]
 
         if human:
-            readable_budgets = []
+            readable_budgets: List[Union[str, float]] = []
             for b in budgets:
                 if b == COMBINED_BUDGET:
                     readable_budgets += ["Combined"]
                 elif b is not None:
                     readable_budgets += [float(np.round(float(b), 2))]
 
             return readable_budgets
 
         return budgets
 
     def get_highest_budget(self, config_id: Optional[int] = None) -> Optional[Union[int, float]]:
         """
-        Returns the highest found budget for a config id. If no config id is specified then
+        Return the highest found budget for a config id.
+
+        If no config id is specified then
         the highest available budget is returned.
         Moreover, if no budget is available None is returned.
 
+        Parameters
+        ----------
+        config_id : Optional[int]
+            The config id for which the highest budget is returned.
+
         Returns
         -------
         Optional[Union[int, float]]
             The highest budget or None if no budget was specified.
         """
         if config_id is None:
             budgets = self.meta["budgets"]
             if len(budgets) == 0:
                 return None
 
             return budgets[-1]
         else:
             return self._highest_budget[config_id]
 
+    def get_seeds(
+        self, human: bool = False, include_combined: bool = True
+    ) -> List[Union[int, str]]:
+        """
+        Return the seeds from the meta data.
+
+        Parameters
+        ----------
+        human : bool, optional
+            Make the output better readable. By default False.
+        include_combined : bool, optional
+            If true, return combined seed as well. By default True.
+
+        Returns
+        -------
+        List[Union[int, str]]
+            List of seeds.
+        """
+        seeds = self.meta["seeds"].copy()
+        if include_combined and len(seeds) > 1 and COMBINED_SEED not in seeds:
+            seeds += [COMBINED_SEED]
+
+        if human:
+            readable_seeds: List[Union[int, str]] = []
+            for s in seeds:
+                if s == COMBINED_SEED:
+                    readable_seeds += ["Combined"]
+                elif s is not None:
+                    readable_seeds += [int(s)]
+
+            return readable_seeds
+
+        return seeds
+
     def _process_costs(self, costs: List[float]) -> List[float]:
         """
-        Processes the costs to get rid of NaNs. NaNs are replaced by the worst value of the
+        Process the costs to get rid of NaNs.
+
+        NaNs are replaced by the worst value of the
         objective.
 
         Parameters
         ----------
         costs : List[float]
-            Costs, which should be processed. Must be the same length as the number of objectives.
+            Costs, which should be processed.
+            Must be the same length as the number of objectives.
 
         Returns
         -------
         List[float]
             Processed costs without NaN values.
         """
         new_costs = []
@@ -350,216 +683,325 @@
             # Replace with the worst cost
             if cost is None:
                 cost = objective.get_worst_value()
             new_costs += [cost]
 
         return new_costs
 
-    def get_costs(self, config_id: int, budget: Optional[Union[int, float]] = None) -> List[float]:
+    def get_avg_costs(
+        self,
+        config_id: int,
+        budget: Optional[Union[int, float]] = None,
+        statuses: Optional[Union[Status, List[Status]]] = None,
+    ) -> Tuple[List[float], List[float]]:
         """
-        Returns the costs of a configuration. In case of multi-objective, multiple costs are
-        returned.
+        Get average costs over all seeds for a config.
+
+        Optionally, only configurations which were evaluated on the passed budget and stati
+        are considered.
+
+        In case of multi-objective, multiple costs are returned in the form of a list.
 
         Parameters
         ----------
         config_id : int
             Configuration id to get the costs for.
-        budget : Optional[Union[int, float]], optional
-            Budget to get the costs from the configuration id for. By default None. If budget is
-            None, the highest budget is chosen.
-
-        Raises
-        ------
-        ValueError
-            If the configuration id is not found.
-        RuntimeError
-            If the budget was not evaluated for the passed config id.
+        budget : Optional[Union[int, float]]
+            Budget to get the costs from the configuration id for. If budget is
+            None, the highest budget is chosen. By default None.
+        statuses : Optional[Union[Status, List[Status]]]
+            Only selected stati are considered. If no status is given, all stati are considered.
+            By default None.
 
         Returns
         -------
         List[float]
-            List of costs from the associated configuration.
+            List of average cost values for the given config_id and budget.
+        List[float]
+            List of std cost values for the given config_id and budget.
         """
-        if budget is None:
-            budget = self.get_highest_budget()
-
-        if config_id not in self.configs:
-            raise ValueError("Configuration id was not found.")
+        objectives = self.get_objectives()
 
-        costs = self.get_all_costs(budget)
-        if config_id not in costs:
-            raise RuntimeError(f"Budget {budget} was not evaluated for config id {config_id}.")
+        # Budget might not be evaluated
+        all_costs = self.get_all_costs(budget=budget, statuses=statuses)
+        if config_id in all_costs:
+            config_costs = all_costs[config_id]
+        else:
+            raise ValueError(f"No costs available for config_id {config_id}.")
 
-        return costs[config_id]
+        avg_costs, std_costs = [], []
+        for idx in range(len(objectives)):
+            costs = [values[idx] for values in config_costs.values() if values[idx] is not None]
+            avg_costs.append(float(np.mean(costs)))
+            std_costs.append(float(np.std(costs)))
+        return avg_costs, std_costs
 
     def get_all_costs(
         self,
         budget: Optional[Union[int, float]] = None,
         statuses: Optional[Union[Status, List[Status]]] = None,
-    ) -> Dict[int, List[float]]:
+        seed: Optional[int] = None,
+        selected_ids: Optional[List[int]] = None,
+    ) -> Dict[int, Dict[int, List[float]]]:
         """
-        Get all costs in the history with their config ids. Only configs from the given budget
-        and statuses are returned.
+        Get all costs in the history with their config ids and seeds.
+
+        Optionally, only configurations which were evaluated on the passed budget, seed, and stati
+        are considered.
+
+        In case of multi-objective, multiple costs are returned in the form of a list.
 
         Parameters
         ----------
-        budget : Optional[Union[int, float]], optional
+        budget : Optional[Union[int, float]]
             Budget to select the costs. If no budget is given, the highest budget is chosen.
             By default None.
-        statuses : Optional[Union[Status, List[Status]]], optional
+        statuses : Optional[Union[Status, List[Status]]]
             Only selected stati are considered. If no status is given, all stati are considered.
             By default None.
+        seed : Optional[int], optional
+            Seed to select the costs. If no seed is given, all seeds are considered.
+            By default None.
+        selected_ids: Optional[List[int]], optional
+            If set, only history ids in the list will be considered. By default None.
 
         Returns
         -------
-        Dict[int, List[float]]
-            Costs with their config ids.
+        Dict[int, Dict[int, List[float]]]
+            Config ids and seeds with their corresponding list of costs.
         """
         if budget is None:
             budget = self.get_highest_budget()
 
-        # In case of COMBINED_BUDGET, we only keep the costs of the highest found budget
+        # In case of COMBINED_BUDGET, only the costs of the highest found budget are kept
         highest_evaluated_budget = {}
 
-        results = {}
-        for trial in self.history:
+        results: Dict[int, Dict[int, List[float]]] = {}
+        if selected_ids is not None:
+            history = [self.history[i] for i in selected_ids]
+        else:
+            history = self.history
+        for trial in history:
             if statuses is not None:
                 if isinstance(statuses, Status):
                     statuses = [statuses]
 
                 if trial.status not in statuses:
                     continue
 
+            if seed is not None:
+                if trial.seed != seed:
+                    continue
+
             if budget == COMBINED_BUDGET:
                 if trial.config_id not in highest_evaluated_budget:
                     highest_evaluated_budget[trial.config_id] = trial.budget
 
                 latest_budget = highest_evaluated_budget[trial.config_id]
-                # We only keep the highest budget
+                # Only the highest budget is kept
                 if trial.budget >= latest_budget:
-                    results[trial.config_id] = trial.costs
+                    if trial.config_id not in results:
+                        results[trial.config_id] = {}
+                    results[trial.config_id][trial.seed] = trial.costs
             else:
                 if trial.budget is not None:
                     if trial.budget != budget:
                         continue
-
-                results[trial.config_id] = trial.costs  # self._process_costs(trial.costs)
-
+                if trial.config_id not in results:
+                    results[trial.config_id] = {}
+                results[trial.config_id][trial.seed] = trial.costs
         return results
 
-    def get_status(self, config_id: int, budget: Optional[Union[int, float]] = None) -> Status:
+    def get_status(
+        self,
+        config_id: int,
+        seed: int,
+        budget: Optional[Union[int, float]] = None,
+    ) -> Status:
         """
-        Returns the status of a configuration.
+        Return the status of a trial (i.e. configuration, budget and seed).
 
         Parameters
         ----------
         config_id : int
             Configuration id to get the status for.
-        budget : Optional[Union[int, float]], optional
-            Budget to get the status from the configuration id for. By default None. If budget is
-            None, the highest budget is chosen.
-
-        Raises
-        ------
-        ValueError
-            If the configuration id is not found.
+        seed : Optional[int]
+            Seed to get the status from the configuration id for.
+        budget : Optional[Union[int, float]]
+            Budget to get the status from the configuration id for. If budget is
+            None, the highest budget is chosen. By default None.
 
         Returns
         -------
         Status
             Status of the configuration.
+
+        Raises
+        ------
+        ValueError
+            If the configuration id is not found.
         """
         if budget == COMBINED_BUDGET:
             return Status.NOT_EVALUATED
 
         if budget is None:
             budget = self.get_highest_budget()
 
         if config_id not in self.configs:
             raise ValueError("Configuration id was not found.")
 
-        trial_key = self.get_trial_key(config_id, budget)
+        trial_key = self.get_trial_key(config_id, budget, seed)
 
-        # Unfortunately, we have to iterate through the history to find the status
+        # Unfortunately, it is necessary to iterate through the history to find the status
         # TODO: Cache the stati
         for trial in self.history:
             if trial_key == trial.get_key():
                 return trial.status
 
         return Status.NOT_EVALUATED
 
     def get_incumbent(
         self,
         objectives: Optional[Union[Objective, List[Objective]]] = None,
         budget: Optional[Union[int, float]] = None,
+        seed: Optional[int] = None,
         statuses: Optional[Union[Status, List[Status]]] = None,
+        selected_ids: Optional[List[int]] = None,
     ) -> Tuple[Configuration, float]:
         """
-        Returns the incumbent with its normalized cost.
+        Return the incumbent with its normalized objective value.
+
+        The incumbent is the configuration with the lowest normalized objective value.
+
+        Optionally, only configurations which were evaluated on the passed budget, seed,
+        and stati are considered.
 
         Parameters
         ----------
         objectives : Optional[Union[Objective, List[Objective]]], optional
-            Considerd objectives. By default None. If None, all objectives are considered.
+            Considered objectives. If None, all objectives are considered. By default None.
         budget : Optional[Union[int, float]], optional
-            Considered budget. By default None. If None, the highest budget is chosen.
+            Considered budget. If None, the highest budget is chosen. By default None.
+        seed : Optional[int], optional
+            Considered seed. If no seed is given, all seeds are considered. By default None.
         statuses : Optional[Union[Status, List[Status]]], optional
-            Considered statuses. By default None. If None, all stati are considered.
+            Considered stati. If None, all stati are considered. By default None.
+        selected_ids: Optional[List[int]], optional
+            If set, only ids in selected_ids will be considered. This can for example be
+            useful if only ids up to a certain end-time shall be considered. By default None.
 
         Returns
         -------
         Tuple[Configuration, float]
             Incumbent with its normalized cost.
 
         Raises
         ------
         RuntimeError
             If no incumbent was found.
         """
-        min_cost = np.inf
+        if isinstance(objectives, Objective):
+            single_objective = objectives
+        elif isinstance(objectives, list) and len(objectives) == 1:
+            single_objective = objectives[0]
+        else:
+            single_objective = None
+
+        if single_objective is not None and single_objective.optimize == "upper":
+            best_cost = -np.inf
+        else:
+            best_cost = np.inf
         best_config_id = None
 
-        results = self.get_all_costs(budget, statuses)
-        for config_id, costs in results.items():
-            cost = self.merge_costs(costs, objectives)
-
-            if cost < min_cost:
-                min_cost = cost
-                best_config_id = config_id
+        results = self.get_all_costs(
+            budget=budget, statuses=statuses, seed=seed, selected_ids=selected_ids
+        )
+
+        if len(results) == 0:
+            raise RuntimeError("No data available, thus no incumbent found.")
+
+        seed_count = {}
+        for config_id, seed_costs_dict in results.items():
+            seed_count[config_id] = len(seed_costs_dict)
+        max_seed_count = max(seed_count.values())
+
+        for config_id, seed_costs_dict in results.items():
+            # If there are multiple seeds, only configurations evaluated on all seeds are
+            # considered. From these configurations, the one with the highest average objective
+            # value over the seeds is considered as the incumbent.
+            if max_seed_count > 1:
+                if len(seed_costs_dict) < max_seed_count:
+                    continue
+
+                # Get average over all seeds
+                config_costs = np.zeros([max_seed_count, len(self.get_objectives())])
+                for i, (_, seed_costs) in enumerate(seed_costs_dict.items()):
+                    config_costs[i] = seed_costs
+                avg_cost = np.mean(config_costs, axis=0)
+
+            # If there is only one seed, the costs can be used directly
+            else:
+                avg_cost = [*seed_costs_dict.values()][0]
+
+            # If there are multiple objectives, the costs are merged to one cost value
+            if single_objective is None:
+                cost = self.merge_costs(avg_cost, objectives)
+            else:
+                cost = avg_cost[self.get_objective_id(single_objective)]
+
+            if cost is None:
+                continue
+
+            if single_objective is not None and single_objective.optimize == "upper":
+                if cost > best_cost:
+                    best_cost = cost
+                    best_config_id = config_id
+            else:
+                if cost < best_cost:
+                    best_cost = cost
+                    best_config_id = config_id
 
         if best_config_id is None:
             raise RuntimeError("No incumbent found.")
 
         config = self.get_config(best_config_id)
         config = Configuration(self.configspace, config)
-        normalized_cost = min_cost
+        normalized_cost = best_cost
 
         return config, normalized_cost
 
     def merge_costs(
         self, costs: List[float], objectives: Optional[Union[Objective, List[Objective]]] = None
     ) -> float:
         """
-        Calculates one cost value from multiple costs.
-        Normalizes the costs first and weight every cost the same.
+        Calculate one cost value from multiple costs.
+
+        Normalizes the costs first and weigh every cost the same.
         The lower the normalized cost, the better.
 
         Parameters
         ----------
         costs : List[float]
-            The costs, which should be merged. Must be the same length as the original number of objectives.
-        objectives : Optional[List[Objective]], optional
+            The costs, which should be merged. Must be the same length as the original number of
+            objectives.
+        objectives : Optional[List[Objective]]
             The considered objectives to the costs. By default None.
             If None, all objectives are considered. The passed objectives can differ from the
             original number objectives.
 
         Returns
         -------
         float
             Merged costs.
+
+        Raises
+        ------
+        RuntimeError
+            If the number of costs is different from the original number of objectives.
+            If the objective was not found.
         """
         # Get rid of NaN values
         costs = self._process_costs(costs)
 
         if objectives is None:
             objectives = self.get_objectives()
 
@@ -589,133 +1031,155 @@
             assert objective.lower != np.inf
             assert objective.upper != -np.inf
 
             a = cost - objective.lower
             b = objective.upper - objective.lower
             normalized_cost = a / b
 
-            # We optimize the lower
-            # So we need to flip the normalized cost
+            # The lower is optimized
+            # So the normalized cost needs to be flipped
             if objective.optimize == "upper":
                 normalized_cost = 1 - normalized_cost
 
             normalized_costs.append(normalized_cost)
             filtered_objectives.append(objective)
 
         # Give the same weight to all objectives (for now)
         objective_weights = [1 / len(objectives) for _ in range(len(objectives))]
 
         costs = [u * v for u, v in zip(normalized_costs, objective_weights)]
         cost = np.mean(costs).item()
 
         return cost
 
-    def get_model(self, config_id: int) -> Optional["torch.nn.Module"]:
+    def get_model(self, config_id: int) -> Optional["torch.nn.Module"]:  # type: ignore # noqa: F821
+        """
+        Get a model associated with the configuration id.
+
+        Parameters
+        ----------
+        config_id : int
+            The configuration id.
+
+        Returns
+        -------
+        Optional["torch.nn.Module]
+            A model for the provided configuration id.
+        """
         import torch
 
-        filename = self.models_dir / f"{str(config_id)}.pth"
+        filename = self.models_dir / f"{str(config_id)}.pth"  # type: ignore
         if not filename.exists():
             return None
 
         return torch.load(filename)
 
     def get_trajectory(
-        self, objective: Objective, budget: Optional[Union[int, float]] = None
+        self,
+        objective: Objective,
+        budget: Optional[Union[int, float]] = None,
+        seed: Optional[int] = None,
     ) -> Tuple[List[float], List[float], List[float], List[int], List[int]]:
         """
-        Calculates the trajectory of the given objective and budget.
+        Calculate the trajectory of the given objective, budget, and seed.
 
         Parameters
         ----------
         objective : Objective
             Objective to calculate the trajectory for.
-        budget : Optional[Union[int, float]], optional
+        budget : Optional[Union[int, float]]
             Budget to calculate the trajectory for. If no budget is given, then the highest budget
             is chosen. By default None.
+        seed : Optional[int], optional
+            Seed to calculate the trajectory for. If no seed is given, then all seeds are
+            considered. By default None.
 
         Returns
         -------
-        times : List[float]
-            Times of the trajectory.
-        costs_mean : List[float]
-            Costs of the trajectory.
-        costs_std : List[float]
-            Standard deviation of the costs of the trajectory. This is particularly useful for
-            grouped runs.
-        ids : List[int]
-            The "global" ids of the selected trials.
-        config_ids : List[int]
-            Config ids of the selected trials.
+        Tuple[List[float], List[float], List[float], List[int], List[int]]
+            times : List[float]
+                Times of the trajectory.
+            costs_mean : List[float]
+                Costs of the trajectory.
+            costs_std : List[float]
+                Standard deviation of the costs of the trajectory. This is particularly useful for
+                grouped runs.
+            ids : List[int]
+                The "global" ids of the selected trials.
+            config_ids : List[int]
+                Config ids of the selected trials.
         """
         if budget is None:
             budget = self.get_highest_budget()
 
-        objective_id = self.get_objective_id(objective)
-
         costs_mean = []
         costs_std = []
         ids = []
         config_ids = []
         times = []
 
         order = []
-        # Sort self.history by end_time
+
+        # Sort self.history by end-time
         for id, trial in enumerate(self.history):
             order.append((id, trial.end_time))
-
         order.sort(key=lambda tup: tup[1])
 
         # Important: Objective can be minimized or maximized
         if objective.optimize == "lower":
             current_cost = np.inf
         else:
             current_cost = -np.inf
 
-        for id, _ in order:
+        # Iterate over the history ordered by end-time and calculate the current incumbent
+        for i, (id, _) in enumerate(order):
             trial = self.history[id]
 
-            # We want to use all budgets
-            if budget != COMBINED_BUDGET:
-                # Only consider selected/last budget
-                if trial.budget != budget:
-                    continue
-
-            cost = trial.costs[objective_id]
-            if cost is None:
+            # Get the incumbent over all trials up to this point
+            try:
+                _, cost = self.get_incumbent(
+                    objectives=objective,
+                    budget=budget,
+                    seed=seed,
+                    selected_ids=[selected_id for selected_id, _ in order[: i + 1]],
+                )
+            except RuntimeError:
                 continue
 
             # Now it's important to check whether the cost was minimized or maximized
             if objective.optimize == "lower":
                 improvement = cost < current_cost
             else:
                 improvement = cost > current_cost
 
             if improvement:
                 current_cost = cost
 
                 costs_mean.append(cost)
-                costs_std.append(0)
+                costs_std.append(0.0)
                 times.append(trial.end_time)
                 ids.append(id)
                 config_ids.append(trial.config_id)
 
         return times, costs_mean, costs_std, ids, config_ids
 
     def encode_config(
         self, config: Union[int, Dict[Any, Any], Configuration], specific: bool = False
     ) -> List:
         """
-        Encodes a given config (id) to a normalized list.
-        If a config is passed, no look-up has to be done.
+        Encode a given configuration (id) to a normalized list.
+
+        If a configuration is passed, no look-up has to be done.
 
         Parameters
         ----------
         config : Union[int, Dict[Any, Any], Configuration]
-            Either the config id, config as dict, or Configuration itself.
-        specific : bool, optional
+            Either the configuration id, as configuration as dict,
+            or a Configuration itself.
+        specific : bool
             Use specific encoding for fanova tree, by default False.
 
         Returns
         -------
         List
             The encoded config as list.
         """
@@ -744,104 +1208,121 @@
                 value = CONSTANT_VALUE
 
             x += [value]
 
         return x
 
     def encode_configs(self, configs: List[Configuration]) -> np.ndarray:
-        X = []
+        """
+        Encode a list of configurations into a corresponding numpy array.
+
+        Parameters
+        ----------
+        configs : List[Configuration]
+            A list containing the configurations to be encoded.
+
+        Returns
+        -------
+        np.ndarray
+            A numpy array with the encoded configurations.
+        """
+        x_set = []
         for config in configs:
             x = self.encode_config(config)
-            X.append(x)
+            x_set.append(x)
 
-        return np.array(X)
+        return np.array(x_set)
 
     def get_encoded_data(
         self,
         objectives: Optional[Union[Objective, List[Objective]]] = None,
         budget: Optional[Union[int, float]] = None,
+        seed: Optional[int] = None,
         statuses: Optional[Union[Status, List[Status]]] = None,
         specific: bool = False,
         include_config_ids: bool = False,
         include_combined_cost: bool = False,
-    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    ) -> pd.DataFrame:
         """
-        Encodes configurations to process them further. After the configurations are encoded,
+        Encode configurations to process them further.
+
+        After the configurations are encoded,
         they can be used in model prediction.
 
         Parameters
         ----------
-        objectives : Optional[Union[Objective, List[Objective]]], optional
-            Which objectives should be considered. If None, all objectives are
-            considered. By default None.
-        budget : Optional[List[Status]], optional
-            Which budget should be considered. By default None. If None, only the highest budget
-            is considered.
-        statuses : Optional[Union[Status, List[Status]]], optional
-            Which statuses should be considered. By default None. If None, all statuses are
-            considered.
-        encode_y : bool, optional
-            Whether y should be normalized too. By default False.
-        specific : bool, optional
+        objectives : Optional[Union[Objective, List[Objective]]]
+            Which objectives should be considered. If None, all objectives are considered.
+            By default None.
+        budget : Optional[List[Status]]
+            Which budget should be considered. If None, only the highest budget is considered.
+            By default None.
+        seed: Optional[int]
+            Which seed should be considered. If None, all seeds are considered.
+            By default None.
+        statuses : Optional[Union[Status, List[Status]]]
+            Which stati should be considered. If None, all stati are considered.
+            By default None.
+        specific : bool
             Whether a specific encoding should be used. This encoding is compatible with pyrfr.
             A wrapper for pyrfr is implemented in ``deepcave.evaluators.epm``.
             By default False.
-        include_config_ids : bool, optional
-            Whether to include config ids. By default False.
+        include_config_ids : bool
+            Whether to include configuration ids. By default False.
         include_combined_cost : bool, optional
             Whether to include combined cost. Note that the combined cost is calculated by the
             passed objectives only. By default False.
 
         Returns
         -------
         df : pd.DataFrame
             Encoded dataframe with the following columns (depending on the parameters):
             [CONFIG_ID, HP1, HP2, ..., HPn, OBJ1, OBJ2, ..., OBJm, COMBINED_COST]
 
         Raises
         ------
         ValueError
-            If a hyperparameter is not supported.
+            If a hyperparameter (HP) is not supported.
         """
-
         if objectives is None:
             objectives = self.get_objectives()
 
         if isinstance(objectives, Objective):
             objectives = [objectives]
 
-        X, Y = [], []
+        x_set, y_set = [], []
         config_ids = []
 
-        results = self.get_all_costs(budget, statuses)
-        for config_id, costs in results.items():
+        results = self.get_all_costs(budget, statuses, seed)
+        for config_id, config_costs in results.items():
             config = self.configs[config_id]
-            x = self.encode_config(config, specific=specific)
-            y = []
-
-            # Add all objectives
-            for objective in objectives:
-                objective_id = self.get_objective_id(objective)
-                y += [costs[objective_id]]
-
-            # Add combined cost
-            if include_combined_cost:
-                y += [self.merge_costs(costs, objectives)]
-
-            X.append(x)
-            Y.append(y)
-            config_ids.append(config_id)
-
-        X = np.array(X)  # type: ignore
-        Y = np.array(Y)  # type: ignore
-        config_ids = np.array(config_ids).reshape(-1, 1)  # type: ignore
+            for seed, costs in config_costs.items():
+                x = self.encode_config(config, specific=specific)
+                y = []
+
+                # Add all objectives
+                for objective in objectives:
+                    objective_id = self.get_objective_id(objective)
+                    y += [costs[objective_id]]
+
+                # Add combined cost
+                if include_combined_cost:
+                    y += [self.merge_costs(costs, objectives)]
+
+                x_set.append(x)
+                y_set.append(y)
+                config_ids.append(config_id)
+
+        x_set_array = np.array(x_set)
+        y_set_array = np.array(y_set)
+        config_ids_array = np.array(config_ids).reshape(-1, 1)
 
         # Imputation: Easiest case is to replace all nans with -1
-        # However, since Stefan used different values for inactives
-        # we also have to use different inactives to be compatible
+        # However, since Stefan used different values for inactive hyperparameters,
+        # Also different inactive hyperparameters have to be used, to be compatible
         # with the random forests.
         # https://github.com/automl/SMAC3/blob/a0c89502f240c1205f83983c8f7c904902ba416d/smac/epm/base_rf.py#L45
         if specific:
             conditional = {}
             impute_values = {}
 
             for idx, hp in enumerate(self.configspace.get_hyperparameters()):
@@ -860,131 +1341,167 @@
                             impute_values[idx] = -1
                         elif isinstance(hp, Constant):
                             impute_values[idx] = 1
                         else:
                             raise ValueError("Hyperparameter not supported.")
 
                 if conditional[idx] is True:
-                    nonfinite_mask = ~np.isfinite(X[:, idx])
-                    X[nonfinite_mask, idx] = impute_values[idx]
+                    non_finite_mask = ~np.isfinite(x_set_array[:, idx])
+                    x_set_array[non_finite_mask, idx] = impute_values[idx]
 
-        # Now we create dataframes for both values and labels
+        # Now dataframes are created for both values and labels
         # [CONFIG_ID, HP1, HP2, ..., HPn, OBJ1, OBJ2, ..., OBJm, COMBINED_COST]
         if include_config_ids:
             columns = ["config_id"]
         else:
             columns = []
 
         columns += [name for name in self.configspace.get_hyperparameter_names()]
         columns += [objective.name for objective in objectives]
 
         if include_combined_cost:
             columns += [COMBINED_COST_NAME]
 
         if include_config_ids:
-            data = np.concatenate((config_ids, X, Y), axis=1)
+            data: np.ndarray = np.concatenate((config_ids_array, x_set_array, y_set_array), axis=1)
         else:
-            data = np.concatenate((X, Y), axis=1)
+            data = np.concatenate((x_set_array, y_set_array), axis=1)
 
         data = pd.DataFrame(data=data, columns=columns)
 
         return data
 
 
 def check_equality(
     runs: List[AbstractRun],
     meta: bool = False,
     configspace: bool = True,
     objectives: bool = True,
     budgets: bool = True,
+    seeds: bool = False,
 ) -> Dict[str, Any]:
     """
-    Checks the passed runs on equality based on the selected runs and returns the requested
-    attributes.
+    Check the passed runs on equality based on the selected runs.
+
+    Return the requested attributes.
 
     Parameters
     ----------
     runs : list[AbstractRun]
         Runs to check for equality.
     meta : bool, optional
-        Meta-Data excluding objectives and budgets, by default True
+        Meta-Data excluding objectives and budgets, by default False.
     configspace : bool, optional
-        ConfigSpace, by default True
+        Wheter to include the configuration space, by default True.
     objectives : bool, optional
-        Objectives, by default True
+        Wheter to include the objectives, by default True.
     budgets : bool, optional
-        Budgets, by default True
+        Whether to include the budgets, by default True.
+    seeds : bool, optional
+        Whether to include the seeds, by default False.
 
     Returns
     -------
     Dict[str, Any]
         Dictionary containing the checked attributes.
+
+    Raises
+    ------
+    NotMergeableError
+        If the meta data of the runs are not equal.
+        If the configuration spaces of the runs are not equal.
+        If the budgets of the runs are not equal.
+        If the objective of the runs are not equal.
     """
-    result = {}
+    result: Dict[str, Any] = {}
 
     if len(runs) == 0:
         return result
 
-    # Check meta
-    if meta:
-        ignore = ["objectives", "budgets", "wallclock_limit"]
-
-        m1 = runs[0].get_meta()
+    # Check if objectives are mergeable
+    if objectives:
+        o1 = None
         for run in runs:
-            m2 = run.get_meta()
-
-            for k, v in m1.items():
-                # Don't check on objectives or budgets
-                if k in ignore:
-                    continue
+            o2 = run.get_objectives()
 
-                if k not in m2 or m2[k] != v:
-                    raise NotMergeableError("Meta data of runs are not equal.")
+            if o1 is None:
+                o1 = o2
+                continue
 
-        result["meta"] = m1
+            if len(o1) != len(o2):
+                raise NotMergeableError(
+                    "Objectives of runs are not equal.", RunInequality.INEQ_OBJECTIVE
+                )
 
-    # Make sure the same configspace is used
-    # Otherwise it does not make sense to merge
-    # the histories
-    if configspace:
-        cs1 = runs[0].configspace
-        for run in runs:
-            cs2 = run.configspace
-            if cs1 != cs2:
-                raise NotMergeableError("Configspace of runs are not equal.")
+            for o1_, o2_ in zip(o1, o2):
+                try:
+                    o1_.merge(o2_)
+                except NotMergeableError:
+                    raise NotMergeableError(
+                        "Objectives of runs are not equal.", RunInequality.INEQ_OBJECTIVE
+                    )
 
-        result["configspace"] = cs1
+        assert o1 is not None
+        serialized_objectives = [o.to_json() for o in o1]
+        result["objectives"] = serialized_objectives
+        if meta:
+            result["meta"]["objectives"] = serialized_objectives
 
     # Also check if budgets are the same
     if budgets:
         b1 = runs[0].get_budgets(include_combined=False)
         for run in runs:
             b2 = run.get_budgets(include_combined=False)
             if b1 != b2:
-                raise NotMergeableError("Budgets of runs are not equal.")
+                raise NotMergeableError("Budgets of runs are not equal.", RunInequality.INEQ_BUDGET)
 
         result["budgets"] = b1
         if meta:
             result["meta"]["budgets"] = b1
 
-    # And if objectives are the same
-    if objectives:
-        o1 = None
+    # Make sure the same configspace is used
+    # Otherwise it does not make sense to merge
+    # the histories
+    if configspace:
+        cs1 = runs[0].configspace
         for run in runs:
-            o2 = run.get_objectives()
+            cs2 = run.configspace
+            if cs1 != cs2:
+                raise NotMergeableError(
+                    "Configspace of runs are not equal.", RunInequality.INEQ_CONFIGSPACE
+                )
 
-            if o1 is None:
-                o1 = o2
-                continue
+        result["configspace"] = cs1
 
-            if len(o1) != len(o2):
-                raise NotMergeableError("Objectives of runs are not equal.")
+    # Check meta
+    if meta:
+        ignore = ["objectives", "budgets", "wallclock_limit"]
 
-            for o1_, o2_ in zip(o1, o2):
-                o1_.merge(o2_)
+        m1 = runs[0].get_meta()
+        for run in runs:
+            m2 = run.get_meta()
 
-        serialized_objectives = [o.to_json() for o in o1]
-        result["objectives"] = serialized_objectives
+            for k, v in m1.items():
+                # Don't check on objectives or budgets
+                if k in ignore:
+                    continue
+
+                if k not in m2 or m2[k] != v:
+                    raise NotMergeableError(
+                        "Meta data of runs are not equal.", RunInequality.INEQ_META
+                    )
+
+        result["meta"] = m1
+
+    # Check if seeds are the same
+    if seeds:
+        s1 = runs[0].get_seeds(include_combined=False)
+        for run in runs:
+            s2 = run.get_seeds(include_combined=False)
+            if s1 != s2:
+                raise NotMergeableError("Seeds of runs are not equal.", RunInequality.INEQ_SEED)
+
+        result["seeds"] = s1
         if meta:
-            result["meta"]["objectives"] = serialized_objectives
+            result["meta"]["seeds"] = s1
 
     return result
```

### Comparing `deepcave-1.1.3/deepcave/runs/converters/smac3v1.py` & `deepcave-1.2/deepcave/runs/converters/smac3v1.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,110 @@
+#  noqa: D400
+"""
+# SMAC3v1Run
+
+This module provides utilities to create a SMAC3v1
+(Sequential Model-based Algorithm Configuration) run.
+
+Version 1.4 is used.
+
+## Classes
+    - SMAC3v1Run: Define a SMAC3v1 run object.
+"""
+from typing import Optional, Union
+
 import json
 from pathlib import Path
 
 import numpy as np
 
 from deepcave.runs import Status
 from deepcave.runs.objective import Objective
 from deepcave.runs.run import Run
 from deepcave.utils.hash import file_to_hash
 
 
 class SMAC3v1Run(Run):
+    """
+    Define a SMAC3v1 (Sequential Model-based Algorithm Configuration) run object.
+
+    Version 1.4 is used.
+
+    Properties
+    ----------
+    path : Path
+        The path to the run.
+    """
+
     prefix = "SMAC3v1"
     _initial_order = 2
 
     @property
-    def hash(self):
+    def hash(self) -> str:
+        """
+        Hash of the current run.
+
+        If the hash changes, the cache has to be cleared.
+        This ensures that the cache always holds the latest results of the run.
+
+        Returns
+        -------
+        str
+            The hash of the run.
+        """
         if self.path is None:
             return ""
 
         # Use hash of history.json as id
         return file_to_hash(self.path / "runhistory.json")
 
     @property
-    def latest_change(self):
+    def latest_change(self) -> Union[float, int]:
+        """
+        Get the timestamp of the latest change.
+
+        Returns
+        -------
+        Union[float, int]
+            The latest change.
+        """
         if self.path is None:
             return 0
 
         return Path(self.path / "runhistory.json").stat().st_mtime
 
     @classmethod
-    def from_path(cls, path):
+    def from_path(cls, path: Union[Path, str]) -> "SMAC3v1Run":
         """
         Based on working_dir/run_name/*, return a new trials object.
+
+        Parameters
+        ----------
+        path : Union[Path, str]
+            The path to base the run on.
+
+        Returns
+        -------
+        A SMAC3v1 run.
+
+        Raises
+        ------
+        RuntimeError
+            Instances are not supported.
         """
         path = Path(path)
 
         # Read configspace
         from ConfigSpace.read_and_write import json as cs_json
 
         with (path / "configspace.json").open("r") as f:
             configspace = cs_json.read(f.read())
 
         # Read objectives
-        # We have to define it ourselves, because we don't know the type of the objective
+        # It has to be defined here, because the type of the objective is not known
         # Only lock lower
         objective1 = Objective("Cost", lower=0)
         objective2 = Objective("Time", lower=0)
 
         # Read meta
         # Everything else is ignored
         ignore = ["train_inst_fn", "pcs_fn", "execdir"]
@@ -65,28 +123,27 @@
                     meta[arg] = value
 
         # Let's create a new run object
         run = SMAC3v1Run(
             name=path.stem, configspace=configspace, objectives=[objective1, objective2], meta=meta
         )
 
-        # We have to set the path manually
+        # The path has to be set manually
         run._path = path
 
         # Iterate over the runhistory
         with (path / "runhistory.json").open() as json_file:
             all_data = json.load(json_file)
             data = all_data["data"]
             config_origins = all_data["config_origins"]
             configs = all_data["configs"]
 
         instance_ids = []
 
         first_starttime = None
-        seeds = []
         for (config_id, instance_id, seed, budget), (
             cost,
             time,
             status,
             starttime,
             endtime,
             additional_info,
@@ -96,20 +153,14 @@
 
             if len(instance_ids) > 1:
                 raise RuntimeError("Instances are not supported.")
 
             config_id = str(config_id)
             config = configs[config_id]
 
-            if seed not in seeds:
-                seeds.append(seed)
-
-            if len(seeds) > 1:
-                raise RuntimeError("Multiple seeds are not supported.")
-
             if first_starttime is None:
                 first_starttime = starttime
 
             starttime = starttime - first_starttime
             endtime = endtime - first_starttime
 
             status = status["__enum__"]
@@ -124,31 +175,32 @@
                 status = Status.MEMORYOUT
             elif "RUNNING" in status:
                 continue
             else:
                 status = Status.CRASHED
 
             if status != Status.SUCCESS:
-                # We don't want cost included which are failed
+                # Costs which failed, should not be included
                 cost = None
                 time = None
             else:
                 time = endtime - starttime
 
             # Round budget
             budget = np.round(budget, 2)
 
-            origin = None
+            origin: Optional[str] = None
             if config_id in config_origins:
                 origin = config_origins[config_id]
 
             run.add(
                 costs=[cost, time],
                 config=config,
                 budget=budget,
+                seed=seed,
                 start_time=starttime,
                 end_time=endtime,
                 status=status,
                 origin=origin,
                 additional=additional_info,
             )
```

### Comparing `deepcave-1.1.3/deepcave/runs/handler.py` & `deepcave-1.2/deepcave/runs/handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,60 @@
+#  noqa: D400
+"""
+# Handler
+
+This module provides utilities to handle a run.
+
+It can retrieve working directories, run paths, run names, as well as groups of runs.
+It provides utilities to update and remove runs as well as groups of runs.
+
+# Classes
+    - RunHandler: Handle the runs.
+"""
+
 from typing import Dict, List, Optional, Type, Union
 
-import logging
 import time
 from pathlib import Path
 
 from deepcave.config import Config
 from deepcave.runs import AbstractRun
 from deepcave.runs.group import Group
 from deepcave.runs.run import Run
+from deepcave.utils.cache import Cache
 from deepcave.utils.logs import get_logger
+from deepcave.utils.run_caches import RunCaches
 
 
 class RunHandler:
     """
-    Handles the runs. Based on the meta data in the cache, automatically selects the right converter
+    Handle the runs.
+
+    Based on the meta data in the cache, automatically selects the right converter
     and switches to the right (plugin) cache.
+
+    Provides utilities to retrieve working directories, run paths, run names, and groups of runs.
+    Also update and remove runs as well a groups of runs.
+
+    Properties
+    ----------
+    c : Cache
+        The cache containing information about a run(s).
+    rc : RunCaches
+        The caches for the selected runs.
+    logger : Logger
+        The logger for the run handler.
+    available_run_yfes : List[Type[Run]]
+        A list of the available converters.
+    runs : Dict[str, AbstractRun]
+        A dictionary of runs with their path as key.
+    groups : Dict[str, Group]
+        A dictionary of the groups.
+    available_run_classes : List[Type[Run]]
+        Contains the available run classes.
     """
 
     def __init__(self, config: Config, cache: "Cache", run_cache: "RunCaches") -> None:
         self.c = cache
         self.rc = run_cache
         # Fields set by self.update()
         self.logger = get_logger("RunHandler")
@@ -33,42 +69,55 @@
         # Read from cache and update
         self.c.read()
         self.update_runs()
         self.update_groups()
 
     def set_working_directory(self, working_directory: Union[Path, str]) -> None:
         """
-        Sets the working directoy to the meta cache.
+        Set the working directory to the meta cache.
 
         Parameters
         ----------
         working_directory : Union[Path, str]
             Directory to be set.
         """
         self.c.set("working_dir", value=str(working_directory))
 
     def get_working_directory(self) -> Path:
         """
-        Returns the current working directory in the cache.
+        Return the current working directory in the cache.
 
         Returns
         -------
         Path
             Path of the working directory.
+
+        Raises
+        ------
+        AssertionError
+            If the working directory is not a string or a Path, an error is thrown.
         """
-        return Path(self.c.get("working_dir"))
+        working_dir = self.c.get("working_dir")
+        assert isinstance(
+            working_dir, (str, Path)
+        ), "Working directory of cache must be a string or a Path like."
+        return Path(working_dir)
 
     def get_available_run_paths(self) -> Dict[str, str]:
         """
-        Returns the available run paths from the current directory.
+        Return the available run paths from the current directory.
 
         Returns
         -------
         Dict[str, str]
             Run path as key and run name as value.
+
+        Exceptions
+        ----------
+        FileNotFoundError
         """
         runs = {}
         working_dir = self.get_working_directory()
 
         try:
             for path in working_dir.iterdir():
                 run_name = path.stem
@@ -85,56 +134,84 @@
         except FileNotFoundError:
             pass
 
         return runs
 
     def get_selected_run_paths(self) -> List[str]:
         """
-        Returns the selected run paths from the cache.
+        Return the selected run paths from the cache.
 
         Returns
         -------
-        Dict[str, str]
+        List[str]
             Run paths as a list.
+
+        Raises
+        ------
+        AssertionError.
+            If the selected run paths are not a list, an error is thrown.
         """
-        return self.c.get("selected_run_paths")
+        selected_run_paths = self.c.get("selected_run_paths")
+        assert isinstance(
+            selected_run_paths, list
+        ), "The selected run paths of the cache must be a list."
+        return selected_run_paths
 
     def get_selected_run_names(self) -> List[str]:
         """
-        Returns the run names of the selected runs.
+        Return the run names of the selected runs.
 
         Returns
         -------
         List[str]
             List of run names of the selected runs.
         """
         return [self.get_run_name(run_path) for run_path in self.runs.keys()]
 
     def get_run_name(self, run_path: Union[Path, str]) -> str:
         """
-        Returns the stem of the path.
+        Return the stem of the path.
 
         Parameters
         ----------
         run_path : Union[Path, str]
             Path, which should be converted to a name.
 
         Returns
         -------
         str
             Run name of the path.
         """
         return Path(run_path).stem
 
     def get_selected_groups(self) -> Dict[str, List[str]]:
-        return self.c.get("groups")
+        """
+        Get the selected groups.
+
+        Returns
+        -------
+        Dict[str, List[str]]
+            Dictionary with the selected groups.
+
+        Raises
+        ------
+        AssertionError
+            If groups in cache is not a dictionary, an error is thrown.
+        """
+        selected_groups = self.c.get("groups")
+        assert isinstance(
+            selected_groups, dict
+        ), "The groups aquired from the cache must be a dictionary."
+        return selected_groups
 
     def add_run(self, run_path: str) -> bool:
         """
-        Adds a run path to the cache. If run path is already in cache, do nothing.
+        Add a run path to the cache.
+
+        If run path is already in cache, do nothing.
 
         Parameters
         ----------
         run_path : str
             Path of a run.
 
         Returns
@@ -149,44 +226,57 @@
             self.c.set("selected_run_paths", value=selected_run_paths)
 
             return self.update_runs()
 
         return True
 
     def remove_run(self, run_path: str) -> None:
-        """Removes a run path from the cache. If run path is not in cache, do nothing.
+        """
+        Remove a run path from the cache.
+
+        If run path is not in cache, do nothing.
 
         Parameters
         ----------
         run_path : str
             Path of a run.
+
+        Raises
+        ------
+        TypeError
+            If `selected_run_paths` or `groups` is None, an error is thrown.
         """
         selected_run_paths = self.c.get("selected_run_paths")
 
+        if selected_run_paths is None:
+            raise TypeError("Selected run paths can not be None.")
+
         if run_path in selected_run_paths:
             selected_run_paths.remove(run_path)
             self.c.set("selected_run_paths", value=selected_run_paths)
 
-            # We have to check the groups here because the removed run_path may
+            # The groups have to be checked here because the removed run_path may
             # still be included
             groups = {}
-            for group_name, run_paths in self.c.get("groups").items():
+            group_it = self.c.get("groups")
+            if group_it is None:
+                raise TypeError("Groups can not be None.")
+            for group_name, run_paths in group_it.items():
                 if run_path in run_paths:
                     run_paths.remove(run_path)
                 groups[group_name] = run_paths
 
             self.c.set("groups", value=groups)
 
-            # We also remove last inputs here
+            # Last inputs are also removed here
             self.c.set("last_inputs", value={})
             self.update_runs()
 
     def update(self) -> None:
-        """Updates the internal run and group instances but only if a hash changed."""
-
+        """Update the internal run and group instances but only if a hash changed."""
         update_required = False
         for run_path in list(self.runs.keys()):
             run = self.runs[run_path]
 
             # Get cache
             if self.rc.update(run):
                 # It's important to delete the run from self.runs here because
@@ -197,25 +287,25 @@
 
         if update_required:
             self.update_runs()
             self.update_groups()
 
     def update_runs(self) -> bool:
         """
-        Loads selected runs and update cache if files changed.
-
-        Raises
-        ------
-        NotValidRunError
-            If directory can not be transformed into a run, an error is thrown.
+        Load selected runs and update cache if files changed.
 
         Returns
         -------
         bool
             True if all selected runs could be loaded, False otherwise.
+
+        Raises
+        ------
+        NotValidRunError
+            If directory can not be transformed into a run, an error is thrown.
         """
         runs: Dict[str, AbstractRun] = {}  # run_path: Run
         success = True
 
         class_hint = None
         updated_paths = []
         for run_path in self.get_selected_run_paths():
@@ -236,23 +326,34 @@
 
         return success
 
     def update_run(
         self, run_path: str, class_hint: Optional[Type[Run]] = None
     ) -> Optional[AbstractRun]:
         """
-        Loads the run from `self.runs` or creates a new one.
+        Load the run from `self.runs` or create a new one.
+
+        Parameters
+        ----------
+        run_path : str
+            The path of the run.
+        class_hint : Optional[Type[Run]], optional
+            A hint/suggestion of what the Type of the Run is.
+            Default is None.
+
+        Returns
+        -------
+        Optional[AbstractRun]
+            The Run added to the cache.
 
         Raises
         ------
         NotValidRunError
             If directory can not be transformed into a run, an error is thrown.
-
         """
-
         # Try to get run from current runs
         if run_path in self.runs:
             run = self.runs[run_path]
 
             # Create cache file and set name/hash. Clear cache if hash got changed.
             self.rc.update(run)
             return run
@@ -270,15 +371,16 @@
         exceptions = {}
         for run_class in self.available_run_classes:
             try:
                 t1 = time.perf_counter()
                 run = run_class.from_path(Path(run_path))
                 t2 = time.perf_counter()
                 self.logger.debug(
-                    f'Run "{Path(run_path).stem}" was successfully loaded (took {round(t2 - t1, 2)} seconds).'
+                    f'Run "{Path(run_path).stem}" was successfully loaded (took {round(t2 - t1, 2)}'
+                    f" seconds)."
                 )
             except KeyboardInterrupt:
                 # Pass KeyboardInterrupt through try-except, so it can actually interrupt.
                 raise
             except Exception as e:
                 exceptions[run_class] = e
 
@@ -291,29 +393,40 @@
                 self.logger.warning(f"{run_class.prefix}: {exception}.")
         else:
             # Add to run cache
             self.rc.update(run)
 
         return run
 
-    def update_groups(self, groups: Optional[Dict[str, str]] = None) -> None:
+    def update_groups(self, groups: Optional[Dict[str, List[str]]] = None) -> None:
         """
-        Loads chosen groups. If `groups` is passed, it is used to instantiate the groups and
+        Load chosen groups.
+
+        If `groups` is passed, it is used to instantiate the groups and
         saved to the cache. Otherwise, `groups` is loaded from the cache.
 
+        Parameters
+        ----------
+        groups : Optional[Dict[str, str]], optional
+            A dictionary with the groups.
+            Default is None.
+
         Raises
         ------
         NotMergeableError
             If runs can not be merged, an error is thrown.
-
+        TypeError
+            If `groups` is None, an error is thrown.
         """
         instantiated_groups = {}
         if groups is None:
             groups = self.c.get("groups")
-
+        # This check is necessary because groups could still be None
+        if groups is None:
+            raise TypeError("Groups can not be None.")
         # Add grouped runs
         for group_name, run_paths in groups.items():
             runs = []
             for run_path, run in self.runs.items():
                 if run_path in run_paths:
                     runs += [run]
 
@@ -332,25 +445,25 @@
         self.c.set("groups", value=groups)
 
         # Save in memory
         self.groups = instantiated_groups
 
     def get_run(self, run_id: str) -> AbstractRun:
         """
-        Looks inside `self.runs` and `self.groups` and if the run id is found, returns the run.
+        Look inside `self.runs` and `self.groups` and if the run id is found, returns the run.
 
         Parameters
         ----------
         run_id : str
             Internal id of the run. Referred to `run.id`.
 
         Returns
         -------
         AbstractRun
-            Run
+            Run.
 
         Raises
         ------
         RuntimeError
             If `run_id` was not found in `self.runs` or `self.groups`.
         """
         runs = self.get_runs(include_groups=True)
@@ -358,33 +471,35 @@
             if run.id == run_id:
                 return run
 
         raise RuntimeError("Run not found.")
 
     def get_groups(self) -> List[Group]:
         """
-        Returns instantiated grouped runs.
+        Return instantiated grouped runs.
 
         Returns
         -------
         List[GroupedRun]
             Instances of grouped runs.
         """
         self.update()
         return list(self.groups.values())
 
-    def get_runs(self, include_groups=False) -> List[AbstractRun]:
+    def get_runs(self, include_groups: bool = False) -> List[AbstractRun]:
         """
-        Returns the runs from the internal cache. The runs are already loaded and ready to use.
+        Return the runs from the internal cache.
+
+        The runs are already loaded and ready to use.
         Optional, if `include_groups` is set to True, the groups are also included.
 
         Parameters
         ----------
         include_groups : bool, optional
-            Includes the groups, by default False
+            Includes the groups, by default False.
 
         Returns
         -------
         List[AbstractRun]
             Instances of runs.
         """
         self.update()
```

### Comparing `deepcave-1.1.3/deepcave/start.sh` & `deepcave-1.2/deepcave/start.sh`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/deepcave/utils/configs.py` & `deepcave-1.2/deepcave/utils/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+#  noqa: D400
+"""
+# Configs
+
+This module provides a utility for parsing the configurations from a filename.
+"""
+
 from typing import Optional
 
 import importlib
 import os
 import sys
 from pathlib import Path
 
 from deepcave.config import Config
 
 
 def parse_config(filename: Optional[str] = None) -> Config:
     """
-    Parses the config given the filename. Both relative and absolute paths are possible.
+    Parse the config given the filename.
+
+    Both relative and absolute paths are possible.
 
     Parameters
     ----------
     filename : Optional[str], optional
         Location of the config. Must be a python file.
         By default None (default configuration will be used).
 
@@ -45,15 +54,15 @@
                 module_name = p.stem
             else:
                 path = Path(os.getcwd()) / p.parent
 
             script_dir = path.stem  # That's the path without the script name
             module_name = p.stem  # That's the script name without the extension
 
-            # Now we add to sys path
+            # Now it is added to sys path
             sys.path.append(str(path))
 
             module = importlib.import_module(f"{script_dir}.{module_name}")
             config = module.Config()
 
         except Exception:
             raise RuntimeError(f"Could not load class Config from {p}.")
```

### Comparing `deepcave-1.1.3/deepcave/utils/configspace.py` & `deepcave-1.2/deepcave/utils/configspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from typing import Generator, Iterator, List, Optional
+#  noqa: D400
+"""
+# ConfigSpace
 
-import random
-from itertools import islice, product
+This module samples random as well as border configurations.
+"""
+
+from typing import Iterator, Optional
 
 import numpy as np
 from ConfigSpace.configuration_space import Configuration, ConfigurationSpace
 from ConfigSpace.hyperparameters import (
     CategoricalHyperparameter,
     Constant,
     IntegerHyperparameter,
     OrdinalHyperparameter,
 )
 from ConfigSpace.util import deactivate_inactive_hyperparameters
 
 
 def sample_border_config(configspace: ConfigurationSpace) -> Iterator[Configuration]:
     """
-    Generates border configurations from the configuration space.
+    Generate border configurations from the configuration space.
 
     Parameters
     ----------
     configspace : ConfigurationSpace
-        The configspace from which the hyperparameters are drawn from.
+        The configuration space from which the hyperparameters are drawn from.
 
     Yields
     ------
     Iterator[Configuration]
         Border configurations.
     """
     rng = np.random.RandomState(0)
@@ -46,36 +50,36 @@
                 borders = [hp.lower, hp.upper]
 
             # Get a random choice
             value = rng.choice(borders)
             config[hp_name] = value
 
         try:
-            config = deactivate_inactive_hyperparameters(config, configspace)
-            config.is_valid_configuration()
+            configuration = deactivate_inactive_hyperparameters(config, configspace)
+            configuration.is_valid_configuration()
         except Exception:
             continue
 
-        yield config
+        yield configuration
 
 
 def sample_random_config(
     configspace: ConfigurationSpace, d: Optional[int] = None
 ) -> Iterator[Configuration]:
     """
-    Generates random configurations from the configuration space.
+    Generate random configurations from the configuration space.
 
     Parameters
     ----------
     configspace : ConfigurationSpace
         The configspace from which the hyperparameters are drawn from.
     d : Optional[int], optional
         The possible hyperparameter values can be reduced by this argument as the range gets
-        discretized. For example, an integer or float hyperparameter has only four possible values
-        if d=4. By default None (no discretization is done).
+        discretized. For example, an integer or float hyperparameter has only four possible
+        values if d=4. By default, None (no discretization is done).
 
     Yields
     ------
     Iterator[Configuration]
         Random configurations.
     """
     if d is None:
@@ -83,15 +87,15 @@
             yield config
 
         return
 
     rng = np.random.RandomState(0)
 
     while True:
-        config = {}
+        config_dict = {}
 
         # Iterates over the hyperparameters to get considered values
         for hp_name, hp in zip(
             configspace.get_hyperparameter_names(), configspace.get_hyperparameters()
         ):
             if isinstance(hp, CategoricalHyperparameter):
                 values = list(hp.choices)
@@ -113,16 +117,16 @@
                     values = list(np.linspace(hp.lower, hp.upper, d))
 
                 if isinstance(hp, IntegerHyperparameter):
                     values = [int(i) for i in values]
 
             # Get a random choice
             value = rng.choice(values)
-            config[hp_name] = value
+            config_dict[hp_name] = value
 
         try:
-            config = deactivate_inactive_hyperparameters(config, configspace)
-            config.is_valid_configuration()
+            configuration = deactivate_inactive_hyperparameters(config_dict, configspace)
+            configuration.is_valid_configuration()
         except Exception:
             continue
 
-        yield config
+        yield configuration
```

### Comparing `deepcave-1.1.3/deepcave/utils/docs.py` & `deepcave-1.2/deepcave/utils/docs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,34 @@
+#  noqa: D400
+"""
+# Docs
+
+This module provides a function to convert reStructuredText (RST) to MarkDown (MD).
+"""
+
 from __future__ import annotations
 
 import re
 from pathlib import Path
 
 
 def rst_to_md(filename: str | Path) -> str:
+    """
+    Convert a subset of reStructuredText (RST) to MarkDown (MD).
+
+    Parameters
+    ----------
+    filename : str | Path
+        The path to the reStructuredText (RST) file.
+
+    Returns
+    -------
+    str
+        The converted data in MarkDown (MD) format.
+    """
     if isinstance(filename, Path):
         filename = str(filename)
 
     with open(filename, "r") as file:
         data = file.read()
 
     # Remove reference
```

### Comparing `deepcave-1.1.3/deepcave/utils/run_caches.py` & `deepcave-1.2/deepcave/utils/run_caches.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,56 @@
-from typing import Any, Dict, Iterator, Optional, Union
+#  noqa: D400
+"""
+# RunCaches
+
+This module defines a class for holding the caches for selected runs.
+
+Utilities provided include updating, getting, setting and clearing.
+
+## Classes
+    - RunCaches: Hold the caches for the selected runs.
+"""
+
+from typing import Any, Dict, Optional
 
 import shutil
 
+from deepcave.config import Config
 from deepcave.runs import AbstractRun
 from deepcave.utils.cache import Cache
-from deepcave.utils.hash import string_to_hash
 from deepcave.utils.logs import get_logger
 
 
 class RunCaches:
     """
-    Holds the caches for the selected runs. The caches are used for the plugins to store the
+    Hold the caches for the selected runs.
+
+    The caches are used for the plugins to store the
     raw outputs so that raw outputs must not be calculated again.
 
     Each input has its own cache. This change was necessary because it ensures that not all data
-    are loaded if they are not needed.
+    is loaded if not needed.
+
+    Properties
+    ----------
+    cache_dir : Path
+        The path to the cache directory of the run.
+    logger : Logger
+        The logger for the run cache.
     """
 
     def __init__(self, config: "Config"):
         self.cache_dir = config.CACHE_DIR / "run_cache"
         self.logger = get_logger("RunCache")
         self._debug = config.DEBUG
 
     def update(self, run: AbstractRun) -> bool:
         """
-        Updates the cache for the given run. If the cache does not exists it will be created.
+        Update the cache for the given run. If the cache does not exists it will be created.
+
         If the run hash is different from the saved variant the cache will be reset.
 
         Parameters
         ----------
         run : AbstractRun
             The run which should be updated.
 
@@ -82,43 +104,51 @@
         cache.set("name", value=run.name, write_file=False)
         cache.set("hash", value=run.hash, write_file=False)
         if run.path is not None:
             cache.set("path", value=str(run.path), write_file=False)
 
         cache.write()
 
-    def get(self, run: AbstractRun, plugin_id: str, inputs_key: str) -> Dict[str, Any]:
+    def get(self, run: AbstractRun, plugin_id: str, inputs_key: str) -> Optional[Dict[str, Any]]:
         """
-        Returns the raw outputs for the given run, plugin and inputs key.
+        Return the raw outputs for the given run, plugin and inputs key.
 
         Parameters
         ----------
         run : AbstractRun
             The run to get the results for.
         plugin_id : str
             The plugin id to get the results for.
         inputs_key : str
             The input key to get the results for. Should be the output from `Plugin._dict_as_key`.
 
         Returns
         -------
-        Dict[str, Any]
+        Optional[Dict[str, Any]]
             Raw outputs for the given run, plugin and inputs key.
+
+        Raises
+        ------
+        AssertionError
+            If the outputs of the cache are not a dict.
         """
         filename = self.cache_dir / run.id / plugin_id / f"{inputs_key}.json"
 
         if not filename.exists():
             return None
 
         cache = Cache(filename, debug=self._debug, write_file=False)
-        return cache.get("outputs")
+        outputs = cache.get("outputs")
+        assert isinstance(outputs, dict), "Outputs of cache must be a dict."
+        return outputs
 
     def set(self, run: AbstractRun, plugin_id: str, inputs_key: str, value: Any) -> None:
         """
-        Sets the value for the given run, plugin and inputs key.
+        Set the value for the given run, plugin and inputs key.
+
         Since each input key has it's own cache, only necessary data are loaded.
 
         Parameters
         ----------
         run : AbstractRun
             The run to set the cache for.
         plugin_id : str
@@ -129,20 +159,16 @@
             The value to set.
         """
         filename = self.cache_dir / run.id / plugin_id / f"{inputs_key}.json"
         cache = Cache(filename, debug=self._debug, write_file=False)
         cache.set("outputs", value=value)
 
     def clear_run(self, run: AbstractRun) -> None:
-        """
-        Removes all caches for the given run.
-        """
+        """Remove all caches for the given run."""
         shutil.rmtree(self.cache_dir / run.id)
 
     def clear(self) -> None:
-        """
-        Removes all caches.
-        """
+        """Remove all caches."""
         try:
             shutil.rmtree(self.cache_dir)
         except Exception:
             pass
```

### Comparing `deepcave-1.1.3/deepcave/utils/styled_plotty.py` & `deepcave-1.2/deepcave/utils/styled_plotty.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# noqa: D400
+"""
+# Styled Plotty
+
+This module provides utilities for styling and customizing different plots with plotly.
+For this, it uses plotly as well as dash.
+"""
+
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import itertools
 import re
 
 import numpy as np
 import plotly.express as px
@@ -13,30 +21,32 @@
     IntegerHyperparameter,
 )
 from dash import html
 from dash.development.base_component import Component
 
 from deepcave import interactive
 from deepcave.constants import CONSTANT_VALUE, NAN_LABEL, NAN_VALUE
+from deepcave.runs import AbstractRun
 from deepcave.utils.logs import get_logger
 
 logger = get_logger(__name__)
 
 
 @interactive
 def save_image(figure: go.Figure, name: str) -> None:
     """
-    Saves a plotly figure as an image.
+    Save a plotly figure as an image.
 
     Parameters
     ----------
-    fig : go.Figure
+    figure : go.Figure
         Plotly figure.
     name : str
-        Name of the image with extension. Will be automatically saved to the cache.
+        Name of the image with extension.
+        Will be automatically saved to the cache.
     """
     from deepcave import config
 
     if not config.SAVE_IMAGES:
         return
 
     ratio = 16 / 9
@@ -46,18 +56,35 @@
 
     figure.write_image(path, width=width, height=height)
     logger.info(f"Saved figure {name} to {path}.")
 
 
 def hex_to_rgb(hex_string: str) -> Tuple[int, int, int]:
     """
-    Converts a hex_string to a tuple of rgb values.
+    Convert a hex_string to a tuple of rgb values.
+
     Requires format including #, e.g.:
     #000000
     #ff00ff
+
+    Parameters
+    ----------
+    hex_string : str
+        The hex string to be converted.
+
+    Returns
+    -------
+    Tuple[int, int, int]
+        A Tuple of the converted RGB values
+
+    Raises
+    ------
+    ValueError
+        If the hex string is longer than 7.
+        If there are invalid characters in the hex string.
     """
     if len(hex_string) != 7:
         raise ValueError(f"Invalid length for #{hex_string}")
 
     if any(c not in "0123456789ABCDEF" for c in hex_string.lstrip("#").upper()):
         raise ValueError(f"Invalid character in #{hex_string}")
 
@@ -65,38 +92,58 @@
     g_hex = hex_string[3:5]
     b_hex = hex_string[5:7]
     return int(r_hex, 16), int(g_hex, 16), int(b_hex, 16)
 
 
 def get_color(id_: int, alpha: float = 1) -> Union[str, Tuple[float, float, float, float]]:
     """
-    Using Plotly palette for the first 10 ids and Alphabet palette for the next 26, currently 36 colors are possible.
+    Get an RGBA Color, currently (Plotly version 5.3.1) there are 10 possible colors.
+
+    Parameters
+    ----------
+    id_ : int
+        ID for retrieving a specific color.
+    alpha : float, optional
+        Alpha value for the color, by default 1.
+
+    Returns
+    -------
+    Union[str, Tuple[float, float, float, float]]
+        The color from the color palette.
     """
     if id_ < 10:
         color = px.colors.qualitative.Plotly[id_]
     else:
         color = px.colors.qualitative.Alphabet[id_ - 10]
 
     r, g, b = hex_to_rgb(color)
     return f"rgba({r}, {g}, {b}, {alpha})"
 
 
-def get_discrete_heatmap(x, y, values: List[Any], labels: List[Any]):
+def get_discrete_heatmap(
+    x: List[Union[float, int]], y: List[int], values: List[Any], labels: List[Any]
+) -> go.Heatmap:
     """
     Generate a discrete colorscale from a (nested) list or numpy array of values.
 
     Parameters
     ----------
-    values : _type_
-        _description_
+    x : List[Union[float, int]]
+        List of values that present the x-axis of the heatmap.
+    y : List[int]
+         List of values that present the y-axis of the heatmap.
+    values : List[Any]
+        Contains the data values for the heatmap.
+    labels : List[Any]
+        Contains the labels corresponding to the values.
 
     Returns
     -------
-    _type_
-        _description_
+    go.Heatmap
+        A Plotly Heatmap object corresponding to the input.
     """
     flattened_values = list(itertools.chain(*values))
     flattened_labels = list(itertools.chain(*labels))
 
     unique_values = []
     unique_labels = []
 
@@ -108,57 +155,62 @@
     sorted_indices = np.argsort(np.array(unique_values))
     unique_sorted_values = []
     unique_sorted_labels = []
     for idx in sorted_indices:
         unique_sorted_values += [unique_values[idx]]
         unique_sorted_labels += [unique_labels[idx]]
 
-    # Now we give them new ids and we want to create new z values
-    # For that we need a mapping from old to new
+    # Now they are given new ids, and new z values should be created
+    # For that a mapping from old to new is needed
     mapping = {}
     v = []
     for new, old in enumerate(unique_sorted_values):
         mapping[old] = new / len(unique_sorted_values)
         v += [new]
 
     z = values
     for i1, v1 in enumerate(values):
         for i2, v2 in enumerate(v1):
             z[i1][i2] = mapping[v2]
 
-    n_intervals = v + [len(v)]
-    n_intervals = [(i - n_intervals[0]) / (n_intervals[-1] - n_intervals[0]) for i in n_intervals]
+    n_intervals_int = v + [len(v)]
+    n_intervals = [
+        (i - n_intervals_int[0]) / (n_intervals_int[-1] - n_intervals_int[0])
+        for i in n_intervals_int
+    ]
     colors = [get_color(i) for i in range(len(n_intervals))]
 
     discrete_colorscale = []
     for k in range(len(v)):
         discrete_colorscale.extend([[n_intervals[k], colors[k]], [n_intervals[k + 1], colors[k]]])
 
     tickvals = [np.mean(n_intervals[k : k + 2]) for k in range(len(n_intervals) - 1)]
     ticktext = unique_sorted_labels
 
-    x = [str(i) for i in x]
-    y = [str(i) for i in y]
+    x_str = [str(i) for i in x]
+    y_str = [str(i) for i in y]
 
     return go.Heatmap(
-        x=x,
-        y=y,
+        x=x_str,
+        y=y_str,
         z=z,
         showscale=True,
         colorscale=discrete_colorscale,
         colorbar={"tickvals": tickvals, "ticktext": ticktext, "tickmode": "array"},
         zmin=0,
         zmax=1,
         # hoverinfo="skip",
     )
 
 
 def prettify_label(label: Union[str, float, int]) -> str:
     """
-    Takes a label and prettifies it. E.g. floats are shortened.
+    Take a label and prettifies it.
+
+    E.g. floats are shortened.
 
     Parameters
     ----------
     label : Union[str, float, int]
         Label, which should be prettified.
 
     Returns
@@ -187,37 +239,39 @@
 def get_hyperparameter_ticks(
     hp: Hyperparameter,
     additional_values: Optional[List] = None,
     ticks: int = 4,
     include_nan: bool = True,
 ) -> Tuple[List, List]:
     """
-    Generates tick data for both tickvals and ticktext. The background is that
-    you might have encoded data but you don't want to show all of them.
-    With this function, only 6 (default) values are shown. This behaviour is
+    Generate tick data for both tickvals and ticktext.
+
+    The background is that
+    you might have encoded data, but you don't want to show all of them.
+    With this function, only 6 (default) values are shown. This behavior is
     ignored if `hp` is categorical.
 
     Parameters
     ----------
     hp : Hyperparameter
         Hyperparameter to generate ticks from.
     additional_values : Optional[List], optional
-        Additional values, which are forced in addition. By default None.
+        Additional values, which are forced in addition. By default, None.
     ticks : int, optional
-        Number of ticks, by default 6
+        Number of ticks, by default 4
     include_nan : bool, optional
         Whether "nan" as tick should be included. By default True.
 
     Returns
     -------
     Tuple[List, List]
         tickvals and ticktext.
     """
-
     # This is basically the inverse of `encode_config`.
+    tickvals: List[Union[float, int]]
     if isinstance(hp, CategoricalHyperparameter):
         ticktext = hp.choices
         if len(ticktext) == 1:
             tickvals = [0]
         else:
             tickvals = [
                 hp._inverse_transform(choice) / (len(hp.choices) - 1) for choice in hp.choices
@@ -226,15 +280,15 @@
     elif isinstance(hp, Constant):
         tickvals = [CONSTANT_VALUE]
         ticktext = [hp.value]
     else:
         min_v = 0
         max_v = 1
 
-        values = [min_v]
+        values: List[Union[float, int]] = [min_v]
 
         # Get values for each tick
         factors = [i / (ticks - 1) for i in range(1, ticks - 1)]
 
         for factor in factors:
             new_v = (factor * (max_v - min_v)) + min_v
             values += [new_v]
@@ -244,40 +298,40 @@
         tickvals = []
         ticktext = []
 
         inverse_values = []
         for value in values:
             inverse_values += [hp._transform_scalar(value)]
 
-        # Integers are rounded, so we map then back
+        # Integers are rounded, they are mapped
         if isinstance(hp, IntegerHyperparameter):
             for label in inverse_values:
                 value = hp._inverse_transform(label)
 
                 if value not in tickvals:
                     tickvals += [value]
                     ticktext += [label]
 
             if additional_values is not None:
-                # Now we add additional values
+                # Now add additional values are added
                 for value in additional_values:
                     if not (value is None or np.isnan(value) or value == NAN_VALUE):
                         label = hp._transform_scalar(value)
                         value = hp._inverse_transform(label)
 
                         if value not in tickvals:
                             tickvals += [value]
                             ticktext += [label]
         else:
             for value, label in zip(values, inverse_values):
                 tickvals += [value]
                 ticktext += [label]
 
             if additional_values is not None:
-                # Now we add additional values
+                # Now additional values are added
                 for value in additional_values:
                     if (
                         not (value is None or np.isnan(value) or value == NAN_VALUE)
                         and value not in tickvals
                     ):
                         tickvals += [value]
                         ticktext += [hp._transform_scalar(value)]
@@ -291,35 +345,42 @@
     return tickvals, ticktext
 
 
 def get_hyperparameter_ticks_from_values(
     values: List, labels: List, forced: Optional[List[bool]] = None, ticks: int = 6
 ) -> Tuple[List, List]:
     """
-    Generates tick data for both values and labels. The background is that
-    you might have encoded data but you don't want to show all of them.
-    With this function, only 6 (default) values are shown. This behaviour is
+    Generate tick data for both values and labels.
+
+    The background is that
+    you might have encoded data, but you don't want to show all of them.
+    With this function, only 6 (default) values are shown. This behavior is
     ignored if `values` is a list of strings.
 
     Parameters
     ----------
     values : List
         List of values.
     labels : List
         List of labels. Must be the same size as `values`.
-    forced : List[bool], optional
+    forced : Optional[List[bool]], optional
         List of booleans. If True, displaying the particular tick is enforced.
-        Independent from `ticks`.
+        Independent of `ticks`.
     ticks : int, optional
         Number of ticks and labels to show. By default 6.
 
     Returns
     -------
     Tuple[List, List]
         Returns tickvals and ticktext as list.
+
+    Raises
+    ------
+    RuntimeError
+        If values contain both strings and non-strings.
     """
     assert len(values) == len(labels)
 
     unique_values = []  # df[hp_name].unique()
     unique_labels = []  # df_labels[hp_name].unique()
     for value, label in zip(values, labels):
         if value not in unique_values and label not in unique_labels:
@@ -333,28 +394,28 @@
                 raise RuntimeError("Values have strings and non-strings.")
 
             return_all = True
 
     tickvals = []
     ticktext = []
 
-    # If we have less than x values, we also show them
+    # If there are less than x values, they are also shown
     if return_all or len(unique_values) <= ticks:
-        # Make sure we don't have multiple (same) labels for the same value
+        # Make sure there are no multiple (same) labels for the same value
         for value, label in zip(unique_values, unique_labels):
             tickvals.append(value)
             ticktext.append(label)
     else:
         # Add min+max values
         for idx in [np.argmin(values), np.argmax(values)]:
             tickvals.append(values[idx])
             ticktext.append(labels[idx])
 
-        # After we added min and max values, we want to add
-        # intermediate values too
+        # After min and max values are added,
+        # intermediate values should be added too
         min_v = np.min(values)
         max_v = np.max(values)
 
         # Get values for each tick
         factors = [i / (ticks - 1) for i in range(1, ticks - 2)]
 
         for factor in factors:
@@ -375,45 +436,98 @@
             if force and value not in tickvals:
                 tickvals.append(value)
                 ticktext.append(label)
 
     return tickvals, ticktext
 
 
-def get_hovertext_from_config(run: "AbstractRun", config_id: int) -> str:
+def get_hovertext_from_config(
+    run: AbstractRun, config_id: int, budget: Optional[Union[int, float]] = None
+) -> str:
+    """
+    Generate hover text with metrics for a configuration.
+
+    The method gets information about a given configuration, including a link, its objectives,
+    budget, costs and hyperparameters.
+
+    Parameters
+    ----------
+    run : AbstractRun
+        The run instance
+    config_id : int
+        The id of the configuration
+    budget : Optional[Union[int, float]]
+            Budget to get the hovertext for. If no budget is given, the highest budget is chosen.
+            By default None.
+
+    Returns
+    -------
+    str
+        The hover text string containing the configuration information.
+    """
     if config_id < 0:
         return ""
 
     # Retrieve the link for the config id
     from deepcave.plugins.summary.configurations import Configurations
 
     link = Configurations.get_link(run, config_id)
 
     string = "<b>Configuration ID: "
     string += f"<a href='{link}' style='color: #ffffff'>{int(config_id)}</a></b><br><br>"
 
     # It's also nice to see the metrics
     objectives = run.get_objectives()
-    budget = run.get_highest_budget(config_id)
-    costs = run.get_costs(config_id, budget)
+    if budget is None or budget == -1:
+        highest_budget = run.get_highest_budget(config_id)
+        assert highest_budget is not None
+        string += f"<b>Objectives</b> (on highest found budget {round(highest_budget, 2)})<br>"
+    else:
+        string += f"<b>Objectives</b> (on budget {round(budget, 2)})<br>"
 
-    string += f"<b>Objectives</b> (on highest found budget {round(budget, 2)})<br>"
-    for objective, cost in zip(objectives, costs):
-        string += f"{objective.name}: {cost}<br>"
+    try:
+        avg_c, std_c = run.get_avg_costs(config_id, budget=budget)
+        avg_costs: List[Optional[float]] = list(avg_c)
+        std_costs: List[Optional[float]] = list(std_c)
+    except ValueError:
+        avg_costs = [None for _ in range(len(objectives))]
+        std_costs = [None for _ in range(len(objectives))]
+
+    for objective, cost, std_cost in zip(objectives, avg_costs, std_costs):
+        if std_cost == 0.0:
+            string += f"{objective.name}: {cost}<br>"
+        else:
+            string += f"{objective.name}: {cost} ± {std_cost}<br>"
 
     string += "<br><b>Hyperparameters</b>:<br>"
 
     config = run.get_config(config_id)
     for k, v in config.items():
         string += f"{k}: {v}<br>"
 
     return string
 
 
 def generate_config_code(register: Callable, variables: List[str]) -> List[Component]:
+    """
+    Generate HTML components to display code.
+
+    Parameters
+    ----------
+    register : Callable
+        A Callable for registering Dash components.
+        The register_input function is located in the Plugin class.
+    variables : List[str]
+        A List of variable names.
+
+    Returns
+    -------
+    List[Component]
+        A List of Dash components.
+    """
     code = """
     from ConfigSpace.configuration_space import ConfigurationSpace, Configuration
     from ConfigSpace.read_and_write import cs_json
 
     # Create configspace
     with open({{path}}, 'r') as f:
         cs = cs_json.read(f.read())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepcave-1.1.3/deepcave.egg-info/PKG-INFO` & `deepcave-1.2/deepcave.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: deepcave
-Version: 1.1.3
+Version: 1.2
 Summary: An interactive framework to visualize and analyze your AutoML process in real-time.
 Home-page: https://www.automl.org
-Author-email: sass@tnt.uni-hannover.de
+Author-email: s.segel@ai.uni-hannover.de
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/automl/deepcave
 Project-URL: Source Code, https://github.com/automl/deepcave
 Platform: Linux
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Python: >=3.9, <3.10
+Requires-Python: >=3.9, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: examples
 License-File: LICENSE.txt
 
+<img src="docs/images/DeepCAVE_Logo_wide.png" alt="Logo"/> 
+
 # DeepCAVE
 
 DeepCAVE is a visualization and analysis tool for AutoML (especially for the sub-problem
 hyperparameter optimization) runs. The framework is programmed on top of Dash and therefore
 entirely interactive. Multiple and diverse plugins make it possible to efficiently generate insights
 and bring the human back in the loop. Moreover, the powerful run interface and the modularized
 plugin structure allow extending the tool at any time effortlessly.
@@ -38,15 +41,15 @@
 
 Following features are provided:
 - Interactive Dashboard (completely written in Python) to self-analyze optimization runs/processes.
 - Analyzing while optimizing (run changes are automatically detected).
 - A large collection of plugins to explore multiple areas like performance, hyperparameter and
 budget analysis.
 - Save your runs using DeepCAVE's native recorder.
-- Support for many optimizers using converter (e.g., DeepCAVE, SMAC and BOHB).
+- Support for many optimizers using converters (e.g., DeepCAVE, SMAC and BOHB).
 - Select runs directly from a working directory in the interface.
 - Select groups of runs for combined analysis.
 - Modularized plugin structure with access to selected runs/groups to provide maximal flexibility.
 - Asynchronous execution of expensive plugins and caching of their results.
 - Help buttons and integrated documentation in the interface helps you to understand the plugins.
 - Use the matplotlib mode to customize and save the plots for your publication.
 - The API mode gives you full access to the code, while you do not have to interact with the 
@@ -65,20 +68,26 @@
 conda install -c anaconda swig
 pip install DeepCAVE
 ```
 
 If you want to contribute to DeepCAVE use the following steps instead:
 ```bash
 git clone https://github.com/automl/DeepCAVE.git
+cd DeepCAVE
 conda create -n DeepCAVE python=3.9
 conda activate DeepCAVE
 conda install -c anaconda swig
 make install-dev
 ```
 
+If you want to use the given examples, run this after installing:
+```bash
+make install-examples
+```
+
 Please visit the [documentation](https://automl.github.io/DeepCAVE/main/installation.html) to get
 further help (e.g. if you can not install redis server or you are on a mac).
 
 
 ## Recording
 
 A minimal example is given to show the simplicity yet powerful API to record runs.
@@ -140,8 +149,7 @@
     publisher = {arXiv},
     year = {2022},
     copyright = {arXiv.org perpetual, non-exclusive license}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org/).
-
```

### Comparing `deepcave-1.1.3/deepcave.egg-info/SOURCES.txt` & `deepcave-1.2/deepcave.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,30 @@
 deepcave.egg-info/top_level.txt
 deepcave/assets/custom.css
 deepcave/docs/api.rst
 deepcave/docs/converters.rst
 deepcave/docs/faq.rst
 deepcave/docs/getting_started.rst
 deepcave/docs/glossary.rst
+deepcave/docs/how_to_contribute.rst
 deepcave/docs/index.rst
 deepcave/docs/installation.rst
 deepcave/docs/redis.rst
 deepcave/docs/plugins/budget_correlation.rst
 deepcave/docs/plugins/configuration_cube.rst
 deepcave/docs/plugins/configuration_footprint.rst
 deepcave/docs/plugins/configurations.rst
 deepcave/docs/plugins/cost_over_time.rst
 deepcave/docs/plugins/importances.rst
 deepcave/docs/plugins/index.rst
 deepcave/docs/plugins/overview.rst
 deepcave/docs/plugins/parallel_coordinates.rst
 deepcave/docs/plugins/pareto_front.rst
 deepcave/docs/plugins/partial_dependencies.rst
+deepcave/docs/plugins/symbolic_explanations.rst
 deepcave/evaluators/__init__.py
 deepcave/evaluators/fanova.py
 deepcave/evaluators/footprint.py
 deepcave/evaluators/lpi.py
 deepcave/evaluators/epm/__init__.py
 deepcave/evaluators/epm/fanova_forest.py
 deepcave/evaluators/epm/random_forest.py
@@ -60,14 +62,15 @@
 deepcave/plugins/dynamic.py
 deepcave/plugins/static.py
 deepcave/plugins/budget/__init__.py
 deepcave/plugins/budget/budget_correlation.py
 deepcave/plugins/hyperparameter/__init__.py
 deepcave/plugins/hyperparameter/importances.py
 deepcave/plugins/hyperparameter/pdp.py
+deepcave/plugins/hyperparameter/symbolic_explanations.py
 deepcave/plugins/objective/__init__.py
 deepcave/plugins/objective/configuration_cube.py
 deepcave/plugins/objective/cost_over_time.py
 deepcave/plugins/objective/parallel_coordinates.py
 deepcave/plugins/objective/pareto_front.py
 deepcave/plugins/summary/__init__.py
 deepcave/plugins/summary/configurations.py
@@ -101,20 +104,22 @@
 deepcave/utils/layout.py
 deepcave/utils/logging.yml
 deepcave/utils/logs.py
 deepcave/utils/notification.py
 deepcave/utils/run_caches.py
 deepcave/utils/styled_plot.py
 deepcave/utils/styled_plotty.py
+deepcave/utils/symbolic_regression.py
 deepcave/utils/url.py
 deepcave/utils/util.py
 docs/plugins/budget_correlation.rst
 docs/plugins/configuration_cube.rst
 docs/plugins/configuration_footprint.rst
 docs/plugins/configurations.rst
 docs/plugins/cost_over_time.rst
 docs/plugins/importances.rst
 docs/plugins/index.rst
 docs/plugins/overview.rst
 docs/plugins/parallel_coordinates.rst
 docs/plugins/pareto_front.rst
-docs/plugins/partial_dependencies.rst
+docs/plugins/partial_dependencies.rst
+docs/plugins/symbolic_explanations.rst
```

### Comparing `deepcave-1.1.3/docs/plugins/budget_correlation.rst` & `deepcave-1.2/docs/plugins/budget_correlation.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/docs/plugins/configuration_cube.rst` & `deepcave-1.2/docs/plugins/configuration_cube.rst`

 * *Files identical despite different names*

### Comparing `deepcave-1.1.3/docs/plugins/configuration_footprint.rst` & `deepcave-1.2/docs/plugins/configuration_footprint.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 grasp on your configuration footprint.
 
 
 Performance plot
 ----------------
 Perhaps the most useful plot of the two is to see how much we know about which configuration will
 achieve which **objective** score. To view this, mousing over the **Incumbent** will tell you the
-best configuration found for the given *objective* and *budget*. The **Evaluated Configuration**
+best configuration found for the given *objective* and *budget*. For non-deterministic runs (i.e.
+multiple seeds evaluated per configuration), only configurations evaluated on the maximum number of
+seeds are considered to choose the best configuration from. The **Evaluated Configuration**
 points will have a true objective score, all be it possibly noisy if the objective is noisy.
 Using these two kind of points, we can try to infer what the performance for the rest of the
 configuration space will be.
 
 It's important to note that the background colour, represnting the objective is a best estimate
 given what we already know and does not indicate the true objective value in regions where there
 are no configurations evaluated. We can increase the resolution using the *Details* option, which
```

### Comparing `deepcave-1.1.3/docs/plugins/configurations.rst` & `deepcave-1.2/docs/plugins/configurations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Configuration
 * Code
 
 Since configurations are used throughout the application, you might find links associated to this
 plugin. This plugin is capable of answering following questions:
 
 * Where is the configuration coming from?
-* How are the objective values wrt the budgets?
+* How are the objective values with respect to the budgets?
 * How is the status of a trial associated with the selected configuration?
 * Which values have been used for a certain configuration?
 * How can I access the configuration in python?
 
 
 Overview
 --------
@@ -39,11 +39,11 @@
 In the configuration section, you see how the hyperparameters were selected in the end. While the
 graph view gives you a nice overview, the table displays the concrete values.
 
 
 Code
 ----
 Often a configuration is selected for deployment, which makes it crucial to access it somehow.
-The code block provides you the code to access the configuration code-wise. 
+The code block provides you the code to access the configuration code-wise.
 
 
 .. image:: ../images/plugins/configurations.png
```

### Comparing `deepcave-1.1.3/docs/plugins/cost_over_time.rst` & `deepcave-1.2/docs/plugins/cost_over_time.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 how the objectives change over time. To see the change based on the time or number of
 configurations, this plugin visualize it for you.
 
 Since multiple runs are supported, you directly see which run performs best to which time.
 If you decide to display groups (which are combined runs), you will see the mean and standard
 deviation too.
 
-.. note:: 
-    The configuration spaces of the selected runs have to be equal. Otherwise, a good comparison
-    is not possible.
+.. note::
+    The configuration spaces of the selected runs should be equal. Otherwise, a good comparison
+    is not possible. They can, however, still be displayed in the same graph.
+
+.. note::
+    For non-deterministic runs (i.e. multiple seeds evaluated per configuration), only
+    configurations evaluated on the maximum number of seeds are considered to choose the best
+    configuration at a given time from.
 
 This plugin is capable of answering following questions:
 
 * Does the optimizer converge?
 * How performs optimizer A in comparison to optimizer B? Is optimizer A better than optimizer B?
 * How long does the optimizer need to reach a certain objective value?
```

### Comparing `deepcave-1.1.3/docs/plugins/index.rst` & `deepcave-1.2/docs/plugins/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Plugins
-=======
+Displaying Data with Plugins
+============================
 
 .. toctree::
    :hidden:
    :maxdepth: 2
 
    overview
    configurations
@@ -11,14 +11,15 @@
    cost_over_time
    configuration_cube
    pareto_front
    parallel_coordinates
    budget_correlation
    importances
    partial_dependencies
+   symbolic_explanations
 
 
 Plugins are used to display data in a specific way. There are plugins to analyse the performance,
 the hyperparameters and the budgets. Since AutoML runs are multi-dimensional, the plugins
 provide a way to look into specific aspects in more detail.
 
 The goal of the plugins are to provide a way to visualize the data in a way that is easy to
@@ -74,10 +75,10 @@
 Custom Plugin
 -------------
 
 DeepCAVE was designed so that the plugins require minimal design. We recommend using any of our
 provided plugins as a starting point and change it to your needs.
 
 After you have created your plugin, you need to register it in your config file. If you work
-on the branch directly, you can adapt ``deepcave/config.py`` to your needs. 
+on the branch directly, you can adapt ``deepcave/config.py`` to your needs.
 We would be very happy to receive pull-requests!
```

### Comparing `deepcave-1.1.3/docs/plugins/overview.rst` & `deepcave-1.2/docs/plugins/overview.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,56 +19,58 @@
 * When was the latest change of the optimizer's data?
 * What is the best configuration?
 * Are the meta data as expected?
 * Are the objectives as expected?
 * Is the configuration space as expected?
 * How many trials have been successful/unsuccessful?
 * Why did certain trials crash?
-* On which budgets were the configurations evaluated?
+* On which multi-fidelity budgets were the configurations evaluated?
 
 
 Quick Information
 -----------------
 
 In the **Quick Information** box you'll information regarding summary statistics about your run or
 group of runs. Notably information on the optimizer used, how many configurations were tried, when
 the runs were last updated and a handy quick link to the best **Configuration**.
 
 Meta
 ----
 Next we show some meta information regarding your runs. Notably, you can see information such as the
-possible **budget** allocations that were considered during the run.
+possible **budget** allocations that were considered during the run. The **budget** is the amount of
+resources that were allocated to a configuration as it was being evaluated using a multi-fidelity
+approach.
 
 
 Objectives
 ----------
 In this section, we see the objectives that were considered during the optimization run. Here we get
 information about it's name and the bounds they were in.
 
 
 Statuses
 --------
 To get a nice overview of the optimization run, we provide a barplot that details how the end status
-of the many trials that occured. You can also view these as a heatmap or get more information from
+of the many trials that occurred. You can also view these as a heatmap or get more information from
 the **Details** tab.
 
-The barplot shows which trial recieved which status and under which budget allocation. These are
+The barplot shows which trial received which status and under which budget allocation. These are
 grouped according to the status and coloured based on the status it exited with.
 
 To see details on how these configurations faired as they progressed in budget, you can refer to
 the **Heatmap** tab. Here you'll see the budget allocation along the x-axis with the configuration
 ID stacked on the y-axis. In an ideal scenario, you would see mostly **Success** bars spanning
 across the entire plot, with some **NOT_EVALUATED** lines indicating there is further configurations
 to try. However if you faced many crashes at high budgets for example, you'll see **CRASHED** bars
 from the highest budget onwards. In general, you can use this to understand how often your optimizer
 balances out between low budget evaluations and full budget evaluations.
 
-In the **Details** tab, you'll recieve an overview of configurations that were not successful.
-Here you'll get some breif information about the config id number, the budget it was evaluated under
-and the status it recieved. If there is an associated error we can provide, such as when it recieved
+In the **Details** tab, you'll receive an overview of configurations that were not successful.
+Here you'll get some brief information about the config id number, the budget it was evaluated under
+and the status it received. If there is an associated error we can provide, such as when it received
 the **CRASHED** status, we will display it in the error column.
 
 
 Configuration Space
 -------------------
 
 Lastly you can find information on the configuration space that was being optimized over.
```

### Comparing `deepcave-1.1.3/docs/plugins/parallel_coordinates.rst` & `deepcave-1.2/docs/plugins/parallel_coordinates.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Parallel Coordinates
 ====================
 
-With parallel coordinates, you can see configurations plotted as a line through their hyperparamter
+With parallel coordinates, you can see configurations plotted as a line through their hyperparameter
 values and to which final score they reach.
 You can use this to identify trends in hyperparamter value ranges that achieve certain scores.
 For example, you may find that high performing configurations may all share the same value for a
 certain categorical hyperparamter, as indicated by many high scoring lines passing through this
 value. These lines will be ordered according to their importance in determining the final score from
 left to right with the default to show the top 10 important ones.
 Lastly, you can place visual filters along these spines to really home-in on hyperparamters
```

### Comparing `deepcave-1.1.3/docs/plugins/pareto_front.rst` & `deepcave-1.2/docs/plugins/pareto_front.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 configuration can be chosen due to multiple important objectives which should be considered.
 For example, I want to find a configuration for my problem which has both a good performance
 and low computational cost. To select a suitable configuration, the pareto front shows you the best
 configurations for two given objectives.
 
 .. note::
     You can enable or disable specific runs if you click on the name right to the plot.
-    If you click on a configuration you a redirected to the configuration plugin to see 
+    If you click on a configuration you are redirected to the configuration plugin to see 
     the configuration in detail.
 
 This plugin is capable of answering following questions:
 
 * Which configuration should I choose if I prefer objective A slightly over objective B?
 * How performs optimizer A in comparison to optimizer B? Is optimizer A better than optimizer B?
```

### Comparing `deepcave-1.1.3/pyproject.toml` & `deepcave-1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,72 @@
 # For TOML reference
 # https://learnxinyminutes.com/docs/toml/
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]      # path to the test directory
-minversion = "3.8"
+minversion = "3.9"
 addopts = "--cov=deepcave" # Should be package name
 
 [tool.coverage.run]
 branch = true
 context = "deepcave" # Should be package name
 omit = [
-    "deepcave/__init__.py", # Has variables only needed for setup.py
+  "deepcave/__init__.py", # Has variables only needed for setup.py
 ]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 exclude_lines = [
-    "pragma: no cover",
-    '\.\.\.',
-    "raise NotImplementedError",
-    "if TYPE_CHECKING",
+  "pragma: no cover",
+  '\.\.\.',
+  "raise NotImplementedError",
+  "if TYPE_CHECKING",
 ] # These are lines to exclude from coverage
 
 [tool.black]
-target-version = ['py38']
+target-version = ['py39']
 line-length = 100
 
 [tool.isort]
-py_version = "38"
+py_version = "39"
 profile = "black" # Play nicely with black
 src_paths = ["deepcave", "tests"]
 known_types = ["typing", "abc"] # We put these in their own section "types"
 known_test = ["tests"]
 known_first_party = ["deepcave"]
 sections = [
-    "FUTURE",
-    "TYPES",
-    "STDLIB",
-    "THIRDPARTY",
-    "FIRSTPARTY",
-    "TEST",
-    "LOCALFOLDER",
+  "FUTURE",
+  "TYPES",
+  "STDLIB",
+  "THIRDPARTY",
+  "FIRSTPARTY",
+  "TEST",
+  "LOCALFOLDER",
 ] # section ordering
 multi_line_output = 3 # https://pycqa.github.io/isort/docs/configuration/multi_line_output_modes.html
 
 [tool.pydocstyle]
 convention = "numpy"
 add-ignore = [ # http://www.pydocstyle.org/en/stable/error_codes.html
-    "D100", # Missing docstring in public module
-    "D101", # Missing docstring in public class
-    "D104", # Missing docstring in public package
-    "D105", # Missing docstring in magic method
-    "D203", # 1 blank line required before class docstring
-    "D205", # 1 blank line required between summary and description
-    "D210", # No whitespaces allowed surrounding docstring text
-    "D212", # Multi-line docstring summary should start at the first line
-    "D213", # Multi-line docstring summary should start at the second line
-    "D400", # First line should end with a period
-    "D401", # First line should be in imperative mood
-    "D404", # First word of docstring should not be this
-    "D413", # Missing blank line after last section
-    "D415", # First line should end with a period, question mark, or exclamation point
+  "D105", # Missing docstring in magic method
+  "D212", # Multi-line docstring summary should start at the first line
 ]
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.9"
 show_error_codes = true
 warn_unused_configs = true         # warn about unused [tool.mypy] lines
 follow_imports = "normal"          # Type check top level api code we use from imports
-ignore_missing_imports = false     # prefer explicit ignores
+ignore_missing_imports = true      # prefer explicit ignores
 disallow_untyped_defs = true       # All functions must have types
 disallow_untyped_decorators = true # ... even decorators
 disallow_incomplete_defs = true    # ... all types
+check_untyped_defs = true          # Problems are shown, even if def is check_untyped_defs
 
 [[tool.mypy.overrides]]
 module = ["setuptools.*"]     # Add modules that give import errors here
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["tests.*"]                # pytest uses decorators which are not typed in 3.8
+module = ["tests.*"]                # pytest uses decorators which are not typed in 3.9
 disallow_untyped_decorators = false # decorators in testing are not all annotated
```

### Comparing `deepcave-1.1.3/requirements.txt` & `deepcave-1.2/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-wheel
-setuptools
+# If something is changed here, change it in the pre-commit-hook under mypy additonal dependencies as well
+# otherwise mypy wont check the dependencies
+wheel>=0.41.2
+setuptools==68.2.2
 absl-py>=1.0.0
 jsonlines>=3.0.0
 pandas>=1.3.4
 numpy>=1.22.2
 matplotlib>=3.5.1
 seaborn>=0.13.0
-pyyaml
+pyyaml>=6.0.1
+kaleido>=0.2.1
+gplearn>=0.4.2
+sympy>=1.12
+requests>=2.31.0
 
 # AutoML packages
 ConfigSpace==0.6.1
 pyrfr>=0.9.0
 hpbandster==0.7.4
 
 # Upgrading to 2.1.0 or higher breaks the slider because string keys in marks
@@ -20,8 +26,8 @@
 dash-bootstrap-components==1.0.3
 redis>=4.1.4
 rq>=1.10.1
 # Pinned due to https://github.com/plotly/dash/issues/1992
 # Pinning might be removed for dash>2.3.0
 werkzeug==2.0.3
 
-pyPDPPartitioner
+pyPDPPartitioner>=0.1.8
```

### Comparing `deepcave-1.1.3/setup.py` & `deepcave-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-# -*- encoding: utf-8 -*-
+from __future__ import annotations
+
 import setuptools
 from deepcave import version
 
 
 def read_file(file_name):
     with open(file_name, encoding="utf-8") as fh:
-        text = fh.read()
-    return text
+        return fh.read()
 
 
 extras_require = {
     "dev": [
         # Tests
         "pytest>=4.6",
-        "pytest-cov",
-        "pytest-xdist",
-        "pytest-timeout",
-        "mypy",
-        "isort",
-        "black",
-        "pydocstyle",
-        "pre-commit",
-        "flake8",
+        "pytest-cov>=4.1.0",
+        "pytest-xdist>=3.3.1",
+        "pytest-timeout>=2.2.0",
+        "mypy>=1.6.1",
+        "isort>=5.12.0",
+        "black>=23.11.0",
+        "pydocstyle>=6.3.0",
+        "pre-commit>=3.5.0",
+        "flake8>=6.1.0",
         # Docs
         "automl-sphinx-theme>=0.1.10",
     ],
     "examples": [
-        "torch",
-        "torchvision",
-        "pytorch-lightning",
+        "torch>=2.1.0",
+        "torchvision>=0.16.0",
+        "pytorch-lightning>=2.1.1",
     ],
 }
 
 
 setuptools.setup(
     name="deepcave",
-    author_email="sass@tnt.uni-hannover.de",
+    author_email="s.segel@ai.uni-hannover.de",
     description="An interactive framework to visualize and analyze your AutoML process in real-time.",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     url="https://www.automl.org",
     project_urls={
         "Documentation": "https://github.com/automl/deepcave",
         "Source Code": "https://github.com/automl/deepcave",
     },
     version=version,
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
     ),
     include_package_data=True,
-    python_requires=">=3.9, <3.10",
+    python_requires=">=3.9, <3.11",
     install_requires=read_file("./requirements.txt").split("\n"),
     extras_require=extras_require,
     entry_points={
         "console_scripts": ["deepcave = deepcave.cli:main"],
     },
     test_suite="pytest",
     platforms=["Linux"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Development Status :: 3 - Alpha",
         "Natural Language :: English",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
```

