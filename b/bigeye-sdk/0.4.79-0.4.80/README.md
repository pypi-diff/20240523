# Comparing `tmp/bigeye_sdk-0.4.79.tar.gz` & `tmp/bigeye_sdk-0.4.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.79.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.80.tar", max compression
```

## Comparing `bigeye_sdk-0.4.79.tar` & `bigeye_sdk-0.4.80.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     2092 2024-03-26 20:10:15.103396 bigeye_sdk-0.4.79/LICENSE
--rw-r--r--   0        0        0      873 2024-03-26 20:10:15.103476 bigeye_sdk-0.4.79/README.md
--rw-r--r--   0        0        0     3727 2024-03-26 20:10:15.103593 bigeye_sdk-0.4.79/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 20:10:15.103676 bigeye_sdk-0.4.79/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.103753 bigeye_sdk-0.4.79/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    20437 2024-04-11 16:32:04.911659 bigeye_sdk-0.4.79/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0    12403 2024-04-15 14:38:37.318540 bigeye_sdk-0.4.79/bigeye_sdk/authentication/config.py
--rw-r--r--   0        0        0     1182 2024-03-26 20:10:15.104056 bigeye_sdk-0.4.79/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2024-03-26 20:10:15.104126 bigeye_sdk-0.4.79/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104202 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10366 2024-03-26 20:10:15.104359 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2024-03-26 20:10:15.104508 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2024-03-26 20:10:15.104585 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      736 2024-03-26 20:10:15.104656 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9363 2024-03-26 20:10:15.104804 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3900 2024-03-26 20:10:15.104890 bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.104964 bigeye_sdk-0.4.79/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2024-03-26 20:10:15.105053 bigeye_sdk-0.4.79/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2024-03-26 20:10:15.105125 bigeye_sdk-0.4.79/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105194 bigeye_sdk-0.4.79/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 20:10:15.105276 bigeye_sdk-0.4.79/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39844 2024-04-11 16:32:04.913155 bigeye_sdk-0.4.79/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2024-03-26 20:10:15.105478 bigeye_sdk-0.4.79/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    52140 2024-03-28 11:45:06.797716 bigeye_sdk-0.4.79/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.105719 bigeye_sdk-0.4.79/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-26 20:10:15.105839 bigeye_sdk-0.4.79/bigeye_sdk/controller/delta_controller.py
--rw-r--r--   0        0        0    15116 2024-03-28 11:45:06.797906 bigeye_sdk-0.4.79/bigeye_sdk/controller/lineage_controller.py
--rw-r--r--   0        0        0     3209 2024-03-26 20:10:15.106039 bigeye_sdk-0.4.79/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    38904 2024-04-12 15:53:26.266034 bigeye_sdk-0.4.79/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106304 bigeye_sdk-0.4.79/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2024-03-26 20:10:15.106404 bigeye_sdk-0.4.79/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2024-03-26 20:10:15.106520 bigeye_sdk-0.4.79/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1582 2024-03-26 20:10:15.106598 bigeye_sdk-0.4.79/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 20:10:15.106671 bigeye_sdk-0.4.79/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2024-03-26 20:10:15.106799 bigeye_sdk-0.4.79/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2024-03-26 20:10:15.106912 bigeye_sdk-0.4.79/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     2450 2024-03-26 20:10:15.106994 bigeye_sdk-0.4.79/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2024-03-26 20:10:15.107087 bigeye_sdk-0.4.79/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2024-03-26 20:10:15.107178 bigeye_sdk-0.4.79/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0      370 2024-03-26 20:10:15.107269 bigeye_sdk-0.4.79/bigeye_sdk/functions/dbt.py
--rw-r--r--   0        0        0     4580 2024-03-26 20:10:15.107401 bigeye_sdk-0.4.79/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2814 2024-03-26 20:10:15.107482 bigeye_sdk-0.4.79/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      706 2024-03-26 20:10:15.107556 bigeye_sdk-0.4.79/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0      410 2024-03-26 20:10:15.107645 bigeye_sdk-0.4.79/bigeye_sdk/functions/issue_functions.py
--rw-r--r--   0        0        0    21897 2024-03-26 20:10:15.107751 bigeye_sdk-0.4.79/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2701 2024-03-26 20:10:15.107850 bigeye_sdk-0.4.79/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2024-03-26 20:10:15.107923 bigeye_sdk-0.4.79/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2024-03-26 20:10:15.107998 bigeye_sdk-0.4.79/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5377 2024-04-15 14:39:08.005416 bigeye_sdk-0.4.79/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2024-03-26 20:10:15.108209 bigeye_sdk-0.4.79/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2024-03-26 20:10:15.108284 bigeye_sdk-0.4.79/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2024-04-15 14:45:26.753938 bigeye_sdk-0.4.79/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:45:26.754066 bigeye_sdk-0.4.79/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:45:26.754171 bigeye_sdk-0.4.79/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:45:26.754267 bigeye_sdk-0.4.79/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   280404 2024-04-15 14:45:26.754376 bigeye_sdk-0.4.79/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2024-04-15 14:45:26.754531 bigeye_sdk-0.4.79/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2024-04-15 14:45:26.754663 bigeye_sdk-0.4.79/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      993 2024-03-26 20:10:15.109440 bigeye_sdk-0.4.79/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2024-03-26 20:10:15.109559 bigeye_sdk-0.4.79/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      492 2024-03-26 20:10:15.109643 bigeye_sdk-0.4.79/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    37552 2024-03-26 20:10:15.109766 bigeye_sdk-0.4.79/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2024-03-26 20:10:15.109855 bigeye_sdk-0.4.79/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0      872 2024-03-26 20:10:15.109935 bigeye_sdk-0.4.79/bigeye_sdk/model/dbt_manifest.py
--rw-r--r--   0        0        0     4518 2024-03-26 20:10:15.110060 bigeye_sdk-0.4.79/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     5521 2024-03-26 20:10:15.110183 bigeye_sdk-0.4.79/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0       89 2024-03-26 20:10:15.110260 bigeye_sdk-0.4.79/bigeye_sdk/model/enums.py
--rw-r--r--   0        0        0     9459 2024-03-26 20:10:15.110414 bigeye_sdk-0.4.79/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     9611 2024-03-26 20:10:15.110560 bigeye_sdk-0.4.79/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      221 2024-03-26 20:10:15.110628 bigeye_sdk-0.4.79/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    56945 2024-03-26 20:10:15.110758 bigeye_sdk-0.4.79/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2024-03-26 20:10:15.110847 bigeye_sdk-0.4.79/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7599 2024-03-26 20:10:15.110966 bigeye_sdk-0.4.79/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3373 2024-04-15 14:40:41.252857 bigeye_sdk-0.4.79/pyproject.toml
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.79/PKG-INFO
+-rw-r--r--   0        0        0     2092 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/LICENSE
+-rw-r--r--   0        0        0      873 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/README.md
+-rw-r--r--   0        0        0     3727 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       76 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    20437 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0    12761 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/authentication/config.py
+-rw-r--r--   0        0        0     1182 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10366 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      736 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9363 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3900 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39844 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    52140 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0     2666 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/controller/delta_controller.py
+-rw-r--r--   0        0        0    15116 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/controller/lineage_controller.py
+-rw-r--r--   0        0        0     3209 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    38904 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2024-05-01 16:37:01.690511 bigeye_sdk-0.4.80/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     2450 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0      370 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/dbt.py
+-rw-r--r--   0        0        0     4580 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2814 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      706 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0      410 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/issue_functions.py
+-rw-r--r--   0        0        0    21897 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2701 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5377 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0     2459 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/functions/version.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   281011 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      993 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    37552 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0      872 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/dbt_manifest.py
+-rw-r--r--   0        0        0     4518 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     5521 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0       89 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/enums.py
+-rw-r--r--   0        0        0     9459 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     9611 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      221 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    56945 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7599 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3383 2024-05-01 16:37:01.694511 bigeye_sdk-0.4.80/pyproject.toml
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.80/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.79/LICENSE` & `bigeye_sdk-0.4.80/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/README.md` & `bigeye_sdk-0.4.80/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.80/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.80/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/authentication/config.py` & `bigeye_sdk-0.4.80/bigeye_sdk/authentication/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,33 +33,41 @@
     """The path used to output bigconfig PLAN reports and FIXME files.'"""
     bigconfig_strict_mode: bool = False
     """API errors cause an exception if True. (Validation errors still cause an exception) Default = False"""
     bigconfig_auto_approve: bool = False
     """Bigconfig applies should be allowed to run without excplit plan approvals. Default = False"""
     dbt_manifest_file: Optional[str] = None
     """The path to the dbt manifest.json file used to ingest model owners into Bigeye."""
