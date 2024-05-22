# Comparing `tmp/scale_egp-1.1.7.tar.gz` & `tmp/scale_egp-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_egp-1.1.7.tar", max compression
+gzip compressed data, was "scale_egp-1.1.8.tar", max compression
```

## Comparing `scale_egp-1.1.7.tar` & `scale_egp-1.1.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    17873 2024-04-18 15:16:35.856385 scale_egp-1.1.7/README.md
--rw-r--r--   0        0        0     1138 2024-04-18 15:16:35.856385 scale_egp-1.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/__init__.py
--rw-r--r--   0        0        0       74 2024-04-18 15:16:35.856385 scale_egp-1.1.7/scale_egp/cli/__init__.py
--rw-r--r--   0        0        0     4737 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/cli_main.py
--rw-r--r--   0        0        0    18102 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/collections.py
--rw-r--r--   0        0        0     7857 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/formatter.py
--rw-r--r--   0        0        0     1469 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/model_instance_description.py
--rw-r--r--   0        0        0     1828 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/parser.py
--rw-r--r--   0        0        0    52384 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/vpc_setup_commands.py
--rw-r--r--   0        0        0     1733 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/client.py
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/__init__.py
--rw-r--r--   0        0        0     2914 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/application_specs.py
--rw-r--r--   0        0        0     3170 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/chunks.py
--rw-r--r--   0        0        0     5272 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/completions.py
--rw-r--r--   0        0        0     2500 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_configs.py
--rw-r--r--   0        0        0    25007 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_datasets.py
--rw-r--r--   0        0        0     8055 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluations.py
--rw-r--r--   0        0        0     4918 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/fine_tuning.py
--rw-r--r--   0        0        0    25810 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/knowledge_bases.py
--rw-r--r--   0        0        0     2685 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/model_groups.py
--rw-r--r--   0        0        0     4798 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/model_templates.py
--rw-r--r--   0        0        0     7667 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/models.py
--rw-r--r--   0        0        0     1862 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/question_sets.py
--rw-r--r--   0        0        0     2588 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/questions.py
--rw-r--r--   0        0        0     1510 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/users.py
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/constants/__init__.py
--rw-r--r--   0        0        0      762 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/constants/model_schemas.py
--rw-r--r--   0        0        0     9257 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/enums.py
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/__init__.py
--rw-r--r--   0        0        0     2712 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/fine_tuning_jobs.py
--rw-r--r--   0        0        0     2069 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/model_enums.py
--rw-r--r--   0        0        0     8403 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/model_vendor_configuration.py
--rw-r--r--   0        0        0      647 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/__init__.py
--rw-r--r--   0        0        0     4651 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/agents.py
--rw-r--r--   0        0        0      741 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/application_specs.py
--rw-r--r--   0        0        0     6125 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/chunks.py
--rw-r--r--   0        0        0     6553 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/completions.py
--rw-r--r--   0        0        0     1016 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/embeddings.py
--rw-r--r--   0        0        0     1019 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_configs.py
--rw-r--r--   0        0        0     3170 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_dataset_test_cases.py
--rw-r--r--   0        0        0     1686 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_datasets.py
--rw-r--r--   0        0        0     4837 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_test_case_results.py
--rw-r--r--   0        0        0     1398 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluations.py
--rw-r--r--   0        0        0     3401 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/fine_tuning.py
--rw-r--r--   0        0        0     1860 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_artifacts.py
--rw-r--r--   0        0        0     1559 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_chunks.py
--rw-r--r--   0        0        0    15686 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_uploads.py
--rw-r--r--   0        0        0     1863 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_bases.py
--rw-r--r--   0        0        0     1112 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/memory_strategy.py
--rw-r--r--   0        0        0     2478 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/message.py
--rw-r--r--   0        0        0     3557 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/model_templates.py
--rw-r--r--   0        0        0    14065 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/models.py
--rw-r--r--   0        0        0     1086 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/models_group.py
--rw-r--r--   0        0        0      891 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/question_sets.py
--rw-r--r--   0        0        0     5234 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/questions.py
--rw-r--r--   0        0        0      410 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/user_info.py
--rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/__init__.py
--rw-r--r--   0        0        0    11461 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/api_utils.py
--rw-r--r--   0        0        0     3639 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/model_utils.py
--rw-r--r--   0        0        0      107 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/strenum_compat.py
--rw-r--r--   0        0        0    18948 1970-01-01 00:00:00.000000 scale_egp-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    17873 2024-05-22 22:08:13.394012 scale_egp-1.1.8/README.md
+-rw-r--r--   0        0        0     1138 2024-05-22 22:08:13.394012 scale_egp-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/__init__.py
+-rw-r--r--   0        0        0       74 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/__init__.py
+-rw-r--r--   0        0        0     4791 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/cli_main.py
+-rw-r--r--   0        0        0    18199 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/collections.py
+-rw-r--r--   0        0        0     7857 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/formatter.py
+-rw-r--r--   0        0        0     1469 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/model_instance_description.py
+-rw-r--r--   0        0        0     1828 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/parser.py
+-rw-r--r--   0        0        0    52384 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/cli/vpc_setup_commands.py
+-rw-r--r--   0        0        0     1733 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/__init__.py
+-rw-r--r--   0        0        0    13096 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/client.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/__init__.py
+-rw-r--r--   0        0        0     2914 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/application_specs.py
+-rw-r--r--   0        0        0     3170 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/chunks.py
+-rw-r--r--   0        0        0     5476 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/completions.py
+-rw-r--r--   0        0        0     2500 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_configs.py
+-rw-r--r--   0        0        0    25385 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_datasets.py
+-rw-r--r--   0        0        0     8055 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/evaluations.py
+-rw-r--r--   0        0        0     4918 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/fine_tuning.py
+-rw-r--r--   0        0        0    25810 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/knowledge_bases.py
+-rw-r--r--   0        0        0     2685 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/model_groups.py
+-rw-r--r--   0        0        0     4798 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/model_templates.py
+-rw-r--r--   0        0        0     7667 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/models.py
+-rw-r--r--   0        0        0     1862 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/question_sets.py
+-rw-r--r--   0        0        0     2588 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/questions.py
+-rw-r--r--   0        0        0     1510 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/collections/users.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/constants/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/constants/model_schemas.py
+-rw-r--r--   0        0        0     9257 2024-05-22 22:08:13.394012 scale_egp-1.1.8/scale_egp/sdk/enums.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/fine_tuning_jobs.py
+-rw-r--r--   0        0        0     2126 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/model_enums.py
+-rw-r--r--   0        0        0     8545 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/models/model_vendor_configuration.py
+-rw-r--r--   0        0        0      647 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/__init__.py
+-rw-r--r--   0        0        0     4651 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/agents.py
+-rw-r--r--   0        0        0      741 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/application_specs.py
+-rw-r--r--   0        0        0     6125 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/chunks.py
+-rw-r--r--   0        0        0     6750 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/completions.py
+-rw-r--r--   0        0        0     1016 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/embeddings.py
+-rw-r--r--   0        0        0     1019 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_configs.py
+-rw-r--r--   0        0        0     3551 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_dataset_test_cases.py
+-rw-r--r--   0        0        0     1686 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_datasets.py
+-rw-r--r--   0        0        0     4837 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluation_test_case_results.py
+-rw-r--r--   0        0        0     1398 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/evaluations.py
+-rw-r--r--   0        0        0     3401 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/fine_tuning.py
+-rw-r--r--   0        0        0     1860 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_artifacts.py
+-rw-r--r--   0        0        0     1559 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_chunks.py
+-rw-r--r--   0        0        0    15686 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_uploads.py
+-rw-r--r--   0        0        0     1863 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/knowledge_bases.py
+-rw-r--r--   0        0        0     1112 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/memory_strategy.py
+-rw-r--r--   0        0        0     2478 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/message.py
+-rw-r--r--   0        0        0     3557 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/model_templates.py
+-rw-r--r--   0        0        0    14065 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/models.py
+-rw-r--r--   0        0        0     1086 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/models_group.py
+-rw-r--r--   0        0        0      891 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/question_sets.py
+-rw-r--r--   0        0        0     5234 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/questions.py
+-rw-r--r--   0        0        0      410 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/sdk/types/user_info.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/__init__.py
+-rw-r--r--   0        0        0    11461 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/api_utils.py
+-rw-r--r--   0        0        0     3639 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/model_utils.py
+-rw-r--r--   0        0        0      107 2024-05-22 22:08:13.398012 scale_egp-1.1.8/scale_egp/utils/strenum_compat.py
+-rw-r--r--   0        0        0    18948 1970-01-01 00:00:00.000000 scale_egp-1.1.8/PKG-INFO
```

### Comparing `scale_egp-1.1.7/README.md` & `scale_egp-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/pyproject.toml` & `scale_egp-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scale-egp"
-version = "1.1.7"
+version = "1.1.8"
 description = "SDK for Scale SGP API"
 license = "Apache 2.0 modified with Commons Clause"
 authors = ["Scale SGP team"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/sgp-py/"
 repository = "https://github.com/scaleapi/egp-py"
 packages = [{include = "scale_egp"}]
```

### Comparing `scale_egp-1.1.7/scale_egp/cli/cli_main.py` & `scale_egp-1.1.8/scale_egp/cli/cli_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     add_commands_to_parser(parser, ModelDeploymentCommands(client_factory))
     add_commands_to_parser(parser, ModelTemplateCommands(client_factory))
     add_commands_to_parser(parser, UserCommands(client_factory))
     add_commands_to_parser(parser, FineTuningJobCommands(client_factory))
     add_commands_to_parser(parser, TrainingDatasetCommands(client_factory))
     add_commands_to_parser(parser, AwsVpcSetupCommands(client_factory))
     for plugin_command_cls in load_plugins(parser):
-        print(f"Loading plugin: {plugin_command_cls.__name__}")
+        # Uncomment to debug plugin loading issues:
+        # print(f"Loading plugin: {plugin_command_cls.__name__}")
         add_commands_to_parser(parser, plugin_command_cls(client_factory))
     args = parser.parse_args(argv)
     try:
         client_factory.set_client_kwargs(
             api_key=args.api_key,
             endpoint_url=args.endpoint_url,
             account_id=args.account_id,
```

### Comparing `scale_egp-1.1.7/scale_egp/cli/collections.py` & `scale_egp-1.1.8/scale_egp/cli/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,18 @@
         assert response.status_code == 200
 
     def list(self) -> Generator[EntityT, None, None]:
         formatting_options = self.list_formatting_options or get_formatting_options()
         formatting_options.force_list = True
         set_formatting_options(formatting_options)
         collection = self._get_collection_instance()
-        response = collection._get(self._get_api_subpath_prefix())
+        response = collection._get(
+            self._get_api_subpath_prefix(),
+            {"account_id": self._client_factory.get_client().account_id},
+        )
         assert response.status_code == 200
         response_list = response.json()
         assert isinstance(response_list, list)
         # TODO: pagination
         for entity_dict in response_list:
             yield self._entity_type(**entity_dict)
```

### Comparing `scale_egp-1.1.7/scale_egp/cli/formatter.py` & `scale_egp-1.1.8/scale_egp/cli/formatter.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/cli/model_instance_description.py` & `scale_egp-1.1.8/scale_egp/cli/model_instance_description.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/cli/parser.py` & `scale_egp-1.1.8/scale_egp/cli/parser.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/cli/vpc_setup_commands.py` & `scale_egp-1.1.8/scale_egp/cli/vpc_setup_commands.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/exceptions.py` & `scale_egp-1.1.8/scale_egp/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/client.py` & `scale_egp-1.1.8/scale_egp/sdk/client.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/application_specs.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/chunks.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/completions.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         model: Union[
             Literal[
                 "gpt-4",
                 "gpt-4-0613",
                 "gpt-4-32k",
                 "gpt-4-32k-0613",
                 "gpt-4-vision-preview",
+                "gpt-4o",
                 "gpt-3.5-turbo",
                 "gpt-3.5-turbo-0613",
                 "gpt-3.5-turbo-16k",
                 "gpt-3.5-turbo-16k-0613",
                 "text-davinci-003",
                 "text-davinci-002",
                 "text-curie-001",
@@ -61,18 +62,20 @@
                 "codellama-13b",
                 "codellama-13b-instruct",
                 "codellama-34b",
                 "codellama-34b-instruct",
                 "codellama-70b",
                 "codellama-70b-instruct",
                 "gemini-pro",
+                "gemini-1.5-pro-preview-0409"
             ],
             str,
         ],
         prompt: str,
+        account_id: str,
         images: Optional[List[ImageCompletionRequests]] = None,
         model_parameters: Optional[ModelParameters] = None,
     ) -> Completion:
         """
         Create a new LLM Completion.
 
         Args:
@@ -87,14 +90,15 @@
             self._post(
                 sub_path=self._sub_path,
                 request=CompletionRequest(
                     model=model,
                     prompt=prompt,
                     images=images,
                     model_parameters=model_parameters,
+                    account_id=account_id,
                 ),
             ).json()
         )
 
     def stream(
         self,
         model: Literal[
@@ -143,14 +147,15 @@
             "codellama-13b-instruct",
             "codellama-34b",
             "codellama-34b-instruct",
             "codellama-70b",
             "codellama-70b-instruct",
         ],
         prompt: str,
+        account_id: str,
         images: Optional[List[ImageCompletionRequests]] = None,
         model_parameters: Optional[ModelParameters] = None,
     ) -> Iterable[Completion]:
         """
         Stream LLM Completions.
 
         Returns:
@@ -160,14 +165,15 @@
             sub_path=self._sub_path,
             request=CompletionRequest(
                 model=model,
                 prompt=prompt,
                 images=images,
                 model_parameters=model_parameters,
                 stream=True,
+                account_id=account_id,
             ),
         )
         if iterable_payloads:
             for response_dict in iterable_payloads:
                 yield Completion.from_dict(response_dict)
         else:
             return []
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_configs.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_datasets.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/evaluation_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 import json
-from typing import Optional, List, Iterable, Union
+from typing import Any, Dict, Optional, List, Iterable, Union
 
 import httpx
 
 from scale_egp.sdk.enums import TestCaseSchemaType
 from scale_egp.sdk.types.evaluation_dataset_test_cases import (
     TestCase, TestCaseRequest, TestCaseSchemaValidator, GenerationTestCaseData,
 )
