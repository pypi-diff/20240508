# Comparing `tmp/mct-nightly-2.0.0.20240506.443.tar.gz` & `tmp/mct-nightly-2.0.0.20240507.417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240506.443.tar", last modified: Mon May  6 00:04:44 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240507.417.tar", last modified: Tue May  7 00:04:18 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240506.443.tar` & `mct-nightly-2.0.0.20240507.417.tar`

### file list

```diff
@@ -1,607 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.402386 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-05-06 00:04:44.000000 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-06 00:04:44.000000 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 00:04:44.000000 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 00:04:44.000000 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 00:04:44.000000 mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.402386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-06 00:04:43.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.402386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.406386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.406386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.406386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.406386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.410386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38265 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.410386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.410386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.410386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.414386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.414386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.414386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.414386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.418386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.418386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.418386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.418386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    26723 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.422386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.422386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.422386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.426386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.426386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.426386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.430386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.430386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.430386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.434386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.438386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.438386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18299 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.438386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.438386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.442386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.442386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.442386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.442386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.442386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.446386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.446386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.446386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.446386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.446386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.450386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.454386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.458387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.462386 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.466387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.470387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.474387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-06 00:04:04.000000 mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 00:04:44.478387 mct-nightly-2.0.0.20240506.443/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 00:04:43.000000 mct-nightly-2.0.0.20240506.443/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.760394 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-05-07 00:04:18.000000 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-07 00:04:18.000000 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:04:18.000000 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 00:04:18.000000 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 00:04:18.000000 mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.760394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-07 00:04:17.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.760394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.760394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.760394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.764394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.764394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.764394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.764394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.764394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.768394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.768394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.768394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.768394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.768394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.772394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.772394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.772394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.776394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.776394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.776394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.776394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.780394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.780394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.780394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.784394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.784394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29716 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.788394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.792394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.796394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.796394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.796394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.796394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.800394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.804394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.808394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.812394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.816394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.820394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.824394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.828394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-07 00:03:47.000000 mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 00:04:18.832394 mct-nightly-2.0.0.20240507.417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-07 00:04:17.000000 mct-nightly-2.0.0.20240507.417/setup.py
```

### Comparing `mct-nightly-2.0.0.20240506.443/LICENSE.md` & `mct-nightly-2.0.0.20240507.417/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/PKG-INFO` & `mct-nightly-2.0.0.20240507.417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240506.443
+Version: 2.0.0.20240507.417
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240506.443/README.md` & `mct-nightly-2.0.0.20240507.417/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240506.443
+Version: 2.0.0.20240507.417
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240506.443/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240507.417/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240506.000443"
+__version__ = "2.0.0.20240507.000417"
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
 
         Args:
             current_node: Node that (possibly) is an input node.
             new_node: New node to set as an input node if the current node is an input node.
 
         """
         if new_node is None:
-            Logger.critical("Cannot replace input node with a None value; new input node is required.")
+            Logger.critical("Cannot replace input node with a None value; new input node is required.")  # pragma: no cover
 
         graph_inputs = self.get_inputs()
         new_graph_inputs = copy(graph_inputs)
         if current_node in graph_inputs:
             new_graph_inputs.remove(current_node)
             new_graph_inputs.append(new_node)
         self.set_inputs(new_graph_inputs)
@@ -824,20 +824,20 @@
             entry_node (BaseNode): The entry node to create the section it starts.
             fw_impl (PruningFrameworkImplementation): Implementation of specific framework methods required for pruning.
 
         Returns: The pruning section that starts with node entry_node.
 
         """
         if not fw_impl.is_node_entry_node(entry_node):
-            Logger.critical(f"Node {entry_node} is not a valid entry node for creating a pruning section")
+            Logger.critical(f"Node {entry_node} is not a valid entry node for creating a pruning section")  # pragma: no cover
 
         intermediate_nodes, exit_node = self._find_intermediate_and_exit_nodes(entry_node, fw_impl)
 
         if not fw_impl.is_node_exit_node(exit_node, entry_node, self.fw_info):
-            Logger.critical(f"Node {exit_node} is not a valid exit node for the pruning section starting with {entry_node}.")
+            Logger.critical(f"Node {exit_node} is not a valid exit node for the pruning section starting with {entry_node}.")   # pragma: no cover
 
         return PruningSection(entry_node=entry_node,
                               intermediate_nodes=intermediate_nodes,
                               exit_node=exit_node)
 
     def _find_intermediate_and_exit_nodes(self, entry_node: BaseNode, fw_impl: Any) -> Tuple[List[BaseNode], BaseNode]:
         """
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         Args:
             node: The prunable node to update the mask for.
             channel_idx: The index of the channel to update in the mask.
             mask_indicator: The new value to set in the mask (either PRUNED or REMAINED).
         """
         if mask_indicator not in [MaskIndicator.PRUNED, MaskIndicator.REMAINED]:
-            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")
+            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")  # pragma: no cover
         self._mask[node][channel_idx] = mask_indicator.value
 
     def has_pruned_channel(self) -> bool:
         """
         Determines if there is at least one pruned channel across all nodes in the model.
 
         Returns:
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         Args:
             node: The prunable node to update the mask for.
             group_index: The index of the SIMD group to update in the mask.
             mask_indicator: The new value to set in the mask (either PRUNED or REMAINED).
         """
         if mask_indicator not in [MaskIndicator.PRUNED, MaskIndicator.REMAINED]:
-            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")
+            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")  # pragma: no cover
 
         # Update the SIMD group mask and corresponding per-channel mask
         self._mask_simd[node][group_index] = mask_indicator.value
         node_mask_indices = self.simd_groups_indices[node][group_index]
         for idx in node_mask_indices:
             self.per_channel_mask.set_mask_value_for_simd_group(node=node,
                                                                 channel_idx=idx,
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                                                    self.float_graph,
                                                    self.fw_impl,
                                                    self.target_platform_capabilities,
                                                    self.simd_groups_indices)
             mask_calculator.compute_mask()
             self.per_oc_mask = mask_calculator.get_mask()
         else:
-            Logger.critical("Only GREEDY ChannelsFilteringStrategy is currently supported.")
+            Logger.critical("Only GREEDY ChannelsFilteringStrategy is currently supported.")  # pragma: no cover
 
         Logger.info("Start pruning graph...")
         _pruned_graph = build_pruned_graph(self.float_graph,
                                            self.per_oc_mask,
                                            self.fw_info,
                                            self.fw_impl)
         return _pruned_graph
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         simd_groups_indices (Dict[BaseNode, List[np.ndarray]]): The indices of channels in each SIMD group.
 
     Returns:
         Dict[BaseNode, np.ndarray]: Expanded scores for each individual channel.
     """
     if simd_scores is None or simd_groups_indices is None:
         Logger.critical(f"Failed to find scores and indices to create unrolled scores for pruning information."
-                        f" Scores: {simd_scores}, Group indices: {simd_groups_indices}.")
+                        f" Scores: {simd_scores}, Group indices: {simd_groups_indices}.")  # pragma: no cover
     _scores = {}
     for node, groups_indices in simd_groups_indices.items():
         node_scores = simd_scores[node]
         total_indices = sum(len(group) for group in groups_indices)
         new_node_scores = np.zeros(total_indices)
 
         for group_score, group_indices in zip(node_scores, groups_indices):
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,16 @@
             Logger.warning(f"Parameter {config_parameter_name} could not be found in the node quantization config and "
                            f"was not updated!")
 
     def __repr__(self) -> str:
         """
         Returns: String to display a NodeQuantizationConfig object.
         """
-        repr_str = ''
-        for k, v in self.__dict__.items():
-            repr_str += f'{k}: {v}\n'
-        return repr_str
+        # Used for debugging, thus no cover.
+        return ''.join(f'{k}: {v}\n' for k, v in self.__dict__.items())  # pragma: no cover
 
 
 class NodeActivationQuantizationConfig(BaseNodeQuantizationConfig):
     """
     Attributes for configuring the quantization of the activations of a node.
     """
     def __init__(self,
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         self.residual_collapsing = residual_collapsing
         self.shift_negative_ratio = shift_negative_ratio
         self.shift_negative_threshold_recalculation = shift_negative_threshold_recalculation
         self.shift_negative_params_search = shift_negative_params_search
         self.concat_threshold_update = concat_threshold_update
 
     def __repr__(self):
-        return str(self.__dict__)
+        # Used for debugging, thus no cover.
+        return str(self.__dict__)  # pragma: no cover
 
 
 # Default quantization configuration the library use.
 DEFAULTCONFIG = QuantizationConfig(QuantizationErrorMethod.MSE, QuantizationErrorMethod.MSE,
                                    relu_bound_to_power_of_2=False, weights_bias_correction=True,
                                    weights_second_moment_correction=False, input_scaling=False, softmax_shift=False)
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
         quantizer_fn = symmetric_quantizer
     elif weights_quantization_method == QuantizationMethod.UNIFORM:
         quantizer_fn = uniform_quantizer
     elif weights_quantization_method in [QuantizationMethod.LUT_POT_QUANTIZER, QuantizationMethod.LUT_SYM_QUANTIZER]:
         quantizer_fn = lut_kmeans_quantizer
     else:
         Logger.critical(
-            f"No quantizer function found for the specified quantization method: {weights_quantization_method}")
+            f"No quantizer function found for the specified quantization method: {weights_quantization_method}")  # pragma: no cover
 
     return quantizer_fn
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/remove_identity.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from model_compression_toolkit.core.common.graph.base_graph import Graph, OutTensor
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
+from model_compression_toolkit.logger import Logger
 
 
 def remove_identity_node(graph: Graph,
                          node: BaseNode) -> Graph:
     """
     The method to perform the substitution of the identity node by
     reconnecting its input directly to its output, effectively removing the node