+    auto_update_enabled: bool = False
+    """Whether or not the CLI should automatically update when newer versions are detected."""
+    disable_auto_update_message: bool = False
+    """Optionally silence warnings for newer versions detected."""
 
     @validator("bigconfig_input_path", pre=True)
     def validate_input_path_is_list(cls, value):
-        if value: return value.split(',')
-        else: return None
+        if value:
+            return value.split(',')
+        else:
+            return None
 
 
 class Config:
     """Advanced configuration for Bigeye clients."""
 
     OPTION_DEFAULTS = OrderedDict(
         [
             ('workspace_id', None),
             ('use_default_credential', True),
             ('bigconfig_input_path', None),
             ('bigconfig_output_path', None),
             ('bigconfig_strict_mode', False),
             ('bigconfig_auto_approve', False),
-            ('dbt_manifest_file', None)
+            ('dbt_manifest_file', None),
+            ('auto_update_enabled', False),
+            ('disable_auto_update_message', False)
         ]
     )
 
     def __init__(self, *args, **kwargs):
         self._user_provided_options = self._record_user_provided_options(args, kwargs)
         # Each section and their settings should be treated independently unless otherwise
         # specified so removing the concept of default section from parser
@@ -205,15 +213,15 @@
                     workspaces[parts[1]] = values
             elif key.lower() == 'default':
                 workspaces[key] = values
             else:
                 raise ConfigParseException(f'Failed to parse section {key}. '
                                            f'Each non-default section should start with `workspace {key}`')
         return workspaces
