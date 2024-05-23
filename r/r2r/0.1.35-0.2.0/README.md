# Comparing `tmp/r2r-0.1.35.tar.gz` & `tmp/r2r-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.35.tar", max compression
+gzip compressed data, was "r2r-0.2.0.tar", max compression
```

## Comparing `r2r-0.1.35.tar` & `r2r-0.2.0.tar`

### file list

```diff
@@ -1,88 +1,96 @@
--rw-r--r--   0        0        0     1082 2024-04-17 01:01:26.034450 r2r-0.1.35/LICENSE.md
--rw-r--r--   0        0        0     7421 2024-04-17 01:01:26.034450 r2r-0.1.35/README.md
--rw-r--r--   0        0        0      680 2024-04-17 01:01:26.034450 r2r-0.1.35/config.json
--rw-r--r--   0        0        0     2218 2024-04-17 01:01:26.066450 r2r-0.1.35/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/client/__init__.py
--rw-r--r--   0        0        0     5956 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/client/base.py
--rw-r--r--   0        0        0     1121 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/__init__.py
--rw-r--r--   0        0        0      139 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      781 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2803 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     1654 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     1815 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6227 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0     1015 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1808 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11889 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66651 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3311 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0      139 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/__init__.py
--rw-r--r--   0        0        0     3244 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_basic_client.py
--rw-r--r--   0        0        0     4063 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_basic_client_old.py
--rw-r--r--   0        0        0     1625 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_synthetic_query_client.py
--rw-r--r--   0        0        0      760 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_embedding_qdrant.json
--rw-r--r--   0        0        0      689 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_llama_cpp.json
--rw-r--r--   0        0        0      687 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_ollama.json
--rw-r--r--   0        0        0   802904 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/data/meditations.pdf
--rw-r--r--   0        0        0    14812 2024-04-17 01:01:26.074450 r2r-0.1.35/r2r/examples/data/test.pdf
--rw-r--r--   0        0        0  1307590 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/data/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/basic_pipeline.py
--rw-r--r--   0        0        0      529 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/reducto_pipeline.py
--rw-r--r--   0        0        0     6746 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/synthetic_query_pipeline.py
--rw-r--r--   0        0        0      479 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/web_search_pipeline.py
--rw-r--r--   0        0        0      147 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1571 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3905 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/serper.py
--rw-r--r--   0        0        0      277 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     4467 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/llama_cpp/base.py
--rw-r--r--   0        0        0        0 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/__init__.py
--rw-r--r--   0        0        0    16309 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/app.py
--rw-r--r--   0        0        0     5108 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/factory.py
--rw-r--r--   0        0        0     3278 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/models.py
--rw-r--r--   0        0        0    10941 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/utils.py
--rw-r--r--   0        0        0      493 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     6331 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1830 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     3059 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3080 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     3766 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5299 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9298 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/client.py
--rw-r--r--   0        0        0    35441 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5919 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9880 1970-01-01 00:00:00.000000 r2r-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-23 09:52:58.844723 r2r-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0    12944 2024-05-23 09:52:58.844723 r2r-0.2.0/README.md
+-rw-r--r--   0        0        0     1181 2024-05-23 09:52:58.844723 r2r-0.2.0/config.json
+-rw-r--r--   0        0        0     1980 2024-05-23 09:52:58.864723 r2r-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2047 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/__init__.py
+-rw-r--r--   0        0        0     3083 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      186 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/llm.py
+-rw-r--r--   0        0        0     1083 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/prompt.py
+-rw-r--r--   0        0        0      813 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/search.py
+-rw-r--r--   0        0        0     1934 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/vector.py
+-rw-r--r--   0        0        0      538 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/base_parser.py
+-rw-r--r--   0        0        0    14096 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/parser_impls.py
+-rw-r--r--   0        0        0     9066 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0     3803 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/base_pipe.py
+-rw-r--r--   0        0        0     2215 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/loggable_pipe.py
+-rw-r--r--   0        0        0    16417 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/pipe_logging.py
+-rw-r--r--   0        0        0     1306 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/base_provider.py
+-rw-r--r--   0        0        0     2267 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/embedding_provider.py
+-rw-r--r--   0        0        0     1306 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/eval_provider.py
+-rw-r--r--   0        0        0     2345 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/llm_provider.py
+-rw-r--r--   0        0        0     1456 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/prompt_provider.py
+-rw-r--r--   0        0        0     2550 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/vector_db_provider.py
+-rw-r--r--   0        0        0      363 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/base_utils.py
+-rw-r--r--   0        0        0       95 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66643 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      332 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     2363 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/dummy/provider.py
+-rw-r--r--   0        0        0     6309 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/openai/openai_base.py
+-rw-r--r--   0        0        0     6238 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/setence_transformer/sentence_transformer_base.py
+-rw-r--r--   0        0        0       78 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/eval/llm/base_llm_eval.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/__init__.py
+-rw-r--r--   0        0        0     3067 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/custom_rag.py
+-rw-r--r--   0        0        0    73353 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/aristotle.txt
+-rw-r--r--   0        0        0       49 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_postgres_logger_config.json
+-rw-r--r--   0        0        0       91 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_qdrant_config.json
+-rw-r--r--   0        0        0      455 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_rerank_config.json
+-rw-r--r--   0        0        0  1440303 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/lyft_2021.pdf
+-rw-r--r--   0        0        0   131542 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_1.html
+-rw-r--r--   0        0        0   125150 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_2.html
+-rw-r--r--   0        0        0   124948 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_3.html
+-rw-r--r--   0        0        0   118147 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_4.html
+-rw-r--r--   0        0        0   123820 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_5.html
+-rw-r--r--   0        0        0   791764 2024-05-23 09:52:58.876723 r2r-0.2.0/r2r/examples/data/screen_shot.png
+-rw-r--r--   0        0        0       19 2024-05-23 09:52:58.876723 r2r-0.2.0/r2r/examples/data/test.txt
+-rw-r--r--   0        0        0  1880483 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/data/uber_2021.pdf
+-rw-r--r--   0        0        0    11969 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/demo.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1569 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/servers/configurable_pipeline.py
+-rw-r--r--   0        0        0      147 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1535 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3940 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      232 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3315 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/litellm/base_litellm.py
+-rw-r--r--   0        0        0     3919 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/llama_cpp/base_llama_cpp.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3462 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/openai/base_openai.py
+-rw-r--r--   0        0        0      410 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/__init__.py
+-rw-r--r--   0        0        0     1102 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_abstractions.py
+-rw-r--r--   0        0        0    23069 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_app.py
+-rw-r--r--   0        0        0     5529 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_client.py
+-rw-r--r--   0        0        0     4632 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_config.py
+-rw-r--r--   0        0        0    11331 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_factory.py
+-rw-r--r--   0        0        0      593 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/__init__.py
+-rw-r--r--   0        0        0     1266 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/abstractions/generator_pipe.py
+-rw-r--r--   0        0        0     1588 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/abstractions/search_pipe.py
+-rw-r--r--   0        0        0     7244 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/embedding_pipe.py
+-rw-r--r--   0        0        0     1407 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/eval_pipe.py
+-rw-r--r--   0        0        0     7590 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/parsing_pipe.py
+-rw-r--r--   0        0        0     3050 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/query_transform_pipe.py
+-rw-r--r--   0        0        0     2738 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/rag_pipe.py
+-rw-r--r--   0        0        0     3317 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/streaming_rag_pipe.py
+-rw-r--r--   0        0        0     2798 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/vector_search_pipe.py
+-rw-r--r--   0        0        0     3073 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/vector_storage_pipe.py
+-rw-r--r--   0        0        0       90 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/__init__.py
+-rw-r--r--   0        0        0     4390 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/defaults.jsonl
+-rw-r--r--   0        0        0     1900 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/r2r_prompt_provider.py
+-rw-r--r--   0        0        0      539 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3263 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5317 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9350 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/client.py
+-rw-r--r--   0        0        0    36863 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      213 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     6379 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/local/r2r_local_vector_db.py
+-rw-r--r--   0        0        0     6268 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/pgvector/pgvector_db.py
+-rw-r--r--   0        0        0     7412 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/qdrant/qdrant_db.py
+-rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.0/PKG-INFO
```

### Comparing `r2r-0.1.35/LICENSE.md` & `r2r-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/client/base.py` & `r2r-0.2.0/r2r/main/r2r_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,166 @@
+"""Module for the R2RClient class."""
+
+import asyncio
 import json
