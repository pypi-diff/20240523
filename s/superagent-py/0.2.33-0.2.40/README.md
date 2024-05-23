# Comparing `tmp/superagent_py-0.2.33.tar.gz` & `tmp/superagent_py-0.2.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.2.33.tar", max compression
+gzip compressed data, was "superagent_py-0.2.40.tar", max compression
```

## Comparing `superagent_py-0.2.33.tar` & `superagent_py-0.2.40.tar`

### file list

```diff
@@ -1,99 +1,102 @@
--rw-r--r--   0        0        0     1073 2024-04-22 09:45:57.869678 superagent_py-0.2.33/LICENSE
--rw-r--r--   0        0        0     3946 2024-04-22 09:45:57.869678 superagent_py-0.2.33/README.md
--rw-r--r--   0        0        0      434 2024-04-22 09:45:57.869678 superagent_py-0.2.33/pyproject.toml
--rw-r--r--   0        0        0     3944 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/__init__.py
--rw-r--r--   0        0        0     6143 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/client.py
--rw-r--r--   0        0        0      790 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1732 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/core/request_options.py
--rw-r--r--   0        0        0      166 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/environment.py
--rw-r--r--   0        0        0      170 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/py.typed
--rw-r--r--   0        0        0      333 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    71786 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/api_key/__init__.py
--rw-r--r--   0        0        0    17585 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/api_key/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/api_user/__init__.py
--rw-r--r--   0        0        0    17007 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/api_user/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/datasource/__init__.py
--rw-r--r--   0        0        0    23365 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/datasource/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/llm/__init__.py
--rw-r--r--   0        0        0    17465 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/llm/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/tool/__init__.py
--rw-r--r--   0        0        0    26029 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/tool/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/vector_database/__init__.py
--rw-r--r--   0        0        0    21946 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/vector_database/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/workflow/__init__.py
--rw-r--r--   0        0        0    43000 2024-04-22 09:45:57.869678 superagent_py-0.2.33/src/superagent/resources/workflow/client.py
--rw-r--r--   0        0        0       65 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/resources/workflow_config/__init__.py
--rw-r--r--   0        0        0     8456 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/resources/workflow_config/client.py
--rw-r--r--   0        0        0     5337 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/__init__.py
--rw-r--r--   0        0        0     1028 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/agent_datasosurce_list.py
--rw-r--r--   0        0        0     1007 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/agent_list.py
--rw-r--r--   0        0        0     1003 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/agent_tool_list.py
--rw-r--r--   0        0        0      708 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/agent_type.py
--rw-r--r--   0        0        0      977 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/api_key_create.py
--rw-r--r--   0        0        0     1435 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/api_key_create_model.py
--rw-r--r--   0        0        0      991 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/api_key_list.py
--rw-r--r--   0        0        0      879 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_api_key.py
--rw-r--r--   0        0        0     1231 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_api_user.py
--rw-r--r--   0        0        0     1436 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_datasource.py
--rw-r--r--   0        0        0     1042 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_llm.py
--rw-r--r--   0        0        0      989 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_vector_db.py
--rw-r--r--   0        0        0      902 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_workflow.py
--rw-r--r--   0        0        0      984 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_request_workflow_step.py
--rw-r--r--   0        0        0      986 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_agent.py
--rw-r--r--   0        0        0      934 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_agent_invoke.py
--rw-r--r--   0        0        0      991 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_api_key.py
--rw-r--r--   0        0        0      995 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_api_user.py
--rw-r--r--   0        0        0     1006 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_datasource.py
--rw-r--r--   0        0        0      978 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_llm.py
--rw-r--r--   0        0        0      982 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_tool.py
--rw-r--r--   0        0        0      999 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_vector_db.py
--rw-r--r--   0        0        0      998 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_workflow.py
--rw-r--r--   0        0        0     1015 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/app_models_response_workflow_step.py
--rw-r--r--   0        0        0     1027 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/datasource_list.py
--rw-r--r--   0        0        0      696 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/datasource_status.py
--rw-r--r--   0        0        0     2649 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/datasource_type.py
--rw-r--r--   0        0        0      560 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/embeddings_model_provider.py
--rw-r--r--   0        0        0     1013 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/function_definition.py
--rw-r--r--   0        0        0      973 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      978 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/llm_list.py
--rw-r--r--   0        0        0     2237 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/llm_model.py
--rw-r--r--   0        0        0      943 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/llm_params.py
--rw-r--r--   0        0        0     1753 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/llm_provider.py
--rw-r--r--   0        0        0     1248 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/open_ai_assistant_parameters.py
--rw-r--r--   0        0        0     1240 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/open_ai_assistant_parameters_tools_item.py
--rw-r--r--   0        0        0     2658 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_agent.py
--rw-r--r--   0        0        0     1560 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_agent_datasource.py
--rw-r--r--   0        0        0     1497 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_agent_llm.py
--rw-r--r--   0        0        0     1506 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_agent_tool.py
--rw-r--r--   0        0        0     1480 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_api_key.py
--rw-r--r--   0        0        0     2497 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_api_user.py
--rw-r--r--   0        0        0     2170 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_datasource.py
--rw-r--r--   0        0        0     1696 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_llm.py
--rw-r--r--   0        0        0     1826 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_tool.py
--rw-r--r--   0        0        0     1687 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_vector_db.py
--rw-r--r--   0        0        0     1814 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_workflow.py
--rw-r--r--   0        0        0     1645 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/prisma_models_workflow_step.py
--rw-r--r--   0        0        0      864 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_code.py
--rw-r--r--   0        0        0      978 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_function.py
--rw-r--r--   0        0        0      869 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_retrieval.py
--rw-r--r--   0        0        0     1003 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/tool_list.py
--rw-r--r--   0        0        0     3767 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/tool_type.py
--rw-r--r--   0        0        0      992 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      999 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/vector_db_list.py
--rw-r--r--   0        0        0     1003 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/vector_db_provider.py
--rw-r--r--   0        0        0     1667 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/workflow_config.py
--rw-r--r--   0        0        0     1019 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/workflow_list.py
--rw-r--r--   0        0        0     1015 2024-04-22 09:45:57.873678 superagent_py-0.2.33/src/superagent/types/workflow_step_list.py
--rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.33/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 06:42:11.711788 superagent_py-0.2.40/LICENSE
+-rw-r--r--   0        0        0     3946 2024-05-23 06:42:11.711788 superagent_py-0.2.40/README.md
+-rw-r--r--   0        0        0      602 2024-05-23 06:42:11.711788 superagent_py-0.2.40/pyproject.toml
+-rw-r--r--   0        0        0     3996 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/__init__.py
+-rw-r--r--   0        0        0     7390 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/client.py
+-rw-r--r--   0        0        0      973 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     2064 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1215 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/core/request_options.py
+-rw-r--r--   0        0        0      166 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/environment.py
+-rw-r--r--   0        0        0      170 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/py.typed
+-rw-r--r--   0        0        0      333 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    88017 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/api_key/__init__.py
+-rw-r--r--   0        0        0    21838 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/api_key/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/api_user/__init__.py
+-rw-r--r--   0        0        0    21588 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/api_user/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/datasource/__init__.py
+-rw-r--r--   0        0        0    30124 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/datasource/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/llm/__init__.py
+-rw-r--r--   0        0        0    22038 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/llm/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/tool/__init__.py
+-rw-r--r--   0        0        0    31320 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/tool/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/vector_database/__init__.py
+-rw-r--r--   0        0        0    27565 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/vector_database/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/workflow/__init__.py
+-rw-r--r--   0        0        0    53161 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/workflow/client.py
+-rw-r--r--   0        0        0       65 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/workflow_config/__init__.py
+-rw-r--r--   0        0        0    10237 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/resources/workflow_config/client.py
+-rw-r--r--   0        0        0     5337 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/agent_datasosurce_list.py
+-rw-r--r--   0        0        0     1244 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/agent_list.py
+-rw-r--r--   0        0        0     1240 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/agent_tool_list.py
+-rw-r--r--   0        0        0      708 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/agent_type.py
+-rw-r--r--   0        0        0     1214 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/api_key_create.py
+-rw-r--r--   0        0        0     1715 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/api_key_create_model.py
+-rw-r--r--   0        0        0     1228 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/api_key_list.py
+-rw-r--r--   0        0        0     1123 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_api_key.py
+-rw-r--r--   0        0        0     1467 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_api_user.py
+-rw-r--r--   0        0        0     1662 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_datasource.py
+-rw-r--r--   0        0        0     1314 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_llm.py
+-rw-r--r--   0        0        0     1233 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_vector_db.py
+-rw-r--r--   0        0        0     1146 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_workflow.py
+-rw-r--r--   0        0        0     1263 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_request_workflow_step.py
+-rw-r--r--   0        0        0     1223 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_agent.py
+-rw-r--r--   0        0        0     1171 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_agent_invoke.py
+-rw-r--r--   0        0        0     1228 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_api_key.py
+-rw-r--r--   0        0        0     1232 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_api_user.py
+-rw-r--r--   0        0        0     1243 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_datasource.py
+-rw-r--r--   0        0        0     1215 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_llm.py
+-rw-r--r--   0        0        0     1219 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_tool.py
+-rw-r--r--   0        0        0     1236 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_vector_db.py
+-rw-r--r--   0        0        0     1235 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_workflow.py
+-rw-r--r--   0        0        0     1252 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/app_models_response_workflow_step.py
+-rw-r--r--   0        0        0     1264 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/datasource_list.py
+-rw-r--r--   0        0        0      696 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/datasource_status.py
+-rw-r--r--   0        0        0     2649 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/datasource_type.py
+-rw-r--r--   0        0        0      560 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/embeddings_model_provider.py
+-rw-r--r--   0        0        0     1236 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/function_definition.py
+-rw-r--r--   0        0        0     1210 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0     1215 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/llm_list.py
+-rw-r--r--   0        0        0     3387 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/llm_model.py
+-rw-r--r--   0        0        0     1173 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/llm_params.py
+-rw-r--r--   0        0        0     1753 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/llm_provider.py
+-rw-r--r--   0        0        0     1499 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/open_ai_assistant_parameters.py
+-rw-r--r--   0        0        0     3450 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/open_ai_assistant_parameters_tools_item.py
+-rw-r--r--   0        0        0     2835 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_agent.py
+-rw-r--r--   0        0        0     1834 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_agent_datasource.py
+-rw-r--r--   0        0        0     1771 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_agent_llm.py
+-rw-r--r--   0        0        0     1780 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_agent_tool.py
+-rw-r--r--   0        0        0     1757 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_api_key.py
+-rw-r--r--   0        0        0     2683 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_api_user.py
+-rw-r--r--   0        0        0     2387 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_datasource.py
+-rw-r--r--   0        0        0     1959 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_llm.py
+-rw-r--r--   0        0        0     2078 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_tool.py
+-rw-r--r--   0        0        0     1947 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_vector_db.py
+-rw-r--r--   0        0        0     2049 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_workflow.py
+-rw-r--r--   0        0        0     1905 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/prisma_models_workflow_step.py
+-rw-r--r--   0        0        0     1108 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_code.py
+-rw-r--r--   0        0        0     1215 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_function.py
+-rw-r--r--   0        0        0     1113 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_retrieval.py
+-rw-r--r--   0        0        0     1240 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/tool_list.py
+-rw-r--r--   0        0        0     3885 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/tool_type.py
+-rw-r--r--   0        0        0     1236 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1236 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/vector_db_list.py
+-rw-r--r--   0        0        0     1003 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/vector_db_provider.py
+-rw-r--r--   0        0        0     1916 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/workflow_config.py
+-rw-r--r--   0        0        0     1256 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/workflow_list.py
+-rw-r--r--   0        0        0     1252 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/types/workflow_step_list.py
+-rw-r--r--   0        0        0       81 2024-05-23 06:42:11.711788 superagent_py-0.2.40/src/superagent/version.py
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.40/PKG-INFO
```

### Comparing `superagent_py-0.2.33/LICENSE` & `superagent_py-0.2.40/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/README.md` & `superagent_py-0.2.40/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/__init__.py` & `superagent_py-0.2.40/src/superagent/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     WorkflowConfig,
     WorkflowList,
     WorkflowStepList,
 )
 from .errors import UnprocessableEntityError
 from .resources import agent, api_key, api_user, datasource, llm, tool, vector_database, workflow, workflow_config
 from .environment import SuperagentEnvironment
