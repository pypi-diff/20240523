# Comparing `tmp/semantic_kernel-1.0.1.tar.gz` & `tmp/semantic_kernel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-1.0.1.tar", max compression
+gzip compressed data, was "semantic_kernel-1.0.2.tar", max compression
```

## Comparing `semantic_kernel-1.0.1.tar` & `semantic_kernel-1.0.2.tar`

### file list

```diff
@@ -1,239 +1,249 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/pip/README.md
--rw-r--r--   0        0        0     4591 2024-05-22 16:18:31.525428 semantic_kernel-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3242 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      527 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7530 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10522 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     4670 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     3208 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6673 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2193 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      779 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8459 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3991 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1882 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2630 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3676 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     3766 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    11076 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5309 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     6096 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     6180 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     3604 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    24070 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3712 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4011 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     3807 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6359 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3743 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1984 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     2871 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
--rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
--rw-r--r--   0        0        0     3879 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1733 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6750 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    13396 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0      831 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
--rw-r--r--   0        0        0     1601 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
--rw-r--r--   0        0        0    17012 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7836 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    11153 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2295 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      634 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
--rw-r--r--   0        0        0     1740 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13097 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
--rw-r--r--   0        0        0     7720 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14357 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4597 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      657 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/memory_settings_base.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16748 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    13206 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0      614 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
--rw-r--r--   0        0        0     2267 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    15682 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0      556 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    21197 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      590 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11743 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15945 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0      582 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_settings.py
--rw-r--r--   0        0        0     3664 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23249 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    12561 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0     1004 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      764 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      498 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0      976 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1350 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    29335 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     3401 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
--rw-r--r--   0        0        0      299 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2954 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1105 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      906 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/const.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    14163 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12555 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     3997 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     4521 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      737 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    10933 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1976 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3336 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     3932 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2378 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9946 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1884 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3662 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1020 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1652 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/exceptions/memory_connector_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
--rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/filter_context_base.py
--rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/filter_types.py
--rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/functions/function_invocation_context.py
--rw-r--r--   0        0        0     6398 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/filters/kernel_filters_extension.py
--rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/prompts/prompt_render_context.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2420 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1711 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0    10643 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5499 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0    18367 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_extension.py
--rw-r--r--   0        0        0     8163 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    16879 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1925 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0     2157 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    24109 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      939 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      252 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    13830 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      462 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2582 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4285 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7211 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1639 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6571 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3675 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12124 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    12968 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1667 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      797 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14329 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      568 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1125 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4678 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4787 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      871 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4972 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     6735 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     5535 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4615 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2450 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     2116 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      545 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/kernel_reliability_extension.py
--rw-r--r--   0        0        0      999 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      679 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     1559 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/schema/kernel_json_schema.py
--rw-r--r--   0        0        0     2587 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/schema/kernel_json_schema_builder.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2624 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     6202 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/kernel_services_extension.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7447 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2413 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3908 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1672 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2376 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2924 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6569 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6271 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      654 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8531 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      498 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      841 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/experimental_decorator.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0      269 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 semantic_kernel-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/pip/README.md
+-rw-r--r--   0        0        0     4591 2024-05-23 18:12:45.972757 semantic_kernel-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3242 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      527 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7530 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10522 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4670 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3208 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6673 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2193 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      779 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8459 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3991 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1882 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2630 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3676 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     3766 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11076 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5309 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6096 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6180 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3604 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    24919 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3712 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4011 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3807 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6359 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3743 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1984 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     3202 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     3879 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1733 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6750 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13396 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      831 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1601 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    17012 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7836 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    11153 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2295 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      634 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1740 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13097 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
+-rw-r--r--   0        0        0     7720 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14357 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4597 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      657 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16748 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13206 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      614 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2267 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15682 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      556 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    21197 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      590 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11743 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15945 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      582 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3664 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23249 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    12561 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0     1004 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0      976 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0    11434 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation.py
+-rw-r--r--   0        0        0      379 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_expected_response.py
+-rw-r--r--   0        0        0     1418 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter.py
+-rw-r--r--   0        0        0      378 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_location.py
+-rw-r--r--   0        0        0      236 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_style.py
+-rw-r--r--   0        0        0      658 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload.py
+-rw-r--r--   0        0        0      731 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload_property.py
+-rw-r--r--   0        0        0      415 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_run_options.py
+-rw-r--r--   0        0        0      426 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_uri.py
+-rw-r--r--   0        0        0     1350 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0     6783 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0     8579 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_parser.py
+-rw-r--r--   0        0        0     7252 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_runner.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3401 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      299 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2954 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1105 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.2/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      906 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14163 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12555 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     3997 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4521 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      737 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    10933 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     1976 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3336 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     3932 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2378 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9946 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1884 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3662 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1020 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1652 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.2/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.2/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
+-rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/filter_context_base.py
+-rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/filter_types.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/functions/function_invocation_context.py
+-rw-r--r--   0        0        0     6398 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/filters/kernel_filters_extension.py
+-rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/prompts/prompt_render_context.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2596 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1711 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0    10643 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5607 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0    18367 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_extension.py
+-rw-r--r--   0        0        0     8262 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    16879 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1930 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0     2229 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    23610 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      939 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      252 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    13830 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      462 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2582 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4285 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7211 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1639 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6571 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3675 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12124 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    12968 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1667 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      797 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14329 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      568 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1125 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4678 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4787 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      871 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4972 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6735 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5535 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2450 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     2116 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.2/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      545 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/kernel_reliability_extension.py
+-rw-r--r--   0        0        0      999 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      679 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2609 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/schema/kernel_json_schema_builder.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2624 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     6202 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/kernel_services_extension.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7447 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2413 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3908 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1672 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2376 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2924 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6569 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6271 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8531 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      841 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0      269 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 semantic_kernel-1.0.2/PKG-INFO
```

### Comparing `semantic_kernel-1.0.1/pip/README.md` & `semantic_kernel-1.0.2/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/pyproject.toml` & `semantic_kernel-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "1.0.1"
+version = "1.0.2"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -470,14 +470,30 @@
             frc = FunctionResultContent.from_function_call_content_and_result(
                 function_call_content=function_call,
                 result="The tool call could not be found, please try again and make sure to validate the name.",
             )
             chat_history.add_message(message=frc.to_chat_message_content())
             return
 
