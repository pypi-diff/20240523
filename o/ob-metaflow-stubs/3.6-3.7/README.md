# Comparing `tmp/ob-metaflow-stubs-3.6.tar.gz` & `tmp/ob-metaflow-stubs-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.6.tar", last modified: Tue May 21 17:36:52 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.7.tar", last modified: Wed May 22 22:08:55 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.6.tar` & `ob-metaflow-stubs-3.7.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 17:36:49.000000 ob-metaflow-stubs-3.6/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.234765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.238765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.242765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.246765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/logs_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:49.000000 ob-metaflow-stubs-3.6/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/tagging_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-21 17:36:50.000000 ob-metaflow-stubs-3.6/metaflow-stubs/tuple_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 17:36:52.000000 ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:36:52.250765 ob-metaflow-stubs-3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 17:36:32.000000 ob-metaflow-stubs-3.6/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.399925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.399925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.403926 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.403926 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/tagging_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/tuple_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/version.py
```

### Comparing `ob-metaflow-stubs-3.6/PKG-INFO` & `ob-metaflow-stubs-3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.6
+Version: 3.7
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.007848                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.490721                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.client.core
     import metaflow.metaflow_current
-    import metaflow.parameters
-    import datetime
+    import io
     import metaflow.events
+    import datetime
+    import metaflow.parameters
     import metaflow.datastore.inputs
     import typing
-    import metaflow._vendor.click.types
-    import metaflow.client.core
-    import io
     import metaflow.plugins.datatools.s3.s3