+from .version import __version__
 
 __all__ = [
     "AgentDatasosurceList",
     "AgentList",
     "AgentToolList",
     "AgentType",
     "ApiKeyCreate",
@@ -131,14 +132,15 @@
     "ValidationError",
     "ValidationErrorLocItem",
     "VectorDbList",
     "VectorDbProvider",
     "WorkflowConfig",
     "WorkflowList",
     "WorkflowStepList",
+    "__version__",
     "agent",
     "api_key",
     "api_user",
     "datasource",
     "llm",
     "tool",
     "vector_database",
```

### Comparing `superagent_py-0.2.33/src/superagent/client.py` & `superagent_py-0.2.40/src/superagent/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,47 +17,67 @@
 from .resources.workflow_config.client import AsyncWorkflowConfigClient, WorkflowConfigClient
 
 
 class Superagent:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: SuperagentEnvironment. The environment to use for requests from the client. from .environment import SuperagentEnvironment
+    environment : SuperagentEnvironment
+        The environment to use for requests from the client. from .environment import SuperagentEnvironment
 
-                                              Defaults to SuperagentEnvironment.DEFAULT
 
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds.
+        Defaults to SuperagentEnvironment.DEFAULT
 
-        - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+
+    token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.Client]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from superagent.client import Superagent
 
     client = Superagent(
         token="YOUR_TOKEN",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: SuperagentEnvironment = SuperagentEnvironment.DEFAULT,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
+        _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             token=token,
-            httpx_client=httpx.Client(timeout=timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.Client(timeout=_defaulted_timeout),
+            timeout=_defaulted_timeout,
         )
         self.agent = AgentClient(client_wrapper=self._client_wrapper)
         self.llm = LlmClient(client_wrapper=self._client_wrapper)
         self.api_user = ApiUserClient(client_wrapper=self._client_wrapper)
         self.api_key = ApiKeyClient(client_wrapper=self._client_wrapper)
         self.datasource = DatasourceClient(client_wrapper=self._client_wrapper)
         self.tool = ToolClient(client_wrapper=self._client_wrapper)
@@ -66,47 +86,67 @@
         self.vector_database = VectorDatabaseClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncSuperagent:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
+
+    environment : SuperagentEnvironment
+        The environment to use for requests from the client. from .environment import SuperagentEnvironment
+
+
+
+        Defaults to SuperagentEnvironment.DEFAULT
+
 
-        - environment: SuperagentEnvironment. The environment to use for requests from the client. from .environment import SuperagentEnvironment
 
-                                              Defaults to SuperagentEnvironment.DEFAULT
+    token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds.
+    httpx_client : typing.Optional[httpx.AsyncClient]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
-        - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+    Examples
+    --------
     from superagent.client import AsyncSuperagent
 
     client = AsyncSuperagent(
         token="YOUR_TOKEN",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: SuperagentEnvironment = SuperagentEnvironment.DEFAULT,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
-        timeout: typing.Optional[float] = 60,
+        timeout: typing.Optional[float] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
+        _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
             token=token,
-            httpx_client=httpx.AsyncClient(timeout=timeout) if httpx_client is None else httpx_client,
+            httpx_client=httpx_client
+            if httpx_client is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
+            if follow_redirects is not None
+            else httpx.AsyncClient(timeout=_defaulted_timeout),
+            timeout=_defaulted_timeout,
         )
         self.agent = AsyncAgentClient(client_wrapper=self._client_wrapper)
         self.llm = AsyncLlmClient(client_wrapper=self._client_wrapper)
         self.api_user = AsyncApiUserClient(client_wrapper=self._client_wrapper)
         self.api_key = AsyncApiKeyClient(client_wrapper=self._client_wrapper)
         self.datasource = AsyncDatasourceClient(client_wrapper=self._client_wrapper)
         self.tool = AsyncToolClient(client_wrapper=self._client_wrapper)
```

### Comparing `superagent_py-0.2.33/src/superagent/core/__init__.py` & `superagent_py-0.2.40/src/superagent/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
+from .pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .query_encoder import encode_query
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "AsyncHttpClient",
     "BaseClientWrapper",
     "File",
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
     "convert_file_dict_to_httpx_tuples",
+    "deep_union_pydantic_dicts",
+    "encode_query",
     "jsonable_encoder",
+    "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `superagent_py-0.2.33/src/superagent/core/client_wrapper.py` & `superagent_py-0.2.40/src/superagent/core/client_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 
 import httpx
 
 from .http_client import AsyncHttpClient, HttpClient
 
 
 class BaseClientWrapper:
-    def __init__(self, *, token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None, base_url: str):
+    def __init__(
+        self,
+        *,
+        token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
+        base_url: str,
+        timeout: typing.Optional[float] = None,
+    ):
         self._token = token
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "superagent-py",
-            "X-Fern-SDK-Version": "v0.2.33",
+            "X-Fern-SDK-Version": "v0.2.40",
         }
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
 
     def _get_token(self) -> typing.Optional[str]:
@@ -28,30 +35,35 @@
             return self._token
         else:
             return self._token()
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         base_url: str,
+        timeout: typing.Optional[float] = None,
         httpx_client: httpx.Client,
     ):
-        super().__init__(token=token, base_url=base_url)
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
         self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         base_url: str,
+        timeout: typing.Optional[float] = None,
         httpx_client: httpx.AsyncClient,
     ):
-        super().__init__(token=token, base_url=base_url)
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
         self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `superagent_py-0.2.33/src/superagent/core/datetime_utils.py` & `superagent_py-0.2.40/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/core/file.py` & `superagent_py-0.2.40/src/superagent/core/file.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/core/http_client.py` & `superagent_py-0.2.40/src/superagent/core/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import asyncio
 import email.utils
 import re
 import time
 import typing
+from contextlib import asynccontextmanager, contextmanager
 from functools import wraps
 from random import random
 
 import httpx
 
 INITIAL_RETRY_DELAY_SECONDS = 0.5
 MAX_RETRY_DELAY_SECONDS = 10
@@ -94,16 +95,18 @@
         if _should_retry(response=response):
             if max_retries > retries:
                 time.sleep(_retry_timeout(response=response, retries=retries))
                 return self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
     @wraps(httpx.Client.stream)
+    @contextmanager
     def stream(self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
 
 
 class AsyncHttpClient:
     def __init__(self, *, httpx_client: httpx.AsyncClient):
         self.httpx_client = httpx_client
 
     # Ensure that the signature of the `request` method is the same as the `httpx.Client.request` method
@@ -114,12 +117,14 @@
         response = await self.httpx_client.request(*args, **kwargs)
         if _should_retry(response=response):
             if max_retries > retries:
                 await asyncio.sleep(_retry_timeout(response=response, retries=retries))
                 return await self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
-    @wraps(httpx.AsyncClient.request)
+    @wraps(httpx.AsyncClient.stream)
+    @asynccontextmanager
     async def stream(
         self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any
     ) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        async with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
```