-from typing import Any, Dict, List, Optional, Union
+from typing import AsyncGenerator, Generator, Optional, Union
 
 import httpx
+import nest_asyncio
 import requests
 
+nest_asyncio.apply()
+
 
 class R2RClient:
     def __init__(self, base_url: str):
         self.base_url = base_url
 
-    def upload_and_process_file(
-        self,
-        document_id: str,
-        file_path: str,
-        metadata: Optional[dict] = None,
-        settings: Optional[dict] = None,
-    ):
-        url = f"{self.base_url}/upload_and_process_file/"
-        with open(file_path, "rb") as file:
-            files = {
-                "file": (file_path.split("/")[-1], file, "application/pdf")
-            }
-            data = {
-                "document_id": document_id,
-                "metadata": (
-                    json.dumps(metadata) if metadata else json.dumps({})
-                ),
-                "settings": (
-                    json.dumps(settings) if settings else json.dumps({})
-                ),
-            }
-            response = requests.post(
-                url,
-                files=files,
-                data=data,
-            )
-        return response.json()
-
-    def add_entry(
-        self,
-        document_id: str,
-        blobs: Dict[str, str],
-        metadata: Optional[Dict[str, Any]] = None,
-        do_upsert: Optional[bool] = False,
-        settings: Optional[Dict[str, Any]] = None,
-    ):
-        url = f"{self.base_url}/add_entry/"
-        json_data = {
-            "entry": {
-                "document_id": document_id,
-                "blobs": blobs,
-                "metadata": metadata or {},
-            },
-            "settings": settings
-            or {"embedding_settings": {"do_upsert": do_upsert}},
-        }
-        response = requests.post(url, json=json_data)
-        return response.json()
-
-    def add_entries(
-        self,
-        entries: List[Dict[str, Any]],
-        do_upsert: Optional[bool] = False,
-        settings: Optional[Dict[str, Any]] = None,
-    ):
-        url = f"{self.base_url}/add_entries/"
-        json_data = {
-            "entries": entries,
-            "settings": settings
-            or {"embedding_settings": {"do_upsert": do_upsert}},
+    def ingest_documents(self, documents: list[dict]) -> dict:
+        url = f"{self.base_url}/ingest_documents/"
+        data = {"documents": documents}
+        response = requests.post(url, json=data)
+        response.raise_for_status()
+        return response.json()
+
+    def ingest_files(
+        self,
+        metadatas: list[dict],
+        files: list[str],
+        ids: Optional[list[str]] = None,
+    ) -> dict:
+        url = f"{self.base_url}/ingest_files/"
+        files_to_upload = [
+            ("files", (file, open(file, "rb"), "application/octet-stream"))
+            for file in files
+        ]
+        data = {
+            "metadatas": None if not metadatas else json.dumps(metadatas),
+            "ids": None if not ids else json.dumps(ids),
         }
-        response = requests.post(url, json=json_data)
+        response = requests.post(url, files=files_to_upload, data=data)
+        response.raise_for_status()
         return response.json()
 
     def search(
-        self,
-        query: str,
-        limit: Optional[int] = 10,
-        filters: Optional[Dict[str, Any]] = None,
-        settings: Optional[Dict[str, Any]] = None,
-    ):
+        self, query: str, search_filters: dict = {}, search_limit: int = 10
+    ) -> dict:
         url = f"{self.base_url}/search/"
