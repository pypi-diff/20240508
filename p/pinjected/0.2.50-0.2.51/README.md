# Comparing `tmp/pinjected-0.2.50.tar.gz` & `tmp/pinjected-0.2.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.50.tar", max compression
+gzip compressed data, was "pinjected-0.2.51.tar", max compression
```

## Comparing `pinjected-0.2.50.tar` & `pinjected-0.2.51.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.50/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.50/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.50/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.50/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.50/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.50/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.50/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.50/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.50/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.50/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.50/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.50/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.50/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14583 2024-05-01 08:01:27.605626 pinjected-0.2.50/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.50/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.50/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.50/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.50/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.50/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54296 2024-05-05 06:25:12.645054 pinjected-0.2.50/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.50/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.50/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.50/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.50/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.50/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.50/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.50/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.50/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.50/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.50/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.50/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.50/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.50/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.50/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.50/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.50/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.50/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.50/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.50/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.50/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.50/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.50/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.50/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.50/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.50/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.50/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.50/pinjected/global_configs.py
--rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.50/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.50/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.50/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.50/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.50/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.50/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.50/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.50/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.50/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.50/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.50/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.50/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.50/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.50/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.50/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.50/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.50/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.50/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.50/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.50/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.50/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.50/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.50/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.50/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.50/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9601 2024-05-01 11:59:22.455243 pinjected-0.2.50/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.50/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.50/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.50/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.50/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.50/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.50/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.50/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.50/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.50/pinjected/v2/di.py
--rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.50/pinjected/v2/keys.py
--rw-r--r--   0        0        0      508 2024-05-01 08:00:14.705856 pinjected-0.2.50/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    10541 2024-05-01 08:05:13.964304 pinjected-0.2.50/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.50/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.50/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.50/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.50/pinjected/with_context.py
--rw-r--r--   0        0        0      656 2024-05-05 08:15:35.426099 pinjected-0.2.50/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.50/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.51/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.51/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.51/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.51/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.51/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.51/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.51/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.51/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.51/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.51/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.51/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.51/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.51/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14766 2024-05-08 06:09:38.125434 pinjected-0.2.51/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.51/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.51/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.51/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.51/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.51/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54296 2024-05-05 06:25:12.645054 pinjected-0.2.51/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.51/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.51/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.51/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.51/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.51/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.51/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.51/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.51/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.51/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.51/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.51/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.51/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.51/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.51/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.51/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.51/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.51/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.51/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.51/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.51/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.51/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.51/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.51/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.51/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.51/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.51/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.51/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.51/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.51/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.51/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.51/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.51/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.51/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.51/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.51/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.51/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.51/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.51/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.51/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.51/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.51/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.51/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.51/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.51/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.51/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.51/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.51/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.51/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.51/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.51/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.51/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.51/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9601 2024-05-01 11:59:22.455243 pinjected-0.2.51/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.51/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.51/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.51/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.51/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.51/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.51/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.51/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.51/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.51/pinjected/v2/di.py
+-rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.51/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      518 2024-05-08 06:06:09.223799 pinjected-0.2.51/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    12425 2024-05-08 06:19:23.364134 pinjected-0.2.51/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.51/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.51/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.51/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.51/pinjected/with_context.py
+-rw-r--r--   0        0        0      656 2024-05-08 06:20:04.812546 pinjected-0.2.51/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.51/PKG-INFO
```

### Comparing `pinjected-0.2.50/LICENSE` & `pinjected-0.2.51/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/decoration.py` & `pinjected-0.2.51/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/demo.py` & `pinjected-0.2.51/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/app_designed.py` & `pinjected-0.2.51/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/app_injected.py` & `pinjected-0.2.51/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/applicative.py` & `pinjected-0.2.51/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/ast.py` & `pinjected-0.2.51/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/decorators.py` & `pinjected-0.2.51/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/design.py` & `pinjected-0.2.51/pinjected/di/design.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,17 +212,24 @@
             bind: IBind = self.bindings[key]
             res += Design(
                 bindings={key: bind.update_metadata(meta)}
             )
         return res
 
     def to_resolver(self):
-        from pinjected.v2.resolver import AsyncResolver
+        from pinjected.v2.resolver import AsyncResolver,BaseResolverCallback
+        from loguru import logger
         bindings = {**IMPLICIT_BINDINGS, **self.bindings}
-        return AsyncResolver(Design(bindings=bindings, modules=self.modules))
+        callback = BaseResolverCallback()
+        return AsyncResolver(
+            Design(bindings=bindings, modules=self.modules),
+            callbacks=[
+                callback
+            ]
+        )
 
     def to_graph(self):
         return self.to_resolver().to_blocking()
 
     def run(self, f, modules=None):
         return self.to_graph(modules).run(f)