+    import metaflow._vendor.click.types
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,59 +722,252 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+@typing.overload
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+    """
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+@typing.overload
+def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    """
+    ...
+
+@typing.overload
+def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
+    """
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    """
+    ...
+
+@typing.overload
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies the Conda environment for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
+    packages : Dict[str, str], default {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    python : str, optional, default: None
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
     """
-    Specifies the PyPI packages for the step.
+    Specifies the Conda environment for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
+    packages : Dict[str, str], default {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    python : str, optional, default: None
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
@@ -918,63 +1111,43 @@
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
-    
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
-    
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
 def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies environment variables to be set prior to the execution of a step.
@@ -1061,228 +1234,59 @@
         Shared memory size (in MiB) required for this step
     port: int, optional
         Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the Conda environment for the step.
+    Specifies the PyPI packages for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    packages : Dict[str, str], default: {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies the Conda environment for the step.
+    Specifies the PyPI packages for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    packages : Dict[str, str], default: {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-@typing.overload
-def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    """
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    """
-    ...
-
-@typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
     """
     ...
 
 @typing.overload
 def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that the step will success under all circumstances.
@@ -1328,67 +1332,63 @@
     print_exception : bool, default True
         Determines whether or not the exception is printed to
         stdout when caught.
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
 def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the times when the flow should be run when running on a
@@ -1433,56 +1433,14 @@
         specified by this expression.
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
-    """
-    ...
-
 @typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
@@ -1524,14 +1482,190 @@
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables Conda.
     """
     ...
 
+@typing.overload
+def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the PyPI packages for all steps of the flow.
+    
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    """
+    ...
+
+@typing.overload
+def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+    """
+    Specifies the PyPI packages for all steps of the flow.
+    
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    """
+    ...
+
+@typing.overload
+def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the event(s) that this flow depends on.
+    
+    ```
+    @trigger(event='foo')
+    ```
+    or
+    ```
+    @trigger(events=['foo', 'bar'])
+    ```
+    
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
+    ```
+    or
+    ```
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
+    ```
+    
+    'parameters' can also be a list of strings and tuples like so:
+    ```
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
+    ```
+    
+    Parameters
+    ----------
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
+    """
+    Specifies the event(s) that this flow depends on.
+    
+    ```
+    @trigger(event='foo')
+    ```
+    or
+    ```
+    @trigger(events=['foo', 'bar'])
+    ```
+    
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
+    ```
+    or
+    ```
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
+    ```
+    
+    'parameters' can also be a list of strings and tuples like so:
+    ```
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
+    ```
+    
+    Parameters
+    ----------
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    """
+    ...
+
 def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
     This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
     
     Parameters
     ----------
@@ -1585,53 +1719,14 @@
         contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
-def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
-def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
     
     ```
     @trigger_on_finish(flow='FooFlow')
     ```
@@ -1726,109 +1821,14 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
-@typing.overload
-def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
-    
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
-    
-    Parameters
-    ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
-    """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
-    
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
-    
-    Parameters
-    ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.028185                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.511701                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
-    import typing
     import metaflow.plugins.cards.card_client
     import metaflow
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.basic
+    import typing
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.033630                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.516442                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.030601                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.514155                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import datetime
     import typing
     import metaflow.client.core
     import metaflow.events
-    import datetime
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.016999                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.499969                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import tarfile
+    import metaflow.exception
+    import metaflow.client.core
+    import metaflow
     import metaflow.metaflow_current
+    import metaflow.events
     import datetime
+    import tarfile
     import typing
-    import metaflow
-    import metaflow.events
-    import metaflow.client.core
-    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/client/filecache.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.034470                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.517338                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.datastore.content_addressed_store
     import metaflow.exception
+    import metaflow.datastore.content_addressed_store
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/clone_util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.031199                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.514710                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.019115                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.502015                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/exception.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.009652                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.492522                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.018350                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.501291                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.unbounded_foreach
+    import metaflow.exception
     import metaflow.parameters
     import metaflow.datastore.inputs
     import typing
-    import metaflow.unbounded_foreach
-    import metaflow.exception
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.026439                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.509863                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import io
     import metaflow.parameters
     import typing
-    import metaflow._vendor.click.types
-    import io
     import metaflow.plugins.datatools.s3.s3
+    import metaflow._vendor.click.types
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/metadata/metadata.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.051902                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.535673                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metadata.metadata
     import metaflow.exception
+    import metaflow.metadata.metadata
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowTaggingError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/metadata/util.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.094351                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.579200                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.010618                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.493577                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_current.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.096690                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.581431                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.plugins.cards.component_serializer
-    import typing
     import metaflow
+    import metaflow.plugins.cards.component_serializer
+    import metaflow.metaflow_current
     import metaflow.events
+    import typing
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,14 +238,27 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
+    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -304,24 +317,11 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
-    @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger_on_finish, or @trigger decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
     ...
 
 current: Current
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/mflog/mflog.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.052216                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.535995                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/multicore_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.011139                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.493996                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/parameters.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.012207                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.495083                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
-    import metaflow.parameters
-    import metaflow._vendor.click.types
     import metaflow.exception
+    import metaflow._vendor.click.types
+    import metaflow.parameters
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.020602                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.503607                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.058065                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.546291                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow._vendor.click.types
     import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow._vendor.click.types
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.058997                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.547269                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.056147                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.544199                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.055778                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.543824                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.056372                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.566452                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,15 +13,16 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
-    def __init__(self, msg):
-        ...
+class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.056605                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.544654                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.084171                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.569177                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
 class AirflowTask(object, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.084546                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.569567                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.084883                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.569911                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.067987                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.559162                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.066635                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.557822                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.071971                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.563290                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
     import metaflow.exception
     import metaflow._vendor.click.types
-    import metaflow.metaflow_current
     import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.073540                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.564849                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
     import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.067427                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.558589                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.metaflow_current
     import metaflow.events
+    import metaflow.decorators
     import metaflow
-    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.030905                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.514455                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.059575                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.550132                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.087596                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.576936                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.088957                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.578239                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.086597                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.575902                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.088299                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.577653                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.093774                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.578630                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
     import metaflow.exception
+    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.089179                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.570368                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.089995                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.571199                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/production_token.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.085457                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.570151                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def new_token(token_prefix, prev_token = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.089727                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.518335                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
+class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.092175                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.573435                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.093376                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.574655                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
     import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.090297                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.527944                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.plugins.logs_cli
+    import metaflow.exception
+    import metaflow._vendor.click.core
 
-AWS_SANDBOX_ENABLED: bool
+LOGGER_TIMESTAMP: str
 
-AWS_SANDBOX_REGION: None
+class CommandException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-SFN_EXECUTION_LOG_GROUP_ARN: None
+LOG_SOURCES: list
 
-class StepFunctionsClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def search(self, name):
+class CustomGroup(metaflow._vendor.click.core.Group, metaclass=type):
+    def __init__(self, name = None, commands = None, default_cmd = None, **attrs):
         ...
-    def push(self, name, definition, role_arn, log_execution_history):
+    def get_command(self, ctx, cmd_name):
         ...
-    def get(self, name):
+    def parse_args(self, ctx, args):
         ...
-    def trigger(self, state_machine_arn, input):
+    def resolve_command(self, ctx, args):
         ...
-    def list_executions(self, state_machine_arn, states):
+    def format_commands(self, ctx, formatter):
         ...
-    def terminate_execution(self, execution_arn):
+    ...
+
+class CustomFormatter(object, metaclass=type):
+    def __init__(self, default_cmd, original_formatter):
         ...
-    def get_state_machine_arn(self, name):
+    def __getattr__(self, name):
         ...
-    def delete(self, name):
+    def write_dl(self, rows):
         ...
     ...
 
+logs: CustomGroup
+
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.089563                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.570755                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.080547                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.566235                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.080765                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.544423                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,16 +13,15 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
+class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
+    def __init__(self, msg):
+        ...
     ...
 
-class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
+class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.081912                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.567586                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
     import metaflow.exception
+    import abc
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.081158                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.566845                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.081477                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.567167                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.046914                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.531135                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -16,39 +16,39 @@
     def __str__(self):
         ...
     ...
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class Azure(object, metaclass=type):
+class GS(object, metaclass=type):
     @classmethod
     def get_root_from_config(cls, echo, create_on_absent = True):
         ...
     def __init__(self):
         ...
     def __enter__(self):
         ...
     def __exit__(self, *args):
         ...
     def get(self, key = None, return_missing = False):
         """
-        Key MUST be a fully qualified path with uri scheme.  azure://<container_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
         """
         ...
     def put(self, key, obj, overwrite = True):
         """
-        Key MUST be a fully qualified path.  <container_name>/b/l/o/b/n/a/m/e
+        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
         """
         ...
     def info(self, key = None, return_missing = False):
         ...
     ...
 
-class AzureObject(object, metaclass=type):
+class GSObject(object, metaclass=type):
     def __init__(self, url, path, exists, size):
         ...
     @property
     def path(self):
         ...
     @property
     def url(self):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.080287                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.542828                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
+    import metaflow.exception
+    import metaflow.client.core
     import datetime
+    import metaflow.parameters
     import typing
-    import metaflow.client.core
-    import metaflow.exception
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.048440                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.532212                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.plugins.cards.card_client
     import metaflow
-    import metaflow.exception
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.076158                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.538742                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.077595                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.540184                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.076862                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.539446                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.074010                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.536466                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.042607                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.526197                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.048834                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.532616                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.085214                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.568606                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.095556                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.580304                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.095167                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.579932                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.094751                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.579562                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.050594                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.534470                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.components
     import typing
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.083432                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.530676                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
-class TypeResolvedObject(tuple, metaclass=type):
-    @staticmethod
-    def __new__(_cls, data, is_image, is_table):
-        """
-        Create new instance of TypeResolvedObject(data, is_image, is_table)
-        """
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class Azure(object, metaclass=type):
+    @classmethod
+    def get_root_from_config(cls, echo, create_on_absent = True):
+        ...
+    def __init__(self):
+        ...
+    def __enter__(self):
+        ...
+    def __exit__(self, *args):
         ...
-    def __repr__(self):
+    def get(self, key = None, return_missing = False):
         """
-        Return a nicely formatted representation string
+        Key MUST be a fully qualified path with uri scheme.  azure://<container_name>/b/l/o/b/n/a/m/e
         """
         ...
-    def __getnewargs__(self):
+    def put(self, key, obj, overwrite = True):
         """
-        Return self as a plain tuple.  Used by copy and pickle.
+        Key MUST be a fully qualified path.  <container_name>/b/l/o/b/n/a/m/e
         """
         ...
+    def info(self, key = None, return_missing = False):
+        ...
     ...
 
-TIME_FORMAT: str
-
-MAX_ARTIFACT_SIZE: int
-
-class TaskToDict(object, metaclass=type):
-    def __init__(self, only_repr = False, runtime = False):
+class AzureObject(object, metaclass=type):
+    def __init__(self, url, path, exists, size):
         ...
-    def __call__(self, task, graph = None):
+    @property
+    def path(self):
         ...
-    def object_type(self, object):
+    @property
+    def url(self):
         ...
-    def parse_image(self, data_object):
+    @property
+    def exists(self):
         ...
-    def infer_object(self, artifact_object):
+    @property
+    def size(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.083624                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.568229                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.043855                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.527350                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.078080                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.540682                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.075898                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.538488                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
     import metaflow.exception
+    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.074559                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.537080                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.038931                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.522244                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.037478                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.520658                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import io
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.046456                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.530201                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.061783                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.552287                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import io
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.023682                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.506921                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.metaflow_current
+    import io
     import metaflow.datastore.inputs
     import typing
-    import io
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.exception
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.094112                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.578963                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.045949                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.529572                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.040459                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.520931                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.event_logger
+    import abc
 
-class DebugEventLogger(metaflow.event_logger.NullEventLogger, metaclass=type):
-    @classmethod
-    def get_worker(cls):
-        ...
-    ...
-
-class DebugEventLoggerSidecar(object, metaclass=type):
-    def __init__(self):
-        ...
-    def process_message(self, msg):
+class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
+    def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
+        """
+        Retrieve the secret from secrets backend, and return a dictionary of
+        environment variables.
+        """
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.040680                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.524190                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.037911                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.521098                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.039609                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.523138                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
-
-current: metaflow.metaflow_current.Current
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    ...
+current: metaflow.metaflow_current.Current
+
+VALID_NAME_RE: str
+
+VALID_NAME_LEN: int
 
-class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.054819                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.557441                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
     import metaflow.decorators
     import metaflow.plugins.parallel_decorator
-    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.083033                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.566041                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
     import metaflow.exception
+    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.082331                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.565328                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.082614                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.565616                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.047395                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.517834                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.unbounded_foreach
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+UBF_CONTROL: str
+
+UBF_TASK: str
 
-class GS(object, metaclass=type):
-    @classmethod
-    def get_root_from_config(cls, echo, create_on_absent = True):
+class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
+    def __init__(self, iterable):
         ...
-    def __init__(self):
+    def __iter__(self):
         ...
-    def __enter__(self):
+    def __next__(self):
         ...
-    def __exit__(self, *args):
+    def __getitem__(self, key):
         ...
-    def get(self, key = None, return_missing = False):
-        """
-        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
-        """
+    def __len__(self):
         ...
-    def put(self, key, obj, overwrite = True):
-        """
-        Key MUST be a fully qualified path.  gs://<bucket_name>/b/l/o/b/n/a/m/e
-        """
+    def __str__(self):
         ...
-    def info(self, key = None, return_missing = False):
+    def __repr__(self):
         ...
     ...
 
-class GSObject(object, metaclass=type):
-    def __init__(self, url, path, exists, size):
+class InternalTestUnboundedForeachDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, attributes = None, statically_defined = False):
         ...
-    @property
-    def path(self):
+    def step_init(self, flow, graph, step_name, decorators, environment, flow_datastore, logger):
         ...
-    @property
-    def url(self):
+    def control_task_step_func(self, flow, graph, retry_count):
         ...
-    @property
-    def exists(self):
+    def task_decorate(self, step_func, flow, graph, retry_count, max_user_code_retries, ubf_context):
         ...
-    @property
-    def size(self):
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.062766                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.554298                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.065458                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.557055                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow._vendor.click.types
     import metaflow.exception
+    import metaflow._vendor.click.types
+    import metaflow.decorators
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.008439                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.491304                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.064598                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.556144                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.063662                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.555178                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/logs_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.044277                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.522494                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.logs_cli
-    import metaflow._vendor.click.core
-    import metaflow.exception
+    import metaflow.decorators
 
-LOGGER_TIMESTAMP: str
-
-class CommandException(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-LOG_SOURCES: list
-
-class CustomGroup(metaflow._vendor.click.core.Group, metaclass=type):
-    def __init__(self, name = None, commands = None, default_cmd = None, **attrs):
-        ...
-    def get_command(self, ctx, cmd_name):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    def parse_args(self, ctx, args):
-        ...
-    def resolve_command(self, ctx, args):
-        ...
-    def format_commands(self, ctx, formatter):
+    def __str__(self):
         ...
     ...
 
-class CustomFormatter(object, metaclass=type):
-    def __init__(self, default_cmd, original_formatter):
-        ...
-    def __getattr__(self, name):
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def write_dl(self, rows):
+    def step_task_retry_count(self):
         ...
     ...
 
-logs: CustomGroup
-
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.035528                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.521532                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.008737                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.491600                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.039292                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.522814                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
+
+current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-current: metaflow.metaflow_current.Current
-
-VALID_NAME_RE: str
-
-VALID_NAME_LEN: int
+class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+        ...
+    ...
 
-class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
-def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
-    ...
-
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.035198                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.518763                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.053014                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.547813                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.054062                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.549152                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import io
-    import metaflow.metaflow_environment
     import metaflow.exception
+    import abc
+    import metaflow.metaflow_environment
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.052481                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.570924                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class PyPIStepDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
-        ...
-    ...
-
-class PyPIFlowDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.054451                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.549557                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.pypi.conda_environment
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.053306                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.548349                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.037755                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.515393                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
         ...
-    def step_task_retry_count(self):
+    def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.066265                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.553229                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.066027                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.552974                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/storage_executor.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.040076                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.523603                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.045410                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.529167                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
+    import metaflow.client.core
     import metaflow.metaflow_current
-    import datetime
     import metaflow.events
-    import metaflow.client.core
-    import metaflow.exception
+    import datetime
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.034949                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.571508                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.unbounded_foreach
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
-        ...
-    ...
+AWS_SANDBOX_ENABLED: bool
 
-UBF_CONTROL: str
+AWS_SANDBOX_REGION: None
 
-UBF_TASK: str
+SFN_EXECUTION_LOG_GROUP_ARN: None
 
-class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
-    def __init__(self, iterable):
-        ...
-    def __iter__(self):
+class StepFunctionsClient(object, metaclass=type):
+    def __init__(self):
         ...
-    def __next__(self):
+    def search(self, name):
         ...
-    def __getitem__(self, key):
+    def push(self, name, definition, role_arn, log_execution_history):
         ...
-    def __len__(self):
+    def get(self, name):
         ...
-    def __str__(self):
-        ...
-    def __repr__(self):
-        ...
-    ...
-
-class InternalTestUnboundedForeachDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def __init__(self, attributes = None, statically_defined = False):
+    def trigger(self, state_machine_arn, input):
         ...
-    def step_init(self, flow, graph, step_name, decorators, environment, flow_datastore, logger):
+    def list_executions(self, state_machine_arn, states):
         ...
-    def control_task_step_func(self, flow, graph, retry_count):
+    def terminate_execution(self, execution_arn):
         ...
-    def task_decorate(self, step_func, flow, graph, retry_count, max_user_code_retries, ubf_context):
+    def get_state_machine_arn(self, name):
         ...
-    def step_task_retry_count(self):
+    def delete(self, name):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.036324                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.518213                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/procpoll.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.031599                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.515112                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/profilers/__init__.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/profilers/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.008967                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.491830                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class gpu_profile(object, metaclass=type):
     def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/tagging_util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.012512                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.495385                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.6/metaflow-stubs/tuple_util.pyi` & `ob-metaflow-stubs-3.7/metaflow-stubs/tuple_util.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.1+ob(v1)                                                   #
-# Generated on 2024-05-21T17:36:50.018537                                        #
+# MF version: 2.11.16.2+ob(v1)                                                   #
+# Generated on 2024-05-22T22:08:54.501475                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def namedtuple_with_defaults(typename, field_descr, defaults = ()):
     ...
```

### Comparing `ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.6
+Version: 3.7
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.6/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-stubs-3.6/setup.py` & `ob-metaflow-stubs-3.7/setup.py`

 * *Files identical despite different names*