@@ -564,14 +564,16 @@
     _sub_path = "v2/evaluation-datasets/{evaluation_dataset_id}/test-cases"
 
     def create(
         self,
         evaluation_dataset: EvaluationDataset,
         schema_type: TestCaseSchemaType,
         test_case_data: Union[GenerationTestCaseData],
+        test_case_metadata: Optional[Dict[str, Any]] = None,
+        chat_history: Optional[Dict[str, Any]] = None,
     ) -> TestCase:
         """
         Create a new test case.
 
         Args:
             evaluation_dataset: The dataset to create the test case in.
             schema_type: The schema type of the test case.
@@ -579,18 +581,19 @@
 
         Returns:
             The newly created test case.
         """
         response = self._post(
             sub_path=self._sub_path.format(evaluation_dataset_id=evaluation_dataset.id),
             request=TestCaseRequest(
-                evaluation_dataset_id=evaluation_dataset.id,
                 schema_type=schema_type,
                 test_case_data=test_case_data,
                 account_id=self._api_client.account_id,
+                test_case_metadata=test_case_metadata,
+                chat_history=chat_history,
             ),
         )
         return TestCase.from_dict(response.json())
 
     def create_batch(
         self,
         evaluation_dataset: EvaluationDataset,
@@ -649,14 +652,16 @@
 
     def update(
         self,
         test_case_id: str,
         evaluation_dataset: EvaluationDataset,
         schema_type: Optional[TestCaseSchemaType] = None,
         test_case_data: Optional[Union[GenerationTestCaseData]] = None,
+        test_case_metadata: Optional[Dict[str, Any]] = None,
+        chat_history: Optional[Dict[str, Any]] = None,
     ) -> TestCase:
         """
         Update an existing test case.
 
         Args:
             test_case_id: The ID of the test case.
             evaluation_dataset: The dataset to update the test case in.
@@ -668,14 +673,16 @@
         """
         response = self._patch(
             sub_path=f"{self._sub_path.format(evaluation_dataset_id=evaluation_dataset.id)}/"
             f"{test_case_id}",
             request=TestCaseRequest.partial(
                 schema_type=schema_type,
                 test_case_data=test_case_data,
+                test_case_metadata=test_case_metadata,
+                chat_history=chat_history,
             ),
         )
         return TestCase.from_dict(response.json())
 
     def iter(self, evaluation_dataset: EvaluationDataset) -> Iterable[TestCase]:
         """
         Iterate over all test cases in a dataset.
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/evaluations.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/fine_tuning.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/knowledge_bases.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/model_groups.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/model_groups.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/model_templates.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/models.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/question_sets.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/questions.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/collections/users.py` & `scale_egp-1.1.8/scale_egp/sdk/collections/users.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/constants/model_schemas.py` & `scale_egp-1.1.8/scale_egp/sdk/constants/model_schemas.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/enums.py` & `scale_egp-1.1.8/scale_egp/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/models/fine_tuning_jobs.py` & `scale_egp-1.1.8/scale_egp/sdk/models/fine_tuning_jobs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/models/model_enums.py` & `scale_egp-1.1.8/scale_egp/sdk/models/model_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class ModelVendor(str, Enum):
     """
     An enum representing the different types of model vendors supported.
 
     Attributes:
         OPENAI: Denotes that the model vendor is OpenAI.
         COHERE: Denotes that the model vendor is Cohere.
+        GOOGLE: Denotes that the model vendor is Google.
         ANTHROPIC: Denotes that the model vendor is Anthropic.
         LLMENGINE: Denotes that the model vendor is LLM Engine.
         OTHER: Denotes that the model vendor is Other.
     """
 
     OPENAI = "OPENAI"
     COHERE = "COHERE"
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/models/model_vendor_configuration.py` & `scale_egp-1.1.8/scale_egp/sdk/models/model_vendor_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,16 @@
     # For example, see: https://github.com/scaleapi/models/blob/19b8c83e88962ac6b6a9d52b998c35345f862e80/enterprise/egp_finetuning/docker_utils/create_docker_bundle.py#L104-L142
     # Note that some
     mount_location: Optional[str] = Field(
         default="/workspace/launch_specific/config.json",
         description="The filesystem location where the fine tuning job's configuration will be available when it is started.",
     )
     training_dataset_schema_type: Optional[TrainingDatasetORMSchemaTypeEnum] = Field(
-        default=None, description="Optionally set required training and validation dataset schema"
+        default=None,
+        description="Optionally set required training and validation dataset schema",
     )
     resources: Optional[RequiredResources] = Field(default_factory=RequiredResources)
 
 
 class LaunchVendorConfiguration(BaseModel):
     """
     Configuration for launching a model using the Launch service which is an internal and
@@ -154,14 +155,16 @@
     num_shards: int = Field(default=4)
     # QUESTION: Is the value of quantize always "bitsandbytes"? If so we can leave it out.
     # TODO: this should probably be a full URI not just a path in S3 relative to a specific bucket
     # since single-tenant EGP instance will have their own buckets, azure instances won't use S3, etc,
     # but I don't want to deviate from create_llm_model_endpoint() parameter names and using a full URL
     # would also require support from model-engine.
     checkpoint_path: Optional[str] = Field(None)
+    # Optionally override the ModelInstance.name field with an explicitly set model name
+    model_name: Optional[str] = Field(None)
 
 
 ModelVendorConfiguration = LaunchVendorConfiguration
 
 
 class DeploymentVendorConfiguration(BaseModel):
     __root__: Union[LaunchDeploymentVendorConfiguration, LLMEngineDeploymentVendorConfiguration] = (
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/__init__.py` & `scale_egp-1.1.8/scale_egp/sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/agents.py` & `scale_egp-1.1.8/scale_egp/sdk/types/agents.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/application_specs.py` & `scale_egp-1.1.8/scale_egp/sdk/types/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/chunks.py` & `scale_egp-1.1.8/scale_egp/sdk/types/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/completions.py` & `scale_egp-1.1.8/scale_egp/sdk/types/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,7 +166,11 @@
                     "- stop_sequences: None",
     )
     stream: bool = Field(
         default=False,
         description="Whether or not to stream the response.\n\n"
                     "Setting this to True will stream the completion in real-time.",
     )
+    account_id: Optional[str] = Field(
+        ...,
+        description="The account ID to use for completions. If you have access to more than one account, you must specify an account_id.",
+    )
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/embeddings.py` & `scale_egp-1.1.8/scale_egp/sdk/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_configs.py` & `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_dataset_test_cases.py` & `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_dataset_test_cases.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,23 +50,31 @@
             data to evaluate an application against.
     """
 
     id: str
     evaluation_dataset_id: str
     schema_type: TestCaseSchemaType
     test_case_data: Union[GenerationTestCaseData]
+    test_case_metadata: Optional[Dict[str, Any]]
+    chat_history: Optional[Dict[str, Any]]
 
 
 class TestCaseRequest(BaseModel):
     schema_type: TestCaseSchemaType
     test_case_data: Union[GenerationTestCaseData]
     account_id: Optional[str] = Field(
         description="Account to create knowledge base in. If you have access to more than one "
         "account, you must specify an account_id"
     )
+    test_case_metadata: Optional[Dict[str, Any]] = Field(
+        description="Additional metadata to associate with the test case"
+    )
+    chat_history: Optional[Dict[str, Any]] = Field(
+        description="Used for tracking previous chat interactions for multi-chat test cases"
+    )
 
     @validator("test_case_data")
     @classmethod
     def test_case_data_matches_schema_type(cls, test_case_data, values):
         schema_type = values.get("schema_type")
         TestCaseSchemaValidator.validate(schema_type, test_case_data)
         return test_case_data
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_datasets.py` & `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_test_case_results.py` & `scale_egp-1.1.8/scale_egp/sdk/types/evaluation_test_case_results.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/evaluations.py` & `scale_egp-1.1.8/scale_egp/sdk/types/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/fine_tuning.py` & `scale_egp-1.1.8/scale_egp/sdk/types/fine_tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # !!!!! DO NOT EVER CHANGE THIS FILE MANUALLY -- AUTOGENERATED by orm2pydantic.py !!!!!
-# Generated on 2024-04-09 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
+# Generated on 2024-04-17 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
 # To regenerate this file, run:
 # scaleapi/packages/egp-api-backend/scripts/orm2pydantic.sh
 
 from scale_egp.utils.model_utils import BaseModel, Entity
 from pydantic import Field
 
 from datetime import (datetime)
```

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_artifacts.py` & `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_artifacts.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_chunks.py` & `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_uploads.py` & `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_base_uploads.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_bases.py` & `scale_egp-1.1.8/scale_egp/sdk/types/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/memory_strategy.py` & `scale_egp-1.1.8/scale_egp/sdk/types/memory_strategy.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/message.py` & `scale_egp-1.1.8/scale_egp/sdk/types/message.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/model_templates.py` & `scale_egp-1.1.8/scale_egp/sdk/types/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/models.py` & `scale_egp-1.1.8/scale_egp/sdk/types/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/models_group.py` & `scale_egp-1.1.8/scale_egp/sdk/types/models_group.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/question_sets.py` & `scale_egp-1.1.8/scale_egp/sdk/types/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/sdk/types/questions.py` & `scale_egp-1.1.8/scale_egp/sdk/types/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/utils/api_utils.py` & `scale_egp-1.1.8/scale_egp/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/scale_egp/utils/model_utils.py` & `scale_egp-1.1.8/scale_egp/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.7/PKG-INFO` & `scale_egp-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-egp
-Version: 1.1.7
+Version: 1.1.8
 Summary: SDK for Scale SGP API
 Home-page: https://scaleapi.github.io/sgp-py/
 License: Apache 2.0 modified with Commons Clause
 Author: Scale SGP team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