```

### Comparing `pinjected-0.2.50/pinjected/di/designed.py` & `pinjected-0.2.51/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.51/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/graph.py` & `pinjected-0.2.51/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/injected.py` & `pinjected-0.2.51/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/injected_analysis.py` & `pinjected-0.2.51/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/modular_injected.py` & `pinjected-0.2.51/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/overload_experimental.py` & `pinjected-0.2.51/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/proxiable.py` & `pinjected-0.2.51/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/session.py` & `pinjected-0.2.51/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/sessioned.py` & `pinjected-0.2.51/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/static_proxy.py` & `pinjected-0.2.51/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.51/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/test_graph.py` & `pinjected-0.2.51/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/test_injected.py` & `pinjected-0.2.51/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/tools/add_overload.py` & `pinjected-0.2.51/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/di/util.py` & `pinjected-0.2.51/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/exceptions.py` & `pinjected-0.2.51/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.51/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.51/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/graph_inspection.py` & `pinjected-0.2.51/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/helper_structure.py` & `pinjected-0.2.51/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/helpers.py` & `pinjected-0.2.51/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.51/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.51/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/ide_supports/default_design.py` & `pinjected-0.2.51/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.51/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.51/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/main_impl.py` & `pinjected-0.2.51/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/maybe_patch.py` & `pinjected-0.2.51/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/module_helper.py` & `pinjected-0.2.51/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/module_inspector.py` & `pinjected-0.2.51/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/module_var_path.py` & `pinjected-0.2.51/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/notification.py` & `pinjected-0.2.51/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/nx_graph_util.py` & `pinjected-0.2.51/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/run_config_utils.py` & `pinjected-0.2.51/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/run_config_utils_v2.py` & `pinjected-0.2.51/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/run_helpers/config.py` & `pinjected-0.2.51/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.51/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/runnables.py` & `pinjected-0.2.51/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/test_package/__init__.py` & `pinjected-0.2.51/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/test_package/child/module1.py` & `pinjected-0.2.51/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/v2/ainjected.py` & `pinjected-0.2.51/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/v2/binds.py` & `pinjected-0.2.51/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/v2/di.py` & `pinjected-0.2.51/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/v2/keys.py` & `pinjected-0.2.51/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pinjected/v2/resolver.py` & `pinjected-0.2.51/pinjected/v2/resolver.py`

 * *Files 25% similar despite different names*

```diff
@@ -87,19 +87,48 @@
         self.src = state
 
     def __hash__(self):
         return hash(f"cached") + hash(self.src)
 
 
 @dataclass
+class ResolverEvent:
+    cxt: ProvideContext
+
+
+@dataclass
+class RequestEvent(ResolverEvent):
+    key: IBindKey
+
+
+@dataclass
+class ProvideEvent(ResolverEvent):
+    key: IBindKey
+    data: Any
+
+
+class IResolverCallback:
+    def __call__(self, event: ResolverEvent):
+        pass
+
+
+@dataclass
 class AsyncResolver:
     design: "Design"
     parent: Optional["AsyncResolver"] = None
     objects: Dict[IBindKey, Any] = field(default_factory=dict)
     locks: AsyncLockMap = field(default_factory=AsyncLockMap)
+    callbacks: list[IResolverCallback] = field(default_factory=list)
+
+    def add_callback(self, callback: IResolverCallback):
+        self.callbacks.append(callback)
+
+    def _callback(self, event: ResolverEvent):
+        for cb in self.callbacks:
+            cb(event)
 
     def __post_init__(self):
         from pinjected import injected, instance, providers
         async def dummy():
             raise RuntimeError('This should never be instantiated')
 
         dummy = Injected.bind(dummy)
@@ -168,67 +197,71 @@
                     f"expr must be Object, Call, BiOp, UnaryOp, Attr or GetItem, got {expr} of type {type(expr)}")
         return res
 
     async def _provide(self, key: IBindKey, cxt: ProvideContext):
         # we need to think which one to ask provider
         # if we have the binding for the key, use our own scope
         async with self.locks.get(key):
+            self._callback(RequestEvent(cxt, key))
             if key in self.objects:
                 data = self.objects[key]
+                self._callback(ProvideEvent(cxt, key, data))
                 return data
             elif key in self.design:
-                logger.info(f"{cxt.trace_str}")
+                #logger.info(f"{cxt.trace_str}")
                 # we are responsible for providing this
                 bind = self.design.bindings[key]
                 dep_keys = list(bind.dependencies)
                 tasks = []
                 for dep_key in dep_keys:
                     n_cxt = ProvideContext(self, key=dep_key, parent=cxt)
                     tasks.append(self._provide(dep_key, n_cxt))
                 res = await asyncio.gather(*tasks)
                 deps = dict(zip(dep_keys, res))
                 data = await bind.provide(cxt, deps)
                 self.objects[key] = data