-        json_data = {
+        data = {
             "query": query,
-            "filters": filters or {},
-            "limit": limit,
-            "settings": settings or {},
+            "search_filters": json.dumps(search_filters),
+            "search_limit": search_limit,
         }
-        response = requests.post(url, json=json_data)
+        response = requests.post(url, json=data)
+        response.raise_for_status()
         return response.json()
 
-    # TODO - Cleanup redundant code in the following methods
-    # TODO - Consider how to improve `rag_completion` and
-    # `stream_rag_completion` workflows.
-    def rag_completion(
+    def rag(
         self,
-        query: str,
-        limit: Optional[int] = 10,
-        filters: Optional[Dict[str, Any]] = None,
-        settings: Optional[Dict[str, Any]] = None,
-        generation_config: Optional[Dict[str, Any]] = None,
-    ):
-        if not generation_config:
-            generation_config = {}
-        stream = generation_config.get("stream", False)
-
-        if stream:
-            raise ValueError(
-                "To stream, use the `stream_rag_completion` method."
+        message: str,
+        search_filters: Optional[dict] = None,
+        search_limit: int = 10,
+        rag_generation_config: Optional[dict] = None,
+        streaming: bool = False,
+    ) -> Union[dict, Generator[str, None, None]]:
+        if streaming:
+            return self._stream_rag_sync(
+                message=message,
+                search_filters=search_filters,
+                search_limit=search_limit,
+                rag_generation_config=rag_generation_config,
             )
-
-        url = f"{self.base_url}/rag_completion/"
-        json_data = {
-            "query": query,
-            "filters": filters or {},
-            "limit": limit,
-            "settings": settings or {},
-            "generation_config": generation_config or {},
-        }
-        response = requests.post(url, json=json_data)
-        return response.json()
-
-    def eval(
-        self,
-        query: str,
-        context: str,
-        completion_text: str,
-        run_id: str,
-        settings: Optional[Dict[str, Any]] = None,
-    ):
-        url = f"{self.base_url}/eval/"
-        payload = {
-            "query": query,
-            "context": context,
-            "completion_text": completion_text,
-            "run_id": run_id,
-            "settings": settings or {},
-        }
-        response = requests.post(url, json=payload)
-        return response.json()
-
-    async def stream_rag_completion(
-        self,
-        query: str,
-        limit: Optional[int] = 10,
-        filters: Optional[Dict[str, Any]] = None,
-        settings: Optional[Dict[str, Any]] = None,
-        generation_config: Optional[Dict[str, Any]] = None,
-    ):
-        if not generation_config:
-            generation_config = {}
-        stream = generation_config.get("stream", False)
-        if not stream:
-            raise ValueError(
-                "`stream_rag_completion` method is only for streaming."
-            )
-
-        url = f"{self.base_url}/rag_completion/"
-
-        headers = {
-            "accept": "application/json",
-            "Content-Type": "application/json",
-        }
-        json_data = {
-            "query": query,
-            "filters": filters or {},
-            "limit": limit,
-            "settings": settings or {},
-            "generation_config": generation_config or {},
+        else:
+            url = f"{self.base_url}/rag/"
+            data = {
+                "message": message,
+                "search_filters": json.dumps(search_filters or {}),
+                "search_limit": search_limit,
+                "streaming": streaming,
+            }
+            if rag_generation_config:
+                data["rag_generation_config"] = json.dumps(
+                    rag_generation_config
+                )
+            response = requests.post(url, json=data)
+            response.raise_for_status()
+            return response.json()
+
+    async def _stream_rag(
+        self,
+        message: str,
+        search_filters: Optional[dict] = None,
+        search_limit: int = 10,
+        rag_generation_config: Optional[dict] = None,
+    ) -> Generator[str, None, None]:
+        url = f"{self.base_url}/rag/"
+        data = {
+            "message": message,
+            "search_filters": json.dumps(search_filters or {}),
+            "search_limit": search_limit,
+            "streaming": True,
         }
-
+        if rag_generation_config:
+            data["rag_generation_config"] = json.dumps(rag_generation_config)
         async with httpx.AsyncClient() as client:
-            async with client.stream(
-                "POST", url, headers=headers, json=json_data
-            ) as response:
-                async for chunk in response.aiter_bytes():
-                    yield chunk.decode()
-
-    def filtered_deletion(self, key: str, value: Union[bool, int, str]):
-        url = f"{self.base_url}/filtered_deletion/"
-        response = requests.delete(url, params={"key": key, "value": value})
+            async with client.stream("POST", url, json=data) as response:
+                response.raise_for_status()
+                async for chunk in response.aiter_text():
+                    yield chunk
+
+    def _stream_rag_sync(
+        self,
+        message: str,
+        search_filters: Optional[dict] = None,
+        search_limit: int = 10,
+        rag_generation_config: Optional[dict] = None,
+    ) -> Generator[str, None, None]:
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        async_gen = self._stream_rag(
+            message=message,
+            search_filters=search_filters,
+            search_limit=search_limit,
+            rag_generation_config=rag_generation_config,
+        )
+        for chunk in loop.run_until_complete(
+            self._iterate_async_gen(async_gen)
+        ):
+            yield chunk
+
+    async def _iterate_async_gen(
+        self, async_gen: AsyncGenerator[str, None]
+    ) -> list[str]:
+        chunks = []
+        async for chunk in async_gen:
+            chunks.append(chunk)
+        return chunks
+
+    def delete(self, key: str, value: str) -> dict:
+        url = f"{self.base_url}/delete/"
+        data = {"key": key, "value": value}
+        response = requests.request("DELETE", url, json=data)
+        response.raise_for_status()
         return response.json()
 
-    def get_logs(self):
-        url = f"{self.base_url}/logs"
+    def get_user_ids(self) -> dict:
+        url = f"{self.base_url}/get_user_ids/"
         response = requests.get(url)
+        response.raise_for_status()
         return response.json()
 
-    def get_logs_summary(self):
-        url = f"{self.base_url}/logs_summary"
-        response = requests.get(url)
+    def get_user_document_data(self, user_id: str) -> dict:
+        url = f"{self.base_url}/get_user_document_data/"
+        data = {"user_id": user_id}
+        response = requests.post(url, json=data)
+        response.raise_for_status()
+        response_json = response.json()
+        return response_json
+
+    def get_logs(
+        self, pipeline_type: Optional[str] = None, filter: Optional[str] = None
+    ) -> dict:
+        url = f"{self.base_url}/get_logs/"
+        data = {"pipeline_type": pipeline_type, "filter": filter}
+        response = requests.post(url, json=data)
+        response.raise_for_status()
         return response.json()
```

### Comparing `r2r-0.1.35/r2r/core/providers/embedding.py` & `r2r-0.2.0/r2r/core/providers/base_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,48 @@
-from abc import ABC, abstractmethod
-from typing import Optional
+from abc import ABC, abstractmethod, abstractproperty
+from typing import Any, Optional, Type
 
+from pydantic import BaseModel
 
-class EmbeddingProvider(ABC):
-    supported_providers = ["openai", "sentence-transformers"]
 
-    def __init__(self, provider: str):
-        if provider not in EmbeddingProvider.supported_providers:
-            raise ValueError(
-                f"Error, `{provider}` is not in EmbeddingProvider's list of supported providers."
-            )
+class ProviderConfig(BaseModel, ABC):
+    """A base provider configuration class"""
 
-    @abstractmethod
-    def _check_inputs(self, model: str, dimensions: Optional[int]) -> None:
-        pass
+    extra_fields: dict[str, Any] = {}
+    provider: Optional[str] = None
 
-    @abstractmethod
-    def get_embedding(
-        self, text: str, model: str, dimensions: Optional[int] = None
-    ):
-        pass
+    class Config:
+        arbitrary_types_allowed = True
+        ignore_extra = True
 
     @abstractmethod
-    def get_embeddings(
-        self, texts: list[str], model: str, dimensions: Optional[int] = None
-    ):
+    def validate(self) -> None:
         pass
 
-    @abstractmethod
-    def tokenize_string(self, text: str, model: str) -> list[int]:
-        """Tokenizes the input string."""
+    @classmethod
+    def create(cls: Type["ProviderConfig"], **kwargs: Any) -> "ProviderConfig":
+        base_args = cls.__fields__.keys()
+        filtered_kwargs = {
+            k: v if v != "None" else None
+            for k, v in kwargs.items()
+            if k in base_args
+        }
+        instance = cls(**filtered_kwargs)
+        for k, v in kwargs.items():
+            if k not in base_args:
+                instance.extra_fields[k] = v
+        return instance
+
+    @abstractproperty
+    @property
+    def supported_providers(self) -> list[str]:
+        """Define a list of supported providers."""
         pass
+
+
+class Provider(ABC):
+    """A base provider class to provide a common interface for all providers."""
+
+    def __init__(self, config: Optional[ProviderConfig] = None):
+        if config:
+            config.validate()
+        self.config = config
```

### Comparing `r2r-0.1.35/r2r/core/providers/llm.py` & `r2r-0.2.0/r2r/core/providers/llm_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 """Base classes for language model providers."""
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field, fields
+import logging
+from abc import abstractmethod
 from typing import Optional
 
-from openai.types.chat import ChatCompletion, ChatCompletionChunk
+from pydantic import BaseModel
 
+from ..abstractions.llm import LLMChatCompletion, LLMChatCompletionChunk
+from .base_provider import Provider, ProviderConfig
 
-@dataclass
-class LLMConfig(ABC):
-    provider: Optional[str] = None
-    version: str = "0.1.0"
-
-    @classmethod
-    def create(cls, **kwargs):
-        valid_keys = {f.name for f in fields(cls)}
-        filtered_kwargs = {k: v for k, v in kwargs.items() if k in valid_keys}
-        return cls(**filtered_kwargs)
+logger = logging.getLogger(__name__)
 
 
-@dataclass
-class GenerationConfig(ABC):
+class GenerationConfig(BaseModel):
     temperature: float = 0.1
     top_p: float = 1.0
     top_k: int = 100
     max_tokens_to_sample: int = 1_024
     model: Optional[str] = None
     stream: bool = False
     functions: Optional[list[dict]] = None
     skip_special_tokens: bool = False
     stop_token: Optional[str] = None
     num_beams: int = 1
     do_sample: bool = True
     # Additional args to pass to the generation config
-    add_generation_kwargs: dict = field(default_factory=dict)
     generate_with_chat: bool = False
+    add_generation_kwargs: Optional[dict] = {}
     api_base: Optional[str] = None
 
 
-class LLMProvider(ABC):
+class LLMConfig(ProviderConfig):
+    """A base LLM config class"""
+
+    provider: Optional[str] = None
+
+    def validate(self) -> None:
+        if not self.provider:
+            raise ValueError("Provider must be set.")
+
+        if self.provider and self.provider not in self.supported_providers:
+            raise ValueError(f"Provider '{self.provider}' is not supported.")
+
+    @property
+    def supported_providers(self) -> list[str]:
+        return ["litellm", "llama-cpp", "openai"]
+
+
+class LLMProvider(Provider):
     """An abstract class to provide a common interface for LLMs."""
 
     def __init__(
         self,
+        config: LLMConfig,
     ) -> None:
-        pass
+        if not isinstance(config, LLMConfig):
+            raise ValueError(
+                "LLMProvider must be initialized with a `LLMConfig`."
+            )
+        logger.info(f"Initializing LLM provider with config: {config}")
+
+        super().__init__(config)
 
     @abstractmethod
     def get_completion(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> ChatCompletion:
+    ) -> LLMChatCompletion:
         """Abstract method to get a chat completion from the provider."""
         pass
 
     @abstractmethod
     def get_completion_stream(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> ChatCompletionChunk:
+    ) -> LLMChatCompletionChunk:
         """Abstract method to get a completion stream from the provider."""
         pass
```

### Comparing `r2r-0.1.35/r2r/core/utils/splitter/text.py` & `r2r-0.2.0/r2r/core/utils/splitter/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,30 +380,30 @@
         """
         raise NotImplementedError("This method is not implemented.")
         # return await langchain_core.runnables.config.run_in_executor(
         #     None, self.transform_documents, documents, **kwargs
         # )
 
 
-def _make_spacy_pipeline_for_splitting(
-    pipeline: str, *, max_length: int = 1_000_000
+def _make_spacy_pipe_for_splitting(
+    pipe: str, *, max_length: int = 1_000_000
 ) -> Any:  # avoid importing spacy
     try:
         import spacy
     except ImportError:
         raise ImportError(
             "Spacy is not installed, please install it with `pip install spacy`."
         )
-    if pipeline == "sentencizer":
+    if pipe == "sentencizer":
         from spacy.lang.en import English
 
         sentencizer = English()
         sentencizer.add_pipe("sentencizer")
     else:
-        sentencizer = spacy.load(pipeline, exclude=["ner", "tagger"])
+        sentencizer = spacy.load(pipe, exclude=["ner", "tagger"])
         sentencizer.max_length = max_length
     return sentencizer
 
 
 def _split_text_with_regex(
     text: str, separator: str, keep_separator: bool
 ) -> List[str]:
@@ -1128,15 +1128,15 @@
             raise ImportError(
                 "Could not import sentence_transformer python package. "
                 "This is needed in order to for SentenceTransformersTokenTextSplitter. "
                 "Please install it with `pip install sentence-transformers`."
             )
 
         self.model = model
-        self._model = SentenceTransformer(self.model)
+        self._model = SentenceTransformer(self.model, trust_remote_code=True)
         self.tokenizer = self._model.tokenizer
         self._initialize_chunk_configuration(tokens_per_chunk=tokens_per_chunk)
 
     def _initialize_chunk_configuration(
         self, *, tokens_per_chunk: Optional[int]
     ) -> None:
         self.maximum_tokens_per_chunk = cast(int, self._model.max_seq_length)
@@ -1772,28 +1772,28 @@
 class SpacyTextSplitter(TextSplitter):
     """Splitting text using Spacy package.
 
 
     Per default, Spacy's `en_core_web_sm` model is used and
     its default max_length is 1000000 (it is the length of maximum character
     this model takes which can be increased for large files). For a faster, but
-    potentially less accurate splitting, you can use `pipeline='sentencizer'`.
+    potentially less accurate splitting, you can use `pipe='sentencizer'`.
     """
 
     def __init__(
         self,
         separator: str = "\n\n",
-        pipeline: str = "en_core_web_sm",
+        pipe: str = "en_core_web_sm",
         max_length: int = 1_000_000,
         **kwargs: Any,
     ) -> None:
         """Initialize the spacy text splitter."""
         super().__init__(**kwargs)
-        self._tokenizer = _make_spacy_pipeline_for_splitting(
-            pipeline, max_length=max_length
+        self._tokenizer = _make_spacy_pipe_for_splitting(
+            pipe, max_length=max_length
         )
         self._separator = separator
 
     def split_text(self, text: str) -> List[str]:
         """Split incoming text and return chunks."""
         splits = (s.text for s in self._tokenizer(text).sents)
         return self._merge_splits(splits, self._separator)
```

### Comparing `r2r-0.1.35/r2r/integrations/exa.py` & `r2r-0.2.0/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/integrations/ionic.py` & `r2r-0.2.0/r2r/integrations/ionic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import os
 from typing import Optional
 
 
 class IonicClient:
     def __init__(self, api_key: str = os.getenv("IONIC_API_KEY")) -> None:
         if not api_key:
@@ -17,23 +16,20 @@
 
     def query(
         self,
         query: str,
         num_results: Optional[int] = 10,
     ):
         # temp local import for dependency mgmt
-        from ionic.models.components import QueryAPIRequest
         from ionic.models.components import Query as SDKQuery
+        from ionic.models.components import QueryAPIRequest
         from ionic.models.operations import QueryResponse, QuerySecurity
 
         request = QueryAPIRequest(
-            query=SDKQuery(
-                query=query,
-                num_results=num_results
-            )
+            query=SDKQuery(query=query, num_results=num_results)
         )
 
         response: QueryResponse = self.client.query(
             request=request,
             security=QuerySecurity(),
         )
 
@@ -41,13 +37,12 @@
             {
                 "name": product.name,
                 "price": product.price,
                 "brand_name": product.brand_name,
                 "upc": product.upc,
                 "merchant_name": product.merchant_name,
                 "thumbnail": product.thumbnail,
-'link': product.links[0].url if product.links else None,
+                "link": product.links[0].url if product.links else None,
             }
             for result in response.query_api_response.results
             for product in result.products
         ]
-
```

### Comparing `r2r-0.1.35/r2r/integrations/serper.py` & `r2r-0.2.0/r2r/integrations/serper.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 formatted_results.append(value)
 
         return formatted_results
 
     # TODO - Add explicit typing for the return value
     def get_raw(self, query: str, limit: int = 10) -> list:
         connection = http.client.HTTPSConnection(self.api_base)
-        payload = json.dumps({"q": query, "num": limit})
+        payload = json.dumps({"q": query, "num_outputs": limit})
         connection.request("POST", "/search", payload, self.headers)
         response = connection.getresponse()
         data = response.read()
         json_data = json.loads(data.decode("utf-8"))
         return SerperClient._extract_results(json_data)
 
     @staticmethod
     def construct_context(results: list) -> str:
         # Organize results by type
         organized_results = {}
         for result in results:
-            result_type = result.pop(
+            result_type = result.metadata.pop(
                 "type", "Unknown"
             )  # Pop the type and use as key
             if result_type not in organized_results:
-                organized_results[result_type] = [result]
+                organized_results[result_type] = [result.metadata]
             else:
-                organized_results[result_type].append(result)
+                organized_results[result_type].append(result.metadata)
 
         context = ""
         # Iterate over each result type
         for result_type, items in organized_results.items():
             context += f"# {result_type} Results:\n"
             for index, item in enumerate(items, start=1):
                 # Process each item under the current type
```

### Comparing `r2r-0.1.35/r2r/llms/litellm/base.py` & `r2r-0.2.0/r2r/llms/litellm/base_litellm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,97 @@
 import logging
-from dataclasses import dataclass
 from typing import Any, Generator, Union
 
-from openai.types.chat import ChatCompletion, ChatCompletionChunk
-
-from r2r.core import GenerationConfig, LLMConfig, LLMProvider
+from r2r.core import (
+    GenerationConfig,
+    LLMChatCompletion,
+    LLMChatCompletionChunk,
+    LLMConfig,
+    LLMProvider,
+)
 
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class LiteLLMConfig(LLMConfig):
-    """Configuration for LiteLLM models."""
-
-    provider_name: str = "litellm"
-
-
 class LiteLLM(LLMProvider):
     """A concrete class for creating LiteLLM models."""
 
     def __init__(
         self,
-        config: LiteLLMConfig,
+        config: LLMConfig,
         *args,
         **kwargs,
     ) -> None:
-        logger.info(f"Initializing `LiteLLM` with config: {config}")
-        super().__init__()
-
-        if not isinstance(config, LiteLLMConfig):
-            raise ValueError(
-                "The provided config must be an instance of LiteLLMConfig."
-            )
-        self.config: LiteLLMConfig = config
-
         try:
             from litellm import completion
 
             self.litellm_completion = completion
         except ImportError:
             raise ImportError(
                 "Error, `litellm` is required to run a LiteLLM. Please install it using `pip install litellm`."
             )
+        super().__init__(config)
 
     def get_completion(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> ChatCompletion:
+    ) -> LLMChatCompletion:
         if generation_config.stream:
             raise ValueError(
                 "Stream must be set to False to use the `get_completion` method."
             )
         return self._get_completion(messages, generation_config, **kwargs)
 
     def get_completion_stream(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> Generator[ChatCompletionChunk, None, None]:
+    ) -> Generator[LLMChatCompletionChunk, None, None]:
         if not generation_config.stream:
             raise ValueError(
                 "Stream must be set to True to use the `get_completion_stream` method."
             )
         return self._get_completion(messages, generation_config, **kwargs)
 
+    def extract_content(self, response: LLMChatCompletion) -> str:
+        return response.choices[0].message.content
+
     def _get_completion(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> Union[ChatCompletion, Generator[ChatCompletionChunk, None, None]]:
+    ) -> Union[
+        LLMChatCompletion, Generator[LLMChatCompletionChunk, None, None]
+    ]:
         # Create a dictionary with the default arguments
         args = self._get_base_args(generation_config)
         args["messages"] = messages
 
         # Conditionally add the 'functions' argument if it's not None
         if generation_config.functions is not None:
             args["functions"] = generation_config.functions
 
         args = {**args, **kwargs}
         response = self.litellm_completion(**args)
 
         if not generation_config.stream:
-            return ChatCompletion(**response.dict())
+            return LLMChatCompletion(**response.dict())
         else:
             return self._get_chat_completion(response)
 
     def _get_chat_completion(
         self,
         response: Any,
-    ) -> Generator[ChatCompletionChunk, None, None]:
+    ) -> Generator[LLMChatCompletionChunk, None, None]:
         for part in response:
-            yield ChatCompletionChunk(**part.dict())
+            yield LLMChatCompletionChunk(**part.dict())
 
     def _get_base_args(
         self,
         generation_config: GenerationConfig,
         prompt=None,
     ) -> dict:
         """Get the base arguments for the LiteLLM API."""
```

### Comparing `r2r-0.1.35/r2r/llms/llama_cpp/base.py` & `r2r-0.2.0/r2r/llms/openai/base_openai.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,109 @@
-"""A module for creating LlamaCpp model abstractions."""
+"""A module for creating OpenAI model abstractions."""
 
-import datetime
 import logging
 import os
-from dataclasses import dataclass
 from typing import Union
 
-from openai.types.chat import ChatCompletion, ChatCompletionChunk
-
-from r2r.core import GenerationConfig, LLMConfig, LLMProvider
+from r2r.core import (
+    GenerationConfig,
+    LLMChatCompletion,
+    LLMChatCompletionChunk,
+    LLMConfig,
+    LLMProvider,
+)
 
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class LlamaCppConfig(LLMConfig):
-    """Configuration for LlamaCpp models."""
-
-    # Base
-    provider_name: str = "llama-cpp"
-    model_path: str = ""
-    model_name: str = ""
-
-    def __post_init__(self):
-        if not self.model_path or self.model_path == "":
-            self.model_path = os.path.join(
-                os.path.expanduser("~"), ".cache", "models"
-            )
-        if not self.model_name or self.model_name == "":
-            self.model_name = "tinyllama-1.1b-chat-v1.0.Q2_K.gguf"
-
-
-class LlamaCPP(LLMProvider):
-    """A concrete class for creating LlamaCpp models."""
+class OpenAILLM(LLMProvider):
+    """A concrete class for creating OpenAI models."""
 
     def __init__(
         self,
-        config: LlamaCppConfig,
+        config: LLMConfig,
         *args,
         **kwargs,
     ) -> None:
-        logger.info(f"Initializing `LlamaCPP` with config: {config}")
-        super().__init__()
-
-        if not isinstance(config, LlamaCppConfig):
+        if not isinstance(config, LLMConfig):
             raise ValueError(
-                "The provided config must be an instance of LlamaCppConfig."
+                "The provided config must be an instance of OpenAIConfig."
             )
-
-        self.config: LlamaCppConfig = config
-
         try:
-            from llama_cpp import Llama
+            from openai import OpenAI  # noqa
         except ImportError:
             raise ImportError(
-                "Error, `llama-cpp-python` is required to run a LlamaCPP. Please install it using `pip install llama-cpp-python`."
+                "Error, `openai` is required to run an OpenAILLM. Please install it using `pip install openai`."
             )
-
-        path = os.path.join(self.config.model_path, self.config.model_name)
-        self.client = Llama(path, n_ctx=2048)
+        if config.provider != "openai":
+            raise ValueError(
+                "OpenAILLM must be initialized with config with `openai` provider."
+            )
+        if not os.getenv("OPENAI_API_KEY"):
+            raise ValueError(
+                "OpenAI API key not found. Please set the OPENAI_API_KEY environment variable."
+            )
+        super().__init__(config)
+        self.config: LLMConfig = config
+        self.client = OpenAI()
 
     def get_completion(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> ChatCompletion:
+    ) -> LLMChatCompletion:
         if generation_config.stream:
             raise ValueError(
                 "Stream must be set to False to use the `get_completion` method."
             )
         return self._get_completion(messages, generation_config, **kwargs)
 
     def get_completion_stream(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> ChatCompletionChunk:
+    ) -> LLMChatCompletionChunk:
         if not generation_config.stream:
             raise ValueError(
                 "Stream must be set to True to use the `get_completion_stream` method."
             )
         return self._get_completion(messages, generation_config, **kwargs)
 
     def _get_completion(
         self,
         messages: list[dict],
         generation_config: GenerationConfig,
         **kwargs,
-    ) -> Union[ChatCompletion, ChatCompletionChunk]:
-        """Get a completion from the LlamaCpp model based on the provided messages."""
+    ) -> Union[LLMChatCompletion, LLMChatCompletionChunk]:
+        """Get a completion from the OpenAI API based on the provided messages."""
 
+        # Create a dictionary with the default arguments
         args = self._get_base_args(generation_config)
 
-        prompt = "\n".join([msg["content"] for msg in messages])
-
-        response = self.client(prompt, **args)
+        args["messages"] = messages
 
-        if not generation_config.stream:
-            return ChatCompletion(
-                # TODO - Set an intelligent id
-                id="777",
-                object="chat.completion",
-                created=int(datetime.datetime.now().timestamp()),
-                model=generation_config.model,
-                choices=[
-                    {
-                        "message": {
-                            "role": "assistant",
-                            "content": str(response),
-                        },
-                        "index": 0,
-                        "finish_reason": "stop",
-                    }
-                ],
-            )
-        else:
-            return ChatCompletionChunk(
-                choices=[
-                    {
-                        "message": {
-                            "role": "assistant",
-                            "content": str(response),
-                        },
-                        "index": 0,
-                        "finish_reason": None,
-                    }
-                ],
-                **kwargs,
-            )
+        # Conditionally add the 'functions' argument if it's not None
+        if generation_config.functions is not None:
+            args["functions"] = generation_config.functions
+
+        args = {**args, **kwargs}
+        # Create the chat completion
+        return self.client.chat.completions.create(**args)
 
     def _get_base_args(
         self,
         generation_config: GenerationConfig,
     ) -> dict:
-        """Get the base arguments for the LlamaCpp model."""
+        """Get the base arguments for the OpenAI API."""
+
         args = {
+            "model": generation_config.model,
             "temperature": generation_config.temperature,
             "top_p": generation_config.top_p,
+            "stream": generation_config.stream,
+            # TODO - We need to cap this to avoid potential errors when exceed max allowable context
             "max_tokens": generation_config.max_tokens_to_sample,
         }
+
         return args
```

### Comparing `r2r-0.1.35/r2r/vecs/__init__.py` & `r2r-0.2.0/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/vecs/adapter/base.py` & `r2r-0.2.0/r2r/vecs/adapter/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 a collection using media types other than vectors.
 
 All public classes, enums, and functions are re-exported by `vecs.adapters` module.
 """
 
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple
+from typing import Any, Dict, Generator, Iterable, Optional, Tuple
 
 from vecs.exc import ArgError
 
 
 class AdapterContext(str, Enum):
     """
     An enum representing the different contexts in which a Pipeline
@@ -59,20 +59,20 @@
 
 
 class Adapter:
     """
     Class representing a sequence of AdapterStep instances forming a pipeline.
     """
 
-    def __init__(self, steps: List[AdapterStep]):
+    def __init__(self, steps: list[AdapterStep]):
         """
         Initialize an Adapter instance with a list of AdapterStep instances.
 
         Args:
-            steps: List of AdapterStep instances.
+            steps: list of AdapterStep instances.
 
         Raises:
             ArgError: Raised if the steps list is empty.
         """
         self.steps = steps
         if len(steps) < 1:
             raise ArgError("Adapter must contain at least 1 step")
```

### Comparing `r2r-0.1.35/r2r/vecs/adapter/markdown.py` & `r2r-0.2.0/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/vecs/adapter/noop.py` & `r2r-0.2.0/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/vecs/adapter/text.py` & `r2r-0.2.0/r2r/vecs/adapter/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 TextEmbeddingModel = Literal[
     "all-mpnet-base-v2",
     "multi-qa-mpnet-base-dot-v1",
     "all-distilroberta-v1",
     "all-MiniLM-L12-v2",
     "multi-qa-distilbert-cos-v1",
-    "all-MiniLM-L6-v2",
+    "mixedbread-ai/mxbai-embed-large-v1",
     "multi-qa-MiniLM-L6-cos-v1",
     "paraphrase-multilingual-mpnet-base-v2",
     "paraphrase-albert-small-v2",
     "paraphrase-multilingual-MiniLM-L12-v2",
     "paraphrase-MiniLM-L3-v2",
     "distiluse-base-multilingual-cased-v1",
     "distiluse-base-multilingual-cased-v2",
```

### Comparing `r2r-0.1.35/r2r/vecs/client.py` & `r2r-0.2.0/r2r/vecs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from typing import TYPE_CHECKING, List, Optional
 
 from deprecated import deprecated
 from sqlalchemy import MetaData, create_engine, text
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import QueuePool
 
-from r2r.vecs.adapter import Adapter
-from r2r.vecs.exc import CollectionNotFound
+from .adapter import Adapter
+from .exc import CollectionNotFound
 
 if TYPE_CHECKING:
     from r2r.vecs.collection import Collection
 
 logger = logging.getLogger(__name__)
 
 
@@ -70,33 +70,34 @@
         self.max_retries = max_retries
         self.retry_delay = retry_delay
         self.vector_version: Optional[str] = None
         self._initialize_database()
 
     def _initialize_database(self):
         retries = 0
+        error = None
         while retries < self.max_retries:
             try:
                 with self.Session() as sess:
                     with sess.begin():
                         self._create_schema(sess)
                         self._create_extension(sess)
                         self._get_vector_version(sess)
                 return
             except Exception as e:
                 logger.warning(
                     f"Database connection error: {str(e)}. Retrying in {self.retry_delay} seconds..."
                 )
                 retries += 1
                 time.sleep(self.retry_delay)
+                error = e
 
-        logger.error(
-            f"Failed to initialize database after {self.max_retries} retries."
-        )
-        raise RuntimeError("Failed to initialize database.")
+        error_message = f"Failed to initialize database after {self.max_retries} retries with error: {str(error)}"
+        logger.error(error_message)
+        raise RuntimeError(error_message)
 
     def _create_schema(self, sess):
         try:
             sess.execute(text("CREATE SCHEMA IF NOT EXISTS vecs;"))
         except Exception as e:
             logger.warning(f"Failed to create schema: {str(e)}")
```

### Comparing `r2r-0.1.35/r2r/vecs/collection.py` & `r2r-0.2.0/r2r/vecs/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,24 @@
     MetaData,
     String,
     Table,
     alias,
     and_,
     cast,
     delete,
+    distinct,
     func,
     or_,
     select,
     text,
 )
 from sqlalchemy.dialects import postgresql
 
-from r2r.vecs.adapter import Adapter, AdapterContext, NoOp
-from r2r.vecs.exc import (
+from .adapter import Adapter, AdapterContext, NoOp
+from .exc import (
     ArgError,
     CollectionAlreadyExists,
     CollectionNotFound,
     FilterError,
     MismatchedDimension,
     Unreachable,
 )
@@ -179,14 +180,16 @@
         `vecs.Client` with `vecs.Client.create_collection(...)` rather than directly.
 
         Args:
             name (str): The name of the collection.
             dimension (int): The dimension of the vectors in the collection.
             client (Client): The client to use for interacting with the database.
         """
+        from r2r.vecs.adapter import Adapter
+
         self.client = client
         self.name = name
         self.dimension = dimension
         self.table = build_table(name, client.meta, dimension)
         self._index: Optional[str] = None
         self.adapter = adapter or Adapter(steps=[NoOp(dimension=dimension)])
 
@@ -330,14 +333,46 @@
 
         with self.client.Session() as sess:
             sess.execute(DropTable(self.table, if_exists=True))
             sess.commit()
 
         return self
 
+    def get_unique_metadata_values(
+        self,
+        field: str,
+        filter_field: Optional[str] = None,
+        filter_value: Optional[MetadataValues] = None,
+    ) -> List[MetadataValues]:
+        """
+        Fetches all unique metadata values of a specific field, optionally filtered by another metadata field.
+        Args:
+            field (str): The metadata field for which to fetch unique values.
+            filter_field (Optional[str], optional): The metadata field to filter on. Defaults to None.
+            filter_value (Optional[MetadataValues], optional): The value to filter the metadata field with. Defaults to None.
+        Returns:
+            List[MetadataValues]: A list of unique metadata values for the specified field.
+        """
+        with self.client.Session() as sess:
+            with sess.begin():
+                stmt = select(
+                    distinct(self.table.c.metadata[field].astext)
+                ).where(self.table.c.metadata[field] != None)
+
+                if filter_field is not None and filter_value is not None:
+                    stmt = stmt.where(
+                        self.table.c.metadata[filter_field].astext
+                        == str(filter_value)
+                    )
+
+                result = sess.execute(stmt)
+                unique_values = result.scalars().all()
+
+        return unique_values
+
     def copy(
         self,
         records: Iterable[Tuple[str, Any, Metadata]],
         skip_adapter: bool = False,
     ) -> None:
         """
         Copies records into the collection.
```

### Comparing `r2r-0.1.35/r2r/vecs/exc.py` & `r2r-0.2.0/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.35/r2r/vector_dbs/local/base.py` & `r2r-0.2.0/r2r/vector_dbs/local/r2r_local_vector_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,103 @@
 import json
 import logging
 import os
 import sqlite3
 from typing import Optional, Union
 
-from r2r.core import VectorDBProvider, VectorEntry, VectorSearchResult
+from r2r.core import (
+    SearchResult,
+    VectorDBConfig,
+    VectorDBProvider,
+    VectorEntry,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class LocalVectorDB(VectorDBProvider):
-    def __init__(
-        self, provider: str = "local", db_path: Optional[str] = None
-    ) -> None:
-        logger.info(
-            "Initializing `LocalVectorDB` to store and retrieve embeddings."
-        )
-
-        super().__init__(provider)
-        if provider != "local":
+class R2RLocalVectorDB(VectorDBProvider):
+    def __init__(self, config: VectorDBConfig) -> None:
+        super().__init__(config)
+        if config.provider != "local":
             raise ValueError(
-                "LocalVectorDB must be initialized with provider `local`."
+                "R2RLocalVectorDB must be initialized with provider `local`."
             )
 
-        self.db_path = db_path
-        self.collection_name: Optional[str] = None
-
     def _get_conn(self):
         conn = sqlite3.connect(
-            self.db_path or os.getenv("LOCAL_DB_PATH", "local.sqlite")
+            self.config.extra_fields.get("db_path")
+            or os.getenv("LOCAL_DB_PATH", "local.sqlite")
         )
         return conn
 
     def _get_cursor(self, conn):
         return conn.cursor()
 
-    def initialize_collection(
-        self, collection_name: str, dimension: int
-    ) -> None:
+    def initialize_collection(self, dimension: int) -> None:
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
         cursor.execute(
             f"""
-            CREATE TABLE IF NOT EXISTS "{collection_name}" (
+            CREATE TABLE IF NOT EXISTS "{self.config.collection_name}" (
                 id TEXT PRIMARY KEY,
                 vector TEXT,
                 metadata TEXT
             )
         """
         )
-        self.collection_name = collection_name
         conn.commit()
         conn.close()
 
     def create_index(self, index_type, column_name, index_options):
         raise NotImplementedError(
-            "LocalVectorDB does not support creating indexes."
+            "R2RLocalVectorDB does not support creating indexes."
         )
 
     def copy(self, entry: VectorEntry, commit=True) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
 
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
+        serializeable_entry = entry.to_serializable()
         cursor.execute(
             f"""
-                INSERT OR IGNORE INTO "{self.collection_name}" (id, vector, metadata)
+                INSERT OR IGNORE INTO "{self.config.collection_name}" (id, vector, metadata)
                 VALUES (?, ?, ?)
             """,
             (
-                str(entry.id),
-                json.dumps(entry.vector),
-                json.dumps(entry.metadata),
+                serializeable_entry["id"],
+                str(serializeable_entry["vector"]),
+                json.dumps(serializeable_entry["metadata"]),
             ),
         )
         if commit:
             conn.commit()
         conn.close()
 
     def upsert(self, entry: VectorEntry, commit=True) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
 
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
+        serializeable_entry = entry.to_serializable()
         cursor.execute(
             f"""
-            INSERT OR REPLACE INTO "{self.collection_name}" (id, vector, metadata)
-            VALUES (?, ?, ?)
-        """,
+                INSERT OR REPLACE INTO "{self.config.collection_name}" (id, vector, metadata)
+                VALUES (?, ?, ?)
+            """,
             (
-                str(entry.id),
-                json.dumps(entry.vector),
-                json.dumps(entry.metadata),
+                serializeable_entry["id"],
+                str(serializeable_entry["vector"]),
+                json.dumps(serializeable_entry["metadata"]),
             ),
         )
         if commit:
             conn.commit()
         conn.close()
 
     def _cosine_similarity(
@@ -115,68 +111,80 @@
     def search(
         self,
         query_vector: list[float],
         filters: dict[str, Union[bool, int, str]] = {},
         limit: int = 10,
         *args,
         **kwargs,
-    ) -> list[VectorSearchResult]:
-        if self.collection_name is None:
+    ) -> list[SearchResult]:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
-        cursor.execute(f'SELECT * FROM "{self.collection_name}"')
+        cursor.execute(f'SELECT * FROM "{self.config.collection_name}"')
         results = []
         for id, vector, metadata in cursor.fetchall():
             vector = json.loads(vector)
-            metadata = json.loads(metadata)
-            if all(metadata.get(k) == v for k, v in filters.items()):
+            json_metadata = json.loads(metadata)
+            if all(json_metadata.get(k) == v for k, v in filters.items()):
                 # Local cosine similarity calculation
                 score = self._cosine_similarity(query_vector, vector)
-                results.append(VectorSearchResult(id, score, metadata))
+                results.append(
+                    SearchResult(id=id, score=score, metadata=json_metadata)
+                )
         results.sort(key=lambda x: x.score, reverse=True)
         conn.close()
         return results[:limit]
 
-    def filtered_deletion(
-        self, key: str, value: Union[bool, int, str]
+    def delete_by_metadata(
+        self, metadata_field: str, metadata_value: Union[bool, int, str]
     ) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
 
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
-        cursor.execute(f'SELECT * FROM "{self.collection_name}"')
+        cursor.execute(f'SELECT * FROM "{self.config.collection_name}"')
         for id, vector, metadata in cursor.fetchall():
-            metadata = json.loads(metadata)
-            if metadata.get(key) == value:
+            metadata_json = json.loads(metadata)
+            if metadata_json.get(metadata_field) == metadata_value:
                 cursor.execute(
-                    f'DELETE FROM "{self.collection_name}" WHERE id = ?', (id,)
+                    f'DELETE FROM "{self.config.collection_name}" WHERE id = ?',
+                    (id,),
                 )
         conn.commit()
         conn.close()
 
-    def get_all_unique_values(
-        self, metadata_field: str, filters: dict = {}
-    ) -> list:
-        if self.collection_name is None:
+    def get_metadatas(
+        self,
+        metadata_fields: list[str],
+        filter_field: Optional[str] = None,
+        filter_value: Optional[str] = None,
+    ) -> list[str]:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
-        cursor.execute(f'SELECT metadata FROM "{self.collection_name}"')
-        unique_values = set()
+        cursor.execute(f'SELECT metadata FROM "{self.config.collection_name}"')
+        results = set([])
         for (metadata,) in cursor.fetchall():
-            metadata = json.loads(metadata)
-            if all(metadata.get(k) == v for k, v in filters.items()):
-                if metadata_field in metadata:
-                    unique_values.add(metadata[metadata_field])
+            metatada_json = json.loads(metadata)
+            if (
+                filter_field is None
+                or metatada_json.get(filter_field) == filter_value
+            ):
+                results.add(
+                    json.dumps(
+                        {
+                            k: metatada_json.get(k, None)
+                            for k in metadata_fields
+                        }
+                    )
+                )
         conn.close()
-        return list(unique_values)
-
-    def close(self):
-        pass
+        return [json.loads(r) for r in results]
```

### Comparing `r2r-0.1.35/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.2.0/r2r/vector_dbs/pgvector/pgvector_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,192 @@
 import logging
 import os
 from typing import Optional, Union
 
-from r2r.core import VectorDBProvider, VectorEntry, VectorSearchResult
+from r2r.core import (
+    SearchResult,
+    VectorDBConfig,
+    VectorDBProvider,
+    VectorEntry,
+)
 from r2r.vecs.client import Client
 from r2r.vecs.collection import Collection
 
 logger = logging.getLogger(__name__)
 
 
 class PGVectorDB(VectorDBProvider):
-    def __init__(self, provider: str = "pgvector") -> None:
-        logger.info(
-            "Initializing `PGVectorDB` to store and retrieve embeddings."
-        )
-
-        super().__init__(provider)
-        if provider != "pgvector":
-            raise ValueError(
-                "PGVectorDB must be initialized with provider `pgvector`."
-            )
+    def __init__(self, config: VectorDBConfig) -> None:
+        super().__init__(config)
         try:
             import r2r.vecs
         except ImportError:
             raise ValueError(
                 f"Error, PGVectorDB requires the vecs library. Please run `poetry add vecs`."
             )
+        user = os.getenv("POSTGRES_USER")
+        password = os.getenv("POSTGRES_PASSWORD")
+        host = os.getenv("POSTGRES_HOST")
+        port = os.getenv("POSTGRES_PORT")
+        db_name = os.getenv("POSTGRES_DBNAME")
+        if not all([user, password, host, port, db_name]):
+            raise ValueError(
+                "Error, please set the POSTGRES_USER, POSTGRES_PASSWORD, POSTGRES_HOST, POSTGRES_PORT, and POSTGRES_DBNAME environment variables."
+            )
         try:
-            user = os.getenv("POSTGRES_USER")
-            password = os.getenv("POSTGRES_PASSWORD")
-            host = os.getenv("POSTGRES_HOST")
-            port = os.getenv("POSTGRES_PORT")
-            db_name = os.getenv("POSTGRES_DBNAME")
-
             DB_CONNECTION = (
                 f"postgresql://{user}:{password}@{host}:{port}/{db_name}"
             )
             self.vx: Client = r2r.vecs.create_client(DB_CONNECTION)
         except Exception as e:
             raise ValueError(
                 f"Error {e} occurred while attempting to connect to the pgvector provider with {DB_CONNECTION}."
             )
         self.collection: Optional[Collection] = None
+        self.config: VectorDBConfig = config
 
-    def initialize_collection(
-        self, collection_name: str, dimension: int
-    ) -> None:
+    def initialize_collection(self, dimension: int) -> None:
         self.collection = self.vx.get_or_create_collection(
-            name=collection_name, dimension=dimension
+            name=self.config.collection_name, dimension=dimension
         )
 
     def copy(self, entry: VectorEntry, commit=True) -> None:
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `copy`."
             )
 
+        serializeable_entry = entry.to_serializable()
+
         self.collection.copy(
-            records=[(str(entry.id), entry.vector, entry.metadata)]
+            records=[
+                (
+                    serializeable_entry["id"],
+                    serializeable_entry["vector"],
+                    serializeable_entry["metadata"],
+                )
+            ]
         )
 
     def copy_entries(
         self, entries: list[VectorEntry], commit: bool = True
     ) -> None:
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `copy_entries`."
             )
 
         self.collection.copy(
             records=[
-                (str(entry.id), entry.vector, entry.metadata)
+                (
+                    str(entry.id),
+                    entry.vector.data,
+                    entry.to_serializable()["metadata"],
+                )
                 for entry in entries
             ]
         )
 
     def upsert(self, entry: VectorEntry, commit=True) -> None:
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `upsert`."
             )
 
         self.collection.upsert(
-            records=[(str(entry.id), entry.vector, entry.metadata)]
+            records=[
+                (
+                    str(entry.id),
+                    entry.vector.data,
+                    entry.to_serializable()["metadata"],
+                )
+            ]
         )
 
     def upsert_entries(
         self, entries: list[VectorEntry], commit: bool = True
     ) -> None:
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `upsert_entries`."
             )
 
         self.collection.upsert(
             records=[
-                (str(entry.id), entry.vector, entry.metadata)
+                (
+                    str(entry.id),
+                    entry.vector.data,
+                    entry.to_serializable()["metadata"],
+                )
                 for entry in entries
             ]
         )
 
     def search(
         self,
         query_vector: list[float],
         filters: dict[str, Union[bool, int, str]] = {},
         limit: int = 10,
         *args,
         **kwargs,
-    ) -> list[VectorSearchResult]:
+    ) -> list[SearchResult]:
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `search`."
             )
         measure = kwargs.get("measure", "cosine_distance")
         mapped_filters = {
             key: {"$eq": value} for key, value in filters.items()
         }
 
         return [
-            VectorSearchResult(ele[0], 1 - ele[1], ele[2])  # type: ignore
+            SearchResult(id=ele[0], score=float(1 - ele[1]), metadata=ele[2])  # type: ignore
             for ele in self.collection.query(
                 data=query_vector,
                 limit=limit,
                 filters=mapped_filters,
                 measure=measure,
                 include_value=True,
                 include_metadata=True,
             )
         ]
 
     def create_index(self, index_type, column_name, index_options):
         pass
 
