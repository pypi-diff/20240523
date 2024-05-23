# Comparing `tmp/infrastack_otel-0.0.2.tar.gz` & `tmp/infrastack_otel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrastack_otel-0.0.2.tar", last modified: Tue May 21 19:10:10 2024, max compression
+gzip compressed data, was "infrastack_otel-0.0.3.tar", last modified: Thu May 23 01:50:36 2024, max compression
```

## Comparing `infrastack_otel-0.0.2.tar` & `infrastack_otel-0.0.3.tar`

### file list

```diff
@@ -1,80 +1,86 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.774751 infrastack_otel-0.0.2/
--rw-r--r--   0 frank      (501) staff       (20)    11357 2024-05-13 21:33:21.000000 infrastack_otel-0.0.2/LICENSE
--rw-r--r--   0 frank      (501) staff       (20)      756 2024-05-21 19:10:10.774534 infrastack_otel-0.0.2/PKG-INFO
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.774310 infrastack_otel-0.0.2/infrastack_otel.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)      756 2024-05-21 19:10:10.000000 infrastack_otel-0.0.2/infrastack_otel.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)     3284 2024-05-21 19:10:10.000000 infrastack_otel-0.0.2/infrastack_otel.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2024-05-21 19:10:10.000000 infrastack_otel-0.0.2/infrastack_otel.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)       70 2024-05-21 19:10:10.000000 infrastack_otel-0.0.2/infrastack_otel.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       25 2024-05-21 19:10:10.000000 infrastack_otel-0.0.2/infrastack_otel.egg-info/top_level.txt
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.761635 infrastack_otel-0.0.2/opentelemetry/
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.761571 infrastack_otel-0.0.2/opentelemetry/instrumentation/
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.764255 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/
--rw-r--r--   0 frank      (501) staff       (20)    21601 2024-05-19 22:11:18.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)       73 2024-05-19 22:09:11.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/config.py
--rw-r--r--   0 frank      (501) staff       (20)     8374 2024-05-19 22:09:11.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/streaming.py
--rw-r--r--   0 frank      (501) staff       (20)     1093 2024-05-19 22:10:28.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:09:11.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/version.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.765462 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/
--rw-r--r--   0 frank      (501) staff       (20)     3212 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/config.py
--rw-r--r--   0 frank      (501) staff       (20)      701 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/version.py
--rw-r--r--   0 frank      (501) staff       (20)     9794 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/wrapper.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.766966 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/
--rw-r--r--   0 frank      (501) staff       (20)     5739 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/config.py
--rw-r--r--   0 frank      (501) staff       (20)     3043 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/custom_chat_wrapper.py
--rw-r--r--   0 frank      (501) staff       (20)     2190 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
--rw-r--r--   0 frank      (501) staff       (20)     2454 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/task_wrapper.py
--rw-r--r--   0 frank      (501) staff       (20)     2390 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/version.py
--rw-r--r--   0 frank      (501) staff       (20)     2277 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/workflow_wrapper.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.769802 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/
--rw-r--r--   0 frank      (501) staff       (20)     2318 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)     2251 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     2060 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     1960 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     1979 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     2364 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/config.py
--rw-r--r--   0 frank      (501) staff       (20)     5936 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     2102 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     2233 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py
--rw-r--r--   0 frank      (501) staff       (20)     1389 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/version.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.770213 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/
--rw-r--r--   0 frank      (501) staff       (20)     1344 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/__init__.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.771593 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/
--rw-r--r--   0 frank      (501) staff       (20)     7359 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)    16608 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0 frank      (501) staff       (20)     6604 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0 frank      (501) staff       (20)      102 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/config.py
--rw-r--r--   0 frank      (501) staff       (20)     6595 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0 frank      (501) staff       (20)     1891 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py
--rw-r--r--   0 frank      (501) staff       (20)     3357 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/utils.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.771748 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v0/
--rw-r--r--   0 frank      (501) staff       (20)     6116 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v0/__init__.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.772418 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/
--rw-r--r--   0 frank      (501) staff       (20)     8652 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)     5874 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/assistant_wrappers.py
--rw-r--r--   0 frank      (501) staff       (20)     2779 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/version.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.773029 infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/
--rw-r--r--   0 frank      (501) staff       (20)     7480 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/config.py
--rw-r--r--   0 frank      (501) staff       (20)      702 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/version.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.773721 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/
--rw-r--r--   0 frank      (501) staff       (20)     2282 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/config.py
--rw-r--r--   0 frank      (501) staff       (20)     3144 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/text_generation_pipeline_wrapper.py
--rw-r--r--   0 frank      (501) staff       (20)     1018 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/version.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.761687 infrastack_otel-0.0.2/opentelemetry/semconv/
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-21 19:10:10.774128 infrastack_otel-0.0.2/opentelemetry/semconv/ai/
--rw-r--r--   0 frank      (501) staff       (20)     3388 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/semconv/ai/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      728 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/semconv/ai/utils.py
--rw-r--r--   0 frank      (501) staff       (20)       22 2024-05-19 22:02:50.000000 infrastack_otel-0.0.2/opentelemetry/semconv/ai/version.py
--rw-r--r--   0 frank      (501) staff       (20)     1011 2024-05-21 19:08:28.000000 infrastack_otel-0.0.2/pyproject.toml
--rw-r--r--   0 frank      (501) staff       (20)       38 2024-05-21 19:10:10.774786 infrastack_otel-0.0.2/setup.cfg
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.442544 infrastack_otel-0.0.3/
+-rw-r--r--   0 frank      (501) staff       (20)    11357 2024-05-13 21:33:21.000000 infrastack_otel-0.0.3/LICENSE
+-rw-r--r--   0 frank      (501) staff       (20)      818 2024-05-23 01:50:36.442352 infrastack_otel-0.0.3/PKG-INFO
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.442167 infrastack_otel-0.0.3/infrastack_otel.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)      818 2024-05-23 01:50:36.000000 infrastack_otel-0.0.3/infrastack_otel.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)     3529 2024-05-23 01:50:36.000000 infrastack_otel-0.0.3/infrastack_otel.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2024-05-23 01:50:36.000000 infrastack_otel-0.0.3/infrastack_otel.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)      117 2024-05-23 01:50:36.000000 infrastack_otel-0.0.3/infrastack_otel.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       25 2024-05-23 01:50:36.000000 infrastack_otel-0.0.3/infrastack_otel.egg-info/top_level.txt
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.426799 infrastack_otel-0.0.3/opentelemetry/
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.426736 infrastack_otel-0.0.3/opentelemetry/instrumentation/
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.429413 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/
+-rw-r--r--   0 frank      (501) staff       (20)    21605 2024-05-22 21:12:33.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       73 2024-05-19 22:09:11.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     8374 2024-05-19 22:09:11.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/streaming.py
+-rw-r--r--   0 frank      (501) staff       (20)     1093 2024-05-19 22:10:28.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:09:11.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.430621 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/
+-rw-r--r--   0 frank      (501) staff       (20)     3212 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/config.py
+-rw-r--r--   0 frank      (501) staff       (20)      701 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/version.py
+-rw-r--r--   0 frank      (501) staff       (20)     9794 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/wrapper.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.432159 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/
+-rw-r--r--   0 frank      (501) staff       (20)     5739 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     3043 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/custom_chat_wrapper.py
+-rw-r--r--   0 frank      (501) staff       (20)     2190 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
+-rw-r--r--   0 frank      (501) staff       (20)     2454 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/task_wrapper.py
+-rw-r--r--   0 frank      (501) staff       (20)     2390 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/version.py
+-rw-r--r--   0 frank      (501) staff       (20)     2277 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/workflow_wrapper.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.435021 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/
+-rw-r--r--   0 frank      (501) staff       (20)     2318 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)     2251 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     2060 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     1960 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     1979 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     2364 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     5938 2024-05-22 21:12:19.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     2102 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     2233 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py
+-rw-r--r--   0 frank      (501) staff       (20)     1389 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.436224 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/
+-rw-r--r--   0 frank      (501) staff       (20)    21605 2024-05-22 21:12:23.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       73 2024-05-21 22:28:13.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     8374 2024-05-21 22:28:13.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/streaming.py
+-rw-r--r--   0 frank      (501) staff       (20)     1093 2024-05-21 22:28:13.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-21 22:28:13.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/mistral/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.436694 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/
+-rw-r--r--   0 frank      (501) staff       (20)     1344 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/__init__.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.438155 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/
+-rw-r--r--   0 frank      (501) staff       (20)     7361 2024-05-22 21:12:27.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)    16608 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0 frank      (501) staff       (20)     6604 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0 frank      (501) staff       (20)      102 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     6595 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0 frank      (501) staff       (20)     1891 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py
+-rw-r--r--   0 frank      (501) staff       (20)     3357 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/utils.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.438285 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v0/
+-rw-r--r--   0 frank      (501) staff       (20)     6116 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v0/__init__.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.439828 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/
+-rw-r--r--   0 frank      (501) staff       (20)     8652 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)     5874 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/assistant_wrappers.py
+-rw-r--r--   0 frank      (501) staff       (20)     2779 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.440660 infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/
+-rw-r--r--   0 frank      (501) staff       (20)     7480 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/config.py
+-rw-r--r--   0 frank      (501) staff       (20)      702 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.441515 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/
+-rw-r--r--   0 frank      (501) staff       (20)     2282 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)       42 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/config.py
+-rw-r--r--   0 frank      (501) staff       (20)     3146 2024-05-22 21:12:30.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/text_generation_pipeline_wrapper.py
+-rw-r--r--   0 frank      (501) staff       (20)     1018 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       23 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/version.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.426849 infrastack_otel-0.0.3/opentelemetry/semconv/
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-05-23 01:50:36.441986 infrastack_otel-0.0.3/opentelemetry/semconv/ai/
+-rw-r--r--   0 frank      (501) staff       (20)     3322 2024-05-22 21:23:38.000000 infrastack_otel-0.0.3/opentelemetry/semconv/ai/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      728 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/semconv/ai/utils.py
+-rw-r--r--   0 frank      (501) staff       (20)       22 2024-05-19 22:02:50.000000 infrastack_otel-0.0.3/opentelemetry/semconv/ai/version.py
+-rw-r--r--   0 frank      (501) staff       (20)     1064 2024-05-22 21:06:17.000000 infrastack_otel-0.0.3/pyproject.toml
+-rw-r--r--   0 frank      (501) staff       (20)       38 2024-05-23 01:50:36.442579 infrastack_otel-0.0.3/setup.cfg
```

### Comparing `infrastack_otel-0.0.2/LICENSE` & `infrastack_otel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/infrastack_otel.egg-info/SOURCES.txt` & `infrastack_otel-0.0.3/infrastack_otel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py
 opentelemetry/instrumentation/llamaindex/config.py
 opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py
 opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py
 opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py
 opentelemetry/instrumentation/llamaindex/utils.py
 opentelemetry/instrumentation/llamaindex/version.py
