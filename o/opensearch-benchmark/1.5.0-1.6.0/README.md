# Comparing `tmp/opensearch_benchmark-1.5.0.tar.gz` & `tmp/opensearch_benchmark-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch_benchmark-1.5.0.tar", last modified: Thu Apr 25 17:39:17 2024, max compression
+gzip compressed data, was "opensearch_benchmark-1.6.0.tar", last modified: Thu May 23 19:17:45 2024, max compression
```

## Comparing `opensearch_benchmark-1.5.0.tar` & `opensearch_benchmark-1.6.0.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/client-options.md
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/execute-test.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/kill-running-process.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/target-hosts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/test-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/api/workload.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/get-started.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.348387 opensearch_benchmark-1.5.0/docs/user-guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/user-guides/create-pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/docs/user-guides/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 17:39:17.000000 opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/async_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51772 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/benchmarkd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31535 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/cluster_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.356387 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/local_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/executors/shell_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.360387 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/bare_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/docker_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/exception_handling_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/java_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/docker_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/local_process_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/no_op_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/architecture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/bootstrap_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster_flavors.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/cluster_infra_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/plugin_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provision_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.364387 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/provisioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/supplier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/artifact_variables_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/binary_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/config_applier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/git_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/host_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/java_home_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/jdk_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/builder/utils/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    99370 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/min-os-version.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/base-workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/benchmark.ini
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/custom-operations.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/custom-test-procedures.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/default-operations.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/default-test-procedures.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/logging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/metrics-template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.368388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.372388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.340387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.376388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.380388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.344387 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.384388 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/results-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/test-executions-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/resources/workload-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    36092 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/results_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    83463 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/test_execution_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.384388 opensearch_benchmark-1.5.0/osbenchmark/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    21980 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/periodic_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/sysstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   107234 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    99934 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/worker_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/workload/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92616 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    76510 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    39027 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/osbenchmark/workload_generator/workload_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10512 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/scripts/expand-data-corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 17:39:17.392388 opensearch_benchmark-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:39:17.388388 opensearch_benchmark-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/tests/test_async_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/tests/test_execution_orchestrator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:38:20.000000 opensearch_benchmark-1.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.014486 opensearch_benchmark-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 19:17:45.014486 opensearch_benchmark-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.970486 opensearch_benchmark-1.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.970486 opensearch_benchmark-1.6.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/client-options.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/execute-test.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/kill-running-process.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/target-hosts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/test-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/api/workload.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/get-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.970486 opensearch_benchmark-1.6.0/docs/user-guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/user-guides/create-pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/docs/user-guides/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.010486 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 19:17:44.000000 opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.974485 opensearch_benchmark-1.6.0/osbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51782 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/benchmarkd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31535 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/cluster_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/listers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/configs/utils/config_path_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.978486 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.982486 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.982486 opensearch_benchmark-1.6.0/osbenchmark/builder/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/executors/local_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/executors/shell_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.982486 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/bare_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/docker_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/exception_handling_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.982486 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/java_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.986486 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/docker_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/exception_handling_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/local_process_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/no_op_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.986486 opensearch_benchmark-1.6.0/osbenchmark/builder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/architecture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/bootstrap_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/cluster_flavors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/cluster_infra_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/plugin_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/provision_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/models/provision_config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/provision_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.986486 opensearch_benchmark-1.6.0/osbenchmark/builder/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/provisioners/provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.990486 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/artifact_variables_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/binary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/config_applier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/git_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/host_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/java_home_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/jdk_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/builder/utils/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99370 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/min-os-version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.990486 opensearch_benchmark-1.6.0/osbenchmark/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/base-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/benchmark.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/custom-operations.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/custom-test-procedures.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/default-operations.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/default-test-procedures.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/logging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/metrics-template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.958485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.990486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.990486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.990486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.994486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.998486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.962485 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:44.966486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.002486 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/results-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/test-executions-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23167 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/resources/workload-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36092 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/results_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83463 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/test_execution_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.006486 opensearch_benchmark-1.6.0/osbenchmark/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21980 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/periodic_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/sysstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.006486 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107234 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99934 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/worker_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.010486 opensearch_benchmark-1.6.0/osbenchmark/workload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92616 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76510 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39027 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.010486 opensearch_benchmark-1.6.0/osbenchmark/workload_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload_generator/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload_generator/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/osbenchmark/workload_generator/workload_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.010486 opensearch_benchmark-1.6.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10512 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/scripts/expand-data-corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 19:17:45.014486 opensearch_benchmark-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:45.010486 opensearch_benchmark-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/tests/test_async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/tests/test_execution_orchestrator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 19:16:47.000000 opensearch_benchmark-1.6.0/version.txt
```

### Comparing `opensearch_benchmark-1.5.0/AUTHORS` & `opensearch_benchmark-1.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/CONTRIBUTING.md` & `opensearch_benchmark-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/LICENSE` & `opensearch_benchmark-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/README.md` & `opensearch_benchmark-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/docs/api/execute-test.md` & `opensearch_benchmark-1.6.0/docs/api/execute-test.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/docs/user-guides/create-pipeline.md` & `opensearch_benchmark-1.6.0/docs/user-guides/create-pipeline.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/opensearch_benchmark.egg-info/SOURCES.txt` & `opensearch_benchmark-1.6.0/opensearch_benchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/actor.py` & `opensearch_benchmark-1.6.0/osbenchmark/actor.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/async_connection.py` & `opensearch_benchmark-1.6.0/osbenchmark/async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/benchmark.py` & `opensearch_benchmark-1.6.0/osbenchmark/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,15 @@
     test_execution_parser.add_argument(
         "--results-numbers-align",
         help="Define the output column number alignment for the command line results (default: right).",
         choices=["right", "center", "left", "decimal"],
         default="right")
     test_execution_parser.add_argument(
         "--show-in-results",
-        help="Define which values are shown in the summary publish (default: available).",
+        help="Define which values are shown in the summary results published (default: available).",
         choices=["available", "all-percentiles", "all"],
         default="available")
     test_execution_parser.add_argument(
         "--results-file",
         help="Write the command line results also to the provided file.",
         default="")
     test_execution_parser.add_argument(
```

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/benchmarkd.py` & `opensearch_benchmark-1.6.0/osbenchmark/benchmarkd.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/builder.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/builder.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/cluster.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/cluster_builder.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/cluster_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/configs/utils/config_path_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/executors/local_shell_executor.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/executors/local_shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/executors/shell_executor.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/executors/shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/bare_installer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/bare_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/docker_installer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/docker_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/exception_handling_installer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/exception_handling_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/installer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/installer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/plugin_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/installers/preparers/preparer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/installers/preparers/preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/java_resolver.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/java_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/launcher.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/docker_launcher.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/docker_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/exception_handling_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/launcher.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/launchers/local_process_launcher.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/launchers/local_process_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/models/architecture_types.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/models/architecture_types.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/models/config_instance_types.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/models/config_instance_types.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/models/plugin_config_instance.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/models/plugin_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/models/provision_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/models/provision_config_instance_descriptor.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/provision_config.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/provision_config.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/provisioner.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/provisioners/provisioner.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/provisioners/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/supplier.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/supplier.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/artifact_variables_provider.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/artifact_variables_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/config_applier.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/config_applier.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/git_manager.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/git_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/host_cleaner.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/host_cleaner.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/java_home_resolver.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/java_home_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/jdk_resolver.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/jdk_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/path_manager.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/builder/utils/template_renderer.py` & `opensearch_benchmark-1.6.0/osbenchmark/builder/utils/template_renderer.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/client.py` & `opensearch_benchmark-1.6.0/osbenchmark/client.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/config.py` & `opensearch_benchmark-1.6.0/osbenchmark/config.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/exceptions.py` & `opensearch_benchmark-1.6.0/osbenchmark/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/log.py` & `opensearch_benchmark-1.6.0/osbenchmark/log.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/metrics.py` & `opensearch_benchmark-1.6.0/osbenchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/paths.py` & `opensearch_benchmark-1.6.0/osbenchmark/paths.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/base-workload.json.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/base-workload.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/benchmark.ini` & `opensearch_benchmark-1.6.0/osbenchmark/resources/benchmark.ini`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/custom-operations.json.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/custom-operations.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/custom-test-procedures.json.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/custom-test-procedures.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/default-operations.json.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/default-operations.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/default-test-procedures.json.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/default-test-procedures.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/docker-compose.yml.j2` & `opensearch_benchmark-1.6.0/osbenchmark/resources/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/logging.json` & `opensearch_benchmark-1.6.0/osbenchmark/resources/logging.json`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/metrics-template.json` & `opensearch_benchmark-1.6.0/osbenchmark/resources/metrics-template.json`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch_benchmark-1.6.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/results-template.json` & `opensearch_benchmark-1.6.0/osbenchmark/resources/results-template.json`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/test-executions-template.json` & `opensearch_benchmark-1.6.0/osbenchmark/resources/test-executions-template.json`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/resources/workload-schema.json` & `opensearch_benchmark-1.6.0/osbenchmark/resources/workload-schema.json`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/results_publisher.py` & `opensearch_benchmark-1.6.0/osbenchmark/results_publisher.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/telemetry.py` & `opensearch_benchmark-1.6.0/osbenchmark/telemetry.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/test_execution_orchestrator.py` & `opensearch_benchmark-1.6.0/osbenchmark/test_execution_orchestrator.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/time.py` & `opensearch_benchmark-1.6.0/osbenchmark/time.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/collections.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/collections.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/console.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/console.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/convert.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/convert.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/dataset.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         path: Data set file path
         context: Dataset Context Enum
     Returns: DataSet instance
     """
     if data_set_format == HDF5DataSet.FORMAT_NAME:
         return HDF5DataSet(path, context)
     if data_set_format == BigANNVectorDataSet.FORMAT_NAME:
-        return BigANNVectorDataSet(path)
+        return create_big_ann_dataset(path)
     raise ConfigurationError("Invalid data set format")
 
 
 class HDF5DataSet(DataSet):
     """ Data-set format corresponding to `ANN Benchmarks
     <https://github.com/erikbern/ann-benchmarks#data-sets>`_
     """
@@ -140,58 +140,40 @@
 
         if context == Context.QUERY:
             return "test"
 
         raise Exception("Unsupported context")
 
 
-class BigANNVectorDataSet(DataSet):
-    """ Data-set format for vector data-sets for `Big ANN Benchmarks
-    <https://big-ann-benchmarks.com/index.html#bench-datasets>`_
-    """
+class BigANNDataSet(DataSet):
 
     DATA_SET_HEADER_LENGTH = 8
-    U8BIN_EXTENSION = "u8bin"
-    FBIN_EXTENSION = "fbin"
     FORMAT_NAME = "bigann"
-    SUPPORTED_EXTENSION = [
-        FBIN_EXTENSION, U8BIN_EXTENSION
-    ]
-
-    BYTES_PER_U8INT = 1
-    BYTES_PER_FLOAT = 4
 
     def __init__(self, dataset_path: str):
         self.dataset_path = dataset_path
         self.file = None
-        self.current = BigANNVectorDataSet.BEGINNING
-        self.num_points = 0
-        self.dimension = 0
+        self.num_bytes = 0
+        self.current = DataSet.BEGINNING
         self.bytes_per_num = 0
+        self.rows = 0
+        self.row_length = 0
 
     def _init_internal_params(self):
         self.file = open(self.dataset_path, 'rb')
-        self.file.seek(BigANNVectorDataSet.BEGINNING, os.SEEK_END)
-        num_bytes = self.file.tell()
-        self.file.seek(BigANNVectorDataSet.BEGINNING)
-
-        if num_bytes < BigANNVectorDataSet.DATA_SET_HEADER_LENGTH:
+        self.file.seek(DataSet.BEGINNING, os.SEEK_END)
+        self.num_bytes = self.file.tell()
+        if self.num_bytes < BigANNDataSet.DATA_SET_HEADER_LENGTH:
             raise Exception("Invalid file: file size cannot be less than {} bytes".format(
-                BigANNVectorDataSet.DATA_SET_HEADER_LENGTH))
-
-        self.num_points = int.from_bytes(self.file.read(4), "little")
-        self.dimension = int.from_bytes(self.file.read(4), "little")
-        self.bytes_per_num = self._get_data_size(self.dataset_path)
-
-        if (num_bytes - BigANNVectorDataSet.DATA_SET_HEADER_LENGTH) != (
-                self.num_points * self.dimension * self.bytes_per_num):
-            raise Exception("Invalid file. File size is not matching with expected estimated "
-                            "value based on number of points, dimension and bytes per point")
-
-        self.reader = self._value_reader(self.dataset_path)
+                BigANNDataSet.DATA_SET_HEADER_LENGTH))
+        self.file.seek(BigANNDataSet.BEGINNING)
+        self.rows = int.from_bytes(self.file.read(4), "little")
+        self.row_length = int.from_bytes(self.file.read(4), "little")
+        self.bytes_per_num = self._get_data_size()
+        self.reader = self._value_reader()
 
     def _load(self):
         # load file if it is not loaded yet
         if self.file is None:
             self._init_internal_params()
 
     def read(self, chunk_size: int):
@@ -206,65 +188,155 @@
 
         vectors = np.asarray(
             [self._read_vector() for _ in range(end_offset - self.current)]
         )
         self.current = end_offset
         return vectors
 
+    def _get_file_byte_offset(self, offset):
+        """Return file byte offset for given offset"""
+        return BigANNDataSet.DATA_SET_HEADER_LENGTH + (self.row_length * self.bytes_per_num * offset)
+
     def seek(self, offset: int):
         # load file first before seek
         self._load()
         if offset < self.BEGINNING:
             raise Exception("Offset must be greater than or equal to 0")
 
         if offset >= self.size():
             raise Exception("Offset must be less than the data set size")
 
-        bytes_offset = BigANNVectorDataSet.DATA_SET_HEADER_LENGTH + (
-                self.dimension * self.bytes_per_num * offset)
+        bytes_offset = self._get_file_byte_offset(offset)
         self.file.seek(bytes_offset)
         self.current = offset
 
     def _read_vector(self):
-        return np.asarray([self.reader(self.file) for _ in
-                           range(self.dimension)])
+        return np.asarray([self.reader(self.file) for _ in range(self.row_length)])
 
     def size(self):
         # load file first before return size
         self._load()
-        return self.num_points
+        return self.rows
 
     def reset(self):
         if self.file:
-            self.file.seek(BigANNVectorDataSet.DATA_SET_HEADER_LENGTH)
-        self.current = BigANNVectorDataSet.BEGINNING
+            self.file.seek(BigANNDataSet.DATA_SET_HEADER_LENGTH)
+        self.current = BigANNDataSet.BEGINNING
 
     def __del__(self):
         if self.file:
             self.file.close()
 
-    @staticmethod
-    def _get_extension(file_name):
-        ext = file_name.split('.')[-1]
-        if ext not in BigANNVectorDataSet.SUPPORTED_EXTENSION:
+    @abstractmethod
+    def _get_supported_extension(self):
+        """Return list of supported extension by this dataset"""
+
+    def _get_extension(self):
+        ext = self.dataset_path.split('.')[-1]
+        supported_extension = self._get_supported_extension()
+        if ext not in supported_extension:
             raise InvalidExtensionException(
                 "Unknown extension :{}, supported extensions are: {}".format(
-                    ext, str(BigANNVectorDataSet.SUPPORTED_EXTENSION)))
+                    ext, str(supported_extension)))
         return ext
 
-    @staticmethod
-    def _get_data_size(file_name):
-        ext = BigANNVectorDataSet._get_extension(file_name)
-        if ext == BigANNVectorDataSet.U8BIN_EXTENSION:
+    @abstractmethod
+    def get_data_size(self, extension):
+        """Return data size based on extension"""
+
+    def _get_data_size(self):
+        """Return data size"""
+        ext = self._get_extension()
+        return self.get_data_size(ext)
+
+    @abstractmethod
+    def _get_value_reader(self, extension):
+        """Return value reader based on extension"""
+
+    def _value_reader(self):
+        ext = self._get_extension()
+        return self._get_value_reader(ext)
+
+
+class BigANNVectorDataSet(BigANNDataSet):
+    """ Data-set format for vector data-sets for `Big ANN Benchmarks
+    <https://big-ann-benchmarks.com/index.html#bench-datasets>`
+    """
+
+    U8BIN_EXTENSION = "u8bin"
+    FBIN_EXTENSION = "fbin"
+    SUPPORTED_EXTENSION = [
+        FBIN_EXTENSION, U8BIN_EXTENSION
+    ]
+
+    BYTES_PER_U8INT = 1
+    BYTES_PER_FLOAT = 4
+
+    def _init_internal_params(self):
+        super()._init_internal_params()
+        if (self.num_bytes - BigANNDataSet.DATA_SET_HEADER_LENGTH) != (
+                self.rows * self.row_length * self.bytes_per_num):
+            raise Exception("Invalid file. File size is not matching with expected estimated "
+                            "value based on number of points, dimension and bytes per point")
+
+    def _get_supported_extension(self):
+        return BigANNVectorDataSet.SUPPORTED_EXTENSION
+
+    def get_data_size(self, extension):
+        if extension == BigANNVectorDataSet.U8BIN_EXTENSION:
             return BigANNVectorDataSet.BYTES_PER_U8INT
 
-        if ext == BigANNVectorDataSet.FBIN_EXTENSION:
+        if extension == BigANNVectorDataSet.FBIN_EXTENSION:
             return BigANNVectorDataSet.BYTES_PER_FLOAT
 
-    @staticmethod
-    def _value_reader(file_name):
-        ext = BigANNVectorDataSet._get_extension(file_name)
-        if ext == BigANNVectorDataSet.U8BIN_EXTENSION:
+        return None
+
+    def _get_value_reader(self, extension):
+        if extension == BigANNVectorDataSet.U8BIN_EXTENSION:
             return lambda file: float(int.from_bytes(file.read(BigANNVectorDataSet.BYTES_PER_U8INT), "little"))
 
-        if ext == BigANNVectorDataSet.FBIN_EXTENSION:
+        if extension == BigANNVectorDataSet.FBIN_EXTENSION:
             return lambda file: struct.unpack('<f', file.read(BigANNVectorDataSet.BYTES_PER_FLOAT))
+
+        return None
+
+
+class BigANNGroundTruthDataSet(BigANNDataSet):
+    """ Data-set format for neighbor data-sets for `Big ANN Benchmarks
+    <https://big-ann-benchmarks.com/index.html#bench-datasets>`"""
+
+    BIN_EXTENSION = "bin"
+    SUPPORTED_EXTENSION = [BIN_EXTENSION]
+
+    BYTES_PER_UNSIGNED_INT32 = 4
+
+    def _init_internal_params(self):
+        super()._init_internal_params()
+        # The ground truth binary files consist of the following information:
+        # num_queries(uint32_t) K-NN(uint32) followed by num_queries X K x sizeof(uint32_t) bytes of data
+        # representing the IDs of the K-nearest neighbors of the queries, followed by num_queries X K x sizeof(float)
+        # bytes of data representing the distances to the corresponding points.
+        if (self.num_bytes - BigANNDataSet.DATA_SET_HEADER_LENGTH) != 2 * (
+                self.rows * self.row_length * self.bytes_per_num):
+            raise Exception("Invalid file. File size is not matching with expected estimated "
+                            "value based on number of queries, k and bytes per query")
+
+    def _get_supported_extension(self):
+        return BigANNGroundTruthDataSet.SUPPORTED_EXTENSION
+
+    def get_data_size(self, extension):
+        return BigANNGroundTruthDataSet.BYTES_PER_UNSIGNED_INT32
+
+    def _get_value_reader(self, extension):
+        return lambda file: int.from_bytes(
+            file.read(BigANNGroundTruthDataSet.BYTES_PER_UNSIGNED_INT32), "little")
+
+
+def create_big_ann_dataset(file_path: str):
+    if not file_path:
+        raise Exception("Invalid file path")
+    extension = file_path.split('.')[-1]
+    if extension in BigANNGroundTruthDataSet.SUPPORTED_EXTENSION:
+        return BigANNGroundTruthDataSet(file_path)
+    if extension in BigANNVectorDataSet.SUPPORTED_EXTENSION:
+        return BigANNVectorDataSet(file_path)
+    raise Exception("Unsupported file")
```

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/git.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/git.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/io.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/io.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/jvm.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/modules.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/modules.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/net.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/net.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/opts.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/opts.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/parse.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/parse.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/periodic_waiter.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/periodic_waiter.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/process.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/process.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/repo.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/repo.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/sysstats.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/sysstats.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/utils/versions.py` & `opensearch_benchmark-1.6.0/osbenchmark/utils/versions.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/version.py` & `opensearch_benchmark-1.6.0/osbenchmark/version.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/errors.py` & `opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/errors.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/runner.py` & `opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/runner.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/scheduler.py` & `opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/scheduler.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/worker_coordinator/worker_coordinator.py` & `opensearch_benchmark-1.6.0/osbenchmark/worker_coordinator/worker_coordinator.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload/loader.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload/loader.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload/params.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload/params.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload/workload.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload/workload.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/__init__.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/corpus.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload_generator/corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/index.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload_generator/index.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/osbenchmark/workload_generator/workload_generator.py` & `opensearch_benchmark-1.6.0/osbenchmark/workload_generator/workload_generator.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/scripts/expand-data-corpus.py` & `opensearch_benchmark-1.6.0/scripts/expand-data-corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/setup.py` & `opensearch_benchmark-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -131,20 +131,27 @@
                               for major, minor in supported_python_versions]
 
 first_supported_version = "{}.{}".format(supported_python_versions[0][0], supported_python_versions[0][1])
 # next minor after the latest supported version
 first_unsupported_version = "{}.{}".format(supported_python_versions[-1][0], supported_python_versions[-1][1] + 1)
 
 setup(name="opensearch-benchmark",
-      maintainer="Ian Hoang, Govind Kamat",
-      maintainer_email="hoangia@amazon.com, govkamat@amazon.com",
+      author="Ian Hoang, Govind Kamat, Mingyang Shi, Chinmay Gadgil, Rishabh Singh, Vijayan Balasubramanian",
+      author_email="ianhoang16@gmail.com, govind_kamat@yahoo.com, mmyyshi@gmail.com, chinmay5j@gmail.com, rishabhksingh@gmail.com, vijayan.balasubramanian@gmail.com",
+      maintainer="Ian Hoang, Govind Kamat, Mingyang Shi, Chinmay Gadgil, Rishabh Singh, Vijayan Balasubramanian",
+      maintainer_email="ianhoang16@gmail.com, govind_kamat@yahoo.com, mmyyshi@gmail.com, chinmay5j@gmail.com, rishabhksingh@gmail.com, vijayan.balasubramanian@gmail.com",
       version=__versionstr__,
       description="Macrobenchmarking framework for OpenSearch",
       long_description=long_description,
       long_description_content_type='text/markdown',
+      project_urls={
+        "Documentation": "https://opensearch.org/docs/benchmark",
+        "Source Code": "https://github.com/opensearch-project/OpenSearch-Benchmark",
+        "Issue Tracker": "https://github.com/opensearch-project/OpenSearch-Benchmark/issues",
+      },
       url="https://github.com/opensearch-project/OpenSearch-Benchmark",
       license="Apache License, Version 2.0",
       packages=find_packages(
           where=".",
           exclude=("tests*", "benchmarks*", "it*")
       ),
       include_package_data=True,
```

### Comparing `opensearch_benchmark-1.5.0/tests/test_async_connection.py` & `opensearch_benchmark-1.6.0/tests/test_async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch_benchmark-1.5.0/tests/test_execution_orchestrator_test.py` & `opensearch_benchmark-1.6.0/tests/test_execution_orchestrator_test.py`

 * *Files identical despite different names*