@@ -32,15 +33,17 @@
         Graph: The updated graph after removing the identity node.
     """
     # Retrieve the predecessor nodes of the identity node.
     prev_identity_nodes = graph.get_prev_nodes(node)
 
     # Ensure there is exactly one predecessor; otherwise, do nothing.
     if len(prev_identity_nodes) != 1:
-        return graph
+        # We do not expect to get here.
+        Logger.error(f"Identity node {node} have {len(prev_identity_nodes)} inputs, while expected to have one. Skipping remove identity substitution.") # pragma: no cover
+        return graph  # pragma: no cover
 
     graph_outputs = graph.get_outputs()
     for i, g_out in enumerate(graph_outputs):
         if g_out.node == node:
             graph_outputs[i] = OutTensor(node=prev_identity_nodes[0], node_out_index=g_out.node_out_index)
 
     # Reconnect the output edges of the identity node to its predecessor,
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 from model_compression_toolkit.core.common.user_info import UserInformation
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras import Input
     from keras.src.layers.core import TFOpLambda
     from keras.src.engine.base_layer import TensorFlowOpLayer, Layer
 else:
-    from keras import Input
-    from keras.layers.core import TFOpLambda
-    from keras.engine.base_layer import TensorFlowOpLayer, Layer
+    from keras import Input   # pragma: no cover
+    from keras.layers.core import TFOpLambda   # pragma: no cover
+    from keras.engine.base_layer import TensorFlowOpLayer, Layer   # pragma: no cover
 
 from typing import Any, Dict, List, Tuple, Callable
 from tensorflow.python.util.object_identity import Reference as TFReference
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Tuple, Any, Dict, Union, List
 
 from packaging import version
 import tensorflow as tf
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.engine.base_layer import Layer
 else:
-    from keras.engine.base_layer import Layer
+    from keras.engine.base_layer import Layer  # pragma: no cover
 
 from keras.models import Model
 from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder, QuantizationTarget
 from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
 from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
 from model_compression_toolkit.core.common import BaseNode
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from model_compression_toolkit.core.keras.quantizer.lut_fake_quant import activation_lut_kmean_quantizer
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
 else:
-    from keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
+    from keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU  # pragma: no cover
 
 from model_compression_toolkit.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.constants import SOFTMAX_THRESHOLD
 from model_compression_toolkit.core.keras.constants import SOFTMAX, LINEAR, RELU, SWISH, SIGMOID, IDENTITY, TANH, SELU, \
     KERNEL, DEPTHWISE_KERNEL
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Returns:
             Graph after applying the substitution.
         """
 
         if ACTIVATION not in op2d_node.framework_attr:
             Logger.warning(f'Op2d node {op2d_node.name} of type {op2d_node.type} is missing an "{ACTIVATION}"'
                            f' attribute -> Skipping substitution ActivationDecomposition')  # pragma: no cover
-            return graph
+            return graph  # pragma: no cover
 
         activation_node_name = op2d_node.name + '_post_activation'
 
         # Softmax is a special case where we need to know the default axis parameter used
         # and for this reason we create a Softmax layer and not Activation layer.
         if op2d_node.framework_attr.get(ACTIVATION) == SOFTMAX:
             activation_fw_attr = {AXIS: SOFTMAX_AXIS_DEFAULT}
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             if bias2 is not None:
                 bias_collapsed += bias2
         elif bias2 is not None:
             bias_collapsed = bias2
 
         return kernel_collapsed, bias_collapsed
     else:
-        Logger.critical(f"Layer collapsing unsupported for combination: {first_node.type} and {second_node.type}.")
+        Logger.critical(f"Layer collapsing unsupported for combination: {first_node.type} and {second_node.type}.")  # pragma: no cover
 
 
 def keras_linear_collapsing() -> Conv2DCollapsing:
     """
     Returns:
         A Conv2DCollapsing initialized for Keras models.
     """
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         idxH = (kH - 1) // 2
         idxW = (kW - 1) // 2
         for i in range(Cout):
             kernel[idxH, idxW, i, i] += 1
 
         return kernel
     else:
-        Logger.critical(f"Residual collapsing is unsupported for {first_node.type} node types.")
+        Logger.critical(f"Residual collapsing is unsupported for {first_node.type} node types.")  # pragma: no cover
 
 
 def keras_residual_collapsing() -> ResidualCollapsing:
     """
     Returns:
         A ResidualCollapsing initialized for Keras models.
     """
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 
 from packaging import version
 import tensorflow as tf
 from tensorflow.python.keras.layers.core import TFOpLambda
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Activation, Conv2D, Dense, DepthwiseConv2D, ZeroPadding2D, Reshape, \
-        GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU
+        GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU  # pragma: no cover
 else:
     from tensorflow.keras.layers import Activation, Conv2D, Dense, DepthwiseConv2D, ZeroPadding2D, Reshape, \
         GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU
 
 from model_compression_toolkit.core import CoreConfig, FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,10 +70,10 @@
         _unfold_tensors = self.unfold_tensors_list(tensors_to_concate)
         _r_tensors = [tf.reshape(tensor, shape=[tensor.shape[0], -1]) for tensor in _unfold_tensors]
 
         # Ensure all tensors have the same shape for concatenation
         concat_axis_dim = [o.shape[0] for o in _r_tensors]
         if not all(d == concat_axis_dim[0] for d in concat_axis_dim):
             Logger.critical(
-                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")# pragma: no cover
+                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.") # pragma: no cover
 
         return tf.concat(_r_tensors, axis=1)
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,19 @@
 from model_compression_toolkit.core.keras.mixed_precision.configurable_weights_quantizer import \
     ConfigurableWeightsQuantizer
 from model_compression_toolkit.core.keras.statistics_correction.apply_second_moment_correction import \
     keras_apply_second_moment_correction
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
-    from keras.src.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, \
-        Concatenate, Add
+    from keras.src.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add
     from keras.src.layers.core import TFOpLambda
 else:
-    from keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, \
-        Concatenate, Add
-    from keras.layers.core import TFOpLambda
+    from keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add   # pragma: no cover
+    from keras.layers.core import TFOpLambda   # pragma: no cover
 
 from model_compression_toolkit.core import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfig
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
@@ -485,15 +483,15 @@
         elif trace_hessian_request.mode == HessianMode.WEIGHTS:
             return WeightsTraceHessianCalculatorKeras(graph=graph,
                                                       trace_hessian_request=trace_hessian_request,
                                                       input_images=input_images,
                                                       fw_impl=self,
                                                       num_iterations_for_approximation=num_iterations_for_approximation)
         else:
-            Logger.critical(f"Unsupported Hessian mode for Keras: {trace_hessian_request.mode}.")
+            Logger.critical(f"Unsupported Hessian mode for Keras: {trace_hessian_request.mode}.")   # pragma: no cover
 
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> Any:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
 
         Args:
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import tensorflow as tf
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Activation, ReLU, BatchNormalization
 else:
-    from keras.layers import Activation, ReLU, BatchNormalization
+    from keras.layers import Activation, ReLU, BatchNormalization  # pragma: no cover
 
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.keras.constants import ACTIVATION, RELU_MAX_VALUE, NEGATIVE_SLOPE, THRESHOLD, \
     GAMMA, BETA, MOVING_MEAN, MOVING_VARIANCE
 from model_compression_toolkit.core.common.graph.base_graph import Graph
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 import numpy as np
 from tensorflow.python.util.object_identity import Reference as TFReference
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 
+################################################################
+################################################################
+# TODO:
+#  These quantizer functions are for internal use. They are currently
+#  used in some features like MP for activation and SNC (where
+#  inference in the framework is needed).
+#  It may worth considering removing these functions and use
+#  activation inferable quantizers in those features like we do
+#  in GPTQ.
+################################################################
+################################################################
 
 def quantizer_min_max_calculator(threshold: np.ndarray,
                                  num_bits: int,
                                  signed: bool) -> Tuple[float, float]:
     """
     Compute quantization range's min/max values given a threshold, number of bits,
      and whether it's signed or not.
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.engine.input_layer import InputLayer
     from keras.src.engine.node import Node as KerasNode
     from keras.src.engine.functional import Functional
     from keras.src.engine.sequential import Sequential
 else:
-    from keras.engine.input_layer import InputLayer
-    from keras.engine.node import Node as KerasNode
-    from keras.engine.functional import Functional
-    from keras.engine.sequential import Sequential
+    from keras.engine.input_layer import InputLayer # pragma: no cover
+    from keras.engine.node import Node as KerasNode # pragma: no cover
+    from keras.engine.functional import Functional # pragma: no cover
+    from keras.engine.sequential import Sequential # pragma: no cover
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 def is_node_an_input_layer(node: BaseNode) -> bool:
     """
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,50 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2024 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import copy
 import torch
-from torch.nn import Module
 
-from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.pytorch.utils import set_model
+from model_compression_toolkit.core.common.substitutions.remove_identity import remove_identity_node
+from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
+from model_compression_toolkit.core import common
+from model_compression_toolkit.core.common.graph.base_graph import Graph
+from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
-def node_builder(n: BaseNode) -> Module:
+class RemoveIdentity(common.BaseSubstitution):
     """
-    Build a Pytorch module from a node.
-
-    Args:
-        n: Node to build its Pytorch layer
-
-    Returns:
-        Pytorch module that was built from the node.
+    Remove `torch.nn.Identity` layers from the graph.
     """
 
-    framework_attr = copy.copy(n.framework_attr)
-    node_instance = n.type(**framework_attr)
-    node_instance.load_state_dict({k: torch.tensor(v) for k, v in n.weights.items()}, strict=False)
-    set_model(node_instance)
-    return node_instance
-
-
-# todo: remove. It is not used anymore
-def identity_wrapper(node: BaseNode,
-                     module: Module,
-                     include_activation_quantizers: bool):
-    """
-    A function which takes a computational graph node and a pytorch module and return an identity wrapping which return the layer itself
-    Args:
-        node: A node of mct graph.
-        layer: A pytorch module
-        include_activation_quantizers: bool flag.
-    Returns: pytorch module
-    """
-    return module
+    def __init__(self):
+        nodes = NodeOperationMatcher(torch.nn.Identity)
+        super().__init__(matcher_instance=nodes)
+
+    def substitute(self,
+                   graph: Graph,
+                   node: BaseNode) -> Graph:
+        """
+        The method to perform the substitution of the `torch.nn.Identity` node by
+        reconnecting its input directly to its output, effectively removing the node
+        from the graph.
+
+        Args:
+            graph: The current graph of operations where the node resides.
+            node: The specific `BaseNode` that is matched to be an Identity operation.
+
+        Returns:
+            Graph: The updated graph after removing the identity node.
+        """
+        return remove_identity_node(graph, node)
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder, identity_wrapper
+from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.pytorch_device_config import get_working_device
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER
 from mct_quantizers import PytorchQuantizationWrapper
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if bias2 is not None:
                 bias_collapsed += bias2
         elif bias2 is not None:
             bias_collapsed = bias2
 
         return kernel_collapsed, bias_collapsed
     else:
-        Logger.critical(f"Layer collapsing is not supported for the combination of {first_node.type} and {second_node.type}.")
+        Logger.critical(f"Layer collapsing is not supported for the combination of {first_node.type} and {second_node.type}.")  # pragma: no cover
 
 
 def pytorch_linear_collapsing() -> Conv2DCollapsing:
     """
     Returns:
         A Conv2DCollapsing initialized for pytorch models.
     """
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,73 @@
-# Copyright 2024 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from typing import Tuple
+import numpy as np
 import torch
-
-from model_compression_toolkit.core.common.substitutions.remove_identity import remove_identity_node
+from torch.nn import Conv2d
+from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common.graph.base_graph import Graph
-from model_compression_toolkit.core.common.graph.base_node import BaseNode
+from model_compression_toolkit.core.common.substitutions.residual_collapsing import ResidualCollapsing
+from model_compression_toolkit.core.pytorch.constants import KERNEL
+from model_compression_toolkit.logger import Logger
 
 
-class RemoveIdentity(common.BaseSubstitution):
+def residual_collapsing_node_matchers() -> Tuple[NodeOperationMatcher, NodeOperationMatcher]:
     """
-    Remove `torch.nn.Identity` layers from the graph.
+    Function generates matchers for matching:
+    (Conv2D, Add)[activation=linear] -> Conv2D.
+    Returns:
+        Matcher for Conv2D node and Add node
     """
+    first_node = NodeOperationMatcher(Conv2d)
+    second_node = NodeOperationMatcher(torch.add)
+    return first_node, second_node
 
-    def __init__(self):
-        nodes = NodeOperationMatcher(torch.nn.Identity)
-        super().__init__(matcher_instance=nodes)
-
-    def substitute(self,
-                   graph: Graph,
-                   node: BaseNode) -> Graph:
-        """
-        The method to perform the substitution of the `torch.nn.Identity` node by
-        reconnecting its input directly to its output, effectively removing the node
-        from the graph.
 
-        Args:
-            graph: The current graph of operations where the node resides.
-            node: The specific `BaseNode` that is matched to be an Identity operation.
-
-        Returns:
-            Graph: The updated graph after removing the identity node.
-        """
-        return remove_identity_node(graph, node)
+def residual_collapsing_fn(first_node: BaseNode,
+                           kernel_str: str) -> np.ndarray:
+    """
+    Collapsing residual addition into convolution
+    Inspired by https://arxiv.org/pdf/2103.09404.pdf - Algorithm2
+    Args:
+        first_node: First layer node to collapse into.
+        kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
+    Returns:
+        The modified layer node's weights: kernel
+    """
+    if first_node.is_match_type(Conv2d):
+        # Get nodes attributes
+        kernel = first_node.get_weights_by_keys(kernel_str)
+        (Cout, Cin, kH, kW) = kernel.shape
+
+        # Collapsing residual by adding "1" to kernel diagonal
+        idxH = (kH - 1) // 2
+        idxW = (kW - 1) // 2
+        for i in range(Cout):
+            kernel[i, i, idxH, idxW] += 1
+        return kernel
+    else:
+        Logger.critical(f"Residual collapsing not supported for node type: {first_node.type}")  # pragma: no cover
 
 
+def pytorch_residual_collapsing() -> ResidualCollapsing:
+    """
+    Returns:
+        A ResidualCollapsing initialized for pytorch models.
+    """
+    first_node, second_node = residual_collapsing_node_matchers()
+    return ResidualCollapsing(first_node,
+                              second_node,
+                              residual_collapsing_fn,
+                              KERNEL)
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,10 +61,10 @@
         """
         _unfold_tensors = self.unfold_tensors_list(tensors_to_concate)
         _r_tensors = [torch.reshape(tensor, shape=[tensor.shape[0], -1]) for tensor in _unfold_tensors]
 
         concat_axis_dim = [o.shape[0] for o in _r_tensors]
         if not all(d == concat_axis_dim[0] for d in concat_axis_dim):
             Logger.critical(
-                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")
+                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")  # pragma: no cover
 
         return torch.concat(_r_tensors, dim=1)
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,24 @@
                 # 'cuda' without a specific index is valid if CUDA is available
                 return True, "Valid device"
 
             try:
                 device_index = int(device_name.split(':')[1])
                 if device_index >= torch.cuda.device_count():
                     return False, f"CUDA device index {device_index} out of range. Number of valid devices: {torch.cuda.device_count()}"
-            except IndexError:
+            except Exception:
                 # Handle cases where the device name is incorrectly formatted
                 return False, "Invalid CUDA device format. Use 'cuda' or 'cuda:x' where x is the device index."
 
             return True, "Valid device"
 
-        return True, "Valid device"
+        if CPU in device_name:
+            return True, "Valid device"
+
+        return False, "Invalid device"
 
 
 
 def set_working_device(device_name: str):
     """
     Set the device for PyTorch operations.
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,26 @@
 import torch
 
 from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import fix_range_to_include_zero
 
 
+################################################################
+################################################################
+# TODO:
+#  These quantizer functions are for internal use. They are currently
+#  used in some features like MP for activation and SNC (where
+#  inference in the framework is needed).
+#  It may worth considering removing these functions and use
+#  activation inferable quantizers in those features like we do
+#  in GPTQ.
+################################################################
+################################################################
+
 def get_symmetric_quantization_range_and_scale(activation_is_signed: bool,
                                                activation_n_bits: int,
                                                activation_threshold: float):
     """
     Calculates lower and upper bounds on the quantization range, along with quantization scale,
     for symmetric quantization (used for the symmetric and power-of-two quantizers),
     according to whether the quantization is signed or unsigned.
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/core/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from typing import Callable, Tuple, Any, List, Dict
 
 import numpy as np
 
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common.hessian.hessian_info_service import HessianInfoService
+from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization_data import \
+    requires_mixed_precision
 from model_compression_toolkit.core.graph_prep_runner import graph_preparation_runner
 from model_compression_toolkit.core.quantization_prep_runner import quantization_preparation_runner
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.mixed_precision.bit_width_setter import set_bit_widths
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization, RUTarget
@@ -85,15 +87,24 @@
                        ' consider increasing the batch size')
 
     # Checking whether to run mixed precision quantization
     if target_resource_utilization is not None:
         if core_config.mixed_precision_config is None:
             Logger.critical("Provided an initialized target_resource_utilization, that means that mixed precision quantization is "
                             "enabled, but the provided MixedPrecisionQuantizationConfig is None.")
-        core_config.mixed_precision_config.set_mixed_precision_enable()
+        # Determine whether to use mixed precision or single precision based on target_resource_utilization.
+        if requires_mixed_precision(in_model,
+                                    target_resource_utilization,
+                                    representative_data_gen,
+                                    core_config,
+                                    tpc,
+                                    fw_info,
+                                    fw_impl):
+            core_config.mixed_precision_config.set_mixed_precision_enable()
+            Logger.info('Mixed precision enabled.')
 
     graph = graph_preparation_runner(in_model,
                                      representative_data_gen,
                                      core_config.quantization_config,
                                      fw_info,
                                      fw_impl,
                                      tpc,
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
         Args:
             model (Any): The framework model.
             bn_layer_types (List): List of batch normalization layer types.
         """
         self.bn_params = self.get_bn_params(model, bn_layer_types)
         if self.get_num_bn_layers() == 0:
-            Logger.critical(
-                f'Data generation requires a model with at least one BatchNorm layer.')
+            Logger.critical(f'Data generation requires a model with at least one BatchNorm layer.')
 
     def get_bn_layer_names(self) -> List[str]:
         """
         Get the names of all batch normalization layers.
 
         Returns:
             List[str]: List of batch normalization layer names.
@@ -101,15 +100,15 @@
         Args:
             model (Any): The model.
             bn_layer_types (List): List of batch normalization layer types.
 
         Returns:
             dict: Dictionary mapping batch normalization layer names to their parameters.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
 
 class ActivationExtractor:
     """
     Extracts activations of input tensors to layers in a model.
     """
 
@@ -119,48 +118,48 @@
         """
         Initializes the ActivationExtractor.
 
         Args:
             model (Any): The model.
             layer_types_to_extract_inputs (List): Tuple or list of layer types.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_layer_input_activation(self, layer_name: str) -> Any:
         """
         Get the input activation tensor of a layer.
 
         Args:
             layer_name (str): Name of the layer.
 
         Returns:
             Any: Input activation tensor of the layer.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_output_layer_input_activation(self) -> List:
         """
         Get the input activation tensors of all the output layers that are Linear or Conv2d.
 
         Returns:
             Any: Input activation tensors of all the output layers that are Linear or Conv2d.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_last_linear_layers_weights(self) -> List:
         """
         Get the weight tensors of all the last linear layers.
 
         Returns:
             List: Weight tensors of all the last linear layers.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     def get_num_extractor_layers(self) -> int:
         """
         Get the number of layers for which to extract input activations.
 
         Returns:
             int: Number of layers for which to extract input activations.
@@ -171,35 +170,35 @@
     def get_extractor_layer_names(self) -> List:
         """
         Get a list of the layer names for which to extract input activations.
 
         Returns:
             List: A list of layer names for which to extract input activations.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def clear(self):
         """
         Clear the stored activation tensors.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def remove(self):
         """
         Remove the hooks from the model.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def run_model(self, inputs: Any) -> Any:
         """
         Run the model on the given inputs and return the output.
 
         Args:
             inputs (Any): Input tensor.
 
         Returns:
             Any: Output tensor.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         Args:
             layer_name (str): the name of the layer.
 
         Returns:
             Tuple[Any, Any]: the averaged activation statistics on all the batches for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def compute_bn_loss(self,
                         input_imgs: Any,
                         batch_index: int,
                         activation_extractor: ActivationExtractor,
                         orig_bn_stats_holder: OriginalBNStatsHolder,
                         bn_alignment_loss_fn: Callable,
@@ -241,35 +241,35 @@
         Perform an optimization step.
 
         Args:
             batch_index (int): Index of the batch.
             loss (Any): The loss value.
             i_ter (int): The current iteration.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     @abstractmethod
     def zero_grad(self, batch_index: int):
         """
         Zero the gradients of the optimizer for the specified batch.
 
         Args:
             batch_index (int): Index of the batch.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     @abstractmethod
     def get_finalized_images(self) -> list:
         """
         Create and return a list of the generated images.
 
         Returns:
             list: a list of the generated images.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
 
 class BatchOptimizationHolder:
     """
     Holds optimization parameters for a batch of images.
 
     This class acts as a container for optimization-related parameters specific to a batch of images. It does not
@@ -287,15 +287,15 @@
 
         Args:
             images (Any): a tensor containing the input images.
             optimizer (Any): optimizer responsible for updating the image parameters during optimization.
             scheduler (Any): scheduler responsible for adjusting the learning rate of the optimizer over time.
             initial_lr (float): the initial learning rate used by the optimizer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def get_images(self) -> Any:
         """Returns the stored images"""
         return self.images
 
     def get_optimizer(self) -> Any:
         """Returns the optimizer"""
@@ -340,15 +340,15 @@
     def get_batches_stats_holder_list(self) -> list:
         """
         Get a list of batches stats holders.
 
         Returns:
             list: List of batches stats holders.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def update_batch_stats(self,
                            batch_index: int,
                            input_imgs: Any,
                            activation_extractor: ActivationExtractor,
                            to_differentiate=False):
         """
@@ -438,27 +438,27 @@
 
         Args:
             bn_layer_name (str): the name of the layer.
 
         Returns:
             Any: the variance for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def get_std(self, bn_layer_name: str) -> Any:
         """
         Calculate the standart deviation for the specified layer.
 
         Args:
             bn_layer_name (str): the name of the layer.
 
         Returns:
             Any: the variance for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def update_layer_stats(self,
                            bn_layer_name: str,
                            mean: Any,
                            second_moment: Any):
         """
         Update the statistics for a layer.
@@ -479,15 +479,15 @@
         Calculate statistics from the input images and activation extractor.
 
         Args:
             input_imgs (Any): the input images tensor for which to calculate the statistics.
             activation_extractor (ActivationExtractor): the activation extractor object.
             to_differentiate (bool): a flag indicating whether to differentiate or not.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def clear(self):
         """Clear the statistics."""
         self.bn_mean.clear()
         self.bn_second_moment.clear()
         self.bn_mean = {}
         self.bn_second_moment = {}
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                                                                        append2output=self.compare_points,
                                                                        fw_info=self.fw_info)
 
         self.fxp_model, self.gptq_user_info = self.build_gptq_model()
         if self.gptq_config.use_hessian_based_weights:
             if not isinstance(hessian_info_service, HessianInfoService):
                 Logger.critical(f"When using Hessian-based approximations for sensitivity evaluation, "
-                                f"an 'HessianInfoService' object must be provided, but received: {hessian_info_service}.")
+                                f"an 'HessianInfoService' object must be provided, but received: {hessian_info_service}.")   # pragma: no cover
             self.hessian_service = hessian_info_service
 
     def get_optimizer_with_param(self,
                                  flattened_trainable_weights: List[Any],
                                  flattened_bias_weights: List[Any],
                                  trainable_quantization_parameters: List[Any]) -> List[Any]:
         """
@@ -234,55 +234,20 @@
         """
         Validates the structure and length of the trace approximation.
 
         Args:
             trace_approx: Trace approximation to validate.
         """
         if not isinstance(trace_approx, list):
-            Logger.critical(f"Trace approximation was expected to be a list but is of type: {type(trace_approx)}.")
+            Logger.critical(f"Trace approximation was expected to be a list but is of type: {type(trace_approx)}.")   # pragma: no cover
         if len(trace_approx) != 1:
             Logger.critical(f"Trace approximation was expected to have a length of 1 "
                             f"(for computations with granularity set to 'HessianInfoGranularity.PER_TENSOR') "
                             f"but has a length of {len(trace_approx)}."
-            )
-
-    @staticmethod
-    def _generate_images_batch(representative_data_gen: Callable, num_samples_for_loss: int) -> np.ndarray:
-        """
-        Construct batches of image samples for inference.
-
-        Args:
-            representative_data_gen: A callable method to retrieve images from Dataset.
-            num_samples_for_loss: Num of total images for evaluation.
-
-        Returns: A tensor of images batches
-        """
-        # First, select images to use for all measurements.
-        samples_count = 0  # Number of images we used so far to compute the distance matrix.
-        images = []
-        for inference_batch_input in representative_data_gen():
-            if samples_count >= num_samples_for_loss:
-                break
-            num_images = inference_batch_input[0].shape[0]
-
-            # If we sampled more images than we should,
-            # we take only a subset of these images and use only them.
-            if num_images > num_samples_for_loss - samples_count:
-                inference_batch_input = [x[:num_samples_for_loss - samples_count] for x in inference_batch_input]
-                assert num_samples_for_loss - samples_count == inference_batch_input[0].shape[0]
-                num_images = num_samples_for_loss - samples_count
-
-            images.append(inference_batch_input[0])
-            samples_count += num_images
-        else:
-            if samples_count < num_samples_for_loss:
-                Logger.warning(f'Not enough images in representative dataset to generate {num_samples_for_loss} data points, '
-                               f'only {samples_count} were generated')
-
-        return np.concatenate(images, axis=0)
+            )   # pragma: no cover
 
 
     @abstractmethod
     def build_gptq_model(self):
         """
         Build the GPTQ model with QuantizationWrappers
         Returns:
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/metadata.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,13 +78,10 @@
                 if quantizer_parameter.trainable and parameter_group == group:
                     quantizer_trainable.append(quantizer_parameter)
             return quantizer_trainable
 
 
 else:
     class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
-        def __init__(self,
-                     quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
-
-            super().__init__(quantization_config)
+        def __init__(self, *args, **kwargs):
             Logger.critical("Tensorflow must be installed to use BaseKerasTrainableQuantizer. "
                             "The 'tensorflow' package is missing.")  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240506.443/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240507.417/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,11 @@
                 quantizer_parameter, parameter_group = parameter_dict[VAR], parameter_dict[GROUP]
                 if quantizer_parameter.requires_grad and parameter_group == group:
                     quantizer_trainable.append(quantizer_parameter)
             return quantizer_trainable
 
 else:
     class BasePytorchTrainableQuantizer(BaseTrainableQuantizer):
-        def __init__(self,
-                     quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
-            super().__init__(quantization_config)
+        def __init__(self, *args, **kwargs):
             Logger.critical("PyTorch must be installed to use 'BasePytorchTrainableQuantizer'. "
                             "The 'torch' package is missing.")  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240506.443/setup.py` & `mct-nightly-2.0.0.20240507.417/setup.py`

 * *Files identical despite different names*

