# Comparing `tmp/mct-nightly-2.0.0.20240522.172031.tar.gz` & `tmp/mct-nightly-2.0.0.20240522.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240522.172031.tar", last modified: Wed May 22 17:20:32 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240522.420.tar", last modified: Wed May 22 00:04:20 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240522.172031.tar` & `mct-nightly-2.0.0.20240522.420.tar`

### file list

```diff
@@ -1,607 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.057306 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.057306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.057306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.057306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.057306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.061306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20896 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.061306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.061306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29722 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.061306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.065306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.065306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.065306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28940 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.069306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.073306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.073306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.077306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.077306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.077306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.081306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.081306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.081306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.081306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.085306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.085306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.085306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.085306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.085306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.089306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.089306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.089306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.089306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.089306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.093306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.093306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.093306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.093306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27516 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.097306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.101306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.105306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.109306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.113306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.117306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.121306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.125306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-22 17:20:01.000000 mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 17:20:32.129306 mct-nightly-2.0.0.20240522.172031/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 17:20:31.000000 mct-nightly-2.0.0.20240522.172031/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.743753 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.743753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.743753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.747753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.747753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.747753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.747753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.751753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.751753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.751753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.751753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.755753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.755753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.755753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.755753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.759753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.759753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.759753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.759753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.763753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.763753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.763753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.767753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.767753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.767753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.771752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.771752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.771752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29716 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.775753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.779753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.779753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.779753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.779753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.783753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.783753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.783753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.783753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.783753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.787752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.791752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.795752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.799752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.803753 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.807752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.811752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.815752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-22 00:03:49.000000 mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 00:04:20.819752 mct-nightly-2.0.0.20240522.420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 00:04:20.000000 mct-nightly-2.0.0.20240522.420/setup.py
```

