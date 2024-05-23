# Comparing `tmp/dagster-1.7.6.tar.gz` & `tmp/dagster-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.6.tar", last modified: Thu May 16 19:27:38 2024, max compression
+gzip compressed data, was "dagster-1.7.7.tar", last modified: Thu May 23 20:22:44 2024, max compression
```

## Comparing `dagster-1.7.6.tar` & `dagster-1.7.7.tar`

### file list

```diff
@@ -1,721 +1,725 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-16 19:27:09.000000 dagster-1.7.6/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 19:27:09.000000 dagster-1.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-16 19:27:09.000000 dagster-1.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-16 19:27:38.256053 dagster-1.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7214 2024-05-16 19:27:09.000000 dagster-1.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.132053 dagster-1.7.6/dagster/
--rw-r--r--   0 root         (0) root         (0)    30192 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.140053 dagster-1.7.6/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30233 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8271 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30627 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.140053 dagster-1.7.6/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.144053 dagster-1.7.6/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.144053 dagster-1.7.6/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11510 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41265 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25057 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.168053 dagster-1.7.6/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7873 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.168053 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7692 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     9763 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)     6122 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)    11378 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/utils.py
--rw-r--r--   0 root         (0) root         (0)     7090 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5628 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    28490 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    30136 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6937 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    11171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79051 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    14208 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    11580 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21722 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)    50974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_impls.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    35401 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/README.md
--rw-r--r--   0 root         (0) root         (0)     1244 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2771 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16847 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
--rw-r--r--   0 root         (0) root         (0)     1642 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4995 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
--rw-r--r--   0 root         (0) root         (0)     4918 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
--rw-r--r--   0 root         (0) root         (0)     4335 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
--rw-r--r--   0 root         (0) root         (0)     2597 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
--rw-r--r--   0 root         (0) root         (0)    14325 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
--rw-r--r--   0 root         (0) root         (0)     5132 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
--rw-r--r--   0 root         (0) root         (0)    10067 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.176053 dagster-1.7.6/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    70075 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    28072 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9808 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_based_auto_materialize.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    54423 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8703 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.176053 dagster-1.7.6/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)     9922 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5848 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/metadata_set.py
--rw-r--r--   0 root         (0) root         (0)    31381 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/metadata_value.py
--rw-r--r--   0 root         (0) root         (0)     4795 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/source_code.py
--rw-r--r--   0 root         (0) root         (0)    12486 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27690 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.180053 dagster-1.7.6/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    45639 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    22389 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102817 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    16727 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.180053 dagster-1.7.6/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.184053 dagster-1.7.6/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    67853 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.184053 dagster-1.7.6/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/data_version_cache.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    49252 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    18608 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.188053 dagster-1.7.6/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17062 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40877 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9764 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/run_metrics_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    15211 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/types.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132126 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5624 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37860 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83881 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.208053 dagster-1.7.6/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.208053 dagster-1.7.6/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3872 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/base_storage.py
--rw-r--r--   0 root         (0) root         (0)     3320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/batch_asset_record_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20682 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   122186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32639 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    18101 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14231 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25156 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19736 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29231 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    42160 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18725 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39411 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.128053 dagster-1.7.6/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     2306 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42035 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8978 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    46494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/datetime.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    26652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5536 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    45456 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    13054 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    32783 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36148 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     4009 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29718 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1483 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-16 19:27:38.260053 dagster-1.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6901 2024-05-16 19:27:10.000000 dagster-1.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-23 20:22:18.000000 dagster-1.7.7/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:22:18.000000 dagster-1.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-23 20:22:18.000000 dagster-1.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-23 20:22:44.801151 dagster-1.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7214 2024-05-23 20:22:18.000000 dagster-1.7.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.681152 dagster-1.7.7/dagster/
+-rw-r--r--   0 root         (0) root         (0)    30281 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52028 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.689152 dagster-1.7.7/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30233 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30627 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.689152 dagster-1.7.7/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.693152 dagster-1.7.7/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.693152 dagster-1.7.7/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11635 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25411 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.697152 dagster-1.7.7/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.713152 dagster-1.7.7/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     8848 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9763 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_factories/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7493 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    20781 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)     6153 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    11507 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    78592 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    14208 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21722 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    50929 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_impls.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    35407 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22967 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30236 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/README.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    17161 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.717151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4889 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
+-rw-r--r--   0 root         (0) root         (0)    14325 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+-rw-r--r--   0 root         (0) root         (0)    10301 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    70075 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    29195 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9808 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_based_auto_materialize.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    54423 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8703 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.721151 dagster-1.7.7/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    10018 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5848 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/metadata_set.py
+-rw-r--r--   0 root         (0) root         (0)    31381 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/metadata_value.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/source_code.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57718 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27690 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.725151 dagster-1.7.7/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    45639 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19238 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   104499 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    16727 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11028 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.725151 dagster-1.7.7/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.729151 dagster-1.7.7/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    68093 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.729151 dagster-1.7.7/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/data_version_cache.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    49252 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    18608 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40877 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9768 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/run_metrics_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15211 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132126 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.737151 dagster-1.7.7/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    84694 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.741151 dagster-1.7.7/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.745151 dagster-1.7.7/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.749151 dagster-1.7.7/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.749151 dagster-1.7.7/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.761151 dagster-1.7.7/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/base_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/batch_asset_record_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21051 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   123419 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    33038 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    18101 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.765151 dagster-1.7.7/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14235 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25156 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19736 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.769151 dagster-1.7.7/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.773151 dagster-1.7.7/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29231 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12950 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39411 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.681152 dagster-1.7.7/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.777151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.781151 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.785151 dagster-1.7.7/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.785151 dagster-1.7.7/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    61307 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42035 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    46494 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.789151 dagster-1.7.7/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.793151 dagster-1.7.7/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.797151 dagster-1.7.7/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    26684 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10818 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/aiodataloader.py
+-rw-r--r--   0 root         (0) root         (0)     9782 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    45800 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    13054 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/cronstring.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11253 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    32783 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36148 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.801151 dagster-1.7.7/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 20:22:18.000000 dagster-1.7.7/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:22:44.685152 dagster-1.7.7/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29940 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:22:44.000000 dagster-1.7.7/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-23 20:22:44.809151 dagster-1.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6901 2024-05-23 20:22:18.000000 dagster-1.7.7/setup.py
```

### Comparing `dagster-1.7.6/COPYING` & `dagster-1.7.7/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/LICENSE` & `dagster-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/MANIFEST.in` & `dagster-1.7.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/PKG-INFO` & `dagster-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.6
+Version: 1.7.7
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.6/README.md` & `dagster-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/__init__.py` & `dagster-1.7.7/dagster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,17 @@
 )
 from dagster._core.definitions.asset_check_factories.freshness_checks.sensor import (
     build_sensor_for_freshness_checks as build_sensor_for_freshness_checks,
 )
 from dagster._core.definitions.asset_check_factories.freshness_checks.time_partition import (
     build_time_partition_freshness_checks as build_time_partition_freshness_checks,
 )
+from dagster._core.definitions.asset_check_factories.metadata_bounds_checks import (
+    build_metadata_bounds_checks as build_metadata_bounds_checks,
+)
 from dagster._core.definitions.asset_check_factories.schema_change_checks import (
     build_column_schema_change_checks as build_column_schema_change_checks,
 )
 from dagster._core.definitions.asset_check_spec import (
     AssetCheckKey as AssetCheckKey,
     AssetCheckSeverity as AssetCheckSeverity,
     AssetCheckSpec as AssetCheckSpec,
@@ -281,15 +284,14 @@
     PythonArtifactMetadataValue as PythonArtifactMetadataValue,
     TableColumnLineageMetadataValue as TableColumnLineageMetadataValue,
     TableMetadataValue as TableMetadataValue,
     TableSchemaMetadataValue as TableSchemaMetadataValue,
     TextMetadataValue as TextMetadataValue,
     TimestampMetadataValue as TimestampMetadataValue,
     UrlMetadataValue as UrlMetadataValue,
-    with_source_code_references as with_source_code_references,
 )
 from dagster._core.definitions.metadata.table import (
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
```

### Comparing `dagster-1.7.6/dagster/_annotations.py` & `dagster-1.7.7/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/get_server_id.py` & `dagster-1.7.7/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/list_repositories.py` & `dagster-1.7.7/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/notebook_data.py` & `dagster-1.7.7/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.7/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_job.py` & `dagster-1.7.7/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_partition.py` & `dagster-1.7.7/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_repository.py` & `dagster-1.7.7/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_schedule.py` & `dagster-1.7.7/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_api/snapshot_sensor.py` & `dagster-1.7.7/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_check/README.md` & `dagster-1.7.7/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_check/__init__.py` & `dagster-1.7.7/dagster/_check/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1185,17 +1185,17 @@
 
 
 def opt_iterable_param(
     obj: Optional[Iterable[T]],
     param_name: str,
     of_type: Optional[TypeOrTupleOfTypes] = None,
     additional_message: Optional[str] = None,
-) -> Optional[Iterable[T]]:
+) -> Iterable[T]:
     if obj is None:
-        return None
+        return []
 
     return iterable_param(obj, param_name, of_type, additional_message)
 
 
 # ########################
 # ##### SET
 # ########################
```

### Comparing `dagster-1.7.6/dagster/_cli/__init__.py` & `dagster-1.7.7/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/api.py` & `dagster-1.7.7/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/asset.py` & `dagster-1.7.7/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/code_server.py` & `dagster-1.7.7/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/config_scaffolder.py` & `dagster-1.7.7/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/debug.py` & `dagster-1.7.7/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/dev.py` & `dagster-1.7.7/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/instance.py` & `dagster-1.7.7/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/job.py` & `dagster-1.7.7/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/load_handle.py` & `dagster-1.7.7/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/project.py` & `dagster-1.7.7/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/run.py` & `dagster-1.7.7/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/schedule.py` & `dagster-1.7.7/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/sensor.py` & `dagster-1.7.7/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/utils.py` & `dagster-1.7.7/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.7/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/__init__.py` & `dagster-1.7.7/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/config_schema.py` & `dagster-1.7.7/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/config_type.py` & `dagster-1.7.7/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/errors.py` & `dagster-1.7.7/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/evaluate_value_result.py` & `dagster-1.7.7/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/field.py` & `dagster-1.7.7/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/field_utils.py` & `dagster-1.7.7/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/post_process.py` & `dagster-1.7.7/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/primitive_mapping.py` & `dagster-1.7.7/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.7/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.7/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/config.py` & `dagster-1.7.7/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.7/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 from dagster import Field, Selector
 from dagster._config.field_utils import (
     FIELD_NO_DEFAULT_PROVIDED,
     Map,
     convert_potential_field,
 )
 from dagster._model.pydantic_compat_layer import ModelFieldCompat, PydanticUndefined, model_fields
+from dagster._utils.typing_api import is_closed_python_optional_type
 
-from .type_check_utils import is_optional, safe_is_subclass
+from .type_check_utils import safe_is_subclass
 
 
 # This is from https://github.com/dagster-io/dagster/pull/11470
 def _apply_defaults_to_schema_field(field: Field, additional_default_values: Any) -> Field:
     # This work by validating the top-level config and then
     # just setting it at that top-level field. Config fields
     # can actually take nested values so we only need to set it
@@ -129,15 +130,15 @@
     if safe_is_subclass(field_type, Config):
         inferred_field = infer_schema_from_config_class(
             field_type,
             description=pydantic_field.description,
         )
         return inferred_field
     else:
-        if not pydantic_field.is_required() and not is_optional(field_type):
+        if not pydantic_field.is_required() and not is_closed_python_optional_type(field_type):
             field_type = Optional[field_type]
 
         config_type = _config_type_for_type_on_pydantic_field(field_type)
 
         default_to_pass = (
             pydantic_field.default
             if pydantic_field.default is not PydanticUndefined
@@ -145,15 +146,16 @@
         )
         if isinstance(default_to_pass, Enum):
             default_to_pass = default_to_pass.name
 
         return Field(
             config=config_type,
             description=pydantic_field.description,
-            is_required=pydantic_field.is_required() and not is_optional(field_type),
+            is_required=pydantic_field.is_required()
+            and not is_closed_python_optional_type(field_type),
             default_value=default_to_pass,
         )
 
 
 def strip_wrapping_annotated_types(potentially_annotated_type: Any) -> Any:
     """For a type that is wrapped in Annotated, return the unwrapped type. Recursive,
     so it will unwrap nested Annotated types.
@@ -190,15 +192,15 @@
     except ImportError:
         # These types do not exist in Pydantic 2.x
         pass
 
     if safe_is_subclass(get_origin(potential_dagster_type), List):
         list_inner_type = get_args(potential_dagster_type)[0]
         return Array(_config_type_for_type_on_pydantic_field(list_inner_type))
-    elif is_optional(potential_dagster_type):
+    elif is_closed_python_optional_type(potential_dagster_type):
         optional_inner_type = next(
             arg for arg in get_args(potential_dagster_type) if arg is not type(None)
         )
         return Noneable(_config_type_for_type_on_pydantic_field(optional_inner_type))
     elif safe_is_subclass(get_origin(potential_dagster_type), Dict) or safe_is_subclass(
         get_origin(potential_dagster_type), Mapping
     ):
```

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.7/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.7/dagster/_config/pythonic_config/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 )
 from dagster._core.errors import DagsterInvalidConfigError
 from dagster._core.execution.context.init import InitResourceContext, build_init_resource_context
 from dagster._model.pydantic_compat_layer import (
     model_fields,
 )
 from dagster._utils.cached_method import cached_method
+from dagster._utils.typing_api import is_closed_python_optional_type
 
 from .attach_other_object_to_context import (
     IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
 )
-from .type_check_utils import is_optional
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
 except ImportError:
 
     class cached_property:
         pass
@@ -894,15 +894,15 @@
 def _is_annotated_as_resource_type(annotation: Type, metadata: List[str]) -> bool:
     """Determines if a field in a structured config class is annotated as a resource type or not."""
     from .type_check_utils import safe_is_subclass
 
     if metadata and metadata[0] == "resource_dependency":
         return True
 
-    if is_optional(annotation):
+    if is_closed_python_optional_type(annotation):
         args = get_args(annotation)
         annotation_inner = next((arg for arg in args if arg is not None), None)
         if not annotation_inner:
             return False
         return _is_annotated_as_resource_type(annotation_inner, [])
 
     is_annotated_as_resource_dependency = get_origin(annotation) == ResourceDependency or getattr(
```

### Comparing `dagster-1.7.6/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.7/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/snap.py` & `dagster-1.7.7/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/source.py` & `dagster-1.7.7/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/stack.py` & `dagster-1.7.7/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/traversal_context.py` & `dagster-1.7.7/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/type_printer.py` & `dagster-1.7.7/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_config/validate.py` & `dagster-1.7.7/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.7/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,21 @@
     def asset_graph(self) -> "BaseAssetGraph[BaseAssetNode]":
         return self._stale_resolver.asset_graph
 
     @property
     def _queryer(self) -> "CachingInstanceQueryer":
         return self._stale_resolver.instance_queryer
 
+    # In our transitional period there are lots of code path that take
+    # a AssetGraphView and then call methods on the queryer. This is
+    # formal accesor to we can do this legally, instead of using noqa accesses
+    # of a private proeprty
+    def get_inner_queryer_for_back_compat(self) -> "CachingInstanceQueryer":
+        return self._queryer
+
     def _get_partitions_def(self, asset_key: "AssetKey") -> Optional["PartitionsDefinition"]:
         return self.asset_graph.get(asset_key).partitions_def
 
     def get_asset_slice(self, asset_key: "AssetKey") -> "AssetSlice":
         # not compute_asset_slice because dynamic partitions store
         # is just passed to AssetSubset.all, not invoked
         return _slice_from_subset(
```

### Comparing `dagster-1.7.6/dagster/_core/assets.py` & `dagster-1.7.7/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/code_pointer.py` & `dagster-1.7.7/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/container_context/config.py` & `dagster-1.7.7/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/debug.py` & `dagster-1.7.7/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/decorator_utils.py` & `dagster-1.7.7/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import Iterator, Optional, Sequence, cast
+import datetime
+from typing import Iterator, Optional, Sequence, Tuple, cast
 
 import pendulum
 
 from dagster import _check as check
 from dagster._annotations import experimental
+from dagster._core.storage.asset_check_execution_record import AssetCheckExecutionRecordStatus
 
 from ...asset_check_spec import AssetCheckKey
 from ...asset_checks import AssetChecksDefinition
 from ...asset_selection import AssetSelection
 from ...decorators import sensor
 from ...run_request import RunRequest
 from ...sensor_definition import DefaultSensorStatus, SensorDefinition, SensorEvaluationContext
@@ -76,68 +78,33 @@
         default_status=default_status,
     )
     def the_sensor(context: SensorEvaluationContext) -> Optional[RunRequest]:
         left_off_asset_check_key = (
             AssetCheckKey.from_user_string(context.cursor) if context.cursor else None
         )
         start_time = pendulum.now("UTC")
-        checks_iter = ordered_iterator_freshness_checks_starting_with_key(
-            left_off_asset_check_key, freshness_checks
-        )
-        check_key = next(checks_iter, None)
         checks_to_evaluate = []
+        checks_iter = freshness_checks_get_evaluations_iter(
+            context=context,
+            start_time=start_time,
+            left_off_asset_check_key=left_off_asset_check_key,
+            freshness_checks=freshness_checks,
+        )
+        # We evaluate checks using an iterator which yields back control to the main loop every
+        # iteration; this allows us to pause the sensor if it runs into the maximum runtime.
+        check_key, should_evaluate = next(checks_iter, (None, False))
         while (
             pendulum.now("UTC").timestamp() - start_time.timestamp() < MAXIMUM_RUNTIME_SECONDS
-            and check_key is not None
+            and check_key
         ):
-            should_evaluate_check = False
-            prev_check_eval_record = context.instance.get_latest_asset_check_evaluation_record(
-                check_key
-            )
-            if prev_check_eval_record:
-                # If we have already executed this check, only run it if the previous result was a success, and the time limit has passed.
-                evaluation = check.not_none(
-                    check.not_none(
-                        prev_check_eval_record.event,
-                        "Expected the check evaluation record to have an associated dagster event.",
-                    ).asset_check_evaluation,
-                    "Expected the dagster event to be an asset check evaluation.",
-                )
-                if evaluation.passed:
-                    next_deadline = cast(float, evaluation.metadata[FRESH_UNTIL_METADATA_KEY].value)
-                    if next_deadline < start_time.timestamp():
-                        context.log.info(
-                            f"Freshness check {check_key.to_user_string()} previously passed, but "
-                            "enough time has passed that it can be overdue again. Adding to run request."
-                        )
-                        should_evaluate_check = True
-                    else:
-                        how_long_until_next_deadline = next_deadline - start_time.timestamp()
-                        context.log.info(
-                            f"Freshness check {check_key.to_user_string()} previously passed, but "
-                            f"cannot be overdue again until {seconds_in_words(how_long_until_next_deadline)}. Skipping..."
-                        )
-                else:
-                    context.log.info(
-                        f"Freshness check {check_key.to_user_string()} is currently overdue. "
-                        "Waiting to re-evaluate until the asset has received an update."
-                    )
-            else:
-                # If we have never before executed this check, we should run it
-                context.log.info(
-                    f"Freshness check {check_key.to_user_string()} has never been executed before. "
-                    "Adding to run request."
-                )
-                should_evaluate_check = True
-            if should_evaluate_check:
+            if should_evaluate:
                 checks_to_evaluate.append(check_key)
-            check_key = next(checks_iter, None)
+            check_key, should_evaluate = next(checks_iter, (None, False))
         new_cursor = check_key.to_user_string() if check_key else None
-        if new_cursor:
-            context.update_cursor(new_cursor)
+        context.update_cursor(new_cursor)
         if checks_to_evaluate:
             return RunRequest(asset_check_keys=checks_to_evaluate)
 
     return the_sensor
 
 
 def ordered_iterator_freshness_checks_starting_with_key(
@@ -151,11 +118,74 @@
             for asset_check_spec in asset_check.check_specs
         ],
         key=lambda key: key.to_user_string(),
     )
     # Offset based on the left off asset check key, but then iterate back through the beginning afterwards
     if left_off_asset_check_key:
         left_off_idx = asset_check_keys_sorted.index(left_off_asset_check_key)
-        yield from asset_check_keys_sorted[left_off_idx:]
-        yield from asset_check_keys_sorted[:left_off_idx]
+        yield from asset_check_keys_sorted[left_off_idx + 1 :]
+        yield from asset_check_keys_sorted[: left_off_idx + 1]
     else:
         yield from asset_check_keys_sorted
+
+
+def freshness_checks_get_evaluations_iter(
+    context: SensorEvaluationContext,
+    start_time: datetime.datetime,
+    left_off_asset_check_key: Optional[AssetCheckKey],
+    freshness_checks: Sequence[AssetChecksDefinition],
+) -> Iterator[Tuple[AssetCheckKey, bool]]:
+    """Yields the set of freshness check keys to evaluate."""
+    for check_key in ordered_iterator_freshness_checks_starting_with_key(
+        left_off_asset_check_key, freshness_checks
+    ):
+        summary_record = context.instance.event_log_storage.get_asset_check_summary_records(
+            [check_key]
+        )[check_key]
+        # Case 1: We have never run the check before. We should run it.
+        if summary_record.last_check_execution_record is None:
+            context.log.info(
+                f"Freshness check {check_key.to_user_string()} has never been executed before. "
+                "Adding to run request."
+            )
+            yield check_key, True
+            continue
+
+        # Case 2: The check is currently evaluating. We shouldn't kick off another evaluation until it's done.
+        if (
+            summary_record.last_check_execution_record.status
+            == AssetCheckExecutionRecordStatus.PLANNED
+        ):
+            context.log.info(
+                f"Freshness check on asset {check_key.asset_key.to_user_string()} is in the planned state, indicating it is currently evaluating. Skipping..."
+            )
+            yield check_key, False
+            continue
+
+        evaluation = check.not_none(
+            summary_record.last_check_execution_record.event
+        ).asset_check_evaluation
+        # Case 3: The check previously failed. We shouldn't kick off another evaluation until the asset has been updated.
+        if not evaluation or not evaluation.passed:
+            context.log.info(
+                f"Freshness check {check_key.to_user_string()} failed its last evaluation. Waiting "
+                "to re-evaluate until the asset has received an update."
+            )
+            yield check_key, False
+            continue
+        # Case 4: The check previously passed. We should re-evaluate if it's possible for the check to be overdue again.
+        next_deadline = cast(float, evaluation.metadata[FRESH_UNTIL_METADATA_KEY].value)
+        if next_deadline < start_time.timestamp():
+            context.log.info(
+                f"Freshness check {check_key.to_user_string()} previously passed, but "
+                "enough time has passed that it can be overdue again. Adding to run request."
+            )
+            yield check_key, True
+            continue
+        else:
+            how_long_until_next_deadline = next_deadline - start_time.timestamp()
+            context.log.info(
+                f"Freshness check {check_key.to_user_string()} previously passed, but "
+                f"cannot be overdue again until {seconds_in_words(how_long_until_next_deadline)} from now. Skipping..."
+            )
+            yield check_key, False
+            continue
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/schema_change_checks.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/schema_change_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from typing import Dict, Mapping, Sequence, Tuple, Union, cast
 
 from pydantic import BaseModel
 
 from dagster._annotations import experimental
 from dagster._core.instance import DagsterInstance
 
-from ..asset_check_result import AssetCheckResult
 from ..asset_check_spec import AssetCheckKey, AssetCheckSeverity, AssetCheckSpec
 from ..asset_checks import AssetChecksDefinition
 from ..asset_key import AssetKey, CoercibleToAssetKey
 from ..assets import AssetsDefinition, SourceAsset
-from ..decorators.asset_check_decorator import multi_asset_check
 from ..events import AssetMaterialization
 from ..metadata import TableColumn, TableMetadataSet, TableSchema
-from .utils import unique_id_from_asset_keys
+from .utils import build_multi_asset_check
 
 
 @experimental
 def build_column_schema_change_checks(
     *,
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
     severity: AssetCheckSeverity = AssetCheckSeverity.WARN,
@@ -82,39 +80,27 @@
                         f"\n- {col_name}: {type_change.old_type} -> {type_change.new_type}"
                     )
 
             return False, description
 
         return True, "No changes to column schema between previous and latest materialization"
 
-    @multi_asset_check(
-        specs=[
+    return build_multi_asset_check(
+        check_specs=[
             AssetCheckSpec(
                 "column_schema_change",
                 asset=asset_key,
                 description="Checks whether there are changes to column schema between the asset's "
                 " two most recent materializations",
             )
             for asset_key in asset_keys
         ],
-        can_subset=True,
-        name=unique_id_from_asset_keys(list(asset_keys)),
+        check_fn=_result_for_check_key,
+        severity=severity,
     )
-    def _checks(context):
-        for asset_check_key in context.selected_asset_check_keys:
-            passed, description = _result_for_check_key(context.instance, asset_check_key)
-            yield AssetCheckResult(
-                passed=passed,
-                description=description,
-                severity=severity,
-                check_name=asset_check_key.name,
-                asset_key=asset_check_key.asset_key,
-            )
-
-    return [_checks]
 
 
 class TypeChange(BaseModel):
     old_type: str
     new_type: str
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/utils.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_factories/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import datetime
-from typing import Iterator, Optional, Sequence, Union, cast
+from typing import Callable, Iterator, Optional, Sequence, Tuple, Union, cast
 
 from dagster import _check as check
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
+from dagster._core.definitions.asset_check_result import AssetCheckResult
+from dagster._core.definitions.asset_check_spec import (
+    AssetCheckKey,
+    AssetCheckSeverity,
+    AssetCheckSpec,
+)
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
 from dagster._core.definitions.decorators.asset_check_decorator import (
     MultiAssetCheckFunction,
     multi_asset_check,
 )
 from dagster._core.definitions.metadata import JsonMetadataValue
 from dagster._core.event_api import AssetRecordsFilter, EventLogRecord
@@ -241,14 +246,19 @@
     """
     sorted_asset_keys = sorted(asset_keys, key=lambda asset_key: asset_key.to_string())
     return non_secure_md5_hash_str(
         ",".join([str(asset_key) for asset_key in sorted_asset_keys]).encode()
     )[:8]
 
 
+def unique_id_from_check_keys(keys: Sequence[AssetCheckKey]) -> str:
+    sorted_keys = sorted(keys, key=lambda key: key.to_user_string())
+    return non_secure_md5_hash_str(",".join([str(key) for key in sorted_keys]).encode())[:8]
+
+
 def freshness_multi_asset_check(params_metadata: JsonMetadataValue, asset_keys: Sequence[AssetKey]):
     def inner(fn: MultiAssetCheckFunction) -> AssetChecksDefinition:
         return multi_asset_check(
             specs=[
                 AssetCheckSpec(
                     "freshness_check",
                     asset=asset_key,
@@ -258,7 +268,31 @@
                 for asset_key in asset_keys
             ],
             can_subset=True,
             name=f"freshness_check_{unique_id_from_asset_keys(asset_keys)}",
         )(fn)
 
     return inner
+
+
+def build_multi_asset_check(
+    check_specs: Sequence[AssetCheckSpec],
+    check_fn: Callable[[DagsterInstance, AssetCheckKey], Tuple[bool, str]],
+    severity: AssetCheckSeverity,
+) -> Sequence[AssetChecksDefinition]:
+    @multi_asset_check(
+        specs=check_specs,
+        can_subset=True,
+        name=f"asset_check_{unique_id_from_check_keys([spec.key for spec in check_specs])}",
+    )
+    def _checks(context):
+        for asset_check_key in context.selected_asset_check_keys:
+            passed, description = check_fn(context.instance, asset_check_key)
+            yield AssetCheckResult(
+                passed=passed,
+                description=description,
+                severity=severity,
+                check_name=asset_check_key.name,
+                asset_key=asset_check_key.asset_key,
+            )
+
+    return [_checks]
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dagster._core.definitions.asset_check_spec import (
     AssetCheckKey,
     AssetCheckSeverity,
 )
 from dagster._core.definitions.events import (
     AssetKey,
     CoercibleToAssetKey,
+    EventWithMetadata,
     MetadataValue,
     RawMetadataValue,
     normalize_metadata,
 )
 from dagster._core.errors import DagsterInvariantViolationError
 
 if TYPE_CHECKING:
@@ -30,15 +31,16 @@
             ("passed", PublicAttr[bool]),
             ("asset_key", PublicAttr[Optional[AssetKey]]),
             ("check_name", PublicAttr[Optional[str]]),
             ("metadata", PublicAttr[Mapping[str, MetadataValue]]),
             ("severity", PublicAttr[AssetCheckSeverity]),
             ("description", PublicAttr[Optional[str]]),
         ],
-    )
+    ),
+    EventWithMetadata,
 ):
     """The result of an asset check.
 
     Attributes:
         asset_key (Optional[AssetKey]):
             The asset key that was checked.
         check_name (Optional[str]):
@@ -167,7 +169,17 @@
             asset_key=check_key.asset_key,
             passed=self.passed,
             metadata=self.metadata,
             target_materialization_data=target_materialization_data,
             severity=self.severity,
             description=self.description,
         )
+
+    def with_metadata(self, metadata: Mapping[str, RawMetadataValue]) -> "AssetCheckResult":
+        return AssetCheckResult(
+            passed=self.passed,
+            asset_key=self.asset_key,
+            check_name=self.check_name,
+            metadata=metadata,
+            severity=self.severity,
+            description=self.description,
+        )
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.7/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.7/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.7/dagster/_core/definitions/asset_daemon_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import dataclasses
 import datetime
 import logging
-import time
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
     FrozenSet,
@@ -22,41 +20,31 @@
 import pendulum
 
 import dagster._check as check
 from dagster._core.asset_graph_view.asset_graph_view import AssetGraphView, TemporalContext
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.data_version import CachingStaleStatusResolver
-from dagster._core.definitions.declarative_scheduling.scheduling_context import (
-    SchedulingContext,
-)
-from dagster._core.definitions.declarative_scheduling.scheduling_evaluation_info import (
-    SchedulingEvaluationInfo,
-)
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.time_window_partitions import (
     get_time_partitions_def,
 )
 from dagster._core.instance import DynamicPartitionsStore
 
 from ... import PartitionKeyRange
 from ..storage.tags import ASSET_PARTITION_RANGE_END_TAG, ASSET_PARTITION_RANGE_START_TAG
 from .asset_daemon_cursor import AssetDaemonCursor
 from .auto_materialize_rule import AutoMaterializeRule
 from .backfill_policy import BackfillPolicy, BackfillPolicyType
 from .base_asset_graph import BaseAssetGraph
-from .declarative_scheduling.legacy.legacy_context import (
-    LegacyRuleEvaluationContext,
-)
 from .declarative_scheduling.serialized_objects import (
     AssetConditionEvaluation,
     AssetConditionEvaluationState,
 )
-from .freshness_based_auto_materialize import get_expected_data_time_for_asset_key
 from .partition import PartitionsDefinition, ScheduleType
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
 
@@ -194,161 +182,36 @@
         """
         self._logger.info(
             f"Prefetching asset records for {len(self.asset_records_to_prefetch)} records."
         )
         self.instance_queryer.prefetch_asset_records(self.asset_records_to_prefetch)
         self._logger.info("Done prefetching asset records.")
 
-    def evaluate_asset(
-        self,
-        asset_key: AssetKey,
-        evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState],
-        expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]],
-        current_evaluation_info_by_key: Mapping[AssetKey, SchedulingEvaluationInfo],
-    ) -> Tuple[AssetConditionEvaluationState, Optional[datetime.datetime]]:
-        """Evaluates the auto materialize policy of a given asset key.
-
-        Params:
-            - asset_key: The asset key to evaluate.
-            - will_materialize_mapping: A mapping of AssetKey to the set of AssetKeyPartitionKeys
-                that will be materialized this tick. As this function is called in topological order,
-                this mapping will contain the expected materializations of all upstream assets.
-            - expected_data_time_mapping: A mapping of AssetKey to the expected data time of the
-                asset after this tick. As this function is called in topological order, this mapping
-                will contain the expected data times of all upstream assets.
-
-        """
-        # convert the legacy AutoMaterializePolicy to an Evaluator
-        asset_condition = check.not_none(
-            self.asset_graph.get(asset_key).auto_materialize_policy
-        ).to_scheduling_condition()
-
-        previous_evaluation_state = self.cursor.get_previous_evaluation_state(asset_key)
-
-        legacy_context = LegacyRuleEvaluationContext.create(
-            asset_key=asset_key,
-            previous_evaluation_state=previous_evaluation_state,
-            condition=asset_condition,
-            instance_queryer=self.instance_queryer,
-            data_time_resolver=self.data_time_resolver,
-            daemon_context=self,
-            evaluation_state_by_key=evaluation_state_by_key,
-            expected_data_time_mapping=expected_data_time_mapping,
-        )
-
-        context = SchedulingContext.create(
-            asset_key=asset_key,
-            asset_graph_view=self.asset_graph_view,
-            logger=self.logger,
-            current_tick_evaluation_info_by_key=current_evaluation_info_by_key,
-            previous_evaluation_info=SchedulingEvaluationInfo.from_asset_condition_evaluation_state(
-                self.asset_graph_view, previous_evaluation_state
-            )
-            if previous_evaluation_state
-            else None,
-            legacy_context=legacy_context,
-        )
-
-        result = asset_condition.evaluate(context)
-
-        expected_data_time = get_expected_data_time_for_asset_key(
-            legacy_context, will_materialize=result.true_subset.size > 0
-        )
-        return AssetConditionEvaluationState.create(context, result), expected_data_time
-
     def get_asset_condition_evaluations(
         self,
     ) -> Tuple[Sequence[AssetConditionEvaluationState], AbstractSet[AssetKeyPartitionKey]]:
         """Returns a mapping from asset key to the AutoMaterializeAssetEvaluation for that key, a
         sequence of new per-asset cursors, and the set of all asset partitions that should be
         materialized or discarded this tick.
         """
-        evaluation_state_by_key: Dict[AssetKey, AssetConditionEvaluationState] = {}
-        current_evaluation_info_by_key: Dict[AssetKey, SchedulingEvaluationInfo] = {}
-        expected_data_time_mapping: Dict[AssetKey, Optional[datetime.datetime]] = defaultdict()
-        to_request: Set[AssetKeyPartitionKey] = set()
-
-        num_checked_assets = 0
-        num_auto_materialize_asset_keys = len(self.auto_materialize_asset_keys)
-
-        for asset_key in self.asset_graph.toposorted_asset_keys:
-            # an asset may have already been visited if it was part of a non-subsettable multi-asset
-            if asset_key not in self.auto_materialize_asset_keys:
-                continue
-
-            num_checked_assets = num_checked_assets + 1
-            start_time = time.time()
-            self._logger.debug(
-                "Evaluating asset"
-                f" {asset_key.to_user_string()} ({num_checked_assets}/{num_auto_materialize_asset_keys})"
-            )
-
-            try:
-                (evaluation_state, expected_data_time) = self.evaluate_asset(
-                    asset_key,
-                    evaluation_state_by_key,
-                    expected_data_time_mapping,
-                    current_evaluation_info_by_key,
-                )
-            except Exception as e:
-                raise Exception(
-                    f"Error while evaluating conditions for asset {asset_key.to_user_string()}"
-                ) from e
-
-            num_requested = evaluation_state.true_subset.size
-            log_fn = self._logger.info if num_requested > 0 else self._logger.debug
-
-            to_request_asset_partitions = evaluation_state.true_subset.asset_partitions
-            to_request_str = ",".join(
-                [(ap.partition_key or "No partition") for ap in to_request_asset_partitions]
-            )
-            to_request |= to_request_asset_partitions
-
-            log_fn(
-                f"Asset {asset_key.to_user_string()} evaluation result: {num_requested}"
-                f" requested ({to_request_str}) ({format(time.time()-start_time, '.3f')} seconds)"
-            )
-
-            evaluation_state_by_key[asset_key] = evaluation_state
-            current_evaluation_info_by_key[asset_key] = (
-                SchedulingEvaluationInfo.from_asset_condition_evaluation_state(
-                    self.asset_graph_view, evaluation_state
-                )
-            )
-            expected_data_time_mapping[asset_key] = expected_data_time
-
-            # if we need to materialize any partitions of a non-subsettable multi-asset, we need to
-            # materialize all of them
-            execution_set_keys = self.asset_graph.get(asset_key).execution_set_asset_keys
-            if len(execution_set_keys) > 1 and num_requested > 0:
-                for neighbor_key in execution_set_keys:
-                    expected_data_time_mapping[neighbor_key] = expected_data_time
-
-                    # make sure that the true_subset of the neighbor is accurate -- when it was
-                    # evaluated it may have had a different requested AssetSubset. however, because
-                    # all these neighbors must be executed as a unit, we need to union together
-                    # the subset of all required neighbors
-                    if neighbor_key in evaluation_state_by_key:
-                        neighbor_evaluation_state = evaluation_state_by_key[neighbor_key]
-                        evaluation_state_by_key[neighbor_key] = dataclasses.replace(
-                            neighbor_evaluation_state,
-                            previous_evaluation=neighbor_evaluation_state.previous_evaluation.copy(
-                                update={
-                                    "true_subset": neighbor_evaluation_state.true_subset.copy(
-                                        update={"asset_key": neighbor_key}
-                                    )
-                                }
-                            ),
-                        )
-                    to_request |= {
-                        ap._replace(asset_key=neighbor_key)
-                        for ap in evaluation_state.true_subset.asset_partitions
-                    }
+        from .declarative_scheduling.scheduling_condition_evaluator import (
+            SchedulingConditionEvaluator,
+        )
 