### Comparing `superagent_py-0.2.33/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.2.40/src/superagent/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `superagent_py-0.2.33/src/superagent/core/request_options.py` & `superagent_py-0.2.40/src/superagent/core/request_options.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/resources/agent/client.py` & `superagent_py-0.2.40/src/superagent/resources/agent/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.agent_datasosurce_list import AgentDatasosurceList
 from ...types.agent_list import AgentList
 from ...types.agent_tool_list import AgentToolList
 from ...types.agent_type import AgentType
 from ...types.app_models_response_agent import AppModelsResponseAgent
 from ...types.app_models_response_agent_invoke import AppModelsResponseAgentInvoke
 from ...types.http_validation_error import HttpValidationError
 from ...types.llm_params import LlmParams
 from ...types.llm_provider import LlmProvider
 from ...types.open_ai_assistant_parameters import OpenAiAssistantParameters
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AgentClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -40,66 +37,89 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AgentList:
         """
         List all agents
 
-        Parameters:
-            - skip: typing.Optional[int].
-
-            - take: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
-        is_active: typing.Optional[bool] = OMIT,
         name: str,
+        is_active: typing.Optional[bool] = OMIT,
         initial_message: typing.Optional[str] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         llm_model: typing.Optional[str] = OMIT,
         llm_provider: typing.Optional[LlmProvider] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[AgentType] = OMIT,
@@ -107,40 +127,79 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Create a new agent
 
-        Parameters:
-            - is_active: typing.Optional[bool].
+        Parameters
+        ----------
+        name : str
 
-            - name: str.
+        is_active : typing.Optional[bool]
 
-            - initial_message: typing.Optional[str].
+        initial_message : typing.Optional[str]
 
-            - prompt: typing.Optional[str].
+        prompt : typing.Optional[str]
 
-            - llm_model: typing.Optional[str].
+        llm_model : typing.Optional[str]
 
-            - llm_provider: typing.Optional[LlmProvider].
+        llm_provider : typing.Optional[LlmProvider]
 
-            - description: typing.Optional[str].
+        description : typing.Optional[str]
 
-            - avatar: typing.Optional[str].
+        avatar : typing.Optional[str]
 
-            - type: typing.Optional[AgentType].
+        type : typing.Optional[AgentType]
 
-            - parameters: typing.Optional[OpenAiAssistantParameters].
+        parameters : typing.Optional[OpenAiAssistantParameters]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - output_schema: typing.Optional[str].
+        output_schema : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent import (
+            AgentType,
+            LlmProvider,
+            OpenAiAssistantParameters,
+            OpenAiAssistantParametersToolsItem_CodeInterpreter,
+        )
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.create(
+            is_active=True,
+            name="string",
+            initial_message="string",
+            prompt="string",
+            llm_model="string",
+            llm_provider=LlmProvider.OPENAI,
+            description="string",
+            avatar="string",
+            type=AgentType.SUPERAGENT,
+            parameters=OpenAiAssistantParameters(
+                metadata={"string": {"key": "value"}},
+                file_ids=["string"],
+                tools=[OpenAiAssistantParametersToolsItem_CodeInterpreter()],
+            ),
+            metadata={"string": {"key": "value"}},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if initial_message is not OMIT:
             _request["initialMessage"] = initial_message
         if prompt is not OMIT:
@@ -158,18 +217,20 @@
         if parameters is not OMIT:
             _request["parameters"] = parameters
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -179,104 +240,150 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseAgent:
         """
         Get a single agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.get(
+            agent_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.delete(
+            agent_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -294,38 +401,66 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Patch an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        is_active : typing.Optional[bool]
+
+        name : typing.Optional[str]
+
+        initial_message : typing.Optional[str]
 
-            - is_active: typing.Optional[bool].
+        prompt : typing.Optional[str]
 
-            - name: typing.Optional[str].
+        llm_model : typing.Optional[str]
 
-            - initial_message: typing.Optional[str].
+        description : typing.Optional[str]
 
-            - prompt: typing.Optional[str].
+        avatar : typing.Optional[str]
 
-            - llm_model: typing.Optional[str].
+        type : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - avatar: typing.Optional[str].
+        output_schema : typing.Optional[str]
 
-            - type: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
 
-            - output_schema: typing.Optional[str].
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.update(
+            agent_id="string",
+            is_active=True,
+            name="string",
+            initial_message="string",
+            prompt="string",
+            llm_model="string",
+            description="string",
+            avatar="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if name is not OMIT:
             _request["name"] = name
         if initial_message is not OMIT:
@@ -341,20 +476,22 @@
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -364,71 +501,102 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def invoke(
         self,
         agent_id: str,
         *,
         input: str,
-        session_id: typing.Optional[str] = OMIT,
         enable_streaming: bool,
+        session_id: typing.Optional[str] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         llm_params: typing.Optional[LlmParams] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgentInvoke:
         """
         Invoke an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        input : str
+
+        enable_streaming : bool
+
+        session_id : typing.Optional[str]
 
-            - input: str.
+        output_schema : typing.Optional[str]
 
-            - session_id: typing.Optional[str].
+        llm_params : typing.Optional[LlmParams]
 
-            - enable_streaming: bool.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - output_schema: typing.Optional[str].
+        Returns
+        -------
+        AppModelsResponseAgentInvoke
+            Successful Response
 
-            - llm_params: typing.Optional[LlmParams].
+        Examples
+        --------
+        from superagent import LlmParams
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.invoke(
+            agent_id="string",
+            input="string",
+            session_id="string",
+            enable_streaming=True,
+            output_schema="string",
+            llm_params=LlmParams(
+                max_tokens=1,
+                temperature=1.1,
+            ),
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         if llm_params is not OMIT:
             _request["llm_params"] = llm_params
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -438,48 +606,71 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgentInvoke, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgentInvoke, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_llm(
         self, agent_id: str, *, llm_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add LLM to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - llm_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        llm_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.add_llm(
+            agent_id="string",
+            llm_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/llms"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"llmId": llm_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"llmId": llm_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -489,135 +680,203 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def remove_llm(
         self, agent_id: str, llm_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove LLM from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - llm_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        llm_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.remove_llm(
+            agent_id="string",
+            llm_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/llms/{jsonable_encoder(llm_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_tools(self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AgentToolList:
         """
         List agent tools
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentToolList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.list_tools(
+            agent_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/tools"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentToolList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentToolList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_tool(
         self, agent_id: str, *, tool_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add tool to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - tool_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.add_tool(
+            agent_id="string",
+            tool_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/tools"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"toolId": tool_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"toolId": tool_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -627,137 +886,205 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def remove_tool(
         self, agent_id: str, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove tool from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - tool_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.remove_tool(
+            agent_id="string",
+            tool_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/tools/{jsonable_encoder(tool_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_datasources(
         self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AgentDatasosurceList:
         """
         List agent datasources
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentDatasosurceList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.list_datasources(
+            agent_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentDatasosurceList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentDatasosurceList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_datasource(
         self, agent_id: str, *, datasource_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add datasource to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - datasource_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        datasource_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.add_datasource(
+            agent_id="string",
+            datasource_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"datasourceId": datasource_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"datasourceId": datasource_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -767,68 +1094,93 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def remove_datasource(
         self, agent_id: str, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove datasource from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - datasource_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        datasource_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.agent.remove_datasource(
+            agent_id="string",
+            datasource_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources/{jsonable_encoder(datasource_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -842,66 +1194,89 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AgentList:
         """
         List all agents
 
-        Parameters:
-            - skip: typing.Optional[int].
-
-            - take: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
-        is_active: typing.Optional[bool] = OMIT,
         name: str,
+        is_active: typing.Optional[bool] = OMIT,
         initial_message: typing.Optional[str] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         llm_model: typing.Optional[str] = OMIT,
         llm_provider: typing.Optional[LlmProvider] = OMIT,
         description: typing.Optional[str] = OMIT,
         avatar: typing.Optional[str] = OMIT,
         type: typing.Optional[AgentType] = OMIT,
@@ -909,40 +1284,79 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Create a new agent
 
-        Parameters:
-            - is_active: typing.Optional[bool].
+        Parameters
+        ----------
+        name : str
+
+        is_active : typing.Optional[bool]
 
-            - name: str.
+        initial_message : typing.Optional[str]
 
-            - initial_message: typing.Optional[str].
+        prompt : typing.Optional[str]
 
-            - prompt: typing.Optional[str].
+        llm_model : typing.Optional[str]
 
-            - llm_model: typing.Optional[str].
+        llm_provider : typing.Optional[LlmProvider]
 
-            - llm_provider: typing.Optional[LlmProvider].
+        description : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        avatar : typing.Optional[str]
 
-            - avatar: typing.Optional[str].
+        type : typing.Optional[AgentType]
 
-            - type: typing.Optional[AgentType].
+        parameters : typing.Optional[OpenAiAssistantParameters]
 
-            - parameters: typing.Optional[OpenAiAssistantParameters].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        output_schema : typing.Optional[str]
 
-            - output_schema: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent import (
+            AgentType,
+            LlmProvider,
+            OpenAiAssistantParameters,
+            OpenAiAssistantParametersToolsItem_CodeInterpreter,
+        )
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.create(
+            is_active=True,
+            name="string",
+            initial_message="string",
+            prompt="string",
+            llm_model="string",
+            llm_provider=LlmProvider.OPENAI,
+            description="string",
+            avatar="string",
+            type=AgentType.SUPERAGENT,
+            parameters=OpenAiAssistantParameters(
+                metadata={"string": {"key": "value"}},
+                file_ids=["string"],
+                tools=[OpenAiAssistantParametersToolsItem_CodeInterpreter()],
+            ),
+            metadata={"string": {"key": "value"}},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if initial_message is not OMIT:
             _request["initialMessage"] = initial_message
         if prompt is not OMIT:
@@ -960,18 +1374,20 @@
         if parameters is not OMIT:
             _request["parameters"] = parameters
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/agents"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -981,106 +1397,152 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Get a single agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.get(
+            agent_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.delete(
+            agent_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -1098,38 +1560,66 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgent:
         """
         Patch an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
 
-            - is_active: typing.Optional[bool].
+        is_active : typing.Optional[bool]
 
-            - name: typing.Optional[str].
+        name : typing.Optional[str]
 
-            - initial_message: typing.Optional[str].
+        initial_message : typing.Optional[str]
 
-            - prompt: typing.Optional[str].
+        prompt : typing.Optional[str]
 
-            - llm_model: typing.Optional[str].
+        llm_model : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        description : typing.Optional[str]
 
-            - avatar: typing.Optional[str].
+        avatar : typing.Optional[str]
 
-            - type: typing.Optional[str].
+        type : typing.Optional[str]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - output_schema: typing.Optional[str].
+        output_schema : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.update(
+            agent_id="string",
+            is_active=True,
+            name="string",
+            initial_message="string",
+            prompt="string",
+            llm_model="string",
+            description="string",
+            avatar="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if is_active is not OMIT:
             _request["isActive"] = is_active
         if name is not OMIT:
             _request["name"] = name
         if initial_message is not OMIT:
@@ -1145,20 +1635,22 @@
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1168,71 +1660,102 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def invoke(
         self,
         agent_id: str,
         *,
         input: str,
-        session_id: typing.Optional[str] = OMIT,
         enable_streaming: bool,
+        session_id: typing.Optional[str] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         llm_params: typing.Optional[LlmParams] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseAgentInvoke:
         """
         Invoke an agent
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
 
-            - input: str.
+        input : str
 
-            - session_id: typing.Optional[str].
+        enable_streaming : bool
 
-            - enable_streaming: bool.
+        session_id : typing.Optional[str]
 
-            - output_schema: typing.Optional[str].
+        output_schema : typing.Optional[str]
 
-            - llm_params: typing.Optional[LlmParams].
+        llm_params : typing.Optional[LlmParams]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgentInvoke
+            Successful Response
+
+        Examples
+        --------
+        from superagent import LlmParams
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.invoke(
+            agent_id="string",
+            input="string",
+            session_id="string",
+            enable_streaming=True,
+            output_schema="string",
+            llm_params=LlmParams(
+                max_tokens=1,
+                temperature=1.1,
+            ),
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         if llm_params is not OMIT:
             _request["llm_params"] = llm_params
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1242,48 +1765,71 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgentInvoke, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgentInvoke, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_llm(
         self, agent_id: str, *, llm_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add LLM to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - llm_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        llm_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.add_llm(
+            agent_id="string",
+            llm_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/llms"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"llmId": llm_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"llmId": llm_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1293,137 +1839,205 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def remove_llm(
         self, agent_id: str, llm_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove LLM from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - llm_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        llm_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.remove_llm(
+            agent_id="string",
+            llm_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/llms/{jsonable_encoder(llm_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_tools(
         self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AgentToolList:
         """
         List agent tools
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentToolList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.list_tools(
+            agent_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/tools"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentToolList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentToolList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_tool(
         self, agent_id: str, *, tool_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add tool to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - tool_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.add_tool(
+            agent_id="string",
+            tool_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/tools"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"toolId": tool_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"toolId": tool_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1433,137 +2047,205 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def remove_tool(
         self, agent_id: str, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove tool from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - tool_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.remove_tool(
+            agent_id="string",
+            tool_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/tools/{jsonable_encoder(tool_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_datasources(
         self, agent_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AgentDatasosurceList:
         """
         List agent datasources
 
-        Parameters:
-            - agent_id: str.
+        Parameters
+        ----------
+        agent_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AgentDatasosurceList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.list_datasources(
+            agent_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AgentDatasosurceList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AgentDatasosurceList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_datasource(
         self, agent_id: str, *, datasource_id: str, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseAgent:
         """
         Add datasource to agent
 
-        Parameters:
-            - agent_id: str.
-
-            - datasource_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        datasource_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseAgent
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.add_datasource(
+            agent_id="string",
+            datasource_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"datasourceId": datasource_id})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"datasourceId": datasource_id}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1573,66 +2255,91 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseAgent, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def remove_datasource(
         self, agent_id: str, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Remove datasource from agent
 
-        Parameters:
-            - agent_id: str.
-
-            - datasource_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        agent_id : str
+
+        datasource_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.agent.remove_datasource(
+            agent_id="string",
+            datasource_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/agents/{jsonable_encoder(agent_id)}/datasources/{jsonable_encoder(datasource_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/api_key/client.py` & `superagent_py-0.2.40/src/superagent/resources/api_key/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,87 +3,125 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.api_key_create import ApiKeyCreate
 from ...types.api_key_list import ApiKeyList
 from ...types.app_models_request_api_key import AppModelsRequestApiKey
 from ...types.app_models_response_api_key import AppModelsResponseApiKey
 from ...types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ApiKeyClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ApiKeyList:
         """
         List API keys
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ApiKeyList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_key.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ApiKeyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self, *, request: AppModelsRequestApiKey, request_options: typing.Optional[RequestOptions] = None
     ) -> ApiKeyCreate:
         """
         Create a new API key
 
-        Parameters:
-            - request: AppModelsRequestApiKey.
+        Parameters
+        ----------
+        request : AppModelsRequestApiKey
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ApiKeyCreate
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiKey
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_key.create(
+            request=AppModelsRequestApiKey(
+                name="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -93,85 +131,137 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyCreate, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ApiKeyCreate, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseApiKey:
         """
         Delete an API key
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiKey
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_key.delete(
+            id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self, id: str, *, request: AppModelsRequestApiKey, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseApiKey:
         """
         Update an API key
 
-        Parameters:
-            - id: str.
-
-            - request: AppModelsRequestApiKey.
+        Parameters
+        ----------
+        id : str
+
+        request : AppModelsRequestApiKey
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiKey
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiKey
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_key.update(
+            id="string",
+            request=AppModelsRequestApiKey(
+                name="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -181,22 +271,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -204,61 +296,102 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ApiKeyList:
         """
         List API keys
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ApiKeyList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_key.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ApiKeyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self, *, request: AppModelsRequestApiKey, request_options: typing.Optional[RequestOptions] = None
     ) -> ApiKeyCreate:
         """
         Create a new API key
 
-        Parameters:
-            - request: AppModelsRequestApiKey.
+        Parameters
+        ----------
+        request : AppModelsRequestApiKey
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ApiKeyCreate
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiKey
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_key.create(
+            request=AppModelsRequestApiKey(
+                name="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-keys"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -268,87 +401,139 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyCreate, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ApiKeyCreate, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseApiKey:
         """
         Delete an API key
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiKey
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_key.delete(
+            id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self, id: str, *, request: AppModelsRequestApiKey, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseApiKey:
         """
         Update an API key
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request : AppModelsRequestApiKey
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiKey
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiKey
+        from superagent.client import AsyncSuperagent
 
-            - request: AppModelsRequestApiKey.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_key.update(
+            id="string",
+            request=AppModelsRequestApiKey(
+                name="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/api-keys/{jsonable_encoder(id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -358,20 +543,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiKey, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/api_user/client.py` & `superagent_py-0.2.40/src/superagent/resources/api_user/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,50 +3,74 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.app_models_request_api_user import AppModelsRequestApiUser
 from ...types.app_models_response_api_user import AppModelsResponseApiUser
 from ...types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ApiUserClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self, *, request: AppModelsRequestApiUser, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseApiUser:
         """
         Create a new API user
 
-        Parameters:
-            - request: AppModelsRequestApiUser.
+        Parameters
+        ----------
+        request : AppModelsRequestApiUser
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiUser
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiUser
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_user.create(
+            request=AppModelsRequestApiUser(
+                email="string",
+                first_name="string",
+                last_name="string",
+                company="string",
+                anonymous_id="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -56,114 +80,179 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseApiUser:
         """
         Get a single api user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiUser
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_user.get()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete an api user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_user.delete()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def indentify(
         self, *, request: AppModelsRequestApiUser, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Indentify an api user
 
-        Parameters:
-            - request: AppModelsRequestApiUser.
+        Parameters
+        ----------
+        request : AppModelsRequestApiUser
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiUser
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.api_user.indentify(
+            request=AppModelsRequestApiUser(
+                email="string",
+                first_name="string",
+                last_name="string",
+                company="string",
+                anonymous_id="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/identify"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/identify"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -173,22 +262,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -198,24 +289,51 @@
 
     async def create(
         self, *, request: AppModelsRequestApiUser, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseApiUser:
         """
         Create a new API user
 
-        Parameters:
-            - request: AppModelsRequestApiUser.
+        Parameters
+        ----------
+        request : AppModelsRequestApiUser
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiUser
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiUser
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_user.create(
+            request=AppModelsRequestApiUser(
+                email="string",
+                first_name="string",
+                last_name="string",
+                company="string",
+                anonymous_id="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -225,114 +343,179 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseApiUser:
         """
         Get a single api user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseApiUser
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_user.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseApiUser, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete an api user
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_user.delete()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/me"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def indentify(
         self, *, request: AppModelsRequestApiUser, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Indentify an api user
 
-        Parameters:
-            - request: AppModelsRequestApiUser.
+        Parameters
+        ----------
+        request : AppModelsRequestApiUser
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestApiUser
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.api_user.indentify(
+            request=AppModelsRequestApiUser(
+                email="string",
+                first_name="string",
+                last_name="string",
+                company="string",
+                anonymous_id="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/identify"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/api-users/identify"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -342,20 +525,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/datasource/client.py` & `superagent_py-0.2.40/src/superagent/resources/llm/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,108 +3,126 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.app_models_request_datasource import AppModelsRequestDatasource
-from ...types.app_models_response_datasource import AppModelsResponseDatasource
-from ...types.datasource_list import DatasourceList
+from ...types.app_models_request_llm import AppModelsRequestLlm
+from ...types.app_models_response_llm import AppModelsResponseLlm
 from ...types.http_validation_error import HttpValidationError
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...types.llm_list import LlmList
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class DatasourceClient:
+class LlmClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
-        self,
-        *,
-        skip: typing.Optional[int] = None,
-        take: typing.Optional[int] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> DatasourceList:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> LlmList:
         """
-        List all datasources
-
-        Parameters:
-            - skip: typing.Optional[int].
+        List all LLMs
 
-            - take: typing.Optional[int].
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        LlmList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.llm.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/datasources"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/llms"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DatasourceList, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(LlmList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
-        self, *, request: AppModelsRequestDatasource, request_options: typing.Optional[RequestOptions] = None
-    ) -> AppModelsResponseDatasource:
+        self, *, request: AppModelsRequestLlm, request_options: typing.Optional[RequestOptions] = None
+    ) -> AppModelsResponseLlm:
         """
-        Create a new datasource
+        Create a new LLM
 
-        Parameters:
-            - request: AppModelsRequestDatasource.
+        Parameters
+        ----------
+        request : AppModelsRequestLlm
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestLlm
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.llm.create(
+            request=AppModelsRequestLlm(
+                provider="string",
+                api_key="string",
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/datasources"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/llms"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -114,136 +132,139 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(
-        self, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> AppModelsResponseDatasource:
+    def get(self, llm_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseLlm:
         """
-        Get a specific datasource
+        Get a single LLM
 
-        Parameters:
-            - datasource_id: str.
+        Parameters
+        ----------
+        llm_id : str
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-    def delete(self, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
-        """
-        Delete a specific datasource
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
 
-        Parameters:
-            - datasource_id: str.
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.llm.get(
+            llm_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/llms/{jsonable_encoder(llm_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
-        self,
-        datasource_id: str,
-        *,
-        request: AppModelsRequestDatasource,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> AppModelsResponseDatasource:
+        self, llm_id: str, *, request: AppModelsRequestLlm, request_options: typing.Optional[RequestOptions] = None
+    ) -> AppModelsResponseLlm:
         """
-        Update a specific datasource
+        Patch an LLM
+
+        Parameters
+        ----------
+        llm_id : str
+
+        request : AppModelsRequestLlm
 
-        Parameters:
-            - datasource_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request: AppModelsRequestDatasource.
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Examples
+        --------
+        from superagent import AppModelsRequestLlm
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.llm.update(
+            llm_id="string",
+            request=AppModelsRequestLlm(
+                provider="string",
+                api_key="string",
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/llms/{jsonable_encoder(llm_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -253,106 +274,129 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncDatasourceClient:
+class AsyncLlmClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
-        self,
-        *,
-        skip: typing.Optional[int] = None,
-        take: typing.Optional[int] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> DatasourceList:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> LlmList:
         """
-        List all datasources
+        List all LLMs
 
-        Parameters:
-            - skip: typing.Optional[int].
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        LlmList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - take: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.llm.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/datasources"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/llms"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DatasourceList, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(LlmList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
-        self, *, request: AppModelsRequestDatasource, request_options: typing.Optional[RequestOptions] = None
-    ) -> AppModelsResponseDatasource:
+        self, *, request: AppModelsRequestLlm, request_options: typing.Optional[RequestOptions] = None
+    ) -> AppModelsResponseLlm:
         """
-        Create a new datasource
+        Create a new LLM
 
-        Parameters:
-            - request: AppModelsRequestDatasource.
+        Parameters
+        ----------
+        request : AppModelsRequestLlm
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestLlm
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.llm.create(
+            request=AppModelsRequestLlm(
+                provider="string",
+                api_key="string",
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/datasources"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/llms"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -362,138 +406,141 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
-        self, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> AppModelsResponseDatasource:
+        self, llm_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> AppModelsResponseLlm:
         """
-        Get a specific datasource
+        Get a single LLM
 
-        Parameters:
-            - datasource_id: str.
+        Parameters
+        ----------
+        llm_id : str
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-    async def delete(
-        self, datasource_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
-        """
-        Delete a specific datasource
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
 
-        Parameters:
-            - datasource_id: str.
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.llm.get(
+            llm_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/llms/{jsonable_encoder(llm_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
-        self,
-        datasource_id: str,
-        *,
-        request: AppModelsRequestDatasource,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> AppModelsResponseDatasource:
+        self, llm_id: str, *, request: AppModelsRequestLlm, request_options: typing.Optional[RequestOptions] = None
+    ) -> AppModelsResponseLlm:
         """
-        Update a specific datasource
+        Patch an LLM
+
+        Parameters
+        ----------
+        llm_id : str
+
+        request : AppModelsRequestLlm
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - datasource_id: str.
+        Returns
+        -------
+        AppModelsResponseLlm
+            Successful Response
 
-            - request: AppModelsRequestDatasource.
+        Examples
+        --------
+        from superagent import AppModelsRequestLlm
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.llm.update(
+            llm_id="string",
+            request=AppModelsRequestLlm(
+                provider="string",
+                api_key="string",
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/v1/datasources/{jsonable_encoder(datasource_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/v1/llms/{jsonable_encoder(llm_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -503,20 +550,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseDatasource, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseLlm, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/tool/client.py` & `superagent_py-0.2.40/src/superagent/resources/tool/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.app_models_response_tool import AppModelsResponseTool
 from ...types.http_validation_error import HttpValidationError
 from ...types.tool_list import ToolList
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ToolClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -33,99 +30,146 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ToolList:
         """
         List all tools
 
-        Parameters:
-            - skip: typing.Optional[int].
-
-            - take: typing.Optional[int].
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ToolList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.tool.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ToolList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ToolList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         name: str,
-        description: typing.Optional[str] = OMIT,
         type: str,
+        description: typing.Optional[str] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         return_direct: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseTool:
         """
         Create a new tool
 
-        Parameters:
-            - name: str.
+        Parameters
+        ----------
+        name : str
+
+        type : str
+
+        description : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - type: str.
+        return_direct : typing.Optional[bool]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - return_direct: typing.Optional[bool].
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.tool.create(
+            name="string",
+            description="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            return_direct=True,
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if description is not OMIT:
             _request["description"] = description
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if return_direct is not OMIT:
             _request["returnDirect"] = return_direct
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -135,104 +179,150 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AppModelsResponseTool:
         """
         Get a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.tool.get(
+            tool_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.tool.delete(
+            tool_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -245,47 +335,72 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         return_direct: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseTool:
         """
         Update a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
 
-            - name: typing.Optional[str].
+        name : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        description : typing.Optional[str]
 
-            - type: typing.Optional[str].
+        type : typing.Optional[str]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - return_direct: typing.Optional[bool].
+        return_direct : typing.Optional[bool]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.tool.update(
+            tool_id="string",
+            name="string",
+            description="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            return_direct=True,
+        )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if description is not OMIT:
             _request["description"] = description
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if return_direct is not OMIT:
             _request["returnDirect"] = return_direct
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -295,22 +410,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -324,99 +441,146 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ToolList:
         """
         List all tools
 
-        Parameters:
-            - skip: typing.Optional[int].
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ToolList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - take: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.tool.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ToolList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ToolList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         name: str,
-        description: typing.Optional[str] = OMIT,
         type: str,
+        description: typing.Optional[str] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         return_direct: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseTool:
         """
         Create a new tool
 
-        Parameters:
-            - name: str.
+        Parameters
+        ----------
+        name : str
+
+        type : str
+
+        description : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - type: str.
+        return_direct : typing.Optional[bool]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - return_direct: typing.Optional[bool].
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.tool.create(
+            name="string",
+            description="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            return_direct=True,
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if description is not OMIT:
             _request["description"] = description
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if return_direct is not OMIT:
             _request["returnDirect"] = return_direct
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/tools"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -426,106 +590,152 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseTool:
         """
         Get a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.tool.get(
+            tool_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, tool_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.tool.delete(
+            tool_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -538,47 +748,72 @@
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         return_direct: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseTool:
         """
         Update a specific tool
 
-        Parameters:
-            - tool_id: str.
+        Parameters
+        ----------
+        tool_id : str
 
-            - name: typing.Optional[str].
+        name : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        description : typing.Optional[str]
 
-            - type: typing.Optional[str].
+        type : typing.Optional[str]
 
-            - metadata: typing.Optional[typing.Dict[str, typing.Any]].
+        metadata : typing.Optional[typing.Dict[str, typing.Any]]
 
-            - return_direct: typing.Optional[bool].
+        return_direct : typing.Optional[bool]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseTool
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.tool.update(
+            tool_id="string",
+            name="string",
+            description="string",
+            type="string",
+            metadata={"string": {"key": "value"}},
+            return_direct=True,
+        )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if description is not OMIT:
             _request["description"] = description
         if type is not OMIT:
             _request["type"] = type
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if return_direct is not OMIT:
             _request["returnDirect"] = return_direct
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/tools/{jsonable_encoder(tool_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -588,20 +823,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseTool, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/vector_database/client.py` & `superagent_py-0.2.40/src/superagent/resources/vector_database/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,51 +3,72 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.app_models_request_vector_db import AppModelsRequestVectorDb
 from ...types.app_models_response_vector_db import AppModelsResponseVectorDb
 from ...types.http_validation_error import HttpValidationError
 from ...types.vector_db_list import VectorDbList
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class VectorDatabaseClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self, *, request: AppModelsRequestVectorDb, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseVectorDb:
         """
         Create a new Vector Database
 
-        Parameters:
-            - request: AppModelsRequestVectorDb.
+        Parameters
+        ----------
+        request : AppModelsRequestVectorDb
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestVectorDb, VectorDbProvider
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.vector_database.create(
+            request=AppModelsRequestVectorDb(
+                provider=VectorDbProvider.PINECONE,
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-db"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-db"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -57,141 +78,205 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> VectorDbList:
         """
         List all Vector Databases
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VectorDbList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.vector_database.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-dbs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-dbs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VectorDbList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(VectorDbList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
         self, vector_db_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseVectorDb:
         """
         Get a single Vector Database
 
-        Parameters:
-            - vector_db_id: str.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.vector_database.get(
+            vector_db_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, vector_db_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a Vector Database
 
-        Parameters:
-            - vector_db_id: str.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.vector_database.delete(
+            vector_db_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -200,28 +285,53 @@
         *,
         request: AppModelsRequestVectorDb,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseVectorDb:
         """
         Patch a Vector Database
 
-        Parameters:
-            - vector_db_id: str.
-
-            - request: AppModelsRequestVectorDb.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request : AppModelsRequestVectorDb
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestVectorDb, VectorDbProvider
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.vector_database.update(
+            vector_db_id="string",
+            request=AppModelsRequestVectorDb(
+                provider=VectorDbProvider.PINECONE,
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -231,22 +341,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -256,24 +368,48 @@
 
     async def create(
         self, *, request: AppModelsRequestVectorDb, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseVectorDb:
         """
         Create a new Vector Database
 
-        Parameters:
-            - request: AppModelsRequestVectorDb.
+        Parameters
+        ----------
+        request : AppModelsRequestVectorDb
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestVectorDb, VectorDbProvider
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.vector_database.create(
+            request=AppModelsRequestVectorDb(
+                provider=VectorDbProvider.PINECONE,
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-db"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-db"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -283,141 +419,205 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> VectorDbList:
         """
         List all Vector Databases
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        VectorDbList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.vector_database.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-dbs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/vector-dbs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(VectorDbList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(VectorDbList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, vector_db_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseVectorDb:
         """
         Get a single Vector Database
 
-        Parameters:
-            - vector_db_id: str.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.vector_database.get(
+            vector_db_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, vector_db_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a Vector Database
 
-        Parameters:
-            - vector_db_id: str.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.vector_database.delete(
+            vector_db_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -426,28 +626,53 @@
         *,
         request: AppModelsRequestVectorDb,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseVectorDb:
         """
         Patch a Vector Database
 
-        Parameters:
-            - vector_db_id: str.
-
-            - request: AppModelsRequestVectorDb.
+        Parameters
+        ----------
+        vector_db_id : str
+
+        request : AppModelsRequestVectorDb
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseVectorDb
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestVectorDb, VectorDbProvider
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.vector_database.update(
+            vector_db_id="string",
+            request=AppModelsRequestVectorDb(
+                provider=VectorDbProvider.PINECONE,
+                options={"string": {"key": "value"}},
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/vector-dbs/{jsonable_encoder(vector_db_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -457,20 +682,22 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseVectorDb, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/workflow/client.py` & `superagent_py-0.2.40/src/superagent/resources/workflow/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.app_models_request_workflow import AppModelsRequestWorkflow
 from ...types.app_models_request_workflow_step import AppModelsRequestWorkflowStep
 from ...types.app_models_response_workflow import AppModelsResponseWorkflow
 from ...types.app_models_response_workflow_step import AppModelsResponseWorkflowStep
 from ...types.http_validation_error import HttpValidationError
 from ...types.workflow_list import WorkflowList
 from ...types.workflow_step_list import WorkflowStepList
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class WorkflowClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
@@ -37,77 +34,124 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WorkflowList:
         """
         List all workflows
 
-        Parameters:
-            - skip: typing.Optional[int].
-
-            - take: typing.Optional[int].
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        WorkflowList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WorkflowList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self, *, request: AppModelsRequestWorkflow, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseWorkflow:
         """
         Create a new workflow
 
-        Parameters:
-            - request: AppModelsRequestWorkflow.
+        Parameters
+        ----------
+        request : AppModelsRequestWorkflow
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflow
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflow
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.create(
+            request=AppModelsRequestWorkflow(
+                name="string",
+                description="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -117,106 +161,152 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
         self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseWorkflow:
         """
         Get a single workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflow
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.get(
+            workflow_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a specific workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.delete(
+            workflow_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -226,31 +316,57 @@
         *,
         request: AppModelsRequestWorkflowStep,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseWorkflowStep:
         """
         Patch a workflow step
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        step_id : str
+
+        request : AppModelsRequestWorkflowStep
 
-            - step_id: str.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request: AppModelsRequestWorkflowStep.
+        Returns
+        -------
+        AppModelsResponseWorkflowStep
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflowStep
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.update(
+            workflow_id="string",
+            step_id="string",
+            request=AppModelsRequestWorkflowStep(
+                order=1,
+                agent_id="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps/{jsonable_encoder(step_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -260,22 +376,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def invoke(
@@ -288,43 +406,68 @@
         output_schemas: typing.Optional[typing.Dict[str, str]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Invoke a specific workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        input : str
+
+        enable_streaming : bool
+
+        session_id : typing.Optional[str]
 
-            - input: str.
+        output_schemas : typing.Optional[typing.Dict[str, str]]
 
-            - enable_streaming: bool.
+        output_schema : typing.Optional[str]
 
-            - session_id: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - output_schemas: typing.Optional[typing.Dict[str, str]].
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - output_schema: typing.Optional[str].
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.invoke(
+            workflow_id="string",
+            input="string",
+            enable_streaming=True,
+            session_id="string",
+            output_schemas={"string": "string"},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
         if output_schemas is not OMIT:
             _request["outputSchemas"] = output_schemas
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -334,65 +477,89 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_steps(
         self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> WorkflowStepList:
         """
         List all steps of a workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        WorkflowStepList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.list_steps(
+            workflow_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WorkflowStepList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowStepList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_step(
@@ -401,28 +568,53 @@
         *,
         request: AppModelsRequestWorkflowStep,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseWorkflowStep:
         """
         Create a new workflow step
 
-        Parameters:
-            - workflow_id: str.
-
-            - request: AppModelsRequestWorkflowStep.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request : AppModelsRequestWorkflowStep
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflowStep
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflowStep
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.add_step(
+            workflow_id="string",
+            request=AppModelsRequestWorkflowStep(
+                order=1,
+                agent_id="string",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -432,68 +624,93 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_step(
         self, workflow_id: str, step_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Delete a specific workflow step
 
-        Parameters:
-            - workflow_id: str.
-
-            - step_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        step_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow.delete_step(
+            workflow_id="string",
+            step_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps/{jsonable_encoder(step_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -507,77 +724,124 @@
         skip: typing.Optional[int] = None,
         take: typing.Optional[int] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> WorkflowList:
         """
         List all workflows
 
-        Parameters:
-            - skip: typing.Optional[int].
+        Parameters
+        ----------
+        skip : typing.Optional[int]
+
+        take : typing.Optional[int]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        WorkflowList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - take: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.list(
+            skip=1,
+            take=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "skip": skip,
-                        "take": take,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "skip": skip,
+                            "take": take,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WorkflowList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self, *, request: AppModelsRequestWorkflow, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseWorkflow:
         """
         Create a new workflow
 
-        Parameters:
-            - request: AppModelsRequestWorkflow.
+        Parameters
+        ----------
+        request : AppModelsRequestWorkflow
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflow
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflow
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.create(
+            request=AppModelsRequestWorkflow(
+                name="string",
+                description="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -587,106 +851,152 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> AppModelsResponseWorkflow:
         """
         Get a single workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflow
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.get(
+            workflow_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflow, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
         Delete a specific workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.delete(
+            workflow_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -696,31 +1006,57 @@
         *,
         request: AppModelsRequestWorkflowStep,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseWorkflowStep:
         """
         Patch a workflow step
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
 
-            - step_id: str.
+        step_id : str
 
-            - request: AppModelsRequestWorkflowStep.
+        request : AppModelsRequestWorkflowStep
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflowStep
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflowStep
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.update(
+            workflow_id="string",
+            step_id="string",
+            request=AppModelsRequestWorkflowStep(
+                order=1,
+                agent_id="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps/{jsonable_encoder(step_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -730,22 +1066,24 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def invoke(
@@ -758,43 +1096,68 @@
         output_schemas: typing.Optional[typing.Dict[str, str]] = OMIT,
         output_schema: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Any:
         """
         Invoke a specific workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        input : str
+
+        enable_streaming : bool
+
+        session_id : typing.Optional[str]
 
-            - input: str.
+        output_schemas : typing.Optional[typing.Dict[str, str]]
 
-            - enable_streaming: bool.
+        output_schema : typing.Optional[str]
 
-            - session_id: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - output_schemas: typing.Optional[typing.Dict[str, str]].
+        Returns
+        -------
+        typing.Any
+            Successful Response
 
-            - output_schema: typing.Optional[str].
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.invoke(
+            workflow_id="string",
+            input="string",
+            enable_streaming=True,
+            session_id="string",
+            output_schemas={"string": "string"},
+            output_schema="string",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"input": input, "enableStreaming": enable_streaming}
         if session_id is not OMIT:
             _request["sessionId"] = session_id
         if output_schemas is not OMIT:
             _request["outputSchemas"] = output_schemas
         if output_schema is not OMIT:
             _request["outputSchema"] = output_schema
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -804,65 +1167,89 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_steps(
         self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> WorkflowStepList:
         """
         List all steps of a workflow
 
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        WorkflowStepList
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.list_steps(
+            workflow_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WorkflowStepList, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(WorkflowStepList, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_step(
@@ -871,28 +1258,53 @@
         *,
         request: AppModelsRequestWorkflowStep,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> AppModelsResponseWorkflowStep:
         """
         Create a new workflow step
 
-        Parameters:
-            - workflow_id: str.
-
-            - request: AppModelsRequestWorkflowStep.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request : AppModelsRequestWorkflowStep
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AppModelsResponseWorkflowStep
+            Successful Response
+
+        Examples
+        --------
+        from superagent import AppModelsRequestWorkflowStep
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.add_step(
+            workflow_id="string",
+            request=AppModelsRequestWorkflowStep(
+                order=1,
+                agent_id="string",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -902,66 +1314,91 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AppModelsResponseWorkflowStep, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_step(
         self, workflow_id: str, step_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
         Delete a specific workflow step
 
-        Parameters:
-            - workflow_id: str.
-
-            - step_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        step_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow.delete_step(
+            workflow_id="string",
+            step_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"api/v1/workflows/{jsonable_encoder(workflow_id)}/steps/{jsonable_encoder(step_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/resources/workflow_config/client.py` & `superagent_py-0.2.40/src/superagent/resources/workflow_config/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,178 +3,255 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class WorkflowConfigClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get_schema(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
+
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow_config.get_schema()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows/config/schema"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows/config/schema"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_config(self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import Superagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = Superagent(
+            token="YOUR_TOKEN",
+        )
+        client.workflow_config.add_config(
+            workflow_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/config"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncWorkflowConfigClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_schema(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
+
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow_config.get_schema()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows/config/schema"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/workflows/config/schema"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_config(
         self, workflow_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Any:
         """
-        Parameters:
-            - workflow_id: str.
+        Parameters
+        ----------
+        workflow_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Any
+            Successful Response
+
+        Examples
+        --------
+        from superagent.client import AsyncSuperagent
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncSuperagent(
+            token="YOUR_TOKEN",
+        )
+        await client.workflow_config.add_config(
+            workflow_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/v1/workflows/{jsonable_encoder(workflow_id)}/config"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.2.33/src/superagent/types/__init__.py` & `superagent_py-0.2.40/src/superagent/types/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/agent_datasosurce_list.py` & `superagent_py-0.2.40/src/superagent/types/agent_datasosurce_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_agent_datasource import PrismaModelsAgentDatasource
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AgentDatasosurceList(pydantic.BaseModel):
+class AgentDatasosurceList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsAgentDatasource]] = None
+    data: typing.Optional[typing.List[PrismaModelsAgentDatasource]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/agent_list.py` & `superagent_py-0.2.40/src/superagent/types/agent_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_agent import PrismaModelsAgent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AgentList(pydantic.BaseModel):
+class AgentList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsAgent]] = None
+    data: typing.Optional[typing.List[PrismaModelsAgent]]
     total_pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/agent_tool_list.py` & `superagent_py-0.2.40/src/superagent/types/llm_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_agent_tool import PrismaModelsAgentTool
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_llm import PrismaModelsLlm
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AgentToolList(pydantic.BaseModel):
+class LlmList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsAgentTool]] = None
+    data: typing.Optional[typing.List[PrismaModelsLlm]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/agent_type.py` & `superagent_py-0.2.40/src/superagent/types/agent_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/api_key_create.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_agent_invoke.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .api_key_create_model import ApiKeyCreateModel
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ApiKeyCreate(pydantic.BaseModel):
+class AppModelsResponseAgentInvoke(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[ApiKeyCreateModel] = None
+    data: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/api_key_create_model.py` & `superagent_py-0.2.40/src/superagent/types/api_key_create_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_api_user import PrismaModelsApiUser
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ApiKeyCreateModel(pydantic.BaseModel):
+class ApiKeyCreateModel(pydantic_v1.BaseModel):
     """
     Represents a ApiKey record
     """
 
     id: str
     name: str
-    display_api_key: str = pydantic.Field(alias="displayApiKey")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
-    api_key: str = pydantic.Field(alias="apiKey")
+    display_api_key: str = pydantic_v1.Field(alias="displayApiKey")
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
+    api_key: str = pydantic_v1.Field(alias="apiKey")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/api_key_list.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_datasource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_api_key import PrismaModelsApiKey
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_datasource import PrismaModelsDatasource
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ApiKeyList(pydantic.BaseModel):
+class AppModelsResponseDatasource(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsApiKey]] = None
+    data: typing.Optional[PrismaModelsDatasource]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_api_key.py` & `superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_retrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AppModelsRequestApiKey(pydantic.BaseModel):
-    name: str
 
+class ToolAssistantToolsRetrieval(pydantic_v1.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_api_user.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_agent import PrismaModelsAgent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsRequestApiUser(pydantic.BaseModel):
-    email: str
-    first_name: typing.Optional[str] = pydantic.Field(alias="firstName", default=None)
-    last_name: typing.Optional[str] = pydantic.Field(alias="lastName", default=None)
-    company: typing.Optional[str] = None
-    anonymous_id: typing.Optional[str] = pydantic.Field(alias="anonymousId", default=None)
+class AppModelsResponseAgent(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[PrismaModelsAgent]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_datasource.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_datasource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .embeddings_model_provider import EmbeddingsModelProvider
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsRequestDatasource(pydantic.BaseModel):
+class AppModelsRequestDatasource(pydantic_v1.BaseModel):
     name: str
-    description: typing.Optional[str] = None
+    description: typing.Optional[str]
     type: str
-    content: typing.Optional[str] = None
-    url: typing.Optional[str] = None
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
-    vector_db_id: typing.Optional[str] = pydantic.Field(alias="vectorDbId", default=None)
-    embeddings_model_provider: typing.Optional[EmbeddingsModelProvider] = pydantic.Field(
-        alias="embeddingsModelProvider", default=None
+    content: typing.Optional[str]
+    url: typing.Optional[str]
+    metadata: typing.Optional[typing.Dict[str, typing.Any]]
+    vector_db_id: typing.Optional[str] = pydantic_v1.Field(alias="vectorDbId")
+    embeddings_model_provider: typing.Optional[EmbeddingsModelProvider] = pydantic_v1.Field(
+        alias="embeddingsModelProvider"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_llm.py` & `superagent_py-0.2.40/src/superagent/types/tool_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_tool import PrismaModelsTool
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsRequestLlm(pydantic.BaseModel):
-    provider: str
-    api_key: str = pydantic.Field(alias="apiKey")
-    options: typing.Optional[typing.Dict[str, typing.Any]] = None
+class ToolList(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[typing.List[PrismaModelsTool]]
+    total_pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_vector_db.py` & `superagent_py-0.2.40/src/superagent/types/agent_tool_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .vector_db_provider import VectorDbProvider
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_agent_tool import PrismaModelsAgentTool
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsRequestVectorDb(pydantic.BaseModel):
-    provider: VectorDbProvider
-    options: typing.Dict[str, typing.Any]
+class AgentToolList(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[typing.List[PrismaModelsAgentTool]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_workflow.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_llm import PrismaModelsLlm
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsRequestWorkflow(pydantic.BaseModel):
-    name: str
-    description: str
+class AppModelsResponseLlm(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[PrismaModelsLlm]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_request_workflow_step.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_agent_llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
-class AppModelsRequestWorkflowStep(pydantic.BaseModel):
-    order: int
-    agent_id: str = pydantic.Field(alias="agentId")
+class PrismaModelsAgentLlm(pydantic_v1.BaseModel):
+    """
+    Represents a AgentLLM record
+    """
+
+    agent_id: str = pydantic_v1.Field(alias="agentId")
+    llm_id: str = pydantic_v1.Field(alias="llmId")
+    agent: typing.Optional[PrismaModelsAgent]
+    llm: typing.Optional[PrismaModelsLlm]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
+from .prisma_models_llm import PrismaModelsLlm  # noqa: E402
+
+PrismaModelsAgentLlm.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_agent.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_agent import PrismaModelsAgent
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_tool import PrismaModelsTool
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseAgent(pydantic.BaseModel):
+class AppModelsResponseTool(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsAgent] = None
+    data: typing.Optional[PrismaModelsTool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_agent_invoke.py` & `superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AppModelsResponseAgentInvoke(pydantic.BaseModel):
-    success: bool
-    data: typing.Optional[typing.Any] = None
 
+class ToolAssistantToolsCode(pydantic_v1.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_api_key.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_api_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_api_key import PrismaModelsApiKey
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseApiKey(pydantic.BaseModel):
+class AppModelsResponseApiKey(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsApiKey] = None
+    data: typing.Optional[PrismaModelsApiKey]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_api_user.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_api_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_api_user import PrismaModelsApiUser
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseApiUser(pydantic.BaseModel):
+class AppModelsResponseApiUser(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsApiUser] = None
+    data: typing.Optional[PrismaModelsApiUser]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_datasource.py` & `superagent_py-0.2.40/src/superagent/types/datasource_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_datasource import PrismaModelsDatasource
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseDatasource(pydantic.BaseModel):
+class DatasourceList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsDatasource] = None
+    data: typing.Optional[typing.List[PrismaModelsDatasource]]
+    total_pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_llm.py` & `superagent_py-0.2.40/src/superagent/types/api_key_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_llm import PrismaModelsLlm
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_api_key import PrismaModelsApiKey
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseLlm(pydantic.BaseModel):
+class ApiKeyList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsLlm] = None
+    data: typing.Optional[typing.List[PrismaModelsApiKey]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_tool.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_api_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_tool import PrismaModelsTool
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseTool(pydantic.BaseModel):
-    success: bool
-    data: typing.Optional[PrismaModelsTool] = None
+class AppModelsRequestApiKey(pydantic_v1.BaseModel):
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_vector_db.py` & `superagent_py-0.2.40/src/superagent/types/tool_assistant_tools_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_vector_db import PrismaModelsVectorDb
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .function_definition import FunctionDefinition
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseVectorDb(pydantic.BaseModel):
-    success: bool
-    data: typing.Optional[PrismaModelsVectorDb] = None
+class ToolAssistantToolsFunction(pydantic_v1.BaseModel):
+    function: typing.Optional[FunctionDefinition]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_workflow.py` & `superagent_py-0.2.40/src/superagent/types/function_definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_workflow import PrismaModelsWorkflow
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseWorkflow(pydantic.BaseModel):
-    success: bool
-    data: typing.Optional[PrismaModelsWorkflow] = None
+class FunctionDefinition(pydantic_v1.BaseModel):
+    name: typing.Optional[str]
+    description: typing.Optional[str]
+    parameters: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/app_models_response_workflow_step.py` & `superagent_py-0.2.40/src/superagent/types/workflow_step_list.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_workflow_step import PrismaModelsWorkflowStep
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AppModelsResponseWorkflowStep(pydantic.BaseModel):
+class WorkflowStepList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[PrismaModelsWorkflowStep] = None
+    data: typing.Optional[typing.List[PrismaModelsWorkflowStep]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/datasource_list.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_workflow_step.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_datasource import PrismaModelsDatasource
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_workflow_step import PrismaModelsWorkflowStep
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DatasourceList(pydantic.BaseModel):
+class AppModelsResponseWorkflowStep(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsDatasource]] = None
-    total_pages: int
+    data: typing.Optional[PrismaModelsWorkflowStep]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/datasource_status.py` & `superagent_py-0.2.40/src/superagent/types/datasource_status.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/datasource_type.py` & `superagent_py-0.2.40/src/superagent/types/datasource_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/embeddings_model_provider.py` & `superagent_py-0.2.40/src/superagent/types/embeddings_model_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/function_definition.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class FunctionDefinition(pydantic.BaseModel):
-    name: typing.Optional[str] = None
-    description: typing.Optional[str] = None
-    parameters: typing.Optional[typing.Dict[str, typing.Any]] = None
+class AppModelsRequestWorkflow(pydantic_v1.BaseModel):
+    name: str
+    description: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/http_validation_error.py` & `superagent_py-0.2.40/src/superagent/types/http_validation_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .validation_error import ValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class HttpValidationError(pydantic.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]] = None
+class HttpValidationError(pydantic_v1.BaseModel):
+    detail: typing.Optional[typing.List[ValidationError]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/llm_list.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_vector_db.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_llm import PrismaModelsLlm
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .vector_db_provider import VectorDbProvider
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class LlmList(pydantic.BaseModel):
-    success: bool
-    data: typing.Optional[typing.List[PrismaModelsLlm]] = None
+class AppModelsRequestVectorDb(pydantic_v1.BaseModel):
+    provider: VectorDbProvider
+    options: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/llm_model.py` & `superagent_py-0.2.40/src/superagent/types/llm_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,51 +7,79 @@
 
 
 class LlmModel(str, enum.Enum):
     """
     An enumeration.
     """
 
+    GPT_3_5_TURBO = "GPT_3_5_TURBO"
     GPT_3_5_TURBO_16_K_0613 = "GPT_3_5_TURBO_16K_0613"
     GPT_3_5_TURBO_0613 = "GPT_3_5_TURBO_0613"
     GPT_3_5_TURBO_1106 = "GPT_3_5_TURBO_1106"
     GPT_3_5_TURBO_0125 = "GPT_3_5_TURBO_0125"
+    GPT_4 = "GPT_4"
     GPT_4_0613 = "GPT_4_0613"
+    GPT_4_32_K = "GPT_4_32K"
     GPT_4_32_K_0613 = "GPT_4_32K_0613"
     GPT_4_1106_PREVIEW = "GPT_4_1106_PREVIEW"
+    GPT_4_0125_PREVIEW = "GPT_4_0125_PREVIEW"
+    GPT_4_TURBO = "GPT_4_TURBO"
     GPT_4_TURBO_PREVIEW = "GPT_4_TURBO_PREVIEW"
+    GPT_4_TURBO_2024_04_09 = "GPT_4_TURBO_2024_04_09"
+    GPT_4_0 = "GPT_4_0"
     MISTRAL_7_B_INSTRUCT_V_01 = "MISTRAL_7B_INSTRUCT_V01"
     MIXTRAL_8_X_7_B_INSTRUCT_V_01 = "MIXTRAL_8X7B_INSTRUCT_V01"
 
     def visit(
         self,
+        gpt_3_5_turbo: typing.Callable[[], T_Result],
         gpt_3_5_turbo_16_k_0613: typing.Callable[[], T_Result],
         gpt_3_5_turbo_0613: typing.Callable[[], T_Result],
         gpt_3_5_turbo_1106: typing.Callable[[], T_Result],
         gpt_3_5_turbo_0125: typing.Callable[[], T_Result],
+        gpt_4: typing.Callable[[], T_Result],
         gpt_4_0613: typing.Callable[[], T_Result],
+        gpt_4_32_k: typing.Callable[[], T_Result],
         gpt_4_32_k_0613: typing.Callable[[], T_Result],
         gpt_4_1106_preview: typing.Callable[[], T_Result],
+        gpt_4_0125_preview: typing.Callable[[], T_Result],
+        gpt_4_turbo: typing.Callable[[], T_Result],
         gpt_4_turbo_preview: typing.Callable[[], T_Result],
+        gpt_4_turbo_2024_04_09: typing.Callable[[], T_Result],
+        gpt_4_0: typing.Callable[[], T_Result],
         mistral_7_b_instruct_v_01: typing.Callable[[], T_Result],
         mixtral_8_x_7_b_instruct_v_01: typing.Callable[[], T_Result],
     ) -> T_Result:
+        if self is LlmModel.GPT_3_5_TURBO:
+            return gpt_3_5_turbo()
         if self is LlmModel.GPT_3_5_TURBO_16_K_0613:
             return gpt_3_5_turbo_16_k_0613()
         if self is LlmModel.GPT_3_5_TURBO_0613:
             return gpt_3_5_turbo_0613()
         if self is LlmModel.GPT_3_5_TURBO_1106:
             return gpt_3_5_turbo_1106()
         if self is LlmModel.GPT_3_5_TURBO_0125:
             return gpt_3_5_turbo_0125()
+        if self is LlmModel.GPT_4:
+            return gpt_4()
         if self is LlmModel.GPT_4_0613:
             return gpt_4_0613()
+        if self is LlmModel.GPT_4_32_K:
+            return gpt_4_32_k()
         if self is LlmModel.GPT_4_32_K_0613:
             return gpt_4_32_k_0613()
         if self is LlmModel.GPT_4_1106_PREVIEW:
             return gpt_4_1106_preview()
+        if self is LlmModel.GPT_4_0125_PREVIEW:
+            return gpt_4_0125_preview()
+        if self is LlmModel.GPT_4_TURBO:
+            return gpt_4_turbo()
         if self is LlmModel.GPT_4_TURBO_PREVIEW:
             return gpt_4_turbo_preview()
+        if self is LlmModel.GPT_4_TURBO_2024_04_09:
+            return gpt_4_turbo_2024_04_09()
+        if self is LlmModel.GPT_4_0:
+            return gpt_4_0()
         if self is LlmModel.MISTRAL_7_B_INSTRUCT_V_01:
             return mistral_7_b_instruct_v_01()
         if self is LlmModel.MIXTRAL_8_X_7_B_INSTRUCT_V_01:
             return mixtral_8_x_7_b_instruct_v_01()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/llm_params.py` & `superagent_py-0.2.40/src/superagent/types/vector_db_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_vector_db import PrismaModelsVectorDb
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class LlmParams(pydantic.BaseModel):
-    max_tokens: typing.Optional[int] = None
-    temperature: typing.Optional[float] = None
+class VectorDbList(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[typing.List[PrismaModelsVectorDb]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/llm_provider.py` & `superagent_py-0.2.40/src/superagent/types/llm_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/open_ai_assistant_parameters.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_llm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .open_ai_assistant_parameters_tools_item import OpenAiAssistantParametersToolsItem
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class OpenAiAssistantParameters(pydantic.BaseModel):
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
-    file_ids: typing.Optional[typing.List[str]] = pydantic.Field(alias="fileIds", default=None)
-    tools: typing.Optional[typing.List[OpenAiAssistantParametersToolsItem]] = None
+class AppModelsRequestLlm(pydantic_v1.BaseModel):
+    provider: str
+    api_key: str = pydantic_v1.Field(alias="apiKey")
+    options: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_agent.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,62 +2,62 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .agent_type import AgentType
 from .llm_model import LlmModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsAgent(pydantic.BaseModel):
+class PrismaModelsAgent(pydantic_v1.BaseModel):
     """
     Represents a Agent record
     """
 
     id: str
     type: AgentType
     name: str
-    avatar: typing.Optional[str] = None
-    initial_message: typing.Optional[str] = pydantic.Field(alias="initialMessage", default=None)
+    avatar: typing.Optional[str]
+    initial_message: typing.Optional[str] = pydantic_v1.Field(alias="initialMessage")
     description: str
-    is_active: bool = pydantic.Field(alias="isActive")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    llms: typing.Optional[typing.List[PrismaModelsAgentLlm]] = None
-    llm_model: typing.Optional[LlmModel] = pydantic.Field(alias="llmModel", default=None)
-    prompt: typing.Optional[str] = None
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
-    datasources: typing.Optional[typing.List[PrismaModelsAgentDatasource]] = None
-    tools: typing.Optional[typing.List[PrismaModelsAgentTool]] = None
-    workflow_steps: typing.Optional[typing.List[PrismaModelsWorkflowStep]] = pydantic.Field(
-        alias="workflowSteps", default=None
-    )
-    metadata: typing.Optional[typing.Any] = None
-    output_schema: typing.Optional[str] = pydantic.Field(alias="outputSchema", default=None)
+    is_active: bool = pydantic_v1.Field(alias="isActive")
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    llms: typing.Optional[typing.List[PrismaModelsAgentLlm]]
+    llm_model: typing.Optional[LlmModel] = pydantic_v1.Field(alias="llmModel")
+    prompt: typing.Optional[str]
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
+    datasources: typing.Optional[typing.List[PrismaModelsAgentDatasource]]
+    tools: typing.Optional[typing.List[PrismaModelsAgentTool]]
+    workflow_steps: typing.Optional[typing.List[PrismaModelsWorkflowStep]] = pydantic_v1.Field(alias="workflowSteps")
+    metadata: typing.Optional[typing.Any]
+    output_schema: typing.Optional[str] = pydantic_v1.Field(alias="outputSchema")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_agent_datasource import PrismaModelsAgentDatasource  # noqa: E402
 from .prisma_models_agent_llm import PrismaModelsAgentLlm  # noqa: E402
 from .prisma_models_agent_tool import PrismaModelsAgentTool  # noqa: E402
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_agent_datasource.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_agent_datasource.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,45 +2,47 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsAgentDatasource(pydantic.BaseModel):
+class PrismaModelsAgentDatasource(pydantic_v1.BaseModel):
     """
     Represents a AgentDatasource record
     """
 
-    agent_id: str = pydantic.Field(alias="agentId")
-    datasource_id: str = pydantic.Field(alias="datasourceId")
-    agent: typing.Optional[PrismaModelsAgent] = None
-    datasource: typing.Optional[PrismaModelsDatasource] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    agent_id: str = pydantic_v1.Field(alias="agentId")
+    datasource_id: str = pydantic_v1.Field(alias="datasourceId")
+    agent: typing.Optional[PrismaModelsAgent]
+    datasource: typing.Optional[PrismaModelsDatasource]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
 from .prisma_models_datasource import PrismaModelsDatasource  # noqa: E402
 
 PrismaModelsAgentDatasource.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_agent_llm.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_workflow_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsAgentLlm(pydantic.BaseModel):
+class PrismaModelsWorkflowStep(pydantic_v1.BaseModel):
     """
-    Represents a AgentLLM record
+    Represents a WorkflowStep record
     """
 
-    agent_id: str = pydantic.Field(alias="agentId")
-    llm_id: str = pydantic.Field(alias="llmId")
-    agent: typing.Optional[PrismaModelsAgent] = None
-    llm: typing.Optional[PrismaModelsLlm] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    id: str
+    order: int
+    workflow_id: str = pydantic_v1.Field(alias="workflowId")
+    workflow: typing.Optional[PrismaModelsWorkflow]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    input: typing.Optional[str]
+    output: typing.Optional[str]
+    agent_id: str = pydantic_v1.Field(alias="agentId")
+    agent: typing.Optional[PrismaModelsAgent]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
-from .prisma_models_llm import PrismaModelsLlm  # noqa: E402
+from .prisma_models_workflow import PrismaModelsWorkflow  # noqa: E402
 
-PrismaModelsAgentLlm.update_forward_refs()
+PrismaModelsWorkflowStep.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_agent_tool.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .llm_provider import LlmProvider
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsAgentTool(pydantic.BaseModel):
+class PrismaModelsLlm(pydantic_v1.BaseModel):
     """
-    Represents a AgentTool record
+    Represents a LLM record
     """
 
-    agent_id: str = pydantic.Field(alias="agentId")
-    tool_id: str = pydantic.Field(alias="toolId")
-    agent: typing.Optional[PrismaModelsAgent] = None
-    tool: typing.Optional[PrismaModelsTool] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    id: str
+    provider: LlmProvider
+    api_key: str = pydantic_v1.Field(alias="apiKey")
+    options: typing.Optional[typing.Any]
+    agents: typing.Optional[typing.List[PrismaModelsAgentLlm]]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
-from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
-from .prisma_models_tool import PrismaModelsTool  # noqa: E402
+from .prisma_models_agent_llm import PrismaModelsAgentLlm  # noqa: E402
+from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
 
-PrismaModelsAgentTool.update_forward_refs()
+PrismaModelsLlm.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_api_key.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_workflow.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsApiKey(pydantic.BaseModel):
+class PrismaModelsWorkflow(pydantic_v1.BaseModel):
     """
-    Represents a ApiKey record
+    Represents a Workflow record
     """
 
     id: str
     name: str
-    display_api_key: str = pydantic.Field(alias="displayApiKey")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
+    description: typing.Optional[str]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    steps: typing.Optional[typing.List[PrismaModelsWorkflowStep]]
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
+    workflow_configs: typing.Optional[typing.List[WorkflowConfig]] = pydantic_v1.Field(alias="workflowConfigs")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
+from .prisma_models_workflow_step import PrismaModelsWorkflowStep  # noqa: E402
+from .workflow_config import WorkflowConfig  # noqa: E402
 
-PrismaModelsApiKey.update_forward_refs()
+PrismaModelsWorkflow.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_datasource.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_datasource.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,56 +2,58 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .datasource_status import DatasourceStatus
 from .datasource_type import DatasourceType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsDatasource(pydantic.BaseModel):
+class PrismaModelsDatasource(pydantic_v1.BaseModel):
     """
     Represents a Datasource record
     """
 
     id: str
     name: str
-    content: typing.Optional[str] = None
-    description: typing.Optional[str] = None
-    url: typing.Optional[str] = None
+    content: typing.Optional[str]
+    description: typing.Optional[str]
+    url: typing.Optional[str]
     type: DatasourceType
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    metadata: typing.Optional[str] = None
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    metadata: typing.Optional[str]
     status: DatasourceStatus
-    datasources: typing.Optional[typing.List[PrismaModelsAgentDatasource]] = None
-    vector_db: typing.Optional[PrismaModelsVectorDb] = pydantic.Field(alias="vectorDb", default=None)
-    vector_db_id: typing.Optional[str] = pydantic.Field(alias="vectorDbId", default=None)
+    datasources: typing.Optional[typing.List[PrismaModelsAgentDatasource]]
+    vector_db: typing.Optional[PrismaModelsVectorDb] = pydantic_v1.Field(alias="vectorDb")
+    vector_db_id: typing.Optional[str] = pydantic_v1.Field(alias="vectorDbId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_agent_datasource import PrismaModelsAgentDatasource  # noqa: E402
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
 from .prisma_models_vector_db import PrismaModelsVectorDb  # noqa: E402
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_llm.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,49 +2,54 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .llm_provider import LlmProvider
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .tool_type import ToolType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsLlm(pydantic.BaseModel):
+class PrismaModelsTool(pydantic_v1.BaseModel):
     """
-    Represents a LLM record
+    Represents a Tool record
     """
 
     id: str
-    provider: LlmProvider
-    api_key: str = pydantic.Field(alias="apiKey")
-    options: typing.Optional[typing.Any] = None
-    agents: typing.Optional[typing.List[PrismaModelsAgentLlm]] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
+    name: str
+    description: str
+    type: ToolType
+    return_direct: bool = pydantic_v1.Field(alias="returnDirect")
+    metadata: typing.Optional[str]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
+    tools: typing.Optional[typing.List[PrismaModelsAgentTool]]
+    tool_config: typing.Optional[typing.Any] = pydantic_v1.Field(alias="toolConfig")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
-from .prisma_models_agent_llm import PrismaModelsAgentLlm  # noqa: E402
+from .prisma_models_agent_tool import PrismaModelsAgentTool  # noqa: E402
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
 
-PrismaModelsLlm.update_forward_refs()
+PrismaModelsTool.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_tool.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_agent_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,52 +2,47 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .tool_type import ToolType
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsTool(pydantic.BaseModel):
+class PrismaModelsAgentTool(pydantic_v1.BaseModel):
     """
-    Represents a Tool record
+    Represents a AgentTool record
     """
 
-    id: str
-    name: str
-    description: str
-    type: ToolType
-    return_direct: bool = pydantic.Field(alias="returnDirect")
-    metadata: typing.Optional[str] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
-    tools: typing.Optional[typing.List[PrismaModelsAgentTool]] = None
-    tool_config: typing.Optional[typing.Any] = pydantic.Field(alias="toolConfig", default=None)
+    agent_id: str = pydantic_v1.Field(alias="agentId")
+    tool_id: str = pydantic_v1.Field(alias="toolId")
+    agent: typing.Optional[PrismaModelsAgent]
+    tool: typing.Optional[PrismaModelsTool]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
-from .prisma_models_agent_tool import PrismaModelsAgentTool  # noqa: E402
-from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
+from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
+from .prisma_models_tool import PrismaModelsTool  # noqa: E402
 
-PrismaModelsTool.update_forward_refs()
+PrismaModelsAgentTool.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_vector_db.py` & `superagent_py-0.2.40/src/superagent/types/prisma_models_vector_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .vector_db_provider import VectorDbProvider
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PrismaModelsVectorDb(pydantic.BaseModel):
+class PrismaModelsVectorDb(pydantic_v1.BaseModel):
     """
     Represents a VectorDb record
     """
 
     id: str
     provider: VectorDbProvider
-    options: typing.Optional[typing.Any] = None
-    datasources: typing.Optional[typing.List[PrismaModelsDatasource]] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    api_user_id: str = pydantic.Field(alias="apiUserId")
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="apiUser", default=None)
+    options: typing.Optional[typing.Any]
+    datasources: typing.Optional[typing.List[PrismaModelsDatasource]]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    api_user_id: str = pydantic_v1.Field(alias="apiUserId")
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="apiUser")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
 from .prisma_models_datasource import PrismaModelsDatasource  # noqa: E402
 
 PrismaModelsVectorDb.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/prisma_models_workflow_step.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_workflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_workflow import PrismaModelsWorkflow
+
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class PrismaModelsWorkflowStep(pydantic.BaseModel):
-    """
-    Represents a WorkflowStep record
-    """
-
-    id: str
-    order: int
-    workflow_id: str = pydantic.Field(alias="workflowId")
-    workflow: typing.Optional[PrismaModelsWorkflow] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    input: typing.Optional[str] = None
-    output: typing.Optional[str] = None
-    agent_id: str = pydantic.Field(alias="agentId")
-    agent: typing.Optional[PrismaModelsAgent] = None
+class AppModelsResponseWorkflow(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[PrismaModelsWorkflow]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .prisma_models_agent import PrismaModelsAgent  # noqa: E402
-from .prisma_models_workflow import PrismaModelsWorkflow  # noqa: E402
-
-PrismaModelsWorkflowStep.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_code.py` & `superagent_py-0.2.40/src/superagent/types/llm_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class LlmParams(pydantic_v1.BaseModel):
+    max_tokens: typing.Optional[int]
+    temperature: typing.Optional[float]
 
-class ToolAssistantToolsCode(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_function.py` & `superagent_py-0.2.40/src/superagent/types/app_models_request_workflow_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .function_definition import FunctionDefinition
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ToolAssistantToolsFunction(pydantic.BaseModel):
-    function: typing.Optional[FunctionDefinition] = None
+class AppModelsRequestWorkflowStep(pydantic_v1.BaseModel):
+    order: int
+    agent_id: str = pydantic_v1.Field(alias="agentId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/tool_assistant_tools_retrieval.py` & `superagent_py-0.2.40/src/superagent/types/api_key_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .api_key_create_model import ApiKeyCreateModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ApiKeyCreate(pydantic_v1.BaseModel):
+    success: bool
+    data: typing.Optional[ApiKeyCreateModel]
 
-class ToolAssistantToolsRetrieval(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/tool_list.py` & `superagent_py-0.2.40/src/superagent/types/workflow_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .prisma_models_tool import PrismaModelsTool
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .prisma_models_workflow import PrismaModelsWorkflow
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ToolList(pydantic.BaseModel):
+class WorkflowList(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsTool]] = None
+    data: typing.Optional[typing.List[PrismaModelsWorkflow]]
     total_pages: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/tool_type.py` & `superagent_py-0.2.40/src/superagent/types/tool_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     HTTP = "HTTP"
     SUPERRAG = "SUPERRAG"
     RESEARCH = "RESEARCH"
     GITHUB = "GITHUB"
     SCRAPER = "SCRAPER"
     ADVANCED_SCRAPER = "ADVANCED_SCRAPER"
     GOOGLE_SEARCH = "GOOGLE_SEARCH"
+    SEC = "SEC"
 
     def visit(
         self,
         algolia: typing.Callable[[], T_Result],
         browser: typing.Callable[[], T_Result],
         bing_search: typing.Callable[[], T_Result],
         replicate: typing.Callable[[], T_Result],
@@ -58,14 +59,15 @@
         http: typing.Callable[[], T_Result],
         superrag: typing.Callable[[], T_Result],
         research: typing.Callable[[], T_Result],
         github: typing.Callable[[], T_Result],
         scraper: typing.Callable[[], T_Result],
         advanced_scraper: typing.Callable[[], T_Result],
         google_search: typing.Callable[[], T_Result],
+        sec: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is ToolType.ALGOLIA:
             return algolia()
         if self is ToolType.BROWSER:
             return browser()
         if self is ToolType.BING_SEARCH:
             return bing_search()
@@ -107,7 +109,9 @@
             return github()
         if self is ToolType.SCRAPER:
             return scraper()
         if self is ToolType.ADVANCED_SCRAPER:
             return advanced_scraper()
         if self is ToolType.GOOGLE_SEARCH:
             return google_search()
+        if self is ToolType.SEC:
+            return sec()
```

### Comparing `superagent_py-0.2.33/src/superagent/types/vector_db_list.py` & `superagent_py-0.2.40/src/superagent/types/app_models_response_vector_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .prisma_models_vector_db import PrismaModelsVectorDb
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VectorDbList(pydantic.BaseModel):
+class AppModelsResponseVectorDb(pydantic_v1.BaseModel):
     success: bool
-    data: typing.Optional[typing.List[PrismaModelsVectorDb]] = None
+    data: typing.Optional[PrismaModelsVectorDb]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `superagent_py-0.2.33/src/superagent/types/vector_db_provider.py` & `superagent_py-0.2.40/src/superagent/types/vector_db_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.33/src/superagent/types/workflow_config.py` & `superagent_py-0.2.40/src/superagent/types/workflow_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,47 +2,49 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WorkflowConfig(pydantic.BaseModel):
+class WorkflowConfig(pydantic_v1.BaseModel):
     """
     Represents a WorkflowConfig record
     """
 
     id: str
-    config: typing.Optional[typing.Any] = None
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    workflow_id: str = pydantic.Field(alias="workflowId")
-    workflow: typing.Optional[PrismaModelsWorkflow] = None
-    api_user: typing.Optional[PrismaModelsApiUser] = pydantic.Field(alias="ApiUser", default=None)
-    api_user_id: typing.Optional[str] = pydantic.Field(alias="apiUserId", default=None)
+    config: typing.Optional[typing.Any]
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic_v1.Field(alias="updatedAt")
+    workflow_id: str = pydantic_v1.Field(alias="workflowId")
+    workflow: typing.Optional[PrismaModelsWorkflow]
+    api_user: typing.Optional[PrismaModelsApiUser] = pydantic_v1.Field(alias="ApiUser")
+    api_user_id: typing.Optional[str] = pydantic_v1.Field(alias="apiUserId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.forbid
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .prisma_models_api_user import PrismaModelsApiUser  # noqa: E402
 from .prisma_models_workflow import PrismaModelsWorkflow  # noqa: E402
 
 WorkflowConfig.update_forward_refs()
```

### Comparing `superagent_py-0.2.33/PKG-INFO` & `superagent_py-0.2.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.2.33
+Version: 0.2.40
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