+opentelemetry/instrumentation/mistral/__init__.py
+opentelemetry/instrumentation/mistral/config.py
+opentelemetry/instrumentation/mistral/streaming.py
+opentelemetry/instrumentation/mistral/utils.py
+opentelemetry/instrumentation/mistral/version.py
 opentelemetry/instrumentation/openai/__init__.py
 opentelemetry/instrumentation/openai/utils.py
 opentelemetry/instrumentation/openai/version.py
 opentelemetry/instrumentation/openai/shared/__init__.py
 opentelemetry/instrumentation/openai/shared/chat_wrappers.py
 opentelemetry/instrumentation/openai/shared/completion_wrappers.py
 opentelemetry/instrumentation/openai/shared/config.py
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         return wrapped(*args, **kwargs)
 
     name = to_wrap.get("span_name")
     span = tracer.start_span(
         name,
         kind=SpanKind.CLIENT,
         attributes={
-            SpanAttributes.LLM_SYSTEM: "Anthropic",
+            SpanAttributes.LLM_PROVIDER: "Anthropic",
             SpanAttributes.LLM_REQUEST_TYPE: LLMRequestTypeValues.COMPLETION.value,
         },
     )
 
     if span.is_recording():
         _set_input_attributes(span, kwargs)
 
@@ -512,15 +512,15 @@
         return wrapped(*args, **kwargs)
 
     name = to_wrap.get("span_name")
     span = tracer.start_span(
         name,
         kind=SpanKind.CLIENT,
         attributes={
-            SpanAttributes.LLM_SYSTEM: "Anthropic",
+            SpanAttributes.LLM_PROVIDER: "Anthropic",
             SpanAttributes.LLM_REQUEST_TYPE: LLMRequestTypeValues.COMPLETION.value,
         },
     )
     try:
         if span.is_recording():
             _set_input_attributes(span, kwargs)
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/streaming.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/streaming.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/anthropic/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/anthropic/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/chromadb/wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/chromadb/wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/custom_chat_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/custom_chat_wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/custom_llm_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/custom_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/task_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/langchain/workflow_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/langchain/workflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         _handle_response(span, llm_request_type, instance, response)
 
         return response
 
 
 @dont_throw
 def _handle_request(span, llm_request_type, args, kwargs, instance: CustomLLM):