-        return (list(evaluation_state_by_key.values()), to_request)
+        evaluator = SchedulingConditionEvaluator(
+            asset_graph=self.asset_graph,
+            asset_keys=self.auto_materialize_asset_keys,
+            asset_graph_view=self.asset_graph_view,
+            logger=self._logger,
+            cursor=self.cursor,
+            data_time_resolver=self.data_time_resolver,
+            respect_materialization_data_versions=self.respect_materialization_data_versions,
+            auto_materialize_run_tags=self.auto_materialize_run_tags,
+        )
+        return evaluator.evaluate()
 
     def evaluate(
         self,
     ) -> Tuple[Sequence[RunRequest], AssetDaemonCursor, Sequence[AssetConditionEvaluation]]:
         observe_request_timestamp = pendulum.now().timestamp()
         auto_observe_run_requests = (
             get_auto_observe_run_requests(
@@ -457,69 +320,51 @@
     asset_partition_keys: Mapping[AssetKey, Set[str]] = {
         asset_key_partition.asset_key: set() for asset_key_partition in asset_partitions
     }
     for asset_partition in asset_partitions:
         if asset_partition.partition_key:
             asset_partition_keys[asset_partition.asset_key].add(asset_partition.partition_key)
 
-    assets_to_reconcile_by_partitions_def_partition_keys: Mapping[
-        Tuple[Optional[PartitionsDefinition], Optional[FrozenSet[str]]], Set[AssetKey]
+    assets_to_reconcile_by_partitions_def_partition_keys_backfill_policy: Mapping[
+        Tuple[Optional[PartitionsDefinition], Optional[FrozenSet[str]], Optional[BackfillPolicy]],
+        Set[AssetKey],
     ] = defaultdict(set)
 
-    # here we are grouping assets by their partitions def and partition keys selected.
+    # here we are grouping assets by their partitions def, selected partition keys, and backfill policy.
     for asset_key, partition_keys in asset_partition_keys.items():
-        assets_to_reconcile_by_partitions_def_partition_keys[
+        assets_to_reconcile_by_partitions_def_partition_keys_backfill_policy[
             asset_graph.get(asset_key).partitions_def,
             frozenset(partition_keys) if partition_keys else None,
+            asset_graph.get(asset_key).backfill_policy,
         ].add(asset_key)
 
     for (
         partitions_def,
         partition_keys,
-    ), asset_keys in assets_to_reconcile_by_partitions_def_partition_keys.items():
+        backfill_policy,
+    ), asset_keys in assets_to_reconcile_by_partitions_def_partition_keys_backfill_policy.items():
         tags = {**(run_tags or {})}
         if partitions_def is None and partition_keys is not None:
             check.failed("Partition key provided for unpartitioned asset")
         if partitions_def is not None and partition_keys is None:
             check.failed("Partition key missing for partitioned asset")
         if partitions_def is None and partition_keys is None:
             # non partitioned assets will be backfilled in a single run
             run_requests.append(RunRequest(asset_selection=list(asset_keys), tags=tags))
         else:
-            backfill_policies = {
-                check.not_none(asset_graph.get(asset_key).backfill_policy)
-                for asset_key in asset_keys
-            }
-            if len(backfill_policies) == 1:
-                # if all backfill policies are the same, we can backfill them together
-                backfill_policy = backfill_policies.pop()
-                run_requests.extend(
-                    _build_run_requests_with_backfill_policy(
-                        list(asset_keys),
-                        check.not_none(backfill_policy),
-                        check.not_none(partition_keys),
-                        check.not_none(partitions_def),
-                        tags,
-                        dynamic_partitions_store=dynamic_partitions_store,
-                    )
+            run_requests.extend(
+                _build_run_requests_with_backfill_policy(
+                    list(asset_keys),
+                    check.not_none(backfill_policy),
+                    check.not_none(partition_keys),
+                    check.not_none(partitions_def),
+                    tags,
+                    dynamic_partitions_store=dynamic_partitions_store,
                 )
-            else:
-                # if backfill policies are different, we need to backfill them separately
-                for asset_key in asset_keys:
-                    backfill_policy = asset_graph.get(asset_key).backfill_policy
-                    run_requests.extend(
-                        _build_run_requests_with_backfill_policy(
-                            [asset_key],
-                            check.not_none(backfill_policy),
-                            check.not_none(partition_keys),
-                            check.not_none(partitions_def),
-                            tags,
-                            dynamic_partitions_store=dynamic_partitions_store,
-                        )
-                    )
+            )
     return run_requests
 
 
 def _build_run_requests_with_backfill_policy(
     asset_keys: Sequence[AssetKey],
     backfill_policy: BackfillPolicy,
     partition_keys: FrozenSet[str],
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.7/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
 @whitelist_for_serdes(
     field_serializers={
         "last_observe_request_timestamp_by_asset_key": ObserveRequestTimestampSerializer
     }
 )
 @dataclass(frozen=True)
+# TODO: rename to scheduling cursor or something
+# 2024-05-16 -- schrockn
 class AssetDaemonCursor:
     """State that's stored between daemon evaluations.
 
     Attributes:
         evaluation_id (int): The ID of the evaluation that produced this cursor.
         previous_evaluation_state (Sequence[AssetConditionEvaluationInfo]): The evaluation info
             recorded for each asset on the previous tick.
@@ -115,18 +117,23 @@
     def with_updates(
         self,
         evaluation_id: int,
         evaluation_timestamp: float,
         newly_observe_requested_asset_keys: Sequence[AssetKey],
         evaluation_state: Sequence["AssetConditionEvaluationState"],
     ) -> "AssetDaemonCursor":
+        # do not "forget" about values for non-evaluated assets
+        new_evaluation_state_by_key = dict(self.previous_evaluation_state_by_key)
+        for new_state in evaluation_state:
+            new_evaluation_state_by_key[new_state.asset_key] = new_state
+
         return dataclasses.replace(
             self,
             evaluation_id=evaluation_id,
-            previous_evaluation_state=evaluation_state,
+            previous_evaluation_state=list(new_evaluation_state_by_key.values()),
             last_observe_request_timestamp_by_asset_key={
                 **self.last_observe_request_timestamp_by_asset_key,
                 **{
                     asset_key: evaluation_timestamp
                     for asset_key in newly_observe_requested_asset_keys
                 },
             },
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.7/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.7/dagster/_core/definitions/asset_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.asset_spec import (
     SYSTEM_METADATA_KEY_AUTO_CREATED_STUB_ASSET,
     AssetExecutionType,
     AssetSpec,
 )
-from dagster._core.definitions.assets import AssetsDefinition, asset_owner_to_str
+from dagster._core.definitions.assets import AssetsDefinition
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.base_asset_graph import (
     AssetKeyOrCheckKey,
     BaseAssetGraph,
     BaseAssetNode,
 )
@@ -74,17 +74,15 @@
 
     @property
     def tags(self) -> Mapping[str, str]:
         return self.assets_def.tags_by_key.get(self.key, {})
 
     @property
     def owners(self) -> Sequence[str]:
-        return [
-            asset_owner_to_str(owner) for owner in self.assets_def.owners_by_key.get(self.key, [])
-        ]
+        return self.assets_def.owners_by_key.get(self.key, [])
 
     @property
     def is_partitioned(self) -> bool:
         return self.assets_def.partitions_def is not None
 
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
@@ -275,7 +273,40 @@
                 ],
             }
         )
 
     @cached_property
     def asset_check_keys(self) -> AbstractSet[AssetCheckKey]:
         return {key for ad in self.assets_defs for key in ad.check_keys}
+
+
+def materializable_in_same_run(
+    asset_graph: BaseAssetGraph, child_key: AssetKey, parent_key: AssetKey
+):
+    """Returns whether a child asset can be materialized in the same run as a parent asset."""
+    from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
+    from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
+    from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
+
+    child_node = asset_graph.get(child_key)
+    parent_node = asset_graph.get(parent_key)
+    return (
+        # both assets must be materializable
+        child_node.is_materializable
+        and parent_node.is_materializable
+        # the parent must have the same partitioning
+        and child_node.partitions_def == parent_node.partitions_def
+        # the parent must have a simple partition mapping to the child
+        and (
+            not parent_node.is_partitioned
+            or isinstance(
+                asset_graph.get_partition_mapping(child_node.key, parent_node.key),
+                (TimeWindowPartitionMapping, IdentityPartitionMapping),
+            )
+        )
+        # the parent must be in the same repository to be materialized alongside the candidate
+        and (
+            not isinstance(asset_graph, RemoteAssetGraph)
+            or asset_graph.get_repository_handle(child_key)
+            == asset_graph.get_repository_handle(parent_key)
+        )
+    )
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.7/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.7/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_in.py` & `dagster-1.7.7/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_job.py` & `dagster-1.7.7/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_key.py` & `dagster-1.7.7/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.7/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_out.py` & `dagster-1.7.7/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.7/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,16 +84,15 @@
         job: Optional[ExecutableDefinition] = None,
         jobs: Optional[Sequence[ExecutableDefinition]] = None,
         default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
         required_resource_keys: Optional[Set[str]] = None,
     ):
         self._asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
 
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventRecordsFilter
+        from dagster._core.event_api import AssetRecordsFilter
 
         resource_arg_names: Set[str] = {
             arg.name for arg in get_resource_args(asset_materialization_fn)
         }
 
         combined_required_resource_keys = (
             check.opt_set_param(required_resource_keys, "required_resource_keys", of_type=str)
@@ -105,23 +104,22 @@
                 after_cursor = None
                 if context.cursor:
                     try:
                         after_cursor = int(context.cursor)
                     except ValueError:
                         after_cursor = None
 
-                event_records = context.instance.get_event_records(
-                    EventRecordsFilter(
-                        event_type=DagsterEventType.ASSET_MATERIALIZATION,
+                event_records = context.instance.fetch_materializations(
+                    AssetRecordsFilter(
                         asset_key=self._asset_key,
-                        after_cursor=after_cursor,
+                        after_storage_id=after_cursor,
                     ),
                     ascending=False,
                     limit=1,
-                )
+                ).records
 
                 if not event_records:
                     yield SkipReason(
                         f"No new materialization events found for asset key {self._asset_key}"
                     )
                     return
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.7/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.7/dagster/_core/definitions/asset_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/assets.py` & `dagster-1.7.7/dagster/_core/definitions/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     AbstractSet,
     Any,
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
     Set,
+    Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import experimental_param, public
@@ -52,59 +52,37 @@
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
 )
 from dagster._core.utils import is_valid_email
 from dagster._utils import IHasInternalInit
 from dagster._utils.merger import merge_dicts
 from dagster._utils.security import non_secure_md5_hash_str
-from dagster._utils.warnings import (
-    disable_dagster_warnings,
-)
+from dagster._utils.warnings import disable_dagster_warnings
 
 from .dependency import NodeHandle
 from .events import AssetKey, CoercibleToAssetKey, CoercibleToAssetKeyPrefix
 from .node_definition import NodeDefinition
 from .op_definition import OpDefinition
 from .partition import PartitionsDefinition
 from .partition_mapping import (
     PartitionMapping,
     get_builtin_partition_mapping_types,
     infer_partition_mapping,
 )
 from .resource_definition import ResourceDefinition
 from .source_asset import SourceAsset
-from .utils import DEFAULT_GROUP_NAME, validate_group_name, validate_tags_strict
+from .utils import DEFAULT_GROUP_NAME, normalize_group_name, validate_tags_strict
 
 if TYPE_CHECKING:
     from .base_asset_graph import AssetKeyOrCheckKey
     from .graph_definition import GraphDefinition
 
 ASSET_SUBSET_INPUT_PREFIX = "__subset_input__"
 
 
-class UserAssetOwner(NamedTuple):
-    email: str
-
-
-class TeamAssetOwner(NamedTuple):
-    team: str
-
-
-AssetOwner = Union[UserAssetOwner, TeamAssetOwner]
-
-
-def asset_owner_to_str(owner: AssetOwner) -> str:
-    if isinstance(owner, UserAssetOwner):
-        return owner.email
-    elif isinstance(owner, TeamAssetOwner):
-        return owner.team
-    else:
-        check.failed(f"Unexpected owner type {type(owner)}")
-
-
 class AssetsDefinition(ResourceAddable, RequiresResources, IHasInternalInit):
     """Defines a set of assets that are produced by the same op or graph.
 
     AssetsDefinitions are typically not instantiated directly, but rather produced using the
     :py:func:`@asset <asset>` or :py:func:`@multi_asset <multi_asset>` decorators.
     """
 
@@ -123,15 +101,15 @@
     _freshness_policies_by_key: Mapping[AssetKey, FreshnessPolicy]
     _auto_materialize_policies_by_key: Mapping[AssetKey, AutoMaterializePolicy]
     _backfill_policy: Optional[BackfillPolicy]
     _code_versions_by_key: Mapping[AssetKey, Optional[str]]
     _descriptions_by_key: Mapping[AssetKey, str]
     _selected_asset_check_keys: AbstractSet[AssetCheckKey]
     _is_subset: bool
-    _owners_by_key: Mapping[AssetKey, Sequence[AssetOwner]]
+    _owners_by_key: Mapping[AssetKey, Sequence[str]]
 
     def __init__(
         self,
         *,
         keys_by_input_name: Mapping[str, AssetKey],
         keys_by_output_name: Mapping[str, AssetKey],
         node_def: NodeDefinition,
@@ -147,15 +125,15 @@
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         check_specs_by_output_name: Optional[Mapping[str, AssetCheckSpec]] = None,
         selected_asset_check_keys: Optional[AbstractSet[AssetCheckKey]] = None,
         is_subset: bool = False,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]] = None,
+        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
         # if adding new fields, make sure to handle them in the with_attributes, from_graph,
         # from_op, and get_attributes_dict methods
     ):
         from dagster._core.execution.build_resources import wrap_resources_for_execution
 
         from .graph_definition import GraphDefinition
 
@@ -179,41 +157,23 @@
         self._check_specs_by_output_name = check.opt_mapping_param(
             check_specs_by_output_name,
             "check_specs_by_output_name",
             key_type=str,
             value_type=AssetCheckSpec,
         )
 
-        # if not specified assume all output assets depend on all input assets
         all_asset_keys = set(keys_by_output_name.values())
-        input_asset_keys = set(keys_by_input_name.values())
 
         self._partitions_def = partitions_def
         self._partition_mappings = partition_mappings or {}
-        builtin_partition_mappings = get_builtin_partition_mapping_types()
-        for asset_key, partition_mapping in self._partition_mappings.items():
-            if not isinstance(partition_mapping, builtin_partition_mappings):
-                warnings.warn(
-                    f"Non-built-in PartitionMappings, such as {type(partition_mapping).__name__} "
-                    "are deprecated and will not work with asset reconciliation. The built-in "
-                    "partition mappings are "
-                    + ", ".join(
-                        builtin_partition_mapping.__name__
-                        for builtin_partition_mapping in builtin_partition_mappings
-                    )
-                    + ".",
-                    category=DeprecationWarning,
-                )
-
-            if asset_key not in input_asset_keys:
-                check.failed(
-                    f"While constructing AssetsDefinition outputting {all_asset_keys}, received a"
-                    f" partition mapping for {asset_key} that is not defined in the set of upstream"
-                    f" assets: {input_asset_keys}"
-                )
+        _validate_partition_mappings(
+            partition_mappings=self._partition_mappings,
+            input_asset_keys=set(keys_by_input_name.values()),
+            all_asset_keys=all_asset_keys,
+        )
 
         self._asset_deps = asset_deps or {
             out_asset_key: set(keys_by_input_name.values()) for out_asset_key in all_asset_keys
         }
         check.invariant(
             set(self._asset_deps.keys()) == all_asset_keys,
             "The set of asset keys with dependencies specified in the asset_deps argument must "
@@ -226,39 +186,25 @@
         )
 
         group_names_by_key = (
             check.mapping_param(group_names_by_key, "group_names_by_key")
             if group_names_by_key
             else {}
         )
+        self._selected_asset_keys, self._selected_asset_check_keys = _resolve_selections(
+            all_asset_keys=all_asset_keys,
+            all_check_keys={spec.key for spec in (check_specs_by_output_name or {}).values()},
+            selected_asset_keys=selected_asset_keys,
+            selected_asset_check_keys=selected_asset_check_keys,
+        )
         self._group_names_by_key = {}
         # assets that don't have a group name get a DEFAULT_GROUP_NAME
         for key in all_asset_keys:
             group_name = group_names_by_key.get(key)
-            self._group_names_by_key[key] = validate_group_name(group_name)
-
-        all_check_keys = {spec.key for spec in (check_specs_by_output_name or {}).values()}
-
-        # NOTE: this logic mirrors subsetting at the asset layer. This is ripe for consolidation.
-        if selected_asset_keys is None and selected_asset_check_keys is None:
-            # if no selections, include everything
-            self._selected_asset_keys = all_asset_keys
-            self._selected_asset_check_keys = all_check_keys
-        else:
-            self._selected_asset_keys = selected_asset_keys or set()
-
-            if selected_asset_check_keys is None:
-                # if assets were selected but checks are None, then include all checks for selected
-                # assets
-                self._selected_asset_check_keys = {
-                    key for key in all_check_keys if key.asset_key in self._selected_asset_keys
-                }
-            else:
-                # otherwise, use the selected checks
-                self._selected_asset_check_keys = selected_asset_check_keys
+            self._group_names_by_key[key] = normalize_group_name(group_name)
 
         self._check_specs_by_key = {
             spec.key: spec
             for spec in self._check_specs_by_output_name.values()
             if spec.key in self._selected_asset_check_keys
         }
 
@@ -350,41 +296,28 @@
             output_keys=self._selected_asset_keys,
             partition_mappings=self._partition_mappings,
             partitions_def=self._partitions_def,
         )
 
         self._is_subset = check.bool_param(is_subset, "is_subset")
 
-        check.opt_mapping_param(owners_by_key, "owners_by_key", key_type=AssetKey, value_type=list)
-        for key, owners in (owners_by_key or {}).items():
+        self._owners_by_key = check.opt_mapping_param(
+            owners_by_key, "owners_by_key", key_type=AssetKey, value_type=list
+        )
+        for key, owners in self._owners_by_key.items():
             for owner in owners:
-                if isinstance(owner, (TeamAssetOwner, UserAssetOwner)):
-                    continue
-                elif is_valid_email(owner):
+                if is_valid_email(owner):
                     continue
                 elif owner.startswith("team:") and len(owner) > 5:
                     continue
                 else:
                     raise DagsterInvalidDefinitionError(
                         f"Invalid owner '{owner}' for asset '{key}'. Owner must be an email address or a team"
                         " name prefixed with 'team:'."
                     )
-        self._owners_by_key = {
-            key: [
-                owner
-                if isinstance(owner, (TeamAssetOwner, UserAssetOwner))
-                else (
-                    UserAssetOwner(email=owner)
-                    if is_valid_email(owner)
-                    else TeamAssetOwner(team=owner[5:])
-                )
-                for owner in owners
-            ]
-            for key, owners in (owners_by_key or {}).items()
-        }
 
     def dagster_internal_init(
         *,
         keys_by_input_name: Mapping[str, AssetKey],
         keys_by_output_name: Mapping[str, AssetKey],
         node_def: NodeDefinition,
         partitions_def: Optional[PartitionsDefinition],
@@ -399,15 +332,15 @@
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]],
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]],
         backfill_policy: Optional[BackfillPolicy],
         descriptions_by_key: Optional[Mapping[AssetKey, str]],
         check_specs_by_output_name: Optional[Mapping[str, AssetCheckSpec]],
         selected_asset_check_keys: Optional[AbstractSet[AssetCheckKey]],
         is_subset: bool,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]],
+        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]],
     ) -> "AssetsDefinition":
         return AssetsDefinition(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             node_def=node_def,
             partitions_def=partitions_def,
             partition_mappings=partition_mappings,
@@ -460,15 +393,15 @@
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
         check_specs: Optional[Sequence[AssetCheckSpec]] = None,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]] = None,
+        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from a GraphDefinition.
 
         Args:
             graph_def (GraphDefinition): The GraphDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
                 names of the decorated graph to their corresponding asset keys. If not provided,
@@ -517,15 +450,15 @@
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
             auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
                 AutoMaterializePolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
                 to the associated asset.
             backfill_policy (Optional[BackfillPolicy]): Defines this asset's BackfillPolicy
-            owners_by_key (Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]]): Defines
+            owners_by_key (Optional[Mapping[AssetKey, Sequence[str]]]): Defines
                 owners to be associated with each of the asset keys for this node.
 
         """
         return AssetsDefinition._from_node(
             node_def=graph_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
@@ -660,15 +593,15 @@
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
         check_specs: Optional[Sequence[AssetCheckSpec]] = None,
-        owners_by_key: Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]] = None,
+        owners_by_key: Optional[Mapping[AssetKey, Sequence[str]]] = None,
     ) -> "AssetsDefinition":
         from dagster._core.definitions.decorators.asset_decorator import (
             _assign_output_names_to_check_specs,
             _validate_check_specs_target_relevant_asset_keys,
         )
 
         node_def = check.inst_param(node_def, "node_def", NodeDefinition)
@@ -1010,15 +943,15 @@
         return self._code_versions_by_key
 
     @property
     def partition_mappings(self) -> Mapping[AssetKey, PartitionMapping]:
         return self._partition_mappings
 
     @property
-    def owners_by_key(self) -> Mapping[AssetKey, Sequence[AssetOwner]]:
+    def owners_by_key(self) -> Mapping[AssetKey, Sequence[str]]:
         return self._owners_by_key
 
     @public
     def get_partition_mapping(self, in_asset_key: AssetKey) -> Optional[PartitionMapping]:
         """Returns the partition mapping between keys in this AssetsDefinition and a given input
         asset key (if any).
         """
@@ -1042,14 +975,24 @@
         Returns:
             AbstractSet[Tuple[AssetKey, str]]: The selected asset checks. An asset check is
                 identified by the asset key and the name of the check.
         """
         return self._selected_asset_check_keys
 
     @property
+    def check_key(self) -> AssetCheckKey:
+        check.invariant(
+            len(self.check_keys) == 1,
+            "Tried to retrieve asset check key from an assets definition with more or less than 1 asset check key: "
+            + ", ".join([ak.to_user_string() for ak in self.check_keys]),
+        )
+
+        return next(iter(self.check_keys))
+
+    @property
     def execution_type(self) -> AssetExecutionType:
         value = self._get_external_asset_metadata_value(SYSTEM_METADATA_KEY_ASSET_EXECUTION_TYPE)
         if value is None:
             return AssetExecutionType.MATERIALIZATION
         elif isinstance(value, str):
             return AssetExecutionType[value]
         else:
@@ -1110,16 +1053,14 @@
 
     def with_attributes(
         self,
         *,
         output_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         input_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
-        descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
-        metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         tags_by_key: Optional[Mapping[AssetKey, Mapping[str, str]]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
         auto_materialize_policy: Optional[
             Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
         ] = None,
@@ -1138,20 +1079,14 @@
             "input_asset_key_replacements",
             key_type=AssetKey,
             value_type=AssetKey,
         )
         group_names_by_key = check.opt_mapping_param(
             group_names_by_key, "group_names_by_key", key_type=AssetKey, value_type=str
         )
-        descriptions_by_key = check.opt_mapping_param(
-            descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
-        )
-        metadata_by_key = check.opt_mapping_param(
-            metadata_by_key, "metadata_by_key", key_type=AssetKey, value_type=dict
-        )
 
         backfill_policy = check.opt_inst_param(backfill_policy, "backfill_policy", BackfillPolicy)
 
         if group_names_by_key:
             group_name_conflicts = [
                 asset_key
                 for asset_key in group_names_by_key
@@ -1219,23 +1154,20 @@
             if replaced_auto_materialize_policy:
                 replaced_auto_materialize_policies_by_key[
                     output_asset_key_replacements.get(key, key)
                 ] = replaced_auto_materialize_policy
 
         replaced_descriptions_by_key = {
             output_asset_key_replacements.get(key, key): description
-            for key, description in descriptions_by_key.items()
+            for key, description in self.descriptions_by_key.items()
         }
 
-        if not metadata_by_key:
-            metadata_by_key = self.metadata_by_key
-
         replaced_metadata_by_key = {
             output_asset_key_replacements.get(key, key): metadata
-            for key, metadata in metadata_by_key.items()
+            for key, metadata in self.metadata_by_key.items()
         }
 
         replaced_tags_by_key = {
             output_asset_key_replacements.get(key, key): tags
             for key, tags in self.tags_by_key.items()
         }
 
@@ -1551,14 +1483,15 @@
             auto_materialize_policies_by_key=self._auto_materialize_policies_by_key,
             backfill_policy=self._backfill_policy,
             descriptions_by_key=self._descriptions_by_key,
             check_specs_by_output_name=self._check_specs_by_output_name,
             selected_asset_check_keys=self._selected_asset_check_keys,
             owners_by_key=self._owners_by_key,
             tags_by_key=self._tags_by_key,
+            is_subset=self._is_subset,
         )
 
 
 def _infer_keys_by_input_names(
     node_def: NodeDefinition, keys_by_input_name: Mapping[str, AssetKey]
 ) -> Mapping[str, AssetKey]:
     all_input_names = [input_def.name for input_def in node_def.input_defs]
@@ -1662,14 +1595,68 @@
         " to outputs of the graph, and produce assets. The following leaf node(s) are"
         f" non-asset producing ops: {unmapped_leaf_nodes}. This behavior is not currently"
         " supported because these ops are not required for the creation of the associated"
         " asset(s).",
     )
 
 
+def _resolve_selections(
+    all_asset_keys: AbstractSet[AssetKey],
+    all_check_keys: AbstractSet[AssetCheckKey],
+    selected_asset_keys: Optional[AbstractSet[AssetKey]],
+    selected_asset_check_keys: Optional[AbstractSet[AssetCheckKey]],
+) -> Tuple[AbstractSet[AssetKey], AbstractSet[AssetCheckKey]]:
+    # NOTE: this logic mirrors subsetting at the asset layer. This is ripe for consolidation.
+    if selected_asset_keys is None and selected_asset_check_keys is None:
+        # if no selections, include everything
+        return all_asset_keys, all_check_keys
+    else:
+        resolved_selected_asset_keys = selected_asset_keys or set()
+
+        if selected_asset_check_keys is None:
+            # if assets were selected but checks are None, then include all checks for selected
+            # assets
+            resolved_selected_asset_check_keys = {
+                key for key in all_check_keys if key.asset_key in resolved_selected_asset_keys
+            }
+        else:
+            # otherwise, use the selected checks
+            resolved_selected_asset_check_keys = selected_asset_check_keys
+
+        return resolved_selected_asset_keys, resolved_selected_asset_check_keys
+
+
+def _validate_partition_mappings(
+    partition_mappings: Mapping[AssetKey, PartitionMapping],
+    input_asset_keys: AbstractSet[AssetKey],
+    all_asset_keys: AbstractSet[AssetKey],
+) -> None:
+    builtin_partition_mappings = get_builtin_partition_mapping_types()
+    for asset_key, partition_mapping in partition_mappings.items():
+        if not isinstance(partition_mapping, builtin_partition_mappings):
+            warnings.warn(
+                f"Non-built-in PartitionMappings, such as {type(partition_mapping).__name__} "
+                "are deprecated and will not work with asset reconciliation. The built-in "
+                "partition mappings are "
+                + ", ".join(
+                    builtin_partition_mapping.__name__
+                    for builtin_partition_mapping in builtin_partition_mappings
+                )
+                + ".",
+                category=DeprecationWarning,
+            )
+
+        if asset_key not in input_asset_keys:
+            check.failed(
+                f"While constructing AssetsDefinition outputting {all_asset_keys}, received a"
+                f" partition mapping for {asset_key} that is not defined in the set of upstream"
+                f" assets: {input_asset_keys}"
+            )
+
+
 def _validate_self_deps(
     input_keys: Iterable[AssetKey],
     output_keys: Iterable[AssetKey],
     partition_mappings: Mapping[AssetKey, PartitionMapping],
     partitions_def: Optional[PartitionsDefinition],
 ) -> None:
     output_keys_set = set(output_keys)
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.7/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_impls.py` & `dagster-1.7.7/dagster/_core/definitions/auto_materialize_rule_impls.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             for asset_partition in run_id_asset_partitions
         }
 
         if (
             self.latest_run_required_tags.items()
             <= {
                 AUTO_MATERIALIZE_TAG: "true",
-                **context.legacy_context.daemon_context.auto_materialize_run_tags,
+                **context.legacy_context.auto_materialize_run_tags,
             }.items()
         ):
             return will_update_asset_partitions | updated_partitions_with_required_tags
         else:
             return updated_partitions_with_required_tags
 
     def __hash__(self):
@@ -368,15 +368,15 @@
             ).parent_partitions
 
             updated_parent_asset_partitions = context.legacy_context.instance_queryer.get_parent_asset_partitions_updated_after_child(
                 asset_partition=asset_partition,
                 parent_asset_partitions=parent_asset_partitions,
                 # do a precise check for updated parents, factoring in data versions, as long as
                 # we're within reasonable limits on the number of partitions to check
-                respect_materialization_data_versions=context.legacy_context.daemon_context.respect_materialization_data_versions
+                respect_materialization_data_versions=context.legacy_context.respect_materialization_data_versions
                 and len(parent_asset_partitions) + subset_to_evaluate.size < 100,
                 # ignore self-dependencies when checking for updated parents, to avoid historical
                 # rematerializations from causing a chain of materializations to be kicked off
                 ignored_parent_keys={context.legacy_context.asset_key},
             )
             for parent in updated_parent_asset_partitions:
                 asset_partitions_by_updated_parents[parent].add(asset_partition)
@@ -704,15 +704,15 @@
                 candidate.partition_key,
             ).parent_partitions
 
             updated_parent_partitions = (
                 context.legacy_context.instance_queryer.get_parent_asset_partitions_updated_after_child(
                     asset_partition=candidate,
                     parent_asset_partitions=parent_partitions,
-                    respect_materialization_data_versions=context.legacy_context.daemon_context.respect_materialization_data_versions,
+                    respect_materialization_data_versions=context.legacy_context.respect_materialization_data_versions,
                     ignored_parent_keys=set(),
                 )
                 | context.legacy_context.parent_will_update_subset.asset_partitions
             )
 
             if self.require_update_for_all_parent_partitions:
                 # All upstream partitions must be updated in order for the candidate to be updated
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.7/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.7/dagster/_core/definitions/base_asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 )
 
 import toposort
 
 import dagster._check as check
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.asset_subset import ValidAssetSubset
-from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.partition_mapping import PartitionMapping
 from dagster._core.errors import DagsterInvalidInvocationError
@@ -53,14 +52,15 @@
 from .time_window_partitions import (
     get_time_partition_key,
     get_time_partitions_def,
 )
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
+    from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 
 AssetKeyOrCheckKey = Union[AssetKey, AssetCheckKey]
 
 
 class ParentsPartitionsResult(NamedTuple):
     """Represents the result of mapping an asset partition to its upstream parent partitions.
 
@@ -133,15 +133,15 @@
 
     @property
     @abstractmethod
     def freshness_policy(self) -> Optional[FreshnessPolicy]: ...
 
     @property
     @abstractmethod
-    def auto_materialize_policy(self) -> Optional[AutoMaterializePolicy]: ...
+    def auto_materialize_policy(self) -> Optional["AutoMaterializePolicy"]: ...
 
     @property
     @abstractmethod
     def auto_observe_interval_minutes(self) -> Optional[float]: ...
 
     @property
     @abstractmethod
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.7/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/composition.py` & `dagster-1.7.7/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/config.py` & `dagster-1.7.7/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/configurable.py` & `dagster-1.7.7/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/data_time.py` & `dagster-1.7.7/dagster/_core/definitions/data_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,17 +449,18 @@
         latest_materialization = asset_record.asset_entry.last_materialization
         if (
             latest_materialization is not None
             and latest_materialization.run_id == latest_run_record.dagster_run.run_id
         ):
             return current_data_time
 
-        run_failure_time = datetime.datetime.utcfromtimestamp(
-            latest_run_record.end_time or datetime_as_float(latest_run_record.create_timestamp)
-        ).replace(tzinfo=datetime.timezone.utc)
+        run_failure_time = datetime.datetime.fromtimestamp(
+            latest_run_record.end_time or datetime_as_float(latest_run_record.create_timestamp),
+            datetime.timezone.utc,
+        )
         return self._get_in_progress_data_time_in_run(
             run_id=run_id, asset_key=asset_key, current_time=run_failure_time
         )
 
     ####################
     # MAIN METHODS
     ####################
@@ -524,16 +525,16 @@
                 "observation"
             )
 
         data_time = observation.metadata.get(DATA_TIME_METADATA_KEY)
         if data_time is None:
             return None
         else:
-            return datetime.datetime.utcfromtimestamp(cast(float, data_time.value)).replace(
-                tzinfo=datetime.timezone.utc
+            return datetime.datetime.fromtimestamp(
+                cast(float, data_time.value), datetime.timezone.utc
             )
 
     def get_minutes_overdue(
         self,
         asset_key: AssetKey,
         evaluation_time: datetime.datetime,
     ) -> Optional[FreshnessMinutes]:
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/data_version.py` & `dagster-1.7.7/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/README.md` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import datetime
 import functools
+import logging
 import os
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
@@ -21,16 +22,14 @@
 
 from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     HistoricalAllPartitionsSubsetSentinel,
 )
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.definitions.partition import PartitionsDefinition
-from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
-from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 
 from ...asset_subset import AssetSubset, ValidAssetSubset
 from ..serialized_objects import (
     AssetConditionEvaluation,
     AssetConditionEvaluationState,
     AssetSubsetWithMetadata,
 )
@@ -67,33 +66,62 @@
     condition: "SchedulingCondition"
     previous_evaluation_state: Optional[AssetConditionEvaluationState]
     previous_evaluation: Optional[AssetConditionEvaluation]
     candidate_subset: ValidAssetSubset
 
     instance_queryer: "CachingInstanceQueryer"
     data_time_resolver: "CachingDataTimeResolver"
-    daemon_context: "AssetDaemonContext"
 
     evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState]
     expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]]
 
     start_timestamp: float
+    respect_materialization_data_versions: bool
+    auto_materialize_run_tags: Mapping[str, str]
+    logger: logging.Logger
     root_ref: Optional["LegacyRuleEvaluationContext"] = None
 
     @staticmethod
-    def create(
+    def create_within_asset_daemon(
         asset_key: AssetKey,
         condition: "SchedulingCondition",
         previous_evaluation_state: Optional[AssetConditionEvaluationState],
         instance_queryer: "CachingInstanceQueryer",
         data_time_resolver: "CachingDataTimeResolver",
         daemon_context: "AssetDaemonContext",
         evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState],
         expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]],
     ) -> "LegacyRuleEvaluationContext":
+        return LegacyRuleEvaluationContext.create(
+            asset_key=asset_key,
+            condition=condition,
+            previous_evaluation_state=previous_evaluation_state,
+            instance_queryer=instance_queryer,
+            data_time_resolver=data_time_resolver,
+            evaluation_state_by_key=evaluation_state_by_key,
+            expected_data_time_mapping=expected_data_time_mapping,
+            respect_materialization_data_versions=daemon_context.respect_materialization_data_versions,
+            auto_materialize_run_tags=daemon_context.auto_materialize_run_tags,
+            logger=daemon_context.logger,
+        )
+
+    @staticmethod
+    def create(
+        *,
+        asset_key: AssetKey,
+        condition: "SchedulingCondition",
+        previous_evaluation_state: Optional[AssetConditionEvaluationState],
+        instance_queryer: "CachingInstanceQueryer",
+        data_time_resolver: "CachingDataTimeResolver",
+        evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState],
+        expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]],
+        respect_materialization_data_versions: bool,
+        auto_materialize_run_tags: Mapping[str, str],
+        logger: logging.Logger,
+    ):
         partitions_def = instance_queryer.asset_graph.get(asset_key).partitions_def
 
         return LegacyRuleEvaluationContext(
             asset_key=asset_key,
             condition=condition,
             previous_evaluation_state=previous_evaluation_state,
             previous_evaluation=previous_evaluation_state.previous_evaluation
@@ -103,18 +131,20 @@
                 asset_key,
                 partitions_def,
                 instance_queryer,
                 instance_queryer.evaluation_time,
             ),
             data_time_resolver=data_time_resolver,
             instance_queryer=instance_queryer,
-            daemon_context=daemon_context,
             evaluation_state_by_key=evaluation_state_by_key,
             expected_data_time_mapping=expected_data_time_mapping,
             start_timestamp=pendulum.now("UTC").timestamp(),
+            respect_materialization_data_versions=respect_materialization_data_versions,
+            auto_materialize_run_tags=auto_materialize_run_tags,
+            logger=logger,
         )
 
     def for_child(
         self,
         child_condition: "SchedulingCondition",
         child_unique_id: str,
         candidate_subset: AssetSubset,
@@ -305,39 +335,17 @@
             self.previous_evaluation.candidate_subset, HistoricalAllPartitionsSubsetSentinel
         ):
             return self.empty_subset()
         return self.candidate_subset - self.previous_evaluation.candidate_subset
 
     def materializable_in_same_run(self, child_key: AssetKey, parent_key: AssetKey) -> bool:
         """Returns whether a child asset can be materialized in the same run as a parent asset."""
-        from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
+        from dagster._core.definitions.asset_graph import materializable_in_same_run
 
-        child_node = self.asset_graph.get(child_key)
-        parent_node = self.asset_graph.get(parent_key)
-        return (
-            # both assets must be materializable
-            child_node.is_materializable
-            and parent_node.is_materializable
-            # the parent must have the same partitioning
-            and child_node.partitions_def == parent_node.partitions_def
-            # the parent must have a simple partition mapping to the child
-            and (
-                not parent_node.is_partitioned
-                or isinstance(
-                    self.asset_graph.get_partition_mapping(child_node.key, parent_node.key),
-                    (TimeWindowPartitionMapping, IdentityPartitionMapping),
-                )
-            )
-            # the parent must be in the same repository to be materialized alongside the candidate
-            and (
-                not isinstance(self.asset_graph, RemoteAssetGraph)
-                or self.asset_graph.get_repository_handle(child_key)
-                == self.asset_graph.get_repository_handle(parent_key)
-            )
-        )
+        return materializable_in_same_run(self.asset_graph, child_key, parent_key)
 
     def get_parents_that_will_not_be_materialized_on_current_tick(
         self, *, asset_partition: AssetKeyPartitionKey
     ) -> AbstractSet[AssetKeyPartitionKey]:
         """Returns the set of parent asset partitions that will not be updated in the same run of
         this asset partition if a run is launched for this asset partition on this tick.
         """
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,16 +24,15 @@
         return non_secure_md5_hash_str("".join(parts).encode())
 
     @property
     def description(self) -> str:
         return self.rule.description
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
-        context.legacy_context.root_context.daemon_context.logger.debug(
-            f"Evaluating rule: {self.rule.to_snapshot()}"
-        )
-        evaluation_result = self.rule.evaluate_for_asset(context)
-        context.legacy_context.root_context.daemon_context.logger.debug(
+        context.logger.debug(f"Evaluating rule: {self.rule.to_snapshot()}")
+        # Allow for access to legacy context in legacy rule evaluation
+        evaluation_result = self.rule.evaluate_for_asset(context._replace(allow_legacy_access=True))
+        context.logger.debug(
             f"Rule returned {evaluation_result.true_subset.size} partitions "
             f"({evaluation_result.end_timestamp - evaluation_result.start_timestamp:.2f} seconds)"
         )
         return evaluation_result
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,18 @@
         )
         parent_slices = candidate_slice.compute_parent_slices()
         all_parent_asset_partitions = {
             ap
             for parent_slice in parent_slices.values()
             for ap in parent_slice.expensively_compute_asset_partitions()
         }
-        return (
-            context.legacy_context.instance_queryer.get_parent_asset_partitions_updated_after_child(
-                asset_partition=candidate,
-                parent_asset_partitions=all_parent_asset_partitions,
-                respect_materialization_data_versions=False,
-                ignored_parent_keys=set(),
-            )
+        return context.non_agv_instance_interface.get_parent_asset_partitions_updated_after_child(
+            asset_partition=candidate,
+            parent_asset_partitions=all_parent_asset_partitions,
+            ignored_parent_keys=set(),
         )
 
     def compute_parent_newer_slice(
         self, context: SchedulingContext, from_slice: AssetSlice
     ) -> AssetSlice:
         """For a given slice, computes the slice for which at least one parent is newer than the
         given asset partition.
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,21 @@
 class RequestedThisTickCondition(SliceSchedulingCondition):
     @property
     def description(self) -> str:
         return "Will be requested this tick"
 
     def _executable_with_root_context_key(self, context: SchedulingContext) -> bool:
         # TODO: once we can launch backfills via the asset daemon, this can be removed
+        from dagster._core.definitions.asset_graph import materializable_in_same_run
+
         root_key = context.root_context.asset_key
-        return context.legacy_context.materializable_in_same_run(
-            child_key=root_key, parent_key=context.asset_key
+        return materializable_in_same_run(
+            asset_graph=context.asset_graph_view.asset_graph,
+            child_key=root_key,
+            parent_key=context.asset_key,
         )
 
     def compute_slice(self, context: SchedulingContext) -> AssetSlice:
         current_info = context.current_tick_evaluation_info_by_key.get(context.asset_key)
         if (
             current_info
             and current_info.requested_slice
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,17 @@
             or context.previous_evaluation_node.true_slice is None
             # not evaluated since latest schedule tick
             or context.previous_evaluation_info.temporal_context.effective_dt < previous_cron_tick
             # has new set of candidates
             or context.previous_evaluation_node.candidate_slice != context.candidate_slice
         ):
             # do a full recomputation
-            updated_subset = (
-                context.legacy_context.instance_queryer.get_asset_subset_updated_after_time(
-                    asset_key=context.asset_key,
-                    after_time=previous_cron_tick,
-                )
+            updated_subset = context.non_agv_instance_interface.get_asset_subset_updated_after_time(
+                asset_key=context.asset_key,
+                after_time=previous_cron_tick,
             )
             # TODO: implement this on the AssetGraphView
             true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(updated_subset)
         else:
             # do an incremental updated, adding in any asset partitions that have been materialized
             # since the previous evaluation
             true_slice = context.previous_evaluation_node.true_slice.compute_union(
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/serialized_objects.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/serialized_objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/utils.py` & `dagster-1.7.7/dagster/_core/definitions/declarative_scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.7/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.7/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.7/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/dependency.py` & `dagster-1.7.7/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/events.py` & `dagster-1.7.7/dagster/_core/definitions/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import ABC, abstractmethod
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Generic,
@@ -11,14 +12,16 @@
     Optional,
     Sequence,
     TypeVar,
     Union,
     cast,
 )
 
+from typing_extensions import Self
+
 import dagster._check as check
 from dagster._annotations import PublicAttr, deprecated, experimental_param, public
 from dagster._core.definitions.asset_key import (
     AssetKey as AssetKey,
     CoercibleToAssetKey as CoercibleToAssetKey,
     CoercibleToAssetKeyPrefix as CoercibleToAssetKeyPrefix,
     parse_asset_key_string,
@@ -64,19 +67,27 @@
 ):
     def __new__(cls, asset_key: AssetKey, partitions: Optional[AbstractSet[str]] = None):
         asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
         partitions = check.opt_set_param(partitions, "partitions", str)
         return super(AssetLineageInfo, cls).__new__(cls, asset_key=asset_key, partitions=partitions)
 
 
+class EventWithMetadata(ABC):
+    @abstractmethod
+    def with_metadata(self, metadata: Optional[Mapping[str, RawMetadataValue]]) -> Self:
+        """Returns a new instance of the event with the same properties as the original,
+        but with metadata replaced by the provided value.
+        """
+
+
 T = TypeVar("T")
 
 
 @experimental_param(param="data_version")
-class Output(Generic[T]):
+class Output(Generic[T], EventWithMetadata):
     """Event corresponding to one of an op's outputs.
 
     Op compute functions must explicitly yield events of this type when they have more than
     one output, or when they also yield events of other types, or when defining a op using the
     :py:class:`OpDefinition` API directly.
 
     Outputs are values produced by ops that will be consumed by downstream ops in a job.
@@ -242,15 +253,16 @@
         [
             ("asset_key", PublicAttr[AssetKey]),
             ("description", PublicAttr[Optional[str]]),
             ("metadata", PublicAttr[Mapping[str, MetadataValue]]),
             ("partition", PublicAttr[Optional[str]]),
             ("tags", PublicAttr[Mapping[str, str]]),
         ],
-    )
+    ),
+    EventWithMetadata,
 ):
     """Event that captures metadata about an asset at a point in time.
 
     Args:
         asset_key (Union[str, List[str], AssetKey]): A key to identify the asset.
         partition (Optional[str]): The name of a partition of the asset that the metadata
             corresponds to.
@@ -296,14 +308,25 @@
     def label(self) -> str:
         return " ".join(self.asset_key.path)
 
     @property
     def data_version(self) -> Optional[str]:
         return self.tags.get(DATA_VERSION_TAG)
 
+    def with_metadata(
+        self, metadata: Optional[Mapping[str, RawMetadataValue]]
+    ) -> "AssetObservation":
+        return AssetObservation(
+            asset_key=self.asset_key,
+            description=self.description,
+            metadata=metadata,
+            partition=self.partition,
+            tags=self.tags,
+        )
+
 
 UNDEFINED_ASSET_KEY_PATH = ["__undefined__"]
 
 
 class AssetMaterializationSerializer(NamedTupleSerializer):
     # There are old `Materialization` objects in storage. We set the default value for asset key to
     # be `AssetKey(["__undefined__"])` to ensure that we can load these objects, without needing to
@@ -327,15 +350,16 @@
         [
             ("asset_key", PublicAttr[AssetKey]),
             ("description", PublicAttr[Optional[str]]),
             ("metadata", PublicAttr[Mapping[str, MetadataValue]]),
             ("partition", PublicAttr[Optional[str]]),
             ("tags", Optional[Mapping[str, str]]),
         ],
-    )
+    ),
+    EventWithMetadata,
 ):
     """Event indicating that an op has materialized an asset.
 
     Op compute functions may yield events of this type whenever they wish to indicate to the
     Dagster framework (and the end user) that they have produced a materialized value as a
     side effect of computation. Unlike outputs, asset materializations can not be passed to other
     ops, and their persistence is controlled by op logic, rather than by the Dagster
@@ -425,14 +449,25 @@
 
         return AssetMaterialization(
             asset_key=cast(Union[str, AssetKey, List[str]], asset_key),
             description=description,
             metadata={"path": MetadataValue.path(path)},
         )
 
+    def with_metadata(
+        self, metadata: Optional[Mapping[str, RawMetadataValue]]
+    ) -> "AssetMaterialization":
+        return AssetMaterialization(
+            asset_key=self.asset_key,
+            description=self.description,
+            metadata=metadata,
+            partition=self.partition,
+            tags=self.tags,
+        )
+
 
 @deprecated(
     breaking_version="2.0",
     additional_warn_text="If using assets, use AssetCheckResult and @asset_check instead.",
 )
 @whitelist_for_serdes(
     storage_field_names={"metadata": "metadata_entries"},
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/external_asset.py` & `dagster-1.7.7/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.7/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.7/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.7/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.7/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.7/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/inference.py` & `dagster-1.7.7/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/input.py` & `dagster-1.7.7/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.7/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/job_base.py` & `dagster-1.7.7/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/job_definition.py` & `dagster-1.7.7/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.7/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.7/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.7/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.7/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/materialize.py` & `dagster-1.7.7/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     UrlMetadataValue as UrlMetadataValue,
 )
 from .source_code import (
     DEFAULT_SOURCE_FILE_KEY as DEFAULT_SOURCE_FILE_KEY,
     CodeReferencesMetadataSet as CodeReferencesMetadataSet,
     CodeReferencesMetadataValue as CodeReferencesMetadataValue,
     LocalFileCodeReference as LocalFileCodeReference,
+    UrlCodeReference as UrlCodeReference,
+    link_to_source_control as link_to_source_control,
     with_source_code_references as with_source_code_references,
 )
 from .table import (  # re-exported
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/metadata/metadata_set.py` & `dagster-1.7.7/dagster/_core/definitions/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/metadata/metadata_value.py` & `dagster-1.7.7/dagster/_core/definitions/metadata/metadata_value.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.7/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
 )
 from dagster._core.instance import DagsterInstance
 from dagster._core.instance.ref import InstanceRef
 from dagster._utils import normalize_to_repository
-from dagster._utils.warnings import normalize_renamed_param
+from dagster._utils.warnings import deprecation_warning, normalize_renamed_param
 
 from .events import AssetKey
 from .run_request import RunRequest, SensorResult, SkipReason
 from .sensor_definition import (
     DefaultSensorStatus,
     SensorDefinition,
     SensorEvaluationContext,
@@ -51,14 +51,15 @@
 
 if TYPE_CHECKING:
     from dagster._core.definitions.definitions_class import Definitions
     from dagster._core.definitions.repository_definition import RepositoryDefinition
     from dagster._core.storage.event_log.base import EventLogRecord
 
 MAX_NUM_UNCONSUMED_EVENTS = 25
+FETCH_MATERIALIZATION_BATCH_SIZE = 1000
 
 
 class MultiAssetSensorAssetCursorComponent(
     NamedTuple(
         "_MultiAssetSensorAssetCursorComponent",
         [
             ("latest_consumed_event_partition", Optional[str]),
@@ -292,33 +293,33 @@
             instance=instance,
             repository_def=repository_def,
             resources=resource_defs,
             last_sensor_start_time=last_sensor_start_time,
         )
 
     def _cache_initial_unconsumed_events(self) -> None:
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventRecordsFilter
+        from dagster._core.event_api import AssetRecordsFilter
 
         # This method caches the initial unconsumed events for each asset key. To generate the
         # current unconsumed events, call get_trailing_unconsumed_events instead.
         if self._fetched_initial_unconsumed_events:
             return
 
         for asset_key in self._monitored_asset_keys:
             unconsumed_event_ids = list(
                 self._get_cursor(asset_key).trailing_unconsumed_partitioned_event_ids.values()
             )
             if unconsumed_event_ids:
-                event_records = self.instance.get_event_records(
-                    EventRecordsFilter(
-                        event_type=DagsterEventType.ASSET_MATERIALIZATION,
+                event_records = self.instance.fetch_materializations(
+                    AssetRecordsFilter(
+                        asset_key=asset_key,
                         storage_ids=unconsumed_event_ids,
-                    )
-                )
+                    ),
+                    limit=len(unconsumed_event_ids),
+                ).records
                 self._initial_unconsumed_events_by_id.update(
                     {event_record.storage_id: event_record for event_record in event_records}
                 )
 
         self._fetched_initial_unconsumed_events = True
 
     def _get_unconsumed_events_with_ids(
@@ -436,34 +437,48 @@
 
         Only fetches events after the latest consumed event ID for the given asset key.
 
         Args:
             asset_key (AssetKey): The asset to fetch materialization events for
             limit (Optional[int]): The number of events to fetch
         """
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventRecordsFilter
+        from dagster._core.event_api import AssetRecordsFilter
 
         asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
         if asset_key not in self._assets_by_key:
             raise DagsterInvalidInvocationError(f"Asset key {asset_key} not monitored by sensor.")
 
-        events = list(
-            self.instance.get_event_records(
-                EventRecordsFilter(
-                    event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                    asset_key=asset_key,
-                    after_cursor=self._get_cursor(asset_key).latest_consumed_event_id,
-                ),
-                ascending=True,
-                limit=limit,
-            )
-        )
+        if not limit:
+            deprecation_warning("Calling materialization_records_for_key without a limit", "1.8")
+            records = []
+            has_more = True
+            cursor = None
+            while has_more:
+                result = self.instance.fetch_materializations(
+                    AssetRecordsFilter(
+                        asset_key=asset_key,
+                        after_storage_id=self._get_cursor(asset_key).latest_consumed_event_id,
+                    ),
+                    ascending=True,
+                    limit=FETCH_MATERIALIZATION_BATCH_SIZE,
+                    cursor=cursor,
+                )
+                cursor = result.cursor
+                has_more = result.has_more
+                records.extend(result.records)
+            return records
 
-        return events
+        return self.instance.fetch_materializations(
+            AssetRecordsFilter(
+                asset_key=asset_key,
+                after_storage_id=self._get_cursor(asset_key).latest_consumed_event_id,
+            ),
+            ascending=True,
+            limit=limit,
+        ).records
 
     def _get_cursor(self, asset_key: AssetKey) -> MultiAssetSensorAssetCursorComponent:
         """Returns the MultiAssetSensorAssetCursorComponent for the asset key.
 
         For more information, view the docstring for the MultiAssetSensorAssetCursorComponent class.
         """
         check.inst_param(asset_key, "asset_key", AssetKey)
@@ -502,16 +517,15 @@
                 def my_sensor(context):
                     context.latest_materialization_records_by_partition(july_asset.key)
 
                 # After materializing july_asset for 2022-07-05, latest_materialization_by_partition
                 # returns {"2022-07-05": EventLogRecord(...)}
 
         """
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventLogRecord, EventRecordsFilter
+        from dagster._core.event_api import AssetRecordsFilter, EventLogRecord
 
         asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
 
         if asset_key not in self._assets_by_key:
             raise DagsterInvalidInvocationError(
                 f"Asset key {asset_key} not monitored in sensor definition"
             )
@@ -543,34 +557,39 @@
                 if partition in materialization_by_partition:
                     # Remove partition to ensure materialization_by_partition preserves
                     # the order of materializations
                     materialization_by_partition.pop(partition)
                 # Add partition and materialization to the end of the OrderedDict
                 materialization_by_partition[partition] = unconsumed_event
 
-        partition_materializations = self.instance.get_event_records(
-            EventRecordsFilter(
-                event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                asset_key=asset_key,
-                asset_partitions=partitions_to_fetch,
-                after_cursor=self._get_cursor(asset_key).latest_consumed_event_id,
-            ),
-            ascending=True,
-        )
-        for materialization in partition_materializations:
-            partition = materialization.partition_key
+        has_more = True
+        cursor = None
+        while has_more:
+            result = self.instance.fetch_materializations(
+                AssetRecordsFilter(
+                    asset_key=asset_key,
+                    asset_partitions=partitions_to_fetch,
+                    after_storage_id=self._get_cursor(asset_key).latest_consumed_event_id,
+                ),
+                ascending=True,
+                limit=FETCH_MATERIALIZATION_BATCH_SIZE,
+                cursor=cursor,
+            )
+            cursor = result.cursor
+            has_more = result.has_more
+            for materialization in result.records:
+                if not isinstance(materialization.partition_key, str):
+                    continue
 
-            if isinstance(partition, str):
-                if partition in materialization_by_partition:
+                if materialization.partition_key in materialization_by_partition:
                     # Remove partition to ensure materialization_by_partition preserves
                     # the order of materializations
-                    materialization_by_partition.pop(partition)
+                    materialization_by_partition.pop(materialization.partition_key)
                 # Add partition and materialization to the end of the OrderedDict
-                materialization_by_partition[partition] = materialization
-
+                materialization_by_partition[materialization.partition_key] = materialization
         return materialization_by_partition
 
     @public
     def latest_materialization_records_by_partition_and_asset(
         self,
     ) -> Mapping[str, Mapping[AssetKey, "EventLogRecord"]]:
         """Finds the most recent unconsumed materialization for each partition for each asset
@@ -925,29 +944,20 @@
             trailing_unconsumed_partitioned_event_ids=latest_unconsumed_record_by_partition,
         )
 
 
 def get_cursor_from_latest_materializations(
     asset_keys: Sequence[AssetKey], instance: DagsterInstance
 ) -> str:
-    from dagster._core.events import DagsterEventType
-    from dagster._core.storage.event_log.base import EventRecordsFilter
-
     cursor_dict: Dict[str, MultiAssetSensorAssetCursorComponent] = {}
 
     for asset_key in asset_keys:
-        materializations = instance.get_event_records(
-            EventRecordsFilter(
-                DagsterEventType.ASSET_MATERIALIZATION,
-                asset_key=asset_key,
-            ),
-            limit=1,
-        )
+        materializations = instance.fetch_materializations(asset_key, limit=1).records
         if materializations:
-            last_materialization = list(materializations)[-1]
+            last_materialization = materializations[0]
 
             cursor_dict[str(asset_key)] = MultiAssetSensorAssetCursorComponent(
                 last_materialization.partition_key,
                 last_materialization.storage_id,
                 {},
             )
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.7/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/node_container.py` & `dagster-1.7.7/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/node_definition.py` & `dagster-1.7.7/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/observe.py` & `dagster-1.7.7/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/op_definition.py` & `dagster-1.7.7/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.7/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/op_selection.py` & `dagster-1.7.7/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/output.py` & `dagster-1.7.7/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/partition.py` & `dagster-1.7.7/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.7/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.7/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.7/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/policy.py` & `dagster-1.7.7/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.7/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.7/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.7/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.7/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,20 +99,27 @@
         # e.g. [snowflake, elementl, key] and [snowflake, elementl, prod, key]
         is_off_by_one_prefix_component_same_name = (
             asset_key.path[-1] == target_asset_key.path[-1]
             and len(set(asset_key.path).symmetric_difference(set(target_asset_key.path))) == 1
             and max(len(asset_key.path), len(target_asset_key.path)) > 1
         )
 
+        # If the asset key provided has no prefix and the upstream key has
+        # the same name but a prefix of any length
+        no_prefix_but_is_match_with_prefix = (
+            len(target_asset_key) == 1 and asset_key.path[-1] == target_asset_key.path[-1]
+        )
+
         matches_slashes_turned_to_prefix_gaps = asset_key.path == target_asset_key_split
 
         if (
             is_same_prefix_similar_name
             or is_similar_prefix_same_name
             or is_off_by_one_prefix_component_same_name
+            or no_prefix_but_is_match_with_prefix
             or matches_slashes_turned_to_prefix_gaps
         ):
             similar_names.append(asset_key)
     return sorted(similar_names, key=lambda key: key.to_string())
 
 
 def resolve_assets_def_deps(
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.7/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.7/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.7/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.7/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/result.py` & `dagster-1.7.7/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/run_config.py` & `dagster-1.7.7/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.7/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/run_request.py` & `dagster-1.7.7/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.7/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.7/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/selector.py` & `dagster-1.7.7/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.7/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/source_asset.py` & `dagster-1.7.7/dagster/_core/definitions/source_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ensure_requirements_satisfied,
     get_resource_key_conflicts,
 )
 from dagster._core.definitions.result import ObserveResult
 from dagster._core.definitions.utils import (
     DEFAULT_GROUP_NAME,
     DEFAULT_IO_MANAGER_KEY,
-    validate_group_name,
+    normalize_group_name,
 )
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidObservationError,
 )
 
@@ -253,15 +253,15 @@
 
         self.resource_defs = wrap_resources_for_execution(resource_defs_dict)
 
         self.io_manager_key = check.opt_str_param(io_manager_key, "io_manager_key")
         self.partitions_def = check.opt_inst_param(
             partitions_def, "partitions_def", PartitionsDefinition
         )
-        self.group_name = validate_group_name(group_name)
+        self.group_name = normalize_group_name(group_name)
         self.description = check.opt_str_param(description, "description")
         self.observe_fn = check.opt_callable_param(observe_fn, "observe_fn")
         self.op_tags = check.opt_mapping_param(op_tags, "op_tags")
         self._required_resource_keys = check.opt_set_param(
             _required_resource_keys, "_required_resource_keys", of_type=str
         )
         self._node_def = None
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.7/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/target.py` & `dagster-1.7.7/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.7/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.7/dagster/_core/definitions/time_window_partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import hashlib
 import json
 import re
 from abc import abstractmethod, abstractproperty
-from datetime import datetime, timedelta
+from datetime import date, datetime, timedelta
 from enum import Enum
 from functools import cached_property
 from typing import (
     AbstractSet,
     Any,
     Callable,
     FrozenSet,
@@ -44,14 +44,15 @@
 from dagster._seven.compat.pendulum import (
     _IS_PENDULUM_1,
     PRE_TRANSITION,
     PendulumDateTime,
     create_pendulum_time,
     to_timezone,
 )
+from dagster._utils.cronstring import get_fixed_minute_interval, is_basic_daily, is_basic_hourly
 from dagster._utils.partitions import DEFAULT_HOURLY_FORMAT_WITHOUT_TIMEZONE
 from dagster._utils.schedules import (
     cron_string_iterator,
     cron_string_repeats_every_hour,
     is_valid_cron_schedule,
     reverse_cron_string_iterator,
 )
@@ -366,22 +367,61 @@
     def get_current_timestamp(self, current_time: Optional[datetime] = None) -> float:
         return (
             pendulum.instance(current_time, tz=self.timezone)
             if current_time
             else pendulum.now(self.timezone)
         ).timestamp()
 
+    def _get_fast_num_partitions(self, current_time: Optional[datetime] = None) -> Optional[int]:
+        """Computes the total number of partitions quickly for common partition windows. Returns
+        None if the count cannot be computed quickly and must enumerate all partitions before
+        counting them.
+        """
+        last_partition_window = self.get_last_partition_window(current_time)
+        first_partition_window = self.get_first_partition_window(current_time)
+
+        if not last_partition_window or not first_partition_window:
+            return None
+
+        if self.is_basic_daily:
+            return (
+                date(
+                    last_partition_window.start.year,
+                    last_partition_window.start.month,
+                    last_partition_window.start.day,
+                )
+                - date(
+                    first_partition_window.start.year,
+                    first_partition_window.start.month,
+                    first_partition_window.start.day,
+                )
+            ).days + 1
+
+        fixed_minute_interval = get_fixed_minute_interval(self.cron_schedule)
+        if fixed_minute_interval:
+            minutes_in_window = (
+                last_partition_window.start.timestamp() - first_partition_window.start.timestamp()
+            ) / 60
+            return int(minutes_in_window // fixed_minute_interval) + 1
+
+        return None
+
     def get_num_partitions(
         self,
         current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> int:
         # Method added for performance reasons.
         # Fetching partition keys requires significantly more compute time to
         # string format datetimes.
+
+        fast_num_partitions = self._get_fast_num_partitions(current_time)
+        if fast_num_partitions is not None:
+            return fast_num_partitions
+
         current_timestamp = self.get_current_timestamp(current_time=current_time)
 
         partitions_past_current_time = 0
 
         num_partitions = 0
         for time_window in self._iterate_time_windows(self.start):
             if self.end and time_window.end.timestamp() > self.end.timestamp():
@@ -1023,19 +1063,19 @@
             and self.fmt == other.fmt
             and self.cron_schedule == other.cron_schedule
             and self.end_offset == other.end_offset
         )
 
     @property
     def is_basic_daily(self) -> bool:
-        return self.cron_schedule == "0 0 * * *"
+        return is_basic_daily(self.cron_schedule)
 
     @property
     def is_basic_hourly(self) -> bool:
-        return self.cron_schedule == "0 * * * *"
+        return is_basic_hourly(self.cron_schedule)
 
 
 class DailyPartitionsDefinition(TimeWindowPartitionsDefinition):
     """A set of daily partitions.
 
     The first partition in the set will start at the start_date at midnight. The last partition
     in the set will end before the current time, unless the end_offset argument is set to a
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.7/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/definitions/utils.py` & `dagster-1.7.7/dagster/_core/definitions/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     if not is_valid_definition_tag_value(value):
         raise DagsterInvalidDefinitionError(
             f"Invalid tag value: {value}, for key: {key}. Allowed characters: alpha-numeric, '_', '-', '.'. "
             "Must have <= 63 characters."
         )
 
 
-def validate_group_name(group_name: Optional[str]) -> str:
+def normalize_group_name(group_name: Optional[str]) -> str:
     """Ensures a string name is valid and returns a default if no name provided."""
     if group_name:
         check_valid_chars(group_name)
         return group_name
     elif group_name == "":
         raise DagsterInvalidDefinitionError(
             "Empty asset group name was provided, which is not permitted."
```

### Comparing `dagster-1.7.6/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.7/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/errors.py` & `dagster-1.7.7/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/event_api.py` & `dagster-1.7.7/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/events/__init__.py` & `dagster-1.7.7/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/events/log.py` & `dagster-1.7.7/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/events/utils.py` & `dagster-1.7.7/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/api.py` & `dagster-1.7.7/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.7/dagster/_core/execution/asset_backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 )
 from dagster._core.errors import (
     DagsterAssetBackfillDataLoadError,
     DagsterBackfillFailedError,
     DagsterDefinitionChangedDeserializationError,
     DagsterInvariantViolationError,
 )
-from dagster._core.event_api import EventRecordsFilter
-from dagster._core.events import DagsterEventType
+from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.dagster_run import (
     CANCELABLE_RUN_STATUSES,
     IN_PROGRESS_RUN_STATUSES,
     DagsterRunStatus,
     RunsFilter,
 )
@@ -75,15 +74,15 @@
 
 from .submit_asset_runs import submit_asset_runs_in_chunks
 
 if TYPE_CHECKING:
     from .backfill import PartitionBackfill
 
 RUN_CHUNK_SIZE = 25
-
+MATERIALIZATION_CHUNK_SIZE = 1000
 
 MAX_RUNS_CANCELED_PER_ITERATION = 50
 
 
 class AssetBackfillStatus(Enum):
     IN_PROGRESS = "IN_PROGRESS"
     MATERIALIZED = "MATERIALIZED"
@@ -1108,37 +1107,42 @@
     """Returns the partitions that have been materialized by the backfill.
 
     This function is a generator so we can return control to the daemon and let it heartbeat
     during expensive operations.
     """
     recently_materialized_asset_partitions = AssetGraphSubset()
     for asset_key in asset_backfill_data.target_subset.asset_keys:
-        records = instance_queryer.instance.get_event_records(
-            EventRecordsFilter(
-                event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                asset_key=asset_key,
-                after_cursor=asset_backfill_data.latest_storage_id,
-            )
-        )
-        records_in_backfill = [
-            record
-            for record in records
-            if instance_queryer.run_has_tag(
-                run_id=record.run_id, tag_key=BACKFILL_ID_TAG, tag_value=backfill_id
-            )
-        ]
-        recently_materialized_asset_partitions |= AssetGraphSubset.from_asset_partition_set(
-            {
-                AssetKeyPartitionKey(asset_key, record.partition_key)
-                for record in records_in_backfill
-            },
-            asset_graph,
-        )
-
-        yield None
+        cursor = None
+        has_more = True
+        while has_more:
+            result = instance_queryer.instance.fetch_materializations(
+                AssetRecordsFilter(
+                    asset_key=asset_key,
+                    after_storage_id=asset_backfill_data.latest_storage_id,
+                ),
+                cursor=cursor,
+                limit=MATERIALIZATION_CHUNK_SIZE,
+            )
+            records_in_backfill = [
+                record
+                for record in result.records
+                if instance_queryer.run_has_tag(
+                    run_id=record.run_id, tag_key=BACKFILL_ID_TAG, tag_value=backfill_id
+                )
+            ]
+            recently_materialized_asset_partitions |= AssetGraphSubset.from_asset_partition_set(
+                {
+                    AssetKeyPartitionKey(asset_key, record.partition_key)
+                    for record in records_in_backfill
+                },
+                asset_graph,
+            )
+            cursor = result.cursor
+            has_more = result.has_more
+            yield None
 
     updated_materialized_subset = (
         asset_backfill_data.materialized_subset | recently_materialized_asset_partitions
     )
 
     yield updated_materialized_subset
```

### Comparing `dagster-1.7.6/dagster/_core/execution/backfill.py` & `dagster-1.7.7/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/build_resources.py` & `dagster-1.7.7/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/compute_logs.py` & `dagster-1.7.7/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/compute.py` & `dagster-1.7.7/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/data_version_cache.py` & `dagster-1.7.7/dagster/_core/execution/context/data_version_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/hook.py` & `dagster-1.7.7/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/init.py` & `dagster-1.7.7/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/input.py` & `dagster-1.7.7/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/invocation.py` & `dagster-1.7.7/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/logger.py` & `dagster-1.7.7/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/output.py` & `dagster-1.7.7/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context/system.py` & `dagster-1.7.7/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.7/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.7/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.7/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/execution_result.py` & `dagster-1.7.7/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/host_mode.py` & `dagster-1.7.7/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/job_backfill.py` & `dagster-1.7.7/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.7/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/memoization.py` & `dagster-1.7.7/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/active.py` & `dagster-1.7.7/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/compute.py` & `dagster-1.7.7/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.7/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.7/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.7/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.7/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/handle.py` & `dagster-1.7.7/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.7/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.7/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.7/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/objects.py` & `dagster-1.7.7/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.7/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/plan.py` & `dagster-1.7.7/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/state.py` & `dagster-1.7.7/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/step.py` & `dagster-1.7.7/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/plan/utils.py` & `dagster-1.7.7/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.7/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.7/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/resources_init.py` & `dagster-1.7.7/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/retries.py` & `dagster-1.7.7/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.7/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/run_metrics_thread.py` & `dagster-1.7.7/dagster/_core/execution/run_metrics_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import os.path
 import threading
 from sys import platform
 from typing import Dict, Optional, Tuple, Union
 
 import dagster._check as check
-from dagster._core.execution.types import RunTelemetryData
+from dagster._core.execution.telemetry import RunTelemetryData
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._utils.container import (
     retrieve_containerized_utilization_metrics,
 )
 
 DEFAULT_RUN_METRICS_POLL_INTERVAL_SECONDS = 15.0
```

### Comparing `dagster-1.7.6/dagster/_core/execution/stats.py` & `dagster-1.7.7/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.7/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/tags.py` & `dagster-1.7.7/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.7/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.7/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/execution/with_resources.py` & `dagster-1.7.7/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/base.py` & `dagster-1.7.7/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.7/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/in_process.py` & `dagster-1.7.7/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/init.py` & `dagster-1.7.7/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/multiprocess.py` & `dagster-1.7.7/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.7/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.7/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/instance/__init__.py` & `dagster-1.7.7/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/instance/config.py` & `dagster-1.7.7/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/instance/ref.py` & `dagster-1.7.7/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/instance_for_test.py` & `dagster-1.7.7/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/launcher/base.py` & `dagster-1.7.7/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.7/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.7/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/log_manager.py` & `dagster-1.7.7/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/nux.py` & `dagster-1.7.7/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.7/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/origin.py` & `dagster-1.7.7/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/pipes/client.py` & `dagster-1.7.7/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/pipes/context.py` & `dagster-1.7.7/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/pipes/subprocess.py` & `dagster-1.7.7/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/pipes/utils.py` & `dagster-1.7.7/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.7/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.7/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/external.py` & `dagster-1.7.7/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.7/dagster/_core/remote_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,18 @@
 )
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.definitions.utils import DEFAULT_GROUP_NAME
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.snap import JobSnapshot
 from dagster._core.snap.mode import ResourceDefSnap, build_resource_def_snap
 from dagster._core.storage.io_manager import IOManagerDefinition
+from dagster._core.utils import is_valid_email
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
+    FieldSerializer,
     is_whitelisted_for_serdes_object,
 )
 from dagster._utils.error import SerializableErrorInfo
 
 DEFAULT_MODE_NAME = "default"
 DEFAULT_PRESET_NAME = "default"
 
@@ -1269,20 +1271,42 @@
         )
 
     @property
     def key(self) -> AssetCheckKey:
         return AssetCheckKey(asset_key=self.asset_key, name=self.name)
 
 