-                show_data = str(data)[:100]
-                logger.info(f"{cxt.trace_str} := {show_data}")
+                #show_data = str(data)[:100]
+                #logger.info(f"{cxt.trace_str} := {show_data}")
+                self._callback(ProvideEvent(cxt, key, data))
                 return data
             else:
                 if self.parent is not None:
                     return await self.parent._provide(key, cxt)
                 else:
                     raise KeyError(f"Key {key} not found in design in {cxt.trace_str}")
 
     def child_session(self, overrides: "Design"):
         return AsyncResolver(overrides, parent=self)
 
     async def _provide_providable(self, tgt: Providable):
+        root_cxt = ProvideContext(self, key=StrBindKey("__root__"), parent=None)
+
         async def resolve_deps(keys: set[IBindKey]):
-            tasks = [self._provide(k, ProvideContext(self, key=k, parent=None)) for k in keys]
+            tasks = [self._provide(k, ProvideContext(self, key=k, parent=root_cxt)) for k in keys]
             return {k: v for k, v in zip(keys, await asyncio.gather(*tasks))}
 
         match tgt:
             case str():
-                return await self._provide(StrBindKey(tgt), ProvideContext(self, key=StrBindKey(tgt), parent=None))
+                return await self._provide(StrBindKey(tgt), ProvideContext(self, key=StrBindKey(tgt), parent=root_cxt))
             case IBindKey():
-                return await self._provide(tgt, ProvideContext(self, key=tgt, parent=None))
+                return await self._provide(tgt, ProvideContext(self, key=tgt, parent=root_cxt))
             case DelegatedVar(value, cxt) as dv:
                 # return await self._provide_providable(tgt.eval())
                 expr = await self._optimize(dv.eval().ast)
                 return await self.eval_expr(expr)
             case EvaledInjected(val, ast):
                 expr = await self._optimize(ast)
                 return await self.eval_expr(expr)
             case Injected() as i_tgt:
                 return await self._provide_providable(BindInjected(i_tgt))
             case IBind():
                 deps = await resolve_deps(tgt.dependencies)
-                return await tgt.provide(ProvideContext(self, key=tgt, parent=None), deps)
+                return await tgt.provide(ProvideContext(self, key=tgt, parent=root_cxt), deps)
             case func if inspect.isfunction:
                 deps = extract_dependency(func)
-                logger.info(f"Resolving deps for {func} -> {deps}")
                 keys = {StrBindKey(d) for d in deps}
                 deps = await resolve_deps(keys)
                 kwargs = {k.name: v for k, v in deps.items()}
                 data = tgt(**kwargs)
                 if inspect.iscoroutinefunction(tgt):
                     return await data
                 else:
@@ -270,14 +303,42 @@
             logger.info(f"waiting for {len(destructions)} destructors to finish.")
             results = await asyncio.gather(*destructions)
             logger.success(f"all destructors finished with results:{results}")
             self.destructed = True
             logger.success(f"Resolver destructed")
             return results
 
+@dataclass
+class BaseResolverCallback(IResolverCallback):
+    def __post_init__(self):
+        self.request_stack = []
+    def __call__(self, event: ResolverEvent):
+        if isinstance(event, RequestEvent):
+            self.on_request(event)
+        elif isinstance(event, ProvideEvent):
+            self.on_provide(event)
+        else:
+            raise TypeError(f"event must be RequestEvent or ProvideEvent, got {event}")
+
+    def status_string(self):
+        items = [k.ide_hint_string() for k in self.request_stack]
+        return f"Pending:{items}"
+
+    def on_request(self, event: RequestEvent):
+        if event.key not in self.request_stack:
+            self.request_stack.append(event.key)
+        logger.info(f"{event.cxt.trace_str}")
+        logger.info(f"{self.status_string()}")
+
+    def on_provide(self, event: ProvideEvent):
+        if event.key in self.request_stack:
+            self.request_stack = [k for k in self.request_stack if k != event.key]
+        data_str = str(event.data)[:50]
+        logger.info(f"{event.cxt.trace_str} := {data_str}")
+        logger.info(f"{self.status_string()}")
 
 @dataclass
 class Resolver:
     resolver: AsyncResolver
 
     def provide(self, tgt: Providable):
         return asyncio.run(self.resolver.provide(tgt))
```

### Comparing `pinjected-0.2.50/pinjected/visualize_di.py` & `pinjected-0.2.51/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.50/pyproject.toml` & `pinjected-0.2.51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.50"
+version = "0.2.51"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.50/PKG-INFO` & `pinjected-0.2.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.50
+Version: 0.2.51
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