### Comparing `mct-nightly-2.0.0.20240522.172031/LICENSE.md` & `mct-nightly-2.0.0.20240522.420/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/PKG-INFO` & `mct-nightly-2.0.0.20240522.420/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,199 +1,185 @@
-Metadata-Version: 2.1
-Name: mct-nightly
-Version: 2.0.0.20240522.172031
-Summary: A Model Compression Toolkit for neural networks
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # Model Compression Toolkit (MCT)
-        
-        Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
-        
-        This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
-        
-        Specifically, this project aims to apply quantization to compress neural networks.
-        
-        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
-        
-        MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
-        
-        
-        
-        ## Table of Contents
-        
-        - [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
-        - [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
-        - [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
-        - [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
-        - [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
-        - [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
-        
-        
-        ## Getting Started
-        
-        This section provides an installation and a quick starting guide.
-        
-        ### Installation
-        
-        To install the latest stable release of MCT, run the following command:
-        ```
-        pip install model-compression-toolkit
-        ```
-        
-        For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
-        
-        
-        ### Quick start & tutorials 
-        
-        Explore the Model Compression Toolkit (MCT) through our tutorials, 
-        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
-        for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
-        * [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
-        
-        
-        ### Supported Versions
-        
-        Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
-        
-        |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
-        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
-        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
-        | Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
-        
-        
-        |             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
-        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
-        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
-        | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
-        
-        
-        ## Supported Features
-        MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
-        
-        ### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-        MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
-        
-        ### Quantization
-        MCT supports different quantization methods:
-        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
-        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-        * Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-        
-        
-        | Quantization Method                           | Complexity | Computational Cost          |
-        |-----------------------------------------------|------------|-----------------------------|
-        | PTQ                                           | Low        | Low (order of minutes)      |
-        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
-        | QAT                                           | High       | High (order of 12-36 hours) |
-        
-        
-        In addition, MCT supports different quantization schemes for quantizing weights and activations:
-        
-        * Power-Of-Two (hardware-friendly quantization [1])
-        * Symmetric
-        * Uniform
-        
-        Main features:
-        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
-        
-        ### Enhanced Post-Training Quantization (EPTQ)
-        As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
-        
-        The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
-        
-        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
-        
-        
-        ### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-        MCT introduces a structured and hardware-aware model pruning.
-        This pruning technique is designed to compress models for specific hardware architectures, 
-        taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
-        By pruning groups of channels (SIMD groups), our approach not only reduces model size 
-        and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
-        for a target Resource Utilization of weights memory footprint.
-        [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
-        [Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
-        
-        #### Experimental features 
-        
-        Some features are experimental and subject to future changes. 
-         
-        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-        
-        
-        ## Results
-        ### Keras
-        Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
-        single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
-        
-        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
-        
-        For more results, please see [1]
-        
-        ### Pytorch
-        We quantized classification networks from the torchvision library. 
-        In the following table we present the ImageNet validation results for these models:
-        
-        | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
-        |---------------------------|-----------------|-----------------|-------------------------|
-        | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
-        | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
-        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
-        
-        
-        #### Pruning Results
-        
-        Results for applying pruning to reduce the parameters of the following models by 50%:
-        
-        | Model           | Dense Model Accuracy | Pruned Model Accuracy |
-        |-----------------|----------------------|-----------------------|
-        | ResNet50 [2]    | 75.1                 | 72.4                  |
-        | DenseNet121 [3] | 74.44                | 71.71                 |
-        
-        
-        ## Trouble Shooting
-        
-        If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
-        for common pitfalls and some tools to improve quantization accuracy.
-        
-        Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
-        
-        
-        ## Contributions
-        MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
-        
-        *You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
-        
-        
-        ## License
-        [Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
-        
-        ## References 
-        
-        [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
-        
-        [2] [Keras Applications](https://keras.io/api/applications/)
-        
-        [3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
-        
-        [4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# Model Compression Toolkit (MCT)
+
+Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
+
+This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
+
+Specifically, this project aims to apply quantization to compress neural networks.
+
+<img src="docsrc/images/mct_block_diagram.svg" width="10000">
+
+MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
+
+
+
+## Table of Contents
+
+- [Getting Started](#getting-started)
+- [Supported features](#supported-features)
+- [Results](#results)
+- [Troubleshooting](#trouble-shooting)
+- [Contributions](#contributions)
+- [License](#license)
+
+
+## Getting Started
+
+This section provides an installation and a quick starting guide.
+
+### Installation
+
+To install the latest stable release of MCT, run the following command:
+```
+pip install model-compression-toolkit
+```
+
+For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
+
+
+### Quick start & tutorials 
+
+Explore the Model Compression Toolkit (MCT) through our tutorials, 
+covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
+for hands-on learning. For example:
+* [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+* [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+* [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+
+
+### Supported Versions
+
+Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
+
+|             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
+|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
+| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
+| Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
+
+
+|             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
+|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
+| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
+| Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
+
+
+## Supported Features
+MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
+
+### Data Generation [*](#experimental-features)
+MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
+You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
+
+### Quantization
+MCT supports different quantization methods:
+* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
+* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
+* Quantization-aware training (QAT) [*](#experimental-features)
+
+
+| Quantization Method                           | Complexity | Computational Cost          |
+|-----------------------------------------------|------------|-----------------------------|
+| PTQ                                           | Low        | Low (order of minutes)      |
+| GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+| QAT                                           | High       | High (order of 12-36 hours) |
+
+
+In addition, MCT supports different quantization schemes for quantizing weights and activations:
+
+* Power-Of-Two (hardware-friendly quantization [1])
+* Symmetric
+* Uniform
+
+Main features:
+* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+
+### Enhanced Post-Training Quantization (EPTQ)
+As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
+
+The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
+
+More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
+
+
+### Structured Pruning [*](#experimental-features)
+MCT introduces a structured and hardware-aware model pruning.
+This pruning technique is designed to compress models for specific hardware architectures, 
+taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
+By pruning groups of channels (SIMD groups), our approach not only reduces model size 
+and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
+for a target Resource Utilization of weights memory footprint.
+[Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
+[Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
+
+#### Experimental features 
+
+Some features are experimental and subject to future changes. 
+ 
+For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
+
+
+## Results
+### Keras
+Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
+single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
+
+<img src="docsrc/images/mbv2_accuracy_graph.png">
+
+For more results, please see [1]
+
+### Pytorch
+We quantized classification networks from the torchvision library. 
+In the following table we present the ImageNet validation results for these models:
+
+| Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
+|---------------------------|-----------------|-----------------|-------------------------|
+| MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
+| ResNet-18 [3]             | 69.86           | 69.63           |69.53|
+| SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
+
+
+#### Pruning Results
+
+Results for applying pruning to reduce the parameters of the following models by 50%:
+
+| Model           | Dense Model Accuracy | Pruned Model Accuracy |
+|-----------------|----------------------|-----------------------|
+| ResNet50 [2]    | 75.1                 | 72.4                  |
+| DenseNet121 [3] | 74.44                | 71.71                 |
+
+
+## Trouble Shooting
+
+If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
+for common pitfalls and some tools to improve quantization accuracy.
+
+Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
+
+
+## Contributions
+MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
+
+*You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
+
+
+## License
+[Apache License 2.0](LICENSE.md).
+
+## References 
+
+[1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
+
+[2] [Keras Applications](https://keras.io/api/applications/)
+
+[3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
+
+[4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
```

### Comparing `mct-nightly-2.0.0.20240522.172031/README.md` & `mct-nightly-2.0.0.20240522.420/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,185 +1,199 @@
-# Model Compression Toolkit (MCT)
-
-Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
-
-This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
-
-Specifically, this project aims to apply quantization to compress neural networks.
-
-<img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
-
-MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
-
-
-
-## Table of Contents
-
-- [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
-- [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
-- [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
-- [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
-- [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
-- [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
-
-
-## Getting Started
-
-This section provides an installation and a quick starting guide.
-
-### Installation
-
-To install the latest stable release of MCT, run the following command:
-```
-pip install model-compression-toolkit
-```
-
-For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
-
-
-### Quick start & tutorials 
-
-Explore the Model Compression Toolkit (MCT) through our tutorials, 
-covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
-for hands-on learning. For example:
-* [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
-* [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
-* [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
-
-
-### Supported Versions
-
-Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
-
-|             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
-| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
-| Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
-
-
-|             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
-| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
-| Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
-
-
-## Supported Features
-MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
-
-### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
-
-### Quantization
-MCT supports different quantization methods:
-* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
-* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-* Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-
-
-| Quantization Method                           | Complexity | Computational Cost          |
-|-----------------------------------------------|------------|-----------------------------|
-| PTQ                                           | Low        | Low (order of minutes)      |
-| GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
-| QAT                                           | High       | High (order of 12-36 hours) |
-
-
-In addition, MCT supports different quantization schemes for quantizing weights and activations:
-
-* Power-Of-Two (hardware-friendly quantization [1])
-* Symmetric
-* Uniform
-
-Main features:
-* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
-
-### Enhanced Post-Training Quantization (EPTQ)
-As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
-
-The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
-
-More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
-
-
-### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
-MCT introduces a structured and hardware-aware model pruning.
-This pruning technique is designed to compress models for specific hardware architectures, 
-taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
-By pruning groups of channels (SIMD groups), our approach not only reduces model size 
-and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
-for a target Resource Utilization of weights memory footprint.
-[Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
-[Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
-
-#### Experimental features 
-
-Some features are experimental and subject to future changes. 
- 
-For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-
-
-## Results
-### Keras
-Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
-single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
-
-<img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
-
-For more results, please see [1]
-
-### Pytorch
-We quantized classification networks from the torchvision library. 
-In the following table we present the ImageNet validation results for these models:
-
-| Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
-|---------------------------|-----------------|-----------------|-------------------------|
-| MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
-| ResNet-18 [3]             | 69.86           | 69.63           |69.53|
-| SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
-
-
-#### Pruning Results
-
-Results for applying pruning to reduce the parameters of the following models by 50%:
-
-| Model           | Dense Model Accuracy | Pruned Model Accuracy |
-|-----------------|----------------------|-----------------------|
-| ResNet50 [2]    | 75.1                 | 72.4                  |
-| DenseNet121 [3] | 74.44                | 71.71                 |
-
-
-## Trouble Shooting
-
-If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
-for common pitfalls and some tools to improve quantization accuracy.
-
-Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
-
-
-## Contributions
-MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
-
-*You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
-
-
-## License
-[Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
-
-## References 
-
-[1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
-
-[2] [Keras Applications](https://keras.io/api/applications/)
-
-[3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
-
-[4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
+Metadata-Version: 2.1
+Name: mct-nightly
+Version: 2.0.0.20240522.420
+Summary: A Model Compression Toolkit for neural networks
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # Model Compression Toolkit (MCT)
+        
+        Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
+        
+        This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
+        
+        Specifically, this project aims to apply quantization to compress neural networks.
+        
+        <img src="docsrc/images/mct_block_diagram.svg" width="10000">
+        
+        MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
+        
+        
+        
+        ## Table of Contents
+        
+        - [Getting Started](#getting-started)
+        - [Supported features](#supported-features)
+        - [Results](#results)
+        - [Troubleshooting](#trouble-shooting)
+        - [Contributions](#contributions)
+        - [License](#license)
+        
+        
+        ## Getting Started
+        
+        This section provides an installation and a quick starting guide.
+        
+        ### Installation
+        
+        To install the latest stable release of MCT, run the following command:
+        ```
+        pip install model-compression-toolkit
+        ```
+        
+        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
+        
+        
+        ### Quick start & tutorials 
+        
+        Explore the Model Compression Toolkit (MCT) through our tutorials, 
+        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
+        for hands-on learning. For example:
+        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+        
+        
+        ### Supported Versions
+        
+        Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
+        
+        |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
+        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
+        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
+        | Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
+        
+        
+        |             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
+        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
+        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
+        | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
+        
+        
+        ## Supported Features
+        MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
+        
+        ### Data Generation [*](#experimental-features)
+        MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
+        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
+        
+        ### Quantization
+        MCT supports different quantization methods:
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
+        * Quantization-aware training (QAT) [*](#experimental-features)
+        
+        
+        | Quantization Method                           | Complexity | Computational Cost          |
+        |-----------------------------------------------|------------|-----------------------------|
+        | PTQ                                           | Low        | Low (order of minutes)      |
+        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+        | QAT                                           | High       | High (order of 12-36 hours) |
+        
+        
+        In addition, MCT supports different quantization schemes for quantizing weights and activations:
+        
+        * Power-Of-Two (hardware-friendly quantization [1])
+        * Symmetric
+        * Uniform
+        
+        Main features:
+        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+        
+        ### Enhanced Post-Training Quantization (EPTQ)
+        As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
+        
+        The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
+        
+        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
+        
+        
+        ### Structured Pruning [*](#experimental-features)
+        MCT introduces a structured and hardware-aware model pruning.
+        This pruning technique is designed to compress models for specific hardware architectures, 
+        taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
+        By pruning groups of channels (SIMD groups), our approach not only reduces model size 
+        and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
+        for a target Resource Utilization of weights memory footprint.
+        [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
+        [Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
+        
+        #### Experimental features 
+        
+        Some features are experimental and subject to future changes. 
+         
+        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
+        
+        
+        ## Results
+        ### Keras
+        Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
+        single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
+        
+        <img src="docsrc/images/mbv2_accuracy_graph.png">
+        
+        For more results, please see [1]
+        
+        ### Pytorch
+        We quantized classification networks from the torchvision library. 
+        In the following table we present the ImageNet validation results for these models:
+        
+        | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
+        |---------------------------|-----------------|-----------------|-------------------------|
+        | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
+        | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
+        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
+        
+        
+        #### Pruning Results
+        
+        Results for applying pruning to reduce the parameters of the following models by 50%:
+        
+        | Model           | Dense Model Accuracy | Pruned Model Accuracy |
+        |-----------------|----------------------|-----------------------|
+        | ResNet50 [2]    | 75.1                 | 72.4                  |
+        | DenseNet121 [3] | 74.44                | 71.71                 |
+        
+        
+        ## Trouble Shooting
+        
+        If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
+        for common pitfalls and some tools to improve quantization accuracy.
+        
+        Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
+        
+        
+        ## Contributions
+        MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
+        
+        *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
+        
+        
+        ## License
+        [Apache License 2.0](LICENSE.md).
+        
+        ## References 
+        
+        [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
+        
+        [2] [Keras Applications](https://keras.io/api/applications/)
+        
+        [3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
+        
+        [4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240522.172031
+Version: 2.0.0.20240522.420
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
         This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
         
         Specifically, this project aims to apply quantization to compress neural networks.
         
-        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
+        <img src="docsrc/images/mct_block_diagram.svg" width="10000">
         
         MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
         
         
         
         ## Table of Contents
         
-        - [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
-        - [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
-        - [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
-        - [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
-        - [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
-        - [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
+        - [Getting Started](#getting-started)
+        - [Supported features](#supported-features)
+        - [Results](#results)
+        - [Troubleshooting](#trouble-shooting)
+        - [Contributions](#contributions)
+        - [License](#license)
         
         
         ## Getting Started
         
         This section provides an installation and a quick starting guide.
         
         ### Installation
         
         To install the latest stable release of MCT, run the following command:
         ```
         pip install model-compression-toolkit
         ```
         
-        For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
+        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
         
         
         ### Quick start & tutorials 
         
         Explore the Model Compression Toolkit (MCT) through our tutorials, 
-        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
+        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
         for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
-        * [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
         
         
         ### Supported Versions
         
         Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
         
         |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
@@ -69,23 +69,23 @@
         | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
         | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
         
         
         ## Supported Features
         MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
         
-        ### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        ### Data Generation [*](#experimental-features)
         MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
+        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
         
         ### Quantization
         MCT supports different quantization methods:
         * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
         * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-        * Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        * Quantization-aware training (QAT) [*](#experimental-features)
         
         
         | Quantization Method                           | Complexity | Computational Cost          |
         |-----------------------------------------------|------------|-----------------------------|
         | PTQ                                           | Low        | Low (order of minutes)      |
         | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
         | QAT                                           | High       | High (order of 12-36 hours) |
@@ -99,28 +99,28 @@
         
         Main features:
         * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
         * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
         * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
           * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
           * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
         * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
         * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
         
         ### Enhanced Post-Training Quantization (EPTQ)
         As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
         
         The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
         
-        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
+        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
         
         
-        ### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        ### Structured Pruning [*](#experimental-features)
         MCT introduces a structured and hardware-aware model pruning.
         This pruning technique is designed to compress models for specific hardware architectures, 
         taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
         By pruning groups of channels (SIMD groups), our approach not only reduces model size 
         and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
         for a target Resource Utilization of weights memory footprint.
         [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
@@ -134,15 +134,15 @@
         
         
         ## Results
         ### Keras
         Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
         single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
         
-        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
+        <img src="docsrc/images/mbv2_accuracy_graph.png">
         
         For more results, please see [1]
         
         ### Pytorch
         We quantized classification networks from the torchvision library. 
         In the following table we present the ImageNet validation results for these models:
         
@@ -170,19 +170,19 @@
         
         Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
         
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
-        *You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
+        *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
         
         
         ## License
-        [Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
+        [Apache License 2.0](LICENSE.md).
         
         ## References 
         
         [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
         
         [2] [Keras Applications](https://keras.io/api/applications/)
```

### Comparing `mct-nightly-2.0.0.20240522.172031/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240522.420/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240522.172031"
+__version__ = "2.0.0.20240522.000420"
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -344,36 +344,34 @@
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s count_node_for_mixed_precision_interest_points method.')  # pragma: no cover
 
-    def get_mp_node_distance_fn(self, layer_class: type,
+    def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None,
-                             norm_mse: bool = False) -> Callable:
+                             axis: int = None) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
-            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_mp_node_distance_fn method.')  # pragma: no cover
+                             f'framework\'s get_node_distance_fn method.')  # pragma: no cover
 
 
     @abstractmethod
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> bool:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,20 +234,16 @@
         Args:
             input_tensors: activation input tensors to node.
         Returns:
             Activation input tensors list with positional weights
         """
         for pos, weight in sorted((pos, weight) for pos, weight in self.weights.items()
                                   if isinstance(pos, int)):
-            if pos > len(input_tensors):
-                Logger.critical("The positional weight index cannot exceed the number of input tensors to the node.")  # pragma: no cover
-            # Insert only positional weights that are not subject to quantization. If the positional weight is
-            # subject to quantization, the quantization wrapper inserts the positional weight into the node.
-            if not self.is_weights_quantization_enabled(pos):
-                input_tensors.insert(pos, weight)
+            assert pos <= len(input_tensors), 'Positional weight index mismatch'
+            input_tensors.insert(pos, weight)
 
         return input_tensors
 
     def get_num_parameters(self, fw_info) -> Tuple[int,int]:
         """
         Compute the number of parameters the node holds.
         It returns a tuple: Number of quantized parameters, number of float parameters.
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,21 +85,18 @@
 
         # Get interest points and output points set for distance measurement and set other helper datasets
         # We define a separate set of output nodes of the model for the purpose of sensitivity computation.
         self.interest_points = get_mp_interest_points(graph,
                                                       fw_impl.count_node_for_mixed_precision_interest_points,
                                                       quant_config.num_interest_points_factor)
 
-        # We use normalized MSE when not running hessian-based. For Hessian-based normalized MSE is not needed
-        # beacause hessian weights already do normalization.
-        use_normalized_mse = self.quant_config.use_hessian_based_scores is False
-        self.ips_distance_fns, self.ips_axis = self._init_metric_points_lists(self.interest_points, use_normalized_mse)
+        self.ips_distance_fns, self.ips_axis = self._init_metric_points_lists(self.interest_points)
 
         self.output_points = get_output_nodes_for_metric(graph)
-        self.out_ps_distance_fns, self.out_ps_axis = self._init_metric_points_lists(self.output_points, use_normalized_mse)
+        self.out_ps_distance_fns, self.out_ps_axis = self._init_metric_points_lists(self.output_points)
 
         # Setting lists with relative position of the interest points
         # and output points in the list of all mp model activation tensors
         graph_sorted_nodes = self.graph.get_topo_sorted_nodes()
         all_out_tensors_indices = [graph_sorted_nodes.index(n) for n in self.interest_points + self.output_points]
         global_ipts_indices = [graph_sorted_nodes.index(n) for n in self.interest_points]
         global_out_pts_indices = [graph_sorted_nodes.index(n) for n in self.output_points]
@@ -127,37 +124,35 @@
         # Computing Hessian-based scores for weighted average distance metric computation (only if requested),
         # and assigning distance_weighting method accordingly.
         self.interest_points_hessians = None
         if self.quant_config.use_hessian_based_scores is True:
             self.interest_points_hessians = self._compute_hessian_based_scores()
             self.quant_config.distance_weighting_method = lambda d: self.interest_points_hessians
 
-    def _init_metric_points_lists(self, points: List[BaseNode], norm_mse: bool = False) -> Tuple[List[Callable], List[int]]:
+    def _init_metric_points_lists(self, points: List[BaseNode]) -> Tuple[List[Callable], List[int]]:
         """
         Initiates required lists for future use when computing the sensitivity metric.
         Each point on which the metric is computed uses a dedicated distance function based on its type.
         In addition, all distance functions preform batch computation. Axis is needed only for KL Divergence computation.
 
         Args:
             points: The set of nodes in the graph for which we need to initiate the lists.
-            norm_mse: whether to normalize mse distance function.
 
         Returns: A lists with distance functions and an axis list for each node.
 
         """
         distance_fns_list = []
         axis_list = []
         for n in points:
             axis = n.framework_attr.get(AXIS) if not isinstance(n, FunctionalNode) else n.op_call_kwargs.get(AXIS)
-            distance_fn = self.fw_impl.get_mp_node_distance_fn(
+            distance_fn = self.fw_impl.get_node_distance_fn(
                 layer_class=n.layer_class,
                 framework_attrs=n.framework_attr,
                 compute_distance_fn=self.quant_config.compute_distance_fn,
-                axis=axis,
-                norm_mse=norm_mse)
+                axis=axis)
             distance_fns_list.append(distance_fn)
             # Axis is needed only for KL Divergence calculation, otherwise we use per-tensor computation
             axis_list.append(axis if distance_fn==compute_kl_divergence else None)
         return distance_fns_list, axis_list
 
     def compute_metric(self,
                        mp_model_configuration: List[int],
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,30 +417,28 @@
         elif any([node.is_match_type(_type) for _type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D,
                                                           DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate, tf.concat,
                                                           Add, tf.add]]):
             return True
 
         return False
 
-    def get_mp_node_distance_fn(self, layer_class: type,
+    def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None,
-                             norm_mse: bool = False) -> Callable:
+                             axis: int = None) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
-            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         if compute_distance_fn is not None:
             return compute_distance_fn
 
@@ -454,15 +452,15 @@
                                    or (layer_class == TFOpLambda and
                                        SOFTMAX in framework_attrs[keras_constants.FUNCTION])):
             return compute_kl_divergence
         elif layer_class == tf.nn.sigmoid:
             return compute_cs
         elif layer_class == Dense:
             return compute_cs
-        return partial(compute_mse, norm=norm_mse)
+        return compute_mse
 
     def get_trace_hessian_calculator(self,
                                      graph: Graph,
                                      input_images: List[Any],
                                      trace_hessian_request: TraceHessianRequest,
                                      num_iterations_for_approximation: int = HESSIAN_NUM_ITERATIONS):
         """
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         input_tensors = []
         # Go over a sorted list of the node's incoming edges, and for each source node get its output tensors.
         # Append them in a result list.
         for ie in graph.incoming_edges(node, sort_by_attr=EDGE_SINK_INDEX):
             _input_tensors = node_to_output_tensors_dict[ie.source_node]
             input_tensors.append(_input_tensors)
         input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
-        input_tensors = node.insert_positional_weights_to_input_list(input_tensors)
+        if not is_op_quantize_wrapper:
+            input_tensors = node.insert_positional_weights_to_input_list(input_tensors)
         # convert inputs from positional weights (numpy arrays) to tensors. Must handle each element in the
         # list separately, because in FX the tensors are FX objects and fail to_torch_tensor
         input_tensors = [to_torch_tensor(t, numpy_type=t.dtype) if isinstance(t, np.ndarray) else t
                          for t in input_tensors]
     return input_tensors
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,44 +399,42 @@
         """
 
         if any([node.is_match_type(_type) for _type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax,
                                                         softmax, operator.add, add, cat, operator.concat]]):
             return True
         return False
 
-    def get_mp_node_distance_fn(self, layer_class: type,
+    def get_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None,
-                             norm_mse: bool = False) -> Callable:
+                             axis: int = None) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
-            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         if compute_distance_fn is not None:
             return compute_distance_fn
 
         elif layer_class in [Softmax, softmax] and axis is not None:
             return compute_kl_divergence
         elif layer_class in [Sigmoid, sigmoid]:
             return compute_cs
         elif layer_class == Linear:
             return compute_cs
-        return partial(compute_mse, norm=norm_mse)
+        return compute_mse
 
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> bool:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
```

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/metadata.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240522.420/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240522.172031/setup.py` & `mct-nightly-2.0.0.20240522.420/setup.py`

 * *Files identical despite different names*