+        num_required_func_params = len([param for param in function_to_call.parameters if param.is_required])
+        if len(parsed_args) < num_required_func_params:
+            msg = (
+                f"There are `{num_required_func_params}` tool call arguments required and "
+                f"only `{len(parsed_args)}` received. The required arguments are: "
+                f"{[param.name for param in function_to_call.parameters if param.is_required]}. "
+                "Please provide the required arguments and try again."
+            )
+            logger.exception(msg)
+            frc = FunctionResultContent.from_function_call_content_and_result(
+                function_call_content=function_call,
+                result=msg,
+            )
+            chat_history.add_message(message=frc.to_chat_message_content())
+            return
+
         _rebuild_auto_function_invocation_context()
         invocation_context = AutoFunctionInvocationContext(
             function=function_to_call,
             kernel=kernel,
             arguments=args_cloned,
             chat_history=chat_history,
             function_result=FunctionResult(function=function_to_call.metadata, value=None),
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,27 +33,38 @@
 
 
 def kernel_function_metadata_to_openai_tool_format(metadata: KernelFunctionMetadata) -> dict[str, Any]:
     """Convert the kernel function metadata to OpenAI format."""
 
     def parse_schema(schema_data):
         """Recursively parse the schema data to include nested properties."""
-        if schema_data.get("type") == "object":
+        if schema_data is None:
+            return {"type": "string", "description": ""}
+
+        schema_type = schema_data.get("type")
+        schema_description = schema_data.get("description", "")
+
+        if schema_type == "object":
+            properties = {key: parse_schema(value) for key, value in schema_data.get("properties", {}).items()}
             return {
                 "type": "object",
-                "properties": {key: parse_schema(value) for key, value in schema_data.get("properties", {}).items()},
-                "description": schema_data.get("description", ""),
-            }
-        else:
-            return {
-                "type": schema_data.get("type", "string"),
-                "description": schema_data.get("description", ""),
-                **({"enum": schema_data.get("enum")} if "enum" in schema_data else {}),
+                "properties": properties,
+                "description": schema_description,
             }
 
+        if schema_type == "array":
+            items = schema_data.get("items", {"type": "string"})
+            return {"type": "array", "description": schema_description, "items": items}
+
+        schema_dict = {"type": schema_type, "description": schema_description}
+        if "enum" in schema_data:
+            schema_dict["enum"] = schema_data["enum"]
+
+        return schema_dict
+
     return {
         "type": "function",
         "function": {
             "name": metadata.fully_qualified_name,
             "description": metadata.description or "",
             "parameters": {
                 "type": "object",
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/memory_settings_base.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/memory_settings_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-1.0.2/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/chat_history.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/function_call_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/function_result_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/text_content.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/contents/types.py` & `semantic_kernel-1.0.2/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-1.0.2/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py` & `semantic_kernel-1.0.2/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/filters/filter_context_base.py` & `semantic_kernel-1.0.2/semantic_kernel/filters/filter_context_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/filters/kernel_filters_extension.py` & `semantic_kernel-1.0.2/semantic_kernel/filters/kernel_filters_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/function_result.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/function_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,19 @@
     metadata: dict[str, Any] = Field(default_factory=dict)
 
     def __str__(self) -> str:
         """Get the string representation of the result."""
         if self.value:
             try:
                 if isinstance(self.value, list):
-                    return str(self.value[0])
+                    return (
+                        str(self.value[0])
+                        if isinstance(self.value[0], KernelContent)
+                        else ",".join(map(str, self.value))
+                    )
                 elif isinstance(self.value, dict):
                     # TODO: remove this once function result doesn't include input args
                     # This is so an integration test can pass.
                     return str(list(self.value.values())[-1])
                 return str(self.value)
             except Exception as e:
                 raise FunctionResultError(f"Failed to convert value to string: {e}") from e
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_arguments.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         logger.debug(f"{annotations=}")
         setattr(func, "__kernel_function_parameters__", annotations)
 
         return_annotation = (
             _parse_parameter("return", func_sig.return_annotation, None) if func_sig.return_annotation else {}
         )
         setattr(func, "__kernel_function_return_type__", return_annotation.get("type_", "None"))
+        setattr(func, "__kernel_function_return_type_object__", return_annotation.get("type_object", None))
         setattr(func, "__kernel_function_return_description__", return_annotation.get("description", ""))
         setattr(func, "__kernel_function_return_required__", return_annotation.get("is_required", False))
         return func
 
     if func:
         return decorator(func)
     return decorator
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_extension.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,28 +54,29 @@
         # all these fields are created when the kernel function decorator is used,
         # so no need to check before using, will raise an exception if not set
         function_name = method.__kernel_function_name__  # type: ignore
         description = method.__kernel_function_description__  # type: ignore
         if parameters is None:
             parameters = [KernelParameterMetadata(**param) for param in method.__kernel_function_parameters__]  # type: ignore
         if return_parameter is None:
-            return_param = KernelParameterMetadata(
+            return_parameter = KernelParameterMetadata(
                 name="return",
                 description=method.__kernel_function_return_description__,  # type: ignore
                 default_value=None,
                 type_=method.__kernel_function_return_type__,  # type: ignore
+                type_object=method.__kernel_function_return_type_object__,  # type: ignore
                 is_required=method.__kernel_function_return_required__,  # type: ignore
             )
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 description=description,
                 parameters=parameters,
-                return_parameter=return_param,
+                return_parameter=return_parameter,
                 is_prompt=False,
                 is_asynchronous=isasyncgenfunction(method) or iscoroutinefunction(method),
                 plugin_name=plugin_name,
                 additional_properties=additional_metadata if additional_metadata is not None else {},
             )
         except ValidationError as exc:
             # reraise the exception to clarify it comes from KernelFunction init
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.utils.validation import FUNCTION_NAME_REGEX, PLUGIN_NAME_REGEX
 
 
 class KernelFunctionMetadata(KernelBaseModel):
-    name: str = Field(pattern=FUNCTION_NAME_REGEX)
+    name: str = Field(..., pattern=FUNCTION_NAME_REGEX)
     plugin_name: str | None = Field(None, pattern=PLUGIN_NAME_REGEX)
     description: str | None = Field(default=None)
     parameters: list[KernelParameterMetadata] = Field(default_factory=list)
     is_prompt: bool
     is_asynchronous: bool | None = Field(default=True)
     return_parameter: KernelParameterMetadata | None = None
     additional_properties: dict[str, Any] | None = Field(default=None)
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     type_object: Any | None = None
     schema_data: dict[str, Any] | None = None
 
     @model_validator(mode="before")
     @classmethod
     def form_schema(cls, data: Any) -> Any:
         if isinstance(data, dict):
-            type_object = data.get("type_object", None)
-            type_ = data.get("type_", None)
-            default_value = data.get("default_value", None)
-            description = data.get("description", None)
-            inferred_schema = cls.infer_schema(type_object, type_, default_value, description)
-            data["schema_data"] = inferred_schema
+            if data.get("schema_data") is None:
+                type_object = data.get("type_object", None)
+                type_ = data.get("type_", None)
+                default_value = data.get("default_value", None)
+                description = data.get("description", None)
+                inferred_schema = cls.infer_schema(type_object, type_, default_value, description)
+                data["schema_data"] = inferred_schema
         return data
 
     @classmethod
     def infer_schema(
         cls, type_object: type | None, parameter_type: str | None, default_value: Any, description: str | None
     ) -> dict[str, Any] | None:
         schema = None
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,23 @@
         name (str): The name of the plugin. The name can be upper/lower
             case letters and underscores.
         description (str): The description of the plugin.
         functions (Dict[str, KernelFunction]): The functions in the plugin,
             indexed by their name.
 
     Methods:
-        set (key: str, value: KernelFunction): Set a function in the plugin.
-        __setitem__ (key: str, value: KernelFunction): Set a function in the plugin.
-        get (key: str, default: KernelFunction | None = None): Get a function from the plugin.
-        __getitem__ (key: str): Get a function from the plugin.
-        __contains__ (key: str): Check if a function is in the plugin.
-        __iter__ (): Iterate over the functions in the plugin.
-        update(*args: Any, **kwargs: Any): Update the plugin with the functions from another.
-        setdefault(key: str, value: KernelFunction | None): Set a default value for a key.
-        get_functions_metadata(): Get the metadata for the functions in the plugin.
+        set: Set a function in the plugin.
+        __setitem__: Set a function in the plugin.
+        get: Get a function from the plugin.
+        __getitem__: Get a function from the plugin.
+        __contains__: Check if a function is in the plugin.
+        __iter__: Iterate over the functions in the plugin.
+        update: Update the plugin with the functions from another.
+        setdefault: Set a default value for a key.
+        get_functions_metadata: Get the metadata for the functions in the plugin.
 
     Class methods:
         from_object(plugin_name: str, plugin_instance: Any | dict[str, Any], description: str | None = None):
             Create a plugin from a existing object, like a custom class with annotated functions.
         from_directory(plugin_name: str, parent_directory: str, description: str | None = None):
             Create a plugin from a directory, parsing:
             .py files, .yaml files and directories with skprompt.txt and config.json files.
@@ -102,25 +102,19 @@
             | list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]
             | dict[str, KERNEL_FUNCTION_TYPE]
             | None
         ) = None,
     ):
         """Create a KernelPlugin
 
-        Attributes:
-            name (str): The name of the plugin. The name can be upper/lower
+        Args:
+            name: The name of the plugin. The name can be upper/lower
                 case letters and underscores.
-            description (str, optional): The description of the plugin.
-            functions (
-                    KernelFunction |
-                    Callable |
-                    list[KernelFunction | Callable | KernelPlugin] |
-                    dict[str, KernelFunction | Callable] |
-                    KernelPlugin |
-                    None):
+            description: The description of the plugin.
+            functions:
                 The functions in the plugin, will be rewritten to a dictionary of functions.
 
         Raises:
             ValueError: If the functions are not of the correct type.
             PydanticError: If the name is not a valid plugin name.
         """
         super().__init__(
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-1.0.2/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/kernel.py` & `semantic_kernel-1.0.2/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-1.0.2/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/plan.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/input_variable.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/input_variable.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/reliability/kernel_reliability_extension.py` & `semantic_kernel-1.0.2/semantic_kernel/reliability/kernel_reliability_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-1.0.2/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-1.0.2/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/schema/kernel_json_schema_builder.py` & `semantic_kernel-1.0.2/semantic_kernel/schema/kernel_json_schema_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "int": "integer",
     "str": "string",
     "bool": "boolean",
     "float": "number",
     "list": "array",
     "dict": "object",
     "object": "object",
+    "array": "array",
 }
 
 
 class KernelJsonSchemaBuilder:
 
     @classmethod
     def build(cls, parameter_type: type | str, description: str | None = None) -> dict[str, Any]:
```

### Comparing `semantic_kernel-1.0.1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-1.0.2/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-1.0.2/semantic_kernel/services/ai_service_selector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/services/kernel_services_extension.py` & `semantic_kernel-1.0.2/semantic_kernel/services/kernel_services_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/README.md` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-1.0.2/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/text/function_extension.py` & `semantic_kernel-1.0.2/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-1.0.2/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/utils/experimental_decorator.py` & `semantic_kernel-1.0.2/semantic_kernel/utils/experimental_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/semantic_kernel/utils/naming.py` & `semantic_kernel-1.0.2/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.1/PKG-INFO` & `semantic_kernel-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 1.0.1
+Version: 1.0.2
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