-    
+
 
     def upsert_workspace_config(self, config_file: str, workspace: str) -> None:
         """
         Read a users current config file and based on the workspace provided, either
         update the user provided options in an existing section or add a new section that includes
         all of the options passed into the constructor.
         """
@@ -229,15 +237,15 @@
         else:
             cp.add_section(f'workspace {workspace}')
             cp[f'workspace {workspace}'] = self._user_provided_options
 
         # Write changes to users config file
         with open(file,'w+') as configfile:
             cp.write(configfile)
-    
+
 
     def set_workspace_config(self, config_file: str, setting: dict, workspace: str) -> None:
         """
         Read a users current config file and sets the value of a provided key/pair accordingly.
 
         Args:
             config_file: file containing the configuration.  If none will look for environment
```

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.80/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.80/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.80/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.80/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.80/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/controller/delta_controller.py` & `bigeye_sdk-0.4.80/bigeye_sdk/controller/delta_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/controller/lineage_controller.py` & `bigeye_sdk-0.4.80/bigeye_sdk/controller/lineage_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/controller/metric_controller.py` & `bigeye_sdk-0.4.80/bigeye_sdk/controller/metric_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.80/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/helpers.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.80/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.80/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     HOURS_SINCE_LAST_LOAD = 68
     COUNT_READ_QUERIES = 69
     PERCENT_NOT_NULL = 70
     FRESHNESS = 71
     VOLUME = 72
     FRESHNESS_DATA = 73
     VOLUME_DATA = 74
+    COUNT_VALUE_IN_LIST = 75
 
 
 class FieldType(betterproto.Enum):
     FIELD_TYPE_UNSPECIFIED = 0
     FIELD_TYPE_STRING = 1
     FIELD_TYPE_UUID = 2
     FIELD_TYPE_BINARY = 3
@@ -478,14 +479,15 @@
     AGGREGATE_FIELD_AUTOMETRICS = 10
     AGGREGATE_FIELD_GROUP_METRIC_STATUS = 11
     AGGREGATE_FIELD_ALERTS = 12
     AGGREGATE_FIELD_ISSUES = 13
     AGGREGATE_FIELD_INTEGRATIONS = 14
     AGGREGATE_FIELD_BI_TOOLS = 15
     AGGREGATE_FIELD_ETL_TOOLS = 16
+    AGGREGATE_FIELD_CUSTOM_RULES = 17
 
 
 class GroupByEntityType(betterproto.Enum):
     GROUP_BY_ENTITY_TYPE_UNSPECIFIED = 0
     GROUP_BY_ENTITY_TYPE_WAREHOUSE = 1
     GROUP_BY_ENTITY_TYPE_SCHEMA = 2
     GROUP_BY_ENTITY_TYPE_TABLE = 3
@@ -636,14 +638,15 @@
 
 class TableSortField(betterproto.Enum):
     TABLE_SORT_FIELD_UNSPECIFIED = 0
     TABLE_SORT_FIELD_NAME = 1
     TABLE_SORT_FIELD_LAST_SCHEMA_CHANGE = 2
     TABLE_SORT_FIELD_FAVORITE = 3
     TABLE_SORT_FIELD_LAST_UPDATED = 4
+    TABLE_SORT_FIELD_POPULARITY = 5
 
 
 class ColumnSortField(betterproto.Enum):
     COLUMN_SORT_FIELD_UNSPECIFIED = 0
     COLUMN_SORT_FIELD_NAME = 1
     COLUMN_SORT_FIELD_FAVORITE = 2
 
@@ -2815,14 +2818,15 @@
     source_ids: List[int] = betterproto.int32_field(4)
     schema_ids: List[int] = betterproto.int32_field(5)
     table_ids: List[int] = betterproto.int32_field(6)
     column_ids: List[int] = betterproto.int32_field(7)
     statuses: List[str] = betterproto.string_field(8)
     metric_types: List["PredefinedMetricName"] = betterproto.enum_field(9)
     workspace_id: int = betterproto.int32_field(10)
+    custom_rule_ids: List[int] = betterproto.int32_field(11)
 
 
 @dataclass
 class BulkIssueUpdateWhereClause(betterproto.Message):
     ids: List[int] = betterproto.int32_field(1)
     search: str = betterproto.string_field(2)
     search_all: bool = betterproto.bool_field(3)
@@ -2955,14 +2959,17 @@
     )
     issue_message_update: "IssueMessageUpdate" = betterproto.message_field(
         5, group="event"
     )
     issue_assignment_update: "IssueAssignmentUpdate" = betterproto.message_field(
         6, group="event"
     )
+    issue_config_update: "IssueConfigUpdate" = betterproto.message_field(
+        7, group="event"
+    )
 
 
 @dataclass
 class Issue(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     metric_configuration: "MetricConfiguration" = betterproto.message_field(3)
@@ -3003,14 +3010,16 @@
 
 
 @dataclass
 class IssueConfigUpdate(betterproto.Message):
     mute_until_timestamp: int = betterproto.int64_field(1)
     summary: str = betterproto.string_field(2)
     description: str = betterproto.string_field(3)
+    created_by: "User" = betterproto.message_field(4)
+    id: int = betterproto.int32_field(5)
 
 
 @dataclass
 class IssueMessageUpdate(betterproto.Message):
     id: int = betterproto.int32_field(1)
     created_by: "User" = betterproto.message_field(2)
     message: str = betterproto.string_field(3)
@@ -3270,14 +3279,15 @@
     request: "VirtualTableRequest" = betterproto.message_field(2)
 
 
 @dataclass
 class UserEventExchangeMessage(betterproto.Message):
     reinitialize_realm: bool = betterproto.bool_field(1)
     email_to_lock: str = betterproto.string_field(2)
+    email_to_unlock: str = betterproto.string_field(3)
 
 
 @dataclass
 class CacheEventExchangeMessage(betterproto.Message):
     cache_operation: "CacheOperation" = betterproto.enum_field(1)
 
 
@@ -4675,14 +4685,17 @@
     custom_rule: "CustomRule" = betterproto.message_field(2)
     created_by: "User" = betterproto.message_field(3)
     created_at_epoch_seconds: int = betterproto.int64_field(4)
     updated_by: "User" = betterproto.message_field(5)
     updated_at_epoch_seconds: int = betterproto.int64_field(6)
     is_favorite: bool = betterproto.bool_field(7)
     latest_runs: List["MetricRun"] = betterproto.message_field(8)
+    collections: List["IdAndDisplayName"] = betterproto.message_field(9)
+    warehouse: "IdAndDisplayName" = betterproto.message_field(10)
+    metric_id: int = betterproto.int32_field(11)
 
 
 @dataclass
 class UpdateCustomRuleRequest(betterproto.Message):
     id: int = betterproto.int32_field(1)
     custom_rule: "CustomRule" = betterproto.message_field(2)
```

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.80/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/log/__init__.py` & `bigeye_sdk-0.4.80/bigeye_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/dbt_manifest.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/dbt_manifest.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.80/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.80/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.79/pyproject.toml` & `bigeye_sdk-0.4.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.79"
+version = "0.4.80"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
@@ -48,15 +48,15 @@
 pytest = "^7.1.3"
 Sphinx = { version = "^5.2.2"}
 sphinx-rtd-theme = { version = "^1.0.0"}
 
 [tool.poe.tasks]
     test = ["python_tests"]
     pre_build = ["protogen"]
-    pre_publish = ["clean"]
+    pre_publish = ["clean", "docgen"]
     pre_install = ["protogen"]
     post_install = []
     post_publish = ["clean"]
 
     [tool.poe.tasks.include_generated]
         help = "Includes generated code for the Poetry build.  Git excluded code is not included in Poetry Build"
         shell = """
```

### Comparing `bigeye_sdk-0.4.79/PKG-INFO` & `bigeye_sdk-0.4.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.79
+Version: 0.4.80
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
 Requires-Dist: boto3 (>=1.26.7,<2.0.0)
 Requires-Dist: botocore (>=1.29.7,<2.0.0)
 Requires-Dist: grpclib (>=0.4.2,<0.5.0)
 Requires-Dist: keyring (>=24.3.1,<25.0.0)
 Requires-Dist: lz4 (>=4.0.1,<5.0.0)
```