+class BackcompatTeamOwnerFieldDeserializer(FieldSerializer):
+    """Up through Dagster 1.7.7, asset owners provided as "team:foo" would be serialized as "foo"
+    going forward, they're serialized as "team:foo".
+    """
+
+    def unpack(self, __unpacked_value, whitelist_map, context):
+        return (
+            [
+                owner if (is_valid_email(owner) or owner.startswith("team:")) else f"team:{owner}"
+                for owner in cast(Sequence[str], __unpacked_value)
+            ]
+            if __unpacked_value is not None
+            else None
+        )
+
+    def pack(self, __unpacked_value, whitelist_map, descent_path):
+        return __unpacked_value
+
+
 @whitelist_for_serdes(
     storage_field_names={
         "metadata": "metadata_entries",
         "execution_set_identifier": "atomic_execution_unit_id",
     },
-    field_serializers={"metadata": MetadataFieldSerializer},
+    field_serializers={
+        "metadata": MetadataFieldSerializer,
+        "owners": BackcompatTeamOwnerFieldDeserializer,
+    },
 )
 class ExternalAssetNode(
     NamedTuple(
         "_ExternalAssetNode",
         [
             ("asset_key", AssetKey),
             ("dependencies", Sequence[ExternalAssetDependency]),
```

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.7/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.7/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.7/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/handle.py` & `dagster-1.7.7/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/historical.py` & `dagster-1.7.7/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.7/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/origin.py` & `dagster-1.7.7/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/remote_representation/represented.py` & `dagster-1.7.7/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/run_coordinator/base.py` & `dagster-1.7.7/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.7/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.7/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/scheduler/__init__.py` & `dagster-1.7.7/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/scheduler/execution.py` & `dagster-1.7.7/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/scheduler/instigation.py` & `dagster-1.7.7/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.7/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/secrets/env_file.py` & `dagster-1.7.7/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/selector/subset_selector.py` & `dagster-1.7.7/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/__init__.py` & `dagster-1.7.7/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/dagster_types.py` & `dagster-1.7.7/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.7/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.7/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.7/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/mode.py` & `dagster-1.7.7/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/node.py` & `dagster-1.7.7/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.7/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.7/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/README.md` & `dagster-1.7.7/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/env.py` & `dagster-1.7.7/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.7/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.7/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.7/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/base_storage.py` & `dagster-1.7.7/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/batch_asset_record_loader.py` & `dagster-1.7.7/dagster/_core/storage/batch_asset_record_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,35 @@
 from dagster import InputContext, OutputContext
 from dagster._config.pythonic_config import (
     ConfigurableIOManager,
     ResourceDependency,
 )
 from dagster._core.definitions.events import AssetKey, AssetMaterialization
 from dagster._core.definitions.metadata import TextMetadataValue
-from dagster._core.event_api import EventRecordsFilter
-from dagster._core.events import DagsterEventType
+from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.events.log import EventLogEntry
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.io_manager import IOManager
 
 
 def get_text_metadata_value(materialization: AssetMaterialization, key: str) -> Optional[str]:
     metadata_value = materialization.metadata.get(key)
     return metadata_value.value if isinstance(metadata_value, TextMetadataValue) else None
 
 
 def latest_materialization_log_entry(
     instance: DagsterInstance, asset_key: AssetKey, partition_key: Optional[str] = None
 ) -> Optional[EventLogEntry]:
-    event_records = [
-        *instance.get_event_records(
-            event_records_filter=EventRecordsFilter(
-                event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                asset_key=asset_key,
-                asset_partitions=[partition_key] if partition_key else None,
-            ),
-            limit=1,
-        )
-    ]
+    event_records = instance.fetch_materializations(
+        AssetRecordsFilter(
+            asset_key=asset_key,
+            asset_partitions=[partition_key] if partition_key else None,
+        ),
+        limit=1,
+    ).records
     return event_records[0].event_log_entry if event_records else None
 
 
 class BranchingIOManager(ConfigurableIOManager):
     """A branching I/O manager composes two I/O managers.
 
     1) The parent I/O manager, typically your production environment.
```

### Comparing `dagster-1.7.6/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.7/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.7/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.7/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/config.py` & `dagster-1.7.7/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/dagster_run.py` & `dagster-1.7.7/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.7/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/base.py` & `dagster-1.7.7/dagster/_core/storage/event_log/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,20 @@
     Users should not invoke this class directly.
     """
 
     storage_id: int
     asset_entry: AssetEntry
 
 
+class AssetCheckSummaryRecord(NamedTuple):
+    asset_check_key: AssetCheckKey
+    last_check_execution_record: Optional[AssetCheckExecutionRecord]
+    last_run_id: Optional[str]
+
+
 class PlannedMaterializationInfo(NamedTuple):
     """Internal representation of an planned materialization event, containing storage_id / run_id.
 
     Users should not invoke this class directly.
     """
 
     storage_id: int
@@ -309,14 +315,20 @@
 
     @abstractmethod
     def get_asset_records(
         self, asset_keys: Optional[Sequence[AssetKey]] = None
     ) -> Sequence[AssetRecord]:
         pass
 
+    @abstractmethod
+    def get_asset_check_summary_records(
+        self, asset_check_keys: Sequence[AssetCheckKey]
+    ) -> Mapping[AssetCheckKey, AssetCheckSummaryRecord]:
+        pass
+
     @property
     def asset_records_have_last_planned_materialization_storage_id(self) -> bool:
         return False
 
     @abstractmethod
     def has_asset_key(self, asset_key: AssetKey) -> bool:
         pass
```

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.7/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.7/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.7/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.7/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.7/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     PendingStepInfo,
     get_max_concurrency_limit_value,
 )
 from dagster._utils.warnings import deprecation_warning
 
 from ..dagster_run import DagsterRunStatsSnapshot
 from .base import (
+    AssetCheckSummaryRecord,
     AssetEntry,
     AssetRecord,
     AssetRecordsFilter,
     EventLogConnection,
     EventLogCursor,
     EventLogRecord,
     EventLogStorage,
@@ -390,15 +391,17 @@
                         dict(
                             event_id=event_id,
                             asset_key=asset_key_str,
                             key=tag,
                             value=new_tags[tag],
                             # Postgres requires a datetime that is in UTC but has no timezone info
                             # set in order to be stored correctly
-                            event_timestamp=datetime.utcfromtimestamp(event_timestamp),
+                            event_timestamp=datetime.fromtimestamp(
+                                event_timestamp, timezone.utc
+                            ).replace(tzinfo=None),
                         )
                         for tag in added_tags
                     ],
                 )
 
     def store_asset_event_tags(
         self, events: Sequence[EventLogEntry], event_ids: Sequence[int]
@@ -877,15 +880,17 @@
             query = query.where(
                 SqlEventLogStorageTable.c.partition.in_(event_records_filter.asset_partitions)
             )
 
         if asset_details and asset_details.last_wipe_timestamp:
             query = query.where(
                 SqlEventLogStorageTable.c.timestamp
-                > datetime.utcfromtimestamp(asset_details.last_wipe_timestamp)
+                > datetime.fromtimestamp(asset_details.last_wipe_timestamp, timezone.utc).replace(
+                    tzinfo=None
+                )
             )
 
         if apply_cursor_filters:
             # allow the run-sharded sqlite implementation to disable this cursor filtering so that
             # it can implement its own custom cursor logic, as cursor ids are not unique across run
             # shards
             if event_records_filter.before_cursor is not None:
@@ -903,21 +908,25 @@
                     else event_records_filter.after_cursor
                 )
                 query = query.where(SqlEventLogStorageTable.c.id > after_cursor_id)
 
         if event_records_filter.before_timestamp:
             query = query.where(
                 SqlEventLogStorageTable.c.timestamp
-                < datetime.utcfromtimestamp(event_records_filter.before_timestamp)
+                < datetime.fromtimestamp(
+                    event_records_filter.before_timestamp, timezone.utc
+                ).replace(tzinfo=None)
             )
 
         if event_records_filter.after_timestamp:
             query = query.where(
                 SqlEventLogStorageTable.c.timestamp
-                > datetime.utcfromtimestamp(event_records_filter.after_timestamp)
+                > datetime.fromtimestamp(
+                    event_records_filter.after_timestamp, timezone.utc
+                ).replace(tzinfo=None)
             )
 
         if event_records_filter.storage_ids:
             query = query.where(SqlEventLogStorageTable.c.id.in_(event_records_filter.storage_ids))
 
         return query
 
@@ -1308,14 +1317,27 @@
                         latest_materialization_records.get(asset_key),
                         can_cache_asset_status_data,
                     )
                 )
 
         return asset_records
 
+    def get_asset_check_summary_records(
+        self, asset_check_keys: Sequence[AssetCheckKey]
+    ) -> Mapping[AssetCheckKey, AssetCheckSummaryRecord]:
+        states = {}
+        for asset_check_key in asset_check_keys:
+            execution_record = self.get_asset_check_execution_history(asset_check_key, limit=1)
+            states[asset_check_key] = AssetCheckSummaryRecord(
+                asset_check_key=asset_check_key,
+                last_check_execution_record=execution_record[0] if execution_record else None,
+                last_run_id=execution_record[0].run_id if execution_record else None,
+            )
+        return states
+
     def has_asset_key(self, asset_key: AssetKey) -> bool:
         check.inst_param(asset_key, "asset_key", AssetKey)
         rows = self._fetch_asset_rows(asset_keys=[asset_key])
         return bool(rows)
 
     def all_asset_keys(self):
         rows = self._fetch_asset_rows()
@@ -1614,15 +1636,17 @@
                 # If asset key is in row, keep the row if the timestamp > wipe timestamp, else remove the row.
                 # If asset key is not in row, keep the row.
                 query = query.where(
                     db.or_(
                         db.and_(
                             asset_key_in_row,
                             SqlEventLogStorageTable.c.timestamp
-                            > datetime.utcfromtimestamp(asset_details.last_wipe_timestamp),
+                            > datetime.fromtimestamp(
+                                asset_details.last_wipe_timestamp, timezone.utc
+                            ).replace(tzinfo=None),
                         ),
                         db.not_(asset_key_in_row),
                     )
                 )
 
         return query
 
@@ -1664,30 +1688,34 @@
                     AssetEventTagsTable.c.value,
                     AssetEventTagsTable.c.event_id,
                 ]
             ).where(AssetEventTagsTable.c.asset_key == asset_key.to_string())
             if asset_details and asset_details.last_wipe_timestamp:
                 tags_query = tags_query.where(
                     AssetEventTagsTable.c.event_timestamp
-                    > datetime.utcfromtimestamp(asset_details.last_wipe_timestamp)
+                    > datetime.fromtimestamp(
+                        asset_details.last_wipe_timestamp, timezone.utc
+                    ).replace(tzinfo=None)
                 )
         else:
             table = self._apply_tags_table_joins(AssetEventTagsTable, filter_tags, asset_key)
             tags_query = db_select(
                 [
                     AssetEventTagsTable.c.key,
                     AssetEventTagsTable.c.value,
                     AssetEventTagsTable.c.event_id,
                 ]
             ).select_from(table)
 
             if asset_details and asset_details.last_wipe_timestamp:
                 tags_query = tags_query.where(
                     AssetEventTagsTable.c.event_timestamp
-                    > datetime.utcfromtimestamp(asset_details.last_wipe_timestamp)
+                    > datetime.fromtimestamp(
+                        asset_details.last_wipe_timestamp, timezone.utc
+                    ).replace(tzinfo=None)
                 )
 
         if filter_event_id is not None:
             tags_query = tags_query.where(AssetEventTagsTable.c.event_id == filter_event_id)
 
         with self.index_connection() as conn:
             results = conn.execute(tags_query).fetchall()
```

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/file_manager.py` & `dagster-1.7.7/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/input_manager.py` & `dagster-1.7.7/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/io_manager.py` & `dagster-1.7.7/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.7/dagster/_core/storage/legacy_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,24 @@
     Union,
 )
 
 from dagster import (
     _check as check,
 )
 from dagster._config.config_schema import UserConfigSchema
+from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluationWithRunIds,
 )
 from dagster._core.definitions.events import AssetKey
 from dagster._core.event_api import EventHandlerFn
 from dagster._core.storage.asset_check_execution_record import (
     AssetCheckExecutionRecord,
 )
+from dagster._core.storage.event_log.base import AssetCheckSummaryRecord
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 from dagster._utils import PrintFn
 from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
 
 from .base_storage import DagsterStorage
 from .event_log.base import (
     AssetRecord,
@@ -501,14 +503,19 @@
         )
 
     def get_asset_records(
         self, asset_keys: Optional[Sequence["AssetKey"]] = None
     ) -> Iterable[AssetRecord]:
         return self._storage.event_log_storage.get_asset_records(asset_keys)
 
+    def get_asset_check_summary_records(
+        self, asset_check_keys: Sequence["AssetCheckKey"]
+    ) -> Mapping["AssetCheckKey", AssetCheckSummaryRecord]:
+        return self._storage.event_log_storage.get_asset_check_summary_records(asset_check_keys)
+
     def has_asset_key(self, asset_key: "AssetKey") -> bool:
         return self._storage.event_log_storage.has_asset_key(asset_key)
 
     def all_asset_keys(self) -> Iterable["AssetKey"]:
         return self._storage.event_log_storage.all_asset_keys()
 
     def get_asset_keys(
```

### Comparing `dagster-1.7.6/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.7/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.7/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/migration/utils.py` & `dagster-1.7.7/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.7/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/output_manager.py` & `dagster-1.7.7/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.7/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/root.py` & `dagster-1.7.7/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/base.py` & `dagster-1.7.7/dagster/_core/storage/runs/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Dict, Mapping, Optional, Sequence, Set, Tuple, Union
 
 from typing_extensions import TypedDict
 
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
-from dagster._core.execution.types import RunTelemetryData
+from dagster._core.execution.telemetry import RunTelemetryData
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.snap import ExecutionPlanSnapshot, JobSnapshot
 from dagster._core.storage.dagster_run import (
     DagsterRun,
     JobBucket,
     RunPartitionData,
     RunRecord,
```

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.7/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/migration.py` & `dagster-1.7.7/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/schema.py` & `dagster-1.7.7/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.7/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/base.py` & `dagster-1.7.7/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.7/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.7/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.7/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/sql.py` & `dagster-1.7.7/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.7/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/sqlite.py` & `dagster-1.7.7/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.7/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/tags.py` & `dagster-1.7.7/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.7/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.7/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.7/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/system_config/objects.py` & `dagster-1.7.7/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/telemetry.py` & `dagster-1.7.7/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/telemetry_upload.py` & `dagster-1.7.7/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/test_utils.py` & `dagster-1.7.7/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.7/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/config_schema.py` & `dagster-1.7.7/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/dagster_type.py` & `dagster-1.7.7/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/decorator.py` & `dagster-1.7.7/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.7/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/python_dict.py` & `dagster-1.7.7/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/python_set.py` & `dagster-1.7.7/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/python_tuple.py` & `dagster-1.7.7/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/types/transform_typing.py` & `dagster-1.7.7/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/utility_ops.py` & `dagster-1.7.7/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/utils.py` & `dagster-1.7.7/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.7/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/config_schema.py` & `dagster-1.7.7/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/context.py` & `dagster-1.7.7/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/load.py` & `dagster-1.7.7/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/load_target.py` & `dagster-1.7.7/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/permissions.py` & `dagster-1.7.7/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_core/workspace/workspace.py` & `dagster-1.7.7/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/__init__.py` & `dagster-1.7.7/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/asset_daemon.py` & `dagster-1.7.7/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/backfill.py` & `dagster-1.7.7/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/cli/__init__.py` & `dagster-1.7.7/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/controller.py` & `dagster-1.7.7/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/daemon.py` & `dagster-1.7.7/dagster/_daemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,26 +226,36 @@
         either NoneType or a SerializableErrorInfo.
 
         returns: generator (SerializableErrorInfo).
         """
 
 
 class IntervalDaemon(DagsterDaemon[TContext], ABC):
-    def __init__(self, interval_seconds, jitter_seconds: float = 0):
+    def __init__(
+        self,
+        interval_seconds,
+        *,
+        interval_jitter_seconds: float = 0,
+        startup_jitter_seconds: float = 0,
+    ):
         self.interval_seconds = check.numeric_param(interval_seconds, "interval_seconds")
-        self.jitter_seconds = jitter_seconds
+        self.interval_jitter_seconds = interval_jitter_seconds
+        self.startup_jitter_seconds = startup_jitter_seconds
         super().__init__()
 
     def core_loop(
         self,
         workspace_process_context: TContext,
         shutdown_event: Event,
     ) -> DaemonIterator:
+        if self.startup_jitter_seconds:
+            time.sleep(random.uniform(0, self.startup_jitter_seconds))
+
         while True:
-            interval = self.interval_seconds + random.uniform(0, self.jitter_seconds)
+            interval = self.interval_seconds + random.uniform(0, self.interval_jitter_seconds)
             start_time = time.time()
             yield SpanMarker.START_SPAN
             try:
                 yield from self.run_iteration(workspace_process_context)
             except Exception:
                 error_info = serializable_error_info_from_exc_info(sys.exc_info())
                 self._logger.error("Caught error:\n%s", error_info)
```

### Comparing `dagster-1.7.6/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.7/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.7/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/sensor.py` & `dagster-1.7.7/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/types.py` & `dagster-1.7.7/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/utils.py` & `dagster-1.7.7/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_daemon/workspace.py` & `dagster-1.7.7/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_generate/download.py` & `dagster-1.7.7/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_generate/generate.py` & `dagster-1.7.7/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.7/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/__init__.py` & `dagster-1.7.7/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/client.py` & `dagster-1.7.7/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/compile.py` & `dagster-1.7.7/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/impl.py` & `dagster-1.7.7/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/protos/api.proto` & `dagster-1.7.7/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/proxy_server.py` & `dagster-1.7.7/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/server.py` & `dagster-1.7.7/dagster/_grpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
     ExternalRepositoryErrorData,
     ExternalScheduleExecutionErrorData,
     ExternalSensorExecutionErrorData,
     external_job_data_from_def,
     external_repository_data_from_def,
 )
 from dagster._core.remote_representation.origin import RemoteRepositoryOrigin
-from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
+from dagster._core.types.loadable_target_origin import (
+    LoadableTargetOrigin,
+    enter_loadable_target_origin_load_context,
+)
 from dagster._core.utils import FuturesAwareThreadPoolExecutor, RequestUtilizationMetrics
 from dagster._core.workspace.autodiscovery import LoadableTarget
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._serdes.ipc import IPCErrorMessage, open_ipc_subprocess
 from dagster._utils import (
     find_free_port,
     get_run_crash_explanation,
@@ -227,57 +230,61 @@
         self._recon_repos_by_name: Dict[str, ReconstructableRepository] = {}
         self._repo_defs_by_name: Dict[str, RepositoryDefinition] = {}
         self._loadable_repository_symbols: List[LoadableRepositorySymbol] = []
 
         if not loadable_target_origin:
             # empty workspace
             return
-
-        with user_code_error_boundary(
-            DagsterUserCodeLoadError,
-            lambda: "Error occurred during the loading of Dagster definitions in\n"
-            + ", ".join(
-                [f"{k}={v}" for k, v in loadable_target_origin._asdict().items() if v is not None]
-            ),
-        ):
-            loadable_targets = get_loadable_targets(
-                loadable_target_origin.python_file,
-                loadable_target_origin.module_name,
-                loadable_target_origin.package_name,
-                loadable_target_origin.working_directory,
-                loadable_target_origin.attribute,
-            )
-        for loadable_target in loadable_targets:
-            pointer = _get_code_pointer(loadable_target_origin, loadable_target)
-            recon_repo = ReconstructableRepository(
-                pointer,
-                container_image,
-                sys.executable,
-                entry_point=entry_point,
-            )
+        with enter_loadable_target_origin_load_context(loadable_target_origin):
             with user_code_error_boundary(
                 DagsterUserCodeLoadError,
-                lambda: "Error occurred during the loading of Dagster definitions in "
-                + pointer.describe(),
+                lambda: "Error occurred during the loading of Dagster definitions in\n"
+                + ", ".join(
+                    [
+                        f"{k}={v}"
+                        for k, v in loadable_target_origin._asdict().items()
+                        if v is not None
+                    ]
+                ),
             ):
-                repo_def = recon_repo.get_definition()
-                # force load of all lazy constructed code artifacts to prevent
-                # any thread-safety issues loading them later on when serving
-                # definitions from multiple threads
-                repo_def.load_all_definitions()
-
-            self._code_pointers_by_repo_name[repo_def.name] = pointer
-            self._recon_repos_by_name[repo_def.name] = recon_repo
-            self._repo_defs_by_name[repo_def.name] = repo_def
-            self._loadable_repository_symbols.append(
-                LoadableRepositorySymbol(
-                    attribute=loadable_target.attribute,
-                    repository_name=repo_def.name,
+                loadable_targets = get_loadable_targets(
+                    loadable_target_origin.python_file,
+                    loadable_target_origin.module_name,
+                    loadable_target_origin.package_name,
+                    loadable_target_origin.working_directory,
+                    loadable_target_origin.attribute,
+                )
+            for loadable_target in loadable_targets:
+                pointer = _get_code_pointer(loadable_target_origin, loadable_target)
+                recon_repo = ReconstructableRepository(
+                    pointer,
+                    container_image,
+                    sys.executable,
+                    entry_point=entry_point,
+                )
+                with user_code_error_boundary(
+                    DagsterUserCodeLoadError,
+                    lambda: "Error occurred during the loading of Dagster definitions in "
+                    + pointer.describe(),
+                ):
+                    repo_def = recon_repo.get_definition()
+                    # force load of all lazy constructed code artifacts to prevent
+                    # any thread-safety issues loading them later on when serving
+                    # definitions from multiple threads
+                    repo_def.load_all_definitions()
+
+                self._code_pointers_by_repo_name[repo_def.name] = pointer
+                self._recon_repos_by_name[repo_def.name] = recon_repo
+                self._repo_defs_by_name[repo_def.name] = repo_def
+                self._loadable_repository_symbols.append(
+                    LoadableRepositorySymbol(
+                        attribute=loadable_target.attribute,
+                        repository_name=repo_def.name,
+                    )
                 )
-            )
 
     @property
     def loadable_repository_symbols(self) -> Sequence[LoadableRepositorySymbol]:
         return self._loadable_repository_symbols
 
     @property
     def code_pointers_by_repo_name(self) -> Mapping[str, CodePointer]:
```

### Comparing `dagster-1.7.6/dagster/_grpc/server_watcher.py` & `dagster-1.7.7/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/types.py` & `dagster-1.7.7/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_grpc/utils.py` & `dagster-1.7.7/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_loggers/__init__.py` & `dagster-1.7.7/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_model/__init__.py` & `dagster-1.7.7/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.7/dagster/_model/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_module_alias_map.py` & `dagster-1.7.7/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_scheduler/scheduler.py` & `dagster-1.7.7/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_scheduler/stale.py` & `dagster-1.7.7/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_serdes/__init__.py` & `dagster-1.7.7/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_serdes/config_class.py` & `dagster-1.7.7/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_serdes/ipc.py` & `dagster-1.7.7/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_serdes/serdes.py` & `dagster-1.7.7/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_serdes/utils.py` & `dagster-1.7.7/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_seven/__init__.py` & `dagster-1.7.7/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_seven/abc.py` & `dagster-1.7.7/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_seven/compat/datetime.py` & `dagster-1.7.7/dagster/_seven/compat/datetime.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_seven/compat/pendulum.py` & `dagster-1.7.7/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/__init__.py` & `dagster-1.7.7/dagster/_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     from dagster._core.events import DagsterEvent
 
 K = TypeVar("K")
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
-EPOCH = datetime.datetime.utcfromtimestamp(0)
+EPOCH = datetime.datetime.fromtimestamp(0, timezone.utc).replace(tzinfo=None)
 
 PICKLE_PROTOCOL = 4
 
 
 DEFAULT_WORKSPACE_YAML_FILENAME = "workspace.yaml"
 
 PrintFn: TypeAlias = Callable[[Any], None]
```

### Comparing `dagster-1.7.6/dagster/_utils/alert.py` & `dagster-1.7.7/dagster/_utils/alert.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,33 +50,35 @@
 def send_email_via_ssl(
     email_from: str,
     email_password: str,
     email_to: Sequence[str],
     message: str,
     smtp_host: str,
     smtp_port: int,
+    smtp_user: str,
 ):
     context = ssl.create_default_context()
     with smtplib.SMTP_SSL(smtp_host, smtp_port, context=context) as server:
-        server.login(email_from, email_password)
+        server.login(smtp_user, email_password)
         server.sendmail(email_from, email_to, message)
 
 
 def send_email_via_starttls(
     email_from: str,
     email_password: str,
     email_to: Sequence[str],
     message: str,
     smtp_host: str,
     smtp_port: int,
+    smtp_user: str,
 ):
     context = ssl.create_default_context()
     with smtplib.SMTP(smtp_host, smtp_port) as server:
         server.starttls(context=context)
-        server.login(email_from, email_password)
+        server.login(smtp_user, email_password)
         server.sendmail(email_from, email_to, message)
 
 
 @deprecated_param(
     param="job_selection",
     breaking_version="2.0",
     additional_warn_text="Use `monitored_jobs` instead.",
@@ -91,14 +93,15 @@
     email_password: str,
     email_to: Sequence[str],
     email_body_fn: Callable[["RunFailureSensorContext"], str] = _default_failure_email_body,
     email_subject_fn: Callable[["RunFailureSensorContext"], str] = _default_failure_email_subject,
     smtp_host: str = "smtp.gmail.com",
     smtp_type: str = "SSL",
     smtp_port: Optional[int] = None,
+    smtp_user: Optional[str] = None,
     name: Optional[str] = None,
     webserver_base_url: Optional[str] = None,
     monitored_jobs: Optional[
         Sequence[
             Union[
                 "JobDefinition",
                 "GraphDefinition",
@@ -134,14 +137,15 @@
             Defaults to the plain text that contains error message, job name, and run ID.
         email_subject_fn (Optional(Callable[[RunFailureSensorContext], str])): Function which
             takes in the ``RunFailureSensorContext`` outputs the email subject you want to send.
             Defaults to "Dagster Run Failed: <job_name>".
         smtp_host (str): The hostname of the SMTP server. Defaults to "smtp.gmail.com".
         smtp_type (str): The protocol; either "SSL" or "STARTTLS". Defaults to SSL.
         smtp_port (Optional[int]): The SMTP port. Defaults to 465 for SSL, 587 for STARTTLS.
+        smtp_user (Optional[str]): The SMTP user for authenticatication in the SMTP server. Defaults to the value of email_from.
         name: (Optional[str]): The name of the sensor. Defaults to "email_on_job_failure".
         webserver_base_url: (Optional[str]): The base url of your dagster-webserver instance. Specify this to allow
             messages to include deeplinks to the failed run.
         monitored_jobs (Optional[List[Union[JobDefinition, GraphDefinition, JobDefinition, RepositorySelector, JobSelector]]]):
             The jobs that will be monitored by this failure sensor. Defaults to None, which means the alert will
             be sent when any job in the repository fails. To monitor jobs in external repositories,
             use RepositorySelector and JobSelector.
@@ -217,17 +221,29 @@
             email_subject=email_subject_fn(context),
             email_body=email_body,
             randomness=datetime.datetime.now(),
         )
 
         if smtp_type == "SSL":
             send_email_via_ssl(
-                email_from, email_password, email_to, message, smtp_host, smtp_port=smtp_port or 465
+                email_from,
+                email_password,
+                email_to,
+                message,
+                smtp_host,
+                smtp_port=smtp_port or 465,
+                smtp_user=smtp_user or email_from,
             )
         elif smtp_type == "STARTTLS":
             send_email_via_starttls(
-                email_from, email_password, email_to, message, smtp_host, smtp_port=smtp_port or 587
+                email_from,
+                email_password,
+                email_to,
+                message,
+                smtp_host,
+                smtp_port=smtp_port or 587,
+                smtp_user=smtp_user or email_from,
             )
         else:
             raise DagsterInvalidDefinitionError(f'smtp_type "{smtp_type}" is not supported.')
 
     return email_on_run_failure
```

### Comparing `dagster-1.7.6/dagster/_utils/backoff.py` & `dagster-1.7.7/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/cached_method.py` & `dagster-1.7.7/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.7/dagster/_utils/caching_instance_queryer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     get_time_partition_key,
     get_time_partitions_def,
 )
 from dagster._core.errors import (
     DagsterDefinitionChangedDeserializationError,
     DagsterInvalidDefinitionError,
 )
-from dagster._core.event_api import AssetRecordsFilter, EventRecordsFilter
+from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.events import DagsterEventType
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
 from dagster._core.storage.dagster_run import (
     IN_PROGRESS_RUN_STATUSES,
     DagsterRun,
     DagsterRunStatus,
@@ -54,14 +54,16 @@
 from dagster._utils.cached_method import cached_method
 
 if TYPE_CHECKING:
     from dagster._core.storage.event_log import EventLogRecord
     from dagster._core.storage.event_log.base import AssetRecord
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
+RECORD_BATCH_SIZE = 1000
+
 
 class CachingInstanceQueryer(DynamicPartitionsStore):
     """Provides utility functions for querying for asset-materialization related data from the
     instance which will attempt to limit redundant expensive calls. Intended for use within the
     scope of a single "request" (e.g. GQL request, sensor tick).
 
     Args:
@@ -255,26 +257,29 @@
             )
         ):
             asset_record = self.get_asset_record(asset_partition.asset_key)
             if asset_record is None:
                 return None
             return asset_record.asset_entry.last_materialization_record
 
-        records = self.instance.get_event_records(
-            EventRecordsFilter(
-                event_type=self._event_type_for_key(asset_partition.asset_key),
-                asset_key=asset_partition.asset_key,
-                asset_partitions=(
-                    [asset_partition.partition_key] if asset_partition.partition_key else None
-                ),
-                before_cursor=before_cursor,
+        records_filter = AssetRecordsFilter(
+            asset_key=asset_partition.asset_key,
+            asset_partitions=(
+                [asset_partition.partition_key] if asset_partition.partition_key else None
             ),
-            ascending=False,
-            limit=1,
+            before_storage_id=before_cursor,
         )
+        if self.asset_graph.get(asset_partition.asset_key).is_observable:
+            records = self.instance.fetch_observations(
+                records_filter, ascending=False, limit=1
+            ).records
+        else:
+            records = self.instance.fetch_materializations(
+                records_filter, ascending=False, limit=1
+            ).records
         return next(iter(records), None)
 
     @cached_method
     def _get_latest_materialization_or_observation_storage_ids_by_asset_partition(
         self, *, asset_key: AssetKey
     ) -> Mapping[AssetKeyPartitionKey, Optional[int]]:
         """Returns a mapping from asset partition to the latest storage id for that asset partition
@@ -396,25 +401,29 @@
     def next_version_record(
         self,
         *,
         asset_key: AssetKey,
         after_cursor: Optional[int],
         data_version: Optional[DataVersion],
     ) -> Optional["EventLogRecord"]:
-        for record in self.instance.get_event_records(
-            EventRecordsFilter(
-                event_type=DagsterEventType.ASSET_OBSERVATION,
-                asset_key=asset_key,
-                after_cursor=after_cursor,
-            ),
-            ascending=True,
-        ):
-            record_version = extract_data_version_from_entry(record.event_log_entry)
-            if record_version is not None and record_version != data_version:
-                return record
+        has_more = True
+        cursor = None
+        while has_more:
+            result = self.instance.fetch_observations(
+                AssetRecordsFilter(asset_key=asset_key, after_storage_id=after_cursor),
+                limit=RECORD_BATCH_SIZE,
+                cursor=cursor,
+                ascending=True,
+            )
+            has_more = result.has_more
+            cursor = result.cursor
+            for record in result.records:
+                record_version = extract_data_version_from_entry(record.event_log_entry)
+                if record_version is not None and record_version != data_version:
+                    return record
 
         # no records found with a new data version
         return None
 
     ####################
     # RUNS
     ####################
```

### Comparing `dagster-1.7.6/dagster/_utils/concurrency.py` & `dagster-1.7.7/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/container.py` & `dagster-1.7.7/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/dagster_type.py` & `dagster-1.7.7/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/env.py` & `dagster-1.7.7/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/error.py` & `dagster-1.7.7/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/external.py` & `dagster-1.7.7/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/forked_pdb.py` & `dagster-1.7.7/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/hosted_user_process.py` & `dagster-1.7.7/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/indenting_printer.py` & `dagster-1.7.7/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/internal_init.py` & `dagster-1.7.7/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/interrupts.py` & `dagster-1.7.7/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/log.py` & `dagster-1.7.7/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/merger.py` & `dagster-1.7.7/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/net.py` & `dagster-1.7.7/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/schedules.py` & `dagster-1.7.7/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/tags.py` & `dagster-1.7.7/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/temp_file.py` & `dagster-1.7.7/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/test/__init__.py` & `dagster-1.7.7/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/test/data_versions.py` & `dagster-1.7.7/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.7/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.7/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.7/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/timing.py` & `dagster-1.7.7/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/typed_dict.py` & `dagster-1.7.7/dagster/_utils/typed_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Type, TypeVar, cast
 
 from typing_extensions import NotRequired, get_origin, is_typeddict
 
+from .typing_api import is_closed_python_optional_type
+
 _TypedDictClass = TypeVar("_TypedDictClass")
 
 
 def init_optional_typeddict(cls: Type[_TypedDictClass]) -> _TypedDictClass:
     """Initialize a TypedDict with optional values."""
-    from dagster._config.pythonic_config.type_check_utils import is_optional
-
     if not is_typeddict(cls):
         raise Exception("Must pass a TypedDict class to init_optional_typeddict")
     result = {}
     for key, value in cls.__annotations__.items():
         # If the value is a typed dict, recursively initialize it
         if is_typeddict(value):
             result[key] = init_optional_typeddict(value)
-        elif is_optional(value):
+        elif is_closed_python_optional_type(value):
             result[key] = None
         elif get_origin(value) is dict:
             result[key] = {}
         elif get_origin(value) is NotRequired:
             continue
         else:
             raise Exception("fields must be either optional or typed dicts")
```

### Comparing `dagster-1.7.6/dagster/_utils/typing_api.py` & `dagster-1.7.7/dagster/_utils/typing_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,20 +4,47 @@
 
 import typing
 
 from typing_extensions import get_args, get_origin
 
 import dagster._check as check
 
+try:
+    # this type only exists in python 3.10+
+    from types import UnionType  # type: ignore
+except ImportError:
+    UnionType = typing.Union
+
+
+def is_closed_python_optional_type(annotation) -> bool:
+    """Returns true if the annotation signifies an Optional type
+    that is closed over a non-None T.
+
+    In particular, this can be:
+    - Optional[T]
+    - Union[T, None]
+    - Union[None, T]
+    - T | None (in Python 3.10+)
+    - None | T (in Python 3.10+).
+
+    """
+    # Optional[T] is equivalent to Union[T, None], see
+    # https://docs.python.org/3/library/typing.html#typing.Optional
+    # A user could also specify a Union themselves
+    if get_origin(annotation) == typing.Union:
+        return len(get_args(annotation)) == 2 and type(None) in get_args(annotation)
+
+    # The Python 3.10 pipe syntax evaluates to a UnionType
+    # rather than a Union, so we need to check for that as well
+    # UnionType values are equivalent to Unions, e.g. str | None == Union[str, None]
+    # but the types themselves are not, e.g. type(str | None) != type(Union[str, None])
+    if get_origin(annotation) == UnionType:
+        return len(get_args(annotation)) == 2 and type(None) in get_args(annotation)
 
-def is_closed_python_optional_type(ttype):
-    # Optional[X] is Union[X, NoneType] which is what we match against here
-    origin = get_origin(ttype)
-    args = get_args(ttype)
-    return origin is typing.Union and len(args) == 2 and args[1] is type(None)
+    return False
 
 
 def is_python_dict_type(ttype):
     origin = get_origin(ttype)
     return ttype is dict or origin is dict
```

### Comparing `dagster-1.7.6/dagster/_utils/warnings.py` & `dagster-1.7.7/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster/_utils/yaml_utils.py` & `dagster-1.7.7/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.6/dagster.egg-info/PKG-INFO` & `dagster-1.7.7/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.6
+Version: 1.7.7
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.6/dagster.egg-info/SOURCES.txt` & `dagster-1.7.7/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -183,23 +183,25 @@
 dagster/_core/definitions/target.py
 dagster/_core/definitions/time_window_partition_mapping.py
 dagster/_core/definitions/time_window_partitions.py
 dagster/_core/definitions/unresolved_asset_job_definition.py
 dagster/_core/definitions/utils.py
 dagster/_core/definitions/version_strategy.py
 dagster/_core/definitions/asset_check_factories/__init__.py
+dagster/_core/definitions/asset_check_factories/metadata_bounds_checks.py
 dagster/_core/definitions/asset_check_factories/schema_change_checks.py
 dagster/_core/definitions/asset_check_factories/utils.py
 dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
 dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
 dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
 dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
 dagster/_core/definitions/declarative_scheduling/README.md
 dagster/_core/definitions/declarative_scheduling/__init__.py
 dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+dagster/_core/definitions/declarative_scheduling/scheduling_condition_evaluator.py
 dagster/_core/definitions/declarative_scheduling/scheduling_context.py
 dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
 dagster/_core/definitions/declarative_scheduling/serialized_objects.py
 dagster/_core/definitions/declarative_scheduling/utils.py
 dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
 dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
 dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
@@ -258,15 +260,15 @@
 dagster/_core/execution/resources_init.py
 dagster/_core/execution/retries.py
 dagster/_core/execution/run_cancellation_thread.py
 dagster/_core/execution/run_metrics_thread.py
 dagster/_core/execution/stats.py
 dagster/_core/execution/submit_asset_runs.py
 dagster/_core/execution/tags.py
-dagster/_core/execution/types.py
+dagster/_core/execution/telemetry.py
 dagster/_core/execution/validate_run_config.py
 dagster/_core/execution/watch_orphans.py
 dagster/_core/execution/with_resources.py
 dagster/_core/execution/context/__init__.py
 dagster/_core/execution/context/compute.py
 dagster/_core/execution/context/data_version_cache.py
 dagster/_core/execution/context/hook.py
@@ -592,20 +594,22 @@
 dagster/_seven/abc.py
 dagster/_seven/json.py
 dagster/_seven/temp_dir.py
 dagster/_seven/compat/__init__.py
 dagster/_seven/compat/datetime.py
 dagster/_seven/compat/pendulum.py
 dagster/_utils/__init__.py
+dagster/_utils/aiodataloader.py
 dagster/_utils/alert.py
 dagster/_utils/backoff.py
 dagster/_utils/cached_method.py
 dagster/_utils/caching_instance_queryer.py
 dagster/_utils/concurrency.py
 dagster/_utils/container.py
+dagster/_utils/cronstring.py
 dagster/_utils/dagster_type.py
 dagster/_utils/env.py
 dagster/_utils/error.py
 dagster/_utils/external.py
 dagster/_utils/forked_pdb.py
 dagster/_utils/hosted_user_process.py
 dagster/_utils/indenting_printer.py
```

### Comparing `dagster-1.7.6/dagster.egg-info/requires.txt` & `dagster-1.7.7/dagster.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
 filelock
-dagster-pipes==1.7.6
+dagster-pipes==1.7.7
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
@@ -75,15 +75,15 @@
 types-six
 types-sqlalchemy==1.4.53.34
 types-tabulate
 types-tzlocal
 types-toml
 
 [ruff]
-ruff==0.3.4
+ruff==0.4.4
 
 [test]
 buildkite-test-collector
 docker
 grpcio-tools>=1.44.0
 mock==3.0.5
 mypy-protobuf
```

### Comparing `dagster-1.7.6/setup.py` & `dagster-1.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
         "filelock",
-        "dagster-pipes==1.7.6",
+        "dagster-pipes==1.7.7",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
@@ -161,15 +161,15 @@
             "types-six",  # needed but not specified by grpcio
             "types-sqlalchemy==1.4.53.34",  # later versions introduce odd errors
             "types-tabulate",  # version will be resolved against tabulate
             "types-tzlocal",  # version will be resolved against tzlocal
             "types-toml",  # version will be resolved against toml
         ],
         "ruff": [
-            "ruff==0.3.4",
+            "ruff==0.4.4",
         ],
     },
     entry_points={
         "console_scripts": [
             "dagster = dagster.cli:main",
             "dagster-daemon = dagster.daemon.cli:main",
         ]
```