-    def close(self):
-        pass
-
-    def filtered_deletion(
-        self, key: str, value: Union[bool, int, str]
+    def delete_by_metadata(
+        self, metadata_field: str, metadata_value: Union[bool, int, str]
     ) -> None:
         if self.collection is None:
             raise ValueError(
-                "Please call `initialize_collection` before attempting to run `filtered_deletion`."
+                "Please call `initialize_collection` before attempting to run `delete_by_metadata`."
             )
-        self.collection.delete(filters={key: {"$eq": value}})  # type: ignore
-
-    def get_all_unique_values(
-        self, metadata_field: str, filters: dict = {}
-    ) -> list:
-        if self.collection is None:
-            raise ValueError(
-                "Please call `initialize_collection` before attempting to run `get_all_unique_values`."
-            )
-
-        mapped_filters = {
-            key: {"$eq": value} for key, value in filters.items()
-        }
-
-        # Pass an empty vector as the `data` argument
-        records = self.collection.query(
-            data=[0] * self.collection.dimension,  # Empty vector
-            filters=mapped_filters,
-            include_metadata=True,
-            include_value=False,
-            # Remove the `limit` argument to retrieve all records
+        self.collection.delete(
+            filters={metadata_field: {"$eq": metadata_value}}
         )
 
-        unique_values = set(
-            record[1].get(metadata_field) for record in records
-        )
+    def get_metadatas(
+        self,
+        metadata_fields: list[str],
+        filter_field: Optional[str] = None,
+        filter_value: Optional[Union[bool, int, str]] = None,
+    ) -> list[dict]:
+        if self.collection is None:
+            raise ValueError(
+                "Please call `initialize_collection` before attempting to run `get_metadatas`."
+            )
+
+        results = {tuple(metadata_fields): {}}
+        for field in metadata_fields:
+            unique_values = self.collection.get_unique_metadata_values(
+                field=field,
+                filter_field=filter_field,
+                filter_value=filter_value,
+            )
+            for value in unique_values:
+                if value not in results:
+                    results[value] = {}
+                results[value][field] = value
 
-        return list(unique_values)
+        return [
+            results[key] for key in results if key != tuple(metadata_fields)
+        ]
```

### Comparing `r2r-0.1.35/r2r/vector_dbs/qdrant/base.py` & `r2r-0.2.0/r2r/vector_dbs/qdrant/qdrant_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import logging
 import os
 from typing import Optional, Union
 
-from r2r.core import VectorDBProvider, VectorEntry, VectorSearchResult
+from r2r.core import (
+    SearchResult,
+    VectorDBConfig,
+    VectorDBProvider,
+    VectorEntry,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class QdrantDB(VectorDBProvider):
-    def __init__(self, provider: str = "qdrant") -> None:
-        logger.info(
-            "Initializing `QdrantDB` to store and retrieve embeddings."
-        )
-
-        super().__init__(provider)
-        if provider != "qdrant":
+    def __init__(self, config: VectorDBConfig) -> None:
+        super().__init__(config)
+        if config.provider != "qdrant":
             raise ValueError(
                 "QdrantDB must be initialized with provider `qdrant`."
             )
+
         try:
             from qdrant_client import QdrantClient
             from qdrant_client.http import models
 
             self.models = models
         except ImportError:
             raise ValueError(
@@ -38,92 +40,88 @@
                 )
 
             self.client = QdrantClient(host, port=int(port), api_key=api_key)
         except Exception as e:
             raise ValueError(
                 f"Error {e} occurred while attempting to connect to the qdrant provider."
             )
-        self.collection_name: Optional[str] = None
 
-    def initialize_collection(
-        self, collection_name: str, dimension: int
-    ) -> None:
-        self.collection_name = collection_name
+    def initialize_collection(self, dimension: int) -> None:
         try:
             result = self.client.create_collection(
-                collection_name=f"{collection_name}",
+                collection_name=f"{self.config.collection_name}",
                 vectors_config=self.models.VectorParams(
                     size=dimension, distance=self.models.Distance.COSINE
                 ),
             )
             if result is False:
                 raise ValueError(
-                    f"Error occurred while attempting to create collection {collection_name}."
+                    f"Error occurred while attempting to create collection {self.config.collection_name}."
                 )
         except Exception:
             # TODO - Handle more appropriately - create collection fails when it already exists
             pass
 
     def copy(self, entry: VectorEntry, commit=True) -> None:
         raise NotImplementedError(
             "QdrantDB does not support the `copy` method."
         )
 
     def upsert(self, entry: VectorEntry, commit=True) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `upsert`."
             )
         points = [
             self.models.PointStruct(
                 id=str(entry.id),
-                vector=list([float(ele) for ele in entry.vector]),
+                vector=list([float(ele) for ele in entry.vector.data]),
                 payload=entry.metadata,
             )
         ]
         self.client.upsert(
-            collection_name=f"{self.collection_name}",
+            collection_name=f"{self.config.collection_name}",
             points=points,
         )
 
     def upsert_entries(
         self, entries: list[VectorEntry], commit: bool = True
     ) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `upsert_entries`."
             )
         points = [
             self.models.PointStruct(
                 id=str(entry.id),
-                vector=list([float(ele) for ele in entry.vector]),
+                vector=list([float(ele) for ele in entry.vector.data]),
                 payload=entry.metadata,
             )
             for entry in entries
         ]
         self.client.upsert(
-            collection_name=f"{self.collection_name}",
+            collection_name=f"{self.config.collection_name}",
             points=points,
         )
 
     def search(
         self,
         query_vector: list[float],
         filters: dict[str, Union[bool, int, str]] = {},
         limit: int = 10,
         *args,
         **kwargs,
-    ) -> list[VectorSearchResult]:
-        if self.collection_name is None:
+    ) -> list[SearchResult]:
+        if self.config.collection_name is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `search`."
             )
 
         results = self.client.search(
-            collection_name=f"{self.collection_name}",
+            collection_name=f"{self.config.collection_name}",
             query_filter=self.models.Filter(
                 must=[
                     self.models.FieldCondition(
                         key=key,
                         match=self.models.MatchValue(
                             value=value,
                         ),
@@ -132,82 +130,88 @@
                 ]
             ),
             query_vector=query_vector,
             limit=limit,
         )
 
         return [
-            VectorSearchResult(
-                str(result.id), result.score, result.payload or {}
+            SearchResult(
+                id=result.id, score=result.score, metadata=result.payload or {}
             )
             for result in results
         ]
 
     def create_index(self, index_type, column_name, index_options):
         pass
 
-    def close(self):
-        pass
-
-    def filtered_deletion(
-        self, key: str, value: Union[bool, int, str]
+    def delete_by_metadata(
+        self, metadata_field: str, metadata_value: Union[bool, int, str]
     ) -> None:
-        if self.collection_name is None:
+        if self.config.collection_name is None:
             raise ValueError(
-                "Please call `initialize_collection` before attempting to run `filtered_deletion`."
+                "Please call `initialize_collection` before attempting to run `delete_by_metadata`."
             )
 
         self.client.delete(
-            collection_name=self.collection_name,
+            collection_name=self.config.collection_name,
             points_selector=self.models.FilterSelector(
                 filter=self.models.Filter(
                     must=[
                         self.models.FieldCondition(
-                            key=key,
-                            match=self.models.MatchValue(value=value),
+                            key=metadata_field,
+                            match=self.models.MatchValue(value=metadata_value),
                         ),
                     ],
                 )
             ),
         )
         return
 
-    def get_all_unique_values(
-        self, collection_name: str, metadata_field: str, filters: dict = {}
-    ) -> list:
-        if self.collection_name is None:
+    def get_metadatas(
+        self,
+        metadata_fields: list[str],
+        filter_field: Optional[str] = None,
+        filter_value: Optional[str] = None,
+    ) -> list[dict]:
+        if self.config.collection_name is None:
             raise ValueError(
-                "Please call `initialize_collection` before attempting to run `get_all_unique_values`."
+                "Please call `initialize_collection` before attempting to run `get_metadatas`."
             )
 
-        # Create a scroll filter based on the provided filters
+        # Create a scroll filter based on the provided filter field and value
         scroll_filter = None
-        if filters:
-            filter_conditions = [
-                self.models.FieldCondition(
-                    key=key, match=self.models.MatchValue(value=value)
-                )
-                for key, value in filters.items()
-            ]
-            scroll_filter = self.models.Filter(must=filter_conditions)
+        if filter_field and filter_value:
+            scroll_filter = self.models.Filter(
+                must=[
+                    self.models.FieldCondition(
+                        key=filter_field,
+                        match=self.models.MatchValue(value=filter_value),
+                    )
+                ]
+            )
 
-        unique_values = set()
+        unique_values = {}
 
         # Scroll through the collection and retrieve points in batches
         next_page_offset = None
         while True:
-            records, next_page_offset = self.scroll(
-                collection_name=collection_name,
+            records, next_page_offset = self.client.scroll(
+                collection_name=self.config.collection_name,
                 scroll_filter=scroll_filter,
                 offset=next_page_offset,
                 limit=100,  # Adjust the batch size as needed
                 with_payload=True,
             )
 
             for record in records:
-                if metadata_field in record.payload:
-                    unique_values.add(record.payload[metadata_field])
+                metadata = record.payload
+                if all(field in metadata for field in metadata_fields):
+                    key = tuple(metadata[field] for field in metadata_fields)
+                    if key not in unique_values:
+                        unique_values[key] = {}
+                    for field in metadata_fields:
+                        unique_values[key][field] = metadata[field]
 
             if next_page_offset is None:
                 break
 
-        return list(unique_values)
+        return list(unique_values.values())
```