-    _set_span_attribute(span, SpanAttributes.LLM_SYSTEM, instance.__class__.__name__)
+    _set_span_attribute(span, SpanAttributes.LLM_PROVIDER, instance.__class__.__name__)
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TYPE, llm_request_type.value)
     _set_span_attribute(
         span, SpanAttributes.LLM_REQUEST_MODEL, instance.metadata.model_name
     )
     _set_span_attribute(
         span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, instance.metadata.context_window
     )
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/llamaindex/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/llamaindex/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 
 def _set_request_attributes(span, kwargs):
     if not span.is_recording():
         return
 
     _set_api_attributes(span)
-    _set_span_attribute(span, SpanAttributes.LLM_SYSTEM, "OpenAI")
+    _set_span_attribute(span, SpanAttributes.LLM_PROVIDER, "OpenAI")
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MODEL, kwargs.get("model"))
     _set_span_attribute(
         span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, kwargs.get("max_tokens")
     )
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TEMPERATURE, kwargs.get("temperature"))
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TOP_P, kwargs.get("top_p"))
     _set_span_attribute(
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/chat_wrappers.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/completion_wrappers.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v0/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/assistant_wrappers.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/assistant_wrappers.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/pinecone/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/text_generation_pipeline_wrapper.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/text_generation_pipeline_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         prompts_list = kwargs.get("args")
 
     _set_span_prompts(span, prompts_list)
     _set_span_attribute(
         span, SpanAttributes.LLM_REQUEST_MODEL, instance.model.config.name_or_path
     )
     _set_span_attribute(
-        span, SpanAttributes.LLM_SYSTEM, instance.model.config.model_type
+        span, SpanAttributes.LLM_PROVIDER, instance.model.config.model_type
     )
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TYPE, "completion")
     _set_span_attribute(
         span, SpanAttributes.LLM_REQUEST_TEMPERATURE, forward_params.get("temperature")
     )
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TOP_P, forward_params.get("top_p"))
     _set_span_attribute(
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/instrumentation/transformers/utils.py` & `infrastack_otel-0.0.3/opentelemetry/instrumentation/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/opentelemetry/semconv/ai/__init__.py` & `infrastack_otel-0.0.3/opentelemetry/semconv/ai/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 class SpanAttributes:
     # Semantic Conventions for LLM requests, this needs to be removed after
     # OpenTelemetry Semantic Conventions support Gen AI.
     # Issue at https://github.com/open-telemetry/opentelemetry-python/issues/3868
     # Refer to https://github.com/open-telemetry/semantic-conventions/blob/main/docs/gen-ai/llm-spans.md
     # for more detail for LLM spans from OpenTelemetry Community.
-    LLM_SYSTEM = "gen_ai.system"
-    LLM_REQUEST_MODEL = "gen_ai.request.model"
-    LLM_REQUEST_MAX_TOKENS = "gen_ai.request.max_tokens"
-    LLM_REQUEST_TEMPERATURE = "gen_ai.request.temperature"
-    LLM_REQUEST_TOP_P = "gen_ai.request.top_p"
-    LLM_PROMPTS = "gen_ai.prompt"
-    LLM_COMPLETIONS = "gen_ai.completion"
-    LLM_RESPONSE_MODEL = "gen_ai.response.model"
-    LLM_USAGE_COMPLETION_TOKENS = "gen_ai.usage.completion_tokens"
-    LLM_USAGE_PROMPT_TOKENS = "gen_ai.usage.prompt_tokens"
+    LLM_PROVIDER = "llm.provider"
+    LLM_REQUEST_MODEL = "llm.model"
+    LLM_REQUEST_MAX_TOKENS = "llm.request.max_tokens"
+    LLM_REQUEST_TEMPERATURE = "llm.request.temperature"
+    LLM_REQUEST_TOP_P = "llm.top_p"
+    LLM_PROMPTS = "llm.prompt"
+    LLM_COMPLETIONS = "llm.completion"
+    LLM_RESPONSE_MODEL = "llm.response.model"
+    LLM_USAGE_COMPLETION_TOKENS = "llm.completion_tokens"
+    LLM_USAGE_PROMPT_TOKENS = "llm.prompt_tokens"
     # To be added
-    # LLM_RESPONSE_FINISH_REASON = "gen_ai.response.finish_reasons"
-    # LLM_RESPONSE_ID = "gen_ai.response.id"
+    # LLM_RESPONSE_FINISH_REASON = "llm.response.finish_reasons"
+    # LLM_RESPONSE_ID = "llm.response.id"
 
     # LLM
     LLM_REQUEST_TYPE = "llm.request.type"
-    LLM_USAGE_TOTAL_TOKENS = "llm.usage.total_tokens"
+    LLM_USAGE_TOTAL_TOKENS = "llm.total_tokens"
     LLM_USER = "llm.user"
     LLM_HEADERS = "llm.headers"
     LLM_TOP_K = "llm.top_k"
     LLM_IS_STREAMING = "llm.is_streaming"
     LLM_FREQUENCY_PENALTY = "llm.frequency_penalty"
     LLM_PRESENCE_PENALTY = "llm.presence_penalty"
     LLM_CHAT_STOP_SEQUENCES = "llm.chat.stop_sequences"
```

### Comparing `infrastack_otel-0.0.2/opentelemetry/semconv/ai/utils.py` & `infrastack_otel-0.0.3/opentelemetry/semconv/ai/utils.py`

 * *Files identical despite different names*

### Comparing `infrastack_otel-0.0.2/pyproject.toml` & `infrastack_otel-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "infrastack-otel"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Frank Kuehnel", email="hello@infrastack.ai" },
 ]
 maintainers = [
   { name="Frank Kuehnel", email="frank@infrastack.ai" },
   { name="Aykut Gedik", email="hello@infrastack.ai" },
 ]
@@ -15,26 +15,26 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "inflection>=0.4.0",
+    "opentelemetry-exporter-otlp-proto-grpc>=1.24.0",
     "opentelemetry-instrumentation>=0.45b0",
     "wrapt>=1.16.0",
 ]
 
-
 [project.urls]
 Homepage = "https://github.com/infrastackai/otel"
 Issues = "https://github.com/infrastackai/otel/issues"
 
 [metadata]
 name = "infrastack-otel"
-version = "0.0.2"
+version = "0.0.3"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
```

