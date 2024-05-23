# Comparing `tmp/LangTorch-1.0.3.tar.gz` & `tmp/LangTorch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LangTorch-1.0.3.tar", last modified: Thu May 23 01:20:11 2024, max compression
+gzip compressed data, was "LangTorch-1.0.4.tar", last modified: Thu May 23 14:47:44 2024, max compression
```

## Comparing `LangTorch-1.0.3.tar` & `LangTorch-1.0.4.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.572054 LangTorch-1.0.3/
--rw-rw-rw-   0        0        0     6673 2024-05-23 01:20:11.570875 LangTorch-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5968 2024-04-14 08:46:21.000000 LangTorch-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 01:20:11.572054 LangTorch-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1467 2024-05-23 01:19:40.000000 LangTorch-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.491490 LangTorch-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.508915 LangTorch-1.0.3/src/LangTorch.egg-info/
--rw-rw-rw-   0        0        0     6673 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3458 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.517924 LangTorch-1.0.3/src/langtorch/
--rw-rw-rw-   0        0        0     9127 2024-05-17 09:29:22.000000 LangTorch-1.0.3/src/langtorch/_VariableFunctions.py
--rw-rw-rw-   0        0        0      597 2024-05-17 13:20:07.000000 LangTorch-1.0.3/src/langtorch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.525426 LangTorch-1.0.3/src/langtorch/api/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.3/src/langtorch/api/TODO_anthropic_parallel_processor.py
--rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/api/TODO_assistant.py
--rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/api/TODO_gcp_parallel_processor.py
--rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/api/__init__.py
--rw-rw-rw-   0        0        0     1111 2024-05-17 01:10:31.000000 LangTorch-1.0.3/src/langtorch/api/api_threading.py
--rw-rw-rw-   0        0        0    13887 2024-05-17 19:49:39.000000 LangTorch-1.0.3/src/langtorch/api/call.py
--rw-rw-rw-   0        0        0        0 2024-05-16 22:19:27.000000 LangTorch-1.0.3/src/langtorch/api/groq.py
--rw-rw-rw-   0        0        0     6810 2024-05-17 01:30:15.000000 LangTorch-1.0.3/src/langtorch/api/openai.py
--rw-rw-rw-   0        0        0     9982 2024-05-17 20:16:36.000000 LangTorch-1.0.3/src/langtorch/api/parallel_processor_utils.py
--rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/api/tools.py
--rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/api/utils.py
--rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.3/src/langtorch/autograd.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.527428 LangTorch-1.0.3/src/langtorch/conf/
--rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.3/src/langtorch/conf/__init__.py
--rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/conf/new_session_template.yaml
--rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.3/src/langtorch/conf/overrides.yaml
--rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.3/src/langtorch/decorators.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.530572 LangTorch-1.0.3/src/langtorch/grammars/
--rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.3/src/langtorch/grammars/__init__.py
--rw-rw-rw-   0        0        0     5850 2024-05-17 10:46:51.000000 LangTorch-1.0.3/src/langtorch/grammars/formatters.py
--rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/grammars/langtorch_default_parser.py
--rw-rw-rw-   0        0        0     5359 2024-05-17 03:05:19.000000 LangTorch-1.0.3/src/langtorch/grammars/pandoc.py
--rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/grammars/parsers.py
--rw-rw-rw-   0        0        0     6102 2024-05-17 02:21:53.000000 LangTorch-1.0.3/src/langtorch/grammars/text_content_ast.py
--rw-rw-rw-   0        0        0     2343 2024-05-17 03:11:04.000000 LangTorch-1.0.3/src/langtorch/grammars/utils.py
--rw-rw-rw-   0        0        0     8093 2024-05-22 23:57:17.000000 LangTorch-1.0.3/src/langtorch/main.py
--rw-rw-rw-   0        0        0     2315 2024-05-22 23:41:02.000000 LangTorch-1.0.3/src/langtorch/main2.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.534572 LangTorch-1.0.3/src/langtorch/methods/
--rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.3/src/langtorch/methods/__init__.py
--rw-rw-rw-   0        0        0     2704 2024-05-17 09:31:29.000000 LangTorch-1.0.3/src/langtorch/methods/chain_of_density.py
--rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/methods/chain_of_thought.py
--rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/methods/embeddings.py
--rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.3/src/langtorch/methods/prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.535571 LangTorch-1.0.3/src/langtorch/optim/
--rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.3/src/langtorch/optim/__init__.py
--rw-rw-rw-   0        0        0     2189 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/optim/optimizer.py
--rw-rw-rw-   0        0        0      574 2024-05-17 09:32:04.000000 LangTorch-1.0.3/src/langtorch/semalg_utils.py
--rw-rw-rw-   0        0        0     4639 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/semantic_algebra.py
--rw-rw-rw-   0        0        0    13200 2024-05-18 10:39:50.000000 LangTorch-1.0.3/src/langtorch/session.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.537869 LangTorch-1.0.3/src/langtorch/tensors/
--rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.3/src/langtorch/tensors/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.3/src/langtorch/tensors/chattensor.py
--rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.3/src/langtorch/tensors/codetensor.py
--rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.3/src/langtorch/tensors/langtorchtensor.py
--rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.3/src/langtorch/tensors/markdowntensor.py
--rw-rw-rw-   0        0        0    42547 2024-05-23 00:01:23.000000 LangTorch-1.0.3/src/langtorch/tensors/texttensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.542867 LangTorch-1.0.3/src/langtorch/texts/
--rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.3/src/langtorch/texts/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-05-15 02:21:06.000000 LangTorch-1.0.3/src/langtorch/texts/chat.py
--rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.3/src/langtorch/texts/code.py
--rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/texts/markdown.py
--rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/texts/markup.py
--rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/texts/string.py
--rw-rw-rw-   0        0        0    36694 2024-05-23 00:04:36.000000 LangTorch-1.0.3/src/langtorch/texts/text.py
--rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.3/src/langtorch/texts/thread.py
--rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.3/src/langtorch/torch_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.543867 LangTorch-1.0.3/src/langtorch/tt/
--rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/__init__.py
--rw-rw-rw-   0        0        0    30608 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/functional.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.543867 LangTorch-1.0.3/src/langtorch/tt/modules/
--rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.3/src/langtorch/tt/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.544882 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/transformers_automodel.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.547908 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/__init__.py
--rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/distance.py
--rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/embedding.py
--rw-rw-rw-   0        0        0     1312 2024-05-17 09:29:49.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.556509 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/
--rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/__init__.py
--rw-rw-rw-   0        0        0    22439 2024-05-17 05:36:08.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/activation.py
--rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/assistantmodule.py
--rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/chatmodule.py
--rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/codemodule.py
--rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/conv.py
--rw-rw-rw-   0        0        0     1623 2024-05-17 18:27:32.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/linear.py
--rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/loss.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/pooling.py
--rw-rw-rw-   0        0        0      883 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/retriever.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/rnn.py
--rw-rw-rw-   0        0        0     7195 2024-05-17 18:27:32.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/textmodule.py
--rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformer.py
--rw-rw-rw-   0        0        0     2009 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformers.py
--rw-rw-rw-   0        0        0     1268 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/types.py
--rw-rw-rw-   0        0        0     8335 2024-05-17 09:34:19.000000 LangTorch-1.0.3/src/langtorch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.570875 LangTorch-1.0.3/tests/
--rw-rw-rw-   0        0        0      845 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_activation.py
--rw-rw-rw-   0        0        0     1358 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_autograd.py
--rw-rw-rw-   0        0        0     6419 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_conv.py
--rw-rw-rw-   0        0        0      292 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_dspy.py
--rw-rw-rw-   0        0        0     2487 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_embedding.py
--rw-rw-rw-   0        0        0     4094 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_functional.py
--rw-rw-rw-   0        0        0     6075 2024-03-30 15:39:03.000000 LangTorch-1.0.3/tests/test_group_operation.py
--rw-rw-rw-   0        0        0      489 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_import.py
--rw-rw-rw-   0        0        0      433 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_markdown.py
--rw-rw-rw-   0        0        0     1056 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_methods.py
--rw-rw-rw-   0        0        0     6393 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_mul.py
--rw-rw-rw-   0        0        0     2274 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_optimizer.py
--rw-rw-rw-   0        0        0     5417 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_pandoc.py
--rw-rw-rw-   0        0        0     1994 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_semantic_algebra.py
--rw-rw-rw-   0        0        0     4400 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_session.py
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_session_api.py
--rw-rw-rw-   0        0        0     1764 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_text.py
--rw-rw-rw-   0        0        0     3935 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_texttensor.py
--rw-rw-rw-   0        0        0      727 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_texttensor_constructor.py
--rw-rw-rw-   0        0        0      938 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.046865 LangTorch-1.0.4/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 14:47:44.045863 LangTorch-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5968 2024-04-14 08:46:21.000000 LangTorch-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:47:44.046865 LangTorch-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2024-05-23 14:47:37.000000 LangTorch-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.938871 LangTorch-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.954867 LangTorch-1.0.4/src/LangTorch.egg-info/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3458 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.966867 LangTorch-1.0.4/src/langtorch/
+-rw-rw-rw-   0        0        0     9127 2024-05-17 09:29:22.000000 LangTorch-1.0.4/src/langtorch/_VariableFunctions.py
+-rw-rw-rw-   0        0        0      597 2024-05-17 13:20:07.000000 LangTorch-1.0.4/src/langtorch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.978026 LangTorch-1.0.4/src/langtorch/api/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.4/src/langtorch/api/TODO_anthropic_parallel_processor.py
+-rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/api/TODO_assistant.py
+-rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/api/TODO_gcp_parallel_processor.py
+-rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/api/__init__.py
+-rw-rw-rw-   0        0        0     1111 2024-05-17 01:10:31.000000 LangTorch-1.0.4/src/langtorch/api/api_threading.py
+-rw-rw-rw-   0        0        0    13895 2024-05-23 10:29:24.000000 LangTorch-1.0.4/src/langtorch/api/call.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 22:19:27.000000 LangTorch-1.0.4/src/langtorch/api/groq.py
+-rw-rw-rw-   0        0        0     6810 2024-05-17 01:30:15.000000 LangTorch-1.0.4/src/langtorch/api/openai.py
+-rw-rw-rw-   0        0        0     9982 2024-05-17 20:16:36.000000 LangTorch-1.0.4/src/langtorch/api/parallel_processor_utils.py
+-rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/api/tools.py
+-rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/api/utils.py
+-rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.4/src/langtorch/autograd.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.980580 LangTorch-1.0.4/src/langtorch/conf/
+-rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.4/src/langtorch/conf/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/conf/new_session_template.yaml
+-rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.4/src/langtorch/conf/overrides.yaml
+-rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.4/src/langtorch/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.987451 LangTorch-1.0.4/src/langtorch/grammars/
+-rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.4/src/langtorch/grammars/__init__.py
+-rw-rw-rw-   0        0        0     5425 2024-05-23 03:22:00.000000 LangTorch-1.0.4/src/langtorch/grammars/formatters.py
+-rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/grammars/langtorch_default_parser.py
+-rw-rw-rw-   0        0        0     5359 2024-05-17 03:05:19.000000 LangTorch-1.0.4/src/langtorch/grammars/pandoc.py
+-rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/grammars/parsers.py
+-rw-rw-rw-   0        0        0     6102 2024-05-17 02:21:53.000000 LangTorch-1.0.4/src/langtorch/grammars/text_content_ast.py
+-rw-rw-rw-   0        0        0     2343 2024-05-17 03:11:04.000000 LangTorch-1.0.4/src/langtorch/grammars/utils.py
+-rw-rw-rw-   0        0        0     7065 2024-05-23 03:19:29.000000 LangTorch-1.0.4/src/langtorch/main.py
+-rw-rw-rw-   0        0        0     2408 2024-05-23 10:25:58.000000 LangTorch-1.0.4/src/langtorch/main2.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.991449 LangTorch-1.0.4/src/langtorch/methods/
+-rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.4/src/langtorch/methods/__init__.py
+-rw-rw-rw-   0        0        0     2704 2024-05-17 09:31:29.000000 LangTorch-1.0.4/src/langtorch/methods/chain_of_density.py
+-rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/methods/chain_of_thought.py
+-rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/methods/embeddings.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.4/src/langtorch/methods/prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.992450 LangTorch-1.0.4/src/langtorch/optim/
+-rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.4/src/langtorch/optim/__init__.py
+-rw-rw-rw-   0        0        0     2189 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/optim/optimizer.py
+-rw-rw-rw-   0        0        0      574 2024-05-17 09:32:04.000000 LangTorch-1.0.4/src/langtorch/semalg_utils.py
+-rw-rw-rw-   0        0        0     4639 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/semantic_algebra.py
+-rw-rw-rw-   0        0        0    13202 2024-05-23 10:27:01.000000 LangTorch-1.0.4/src/langtorch/session.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.998457 LangTorch-1.0.4/src/langtorch/tensors/
+-rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.4/src/langtorch/tensors/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.4/src/langtorch/tensors/chattensor.py
+-rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.4/src/langtorch/tensors/codetensor.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.4/src/langtorch/tensors/langtorchtensor.py
+-rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.4/src/langtorch/tensors/markdowntensor.py
+-rw-rw-rw-   0        0        0    43291 2024-05-23 07:39:05.000000 LangTorch-1.0.4/src/langtorch/tensors/texttensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.006485 LangTorch-1.0.4/src/langtorch/texts/
+-rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.4/src/langtorch/texts/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-05-15 02:21:06.000000 LangTorch-1.0.4/src/langtorch/texts/chat.py
+-rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.4/src/langtorch/texts/code.py
+-rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/texts/markdown.py
+-rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/texts/markup.py
+-rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/texts/string.py
+-rw-rw-rw-   0        0        0    36660 2024-05-23 10:35:29.000000 LangTorch-1.0.4/src/langtorch/texts/text.py
+-rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.4/src/langtorch/texts/thread.py
+-rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.4/src/langtorch/torch_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.007483 LangTorch-1.0.4/src/langtorch/tt/
+-rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/__init__.py
+-rw-rw-rw-   0        0        0    30677 2024-05-23 01:51:12.000000 LangTorch-1.0.4/src/langtorch/tt/functional.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.009582 LangTorch-1.0.4/src/langtorch/tt/modules/
+-rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.4/src/langtorch/tt/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.011103 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/transformers_automodel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.014092 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/__init__.py
+-rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/distance.py
+-rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/embedding.py
+-rw-rw-rw-   0        0        0     1312 2024-05-17 09:29:49.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.028614 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/
+-rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/__init__.py
+-rw-rw-rw-   0        0        0    22439 2024-05-17 05:36:08.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/activation.py
+-rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/assistantmodule.py
+-rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/chatmodule.py
+-rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/codemodule.py
+-rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/conv.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 18:27:32.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/linear.py
+-rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/loss.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/pooling.py
+-rw-rw-rw-   0        0        0      883 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/retriever.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/rnn.py
+-rw-rw-rw-   0        0        0     7195 2024-05-17 18:27:32.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/textmodule.py
+-rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformer.py
+-rw-rw-rw-   0        0        0     1942 2024-05-23 01:25:33.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformers.py
+-rw-rw-rw-   0        0        0     1268 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/types.py
+-rw-rw-rw-   0        0        0     8335 2024-05-17 09:34:19.000000 LangTorch-1.0.4/src/langtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.045863 LangTorch-1.0.4/tests/
+-rw-rw-rw-   0        0        0      845 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_activation.py
+-rw-rw-rw-   0        0        0     1358 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_autograd.py
+-rw-rw-rw-   0        0        0     6419 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_conv.py
+-rw-rw-rw-   0        0        0      292 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_dspy.py
+-rw-rw-rw-   0        0        0     2487 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_embedding.py
+-rw-rw-rw-   0        0        0     4094 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6075 2024-03-30 15:39:03.000000 LangTorch-1.0.4/tests/test_group_operation.py
+-rw-rw-rw-   0        0        0      489 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_import.py
+-rw-rw-rw-   0        0        0      433 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_markdown.py
+-rw-rw-rw-   0        0        0     1056 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_methods.py
+-rw-rw-rw-   0        0        0     6393 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_mul.py
+-rw-rw-rw-   0        0        0     2274 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_optimizer.py
+-rw-rw-rw-   0        0        0     5417 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_pandoc.py
+-rw-rw-rw-   0        0        0     1994 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_semantic_algebra.py
+-rw-rw-rw-   0        0        0     4400 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_session.py
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_session_api.py
+-rw-rw-rw-   0        0        0     1764 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_text.py
+-rw-rw-rw-   0        0        0     3935 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_texttensor.py
+-rw-rw-rw-   0        0        0      727 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_texttensor_constructor.py
+-rw-rw-rw-   0        0        0      938 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_visualize.py
```

### Comparing `LangTorch-1.0.3/PKG-INFO` & `LangTorch-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LangTorch-1.0.3/README.md` & `LangTorch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/setup.py` & `LangTorch-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LangTorch",
-    version="1.0.3",
+    version="1.0.4",
     description="Framework for intuitive LLM application development with tensors.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Adam Sobieszek",
     author_email="contact@langtorch.org",
     url="https://github.com/AdamSobieszek/LangTorch",
     packages=find_packages(where="src"),
```

### Comparing `LangTorch-1.0.3/src/LangTorch.egg-info/PKG-INFO` & `LangTorch-1.0.4/src/LangTorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LangTorch-1.0.3/src/LangTorch.egg-info/SOURCES.txt` & `LangTorch-1.0.4/src/LangTorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/_VariableFunctions.py` & `LangTorch-1.0.4/src/langtorch/_VariableFunctions.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/__init__.py` & `LangTorch-1.0.4/src/langtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/TODO_assistant.py` & `LangTorch-1.0.4/src/langtorch/api/TODO_assistant.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/TODO_gcp_parallel_processor.py` & `LangTorch-1.0.4/src/langtorch/api/TODO_gcp_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/api_threading.py` & `LangTorch-1.0.4/src/langtorch/api/api_threading.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/call.py` & `LangTorch-1.0.4/src/langtorch/api/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,33 +219,31 @@
                 except RuntimeError as E2:
                     raise RuntimeError(
                         f"Asyncio get current event loop failed with {E1}. Tried to fall back on new event loop with asyncio.run(job) but failed with error: {E2}.\nThis indicates error with the API code or provider and could be hard to fix.")
 
         return session.completions("chat", provider, request_strings)
 
 
-def get_embedding(texts, model="text-embedding-3-small", cache=True, as_np=False, api_key=None, verbose=False):
+def get_embedding(texts, model="text-embedding-3-small", cache=True,  api_key=None, verbose=False):
     """
     Retrieves embeddings for the given texts from the OpenAI API and saves the results in a file.
 
     Parameters:
         texts (List[str], TextTensor): List of texts for which to get embeddings.
-        cache (bool, optional):
-        as_np (bool, optional):
+        cache (bool, optional): If True, reuse previous call results. Default is True.
         api_key (str, optional): API key for authentication. If None, uses environment variable.
         verbose (bool, optional): If True, enables detailed logging. Default is True.
 
     Returns:
         dict: The embeddings from the saved results file, loaded as a Python dictionary.
     """
     from langtorch import TextTensor
     session = Session()
 
     if api_key is None:
-
         try:
             api_key = os.environ["OPENAI_API_KEY"]
         except KeyError:
             raise KeyError('No OpenAI API key. Set os.environ["OPENAI_API_KEY"] = YOUR KEY')
     if isinstance(texts, str): texts = [str(texts)]
     if isinstance(texts, TextTensor):
         shape = texts.content.shape
```

### Comparing `LangTorch-1.0.3/src/langtorch/api/openai.py` & `LangTorch-1.0.4/src/langtorch/api/openai.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/parallel_processor_utils.py` & `LangTorch-1.0.4/src/langtorch/api/parallel_processor_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/tools.py` & `LangTorch-1.0.4/src/langtorch/api/tools.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/api/utils.py` & `LangTorch-1.0.4/src/langtorch/api/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/autograd.py` & `LangTorch-1.0.4/src/langtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/conf/__init__.py` & `LangTorch-1.0.4/src/langtorch/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/decorators.py` & `LangTorch-1.0.4/src/langtorch/decorators.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/formatters.py` & `LangTorch-1.0.4/src/langtorch/grammars/formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,51 +61,45 @@
     # and ensure each entry has the same number of lines
     lines = entry.split('\n')
     processed_lines = [line for line in lines for line in process_line(str(line), max_width, wrap_text)]
     padded_lines = [str(line).ljust(max_width) for line in processed_lines]
     padded_lines += [' ' * max_width] * (max_lines - len(processed_lines))  # Pad with empty lines if needed
     return padded_lines
 
-def format_2d(array_2d, max_width=200, wrap_text=False, indent=" "):
+def format_2d(array_2d, max_width=200, wrap_text=False, indent=" ", spacing=2):
     # Calculate max width for each column, but limit the width to column_limit
     n_columns = len(array_2d[0])
     max_width_per_col = [
         min(max(max([len(str(line)) for line in element.split('\n')]) for element in col), max_width // n_columns)
         for col in zip(*array_2d)]
     # Create a list of lists for each formatted line
     formatted_rows = []
+    spacer = ' ' * spacing
     for row in array_2d:
         max_lines_in_row = max(len(process_line(str(line), max_width_per_col[i], wrap_text)) for i, line in enumerate(row))
         formatted_entries = [format_entry(entry, max_lines_in_row, max_width, wrap_text)
                              for entry, max_width in zip(row, max_width_per_col)]
         max_lines_in_row = max(len(m) for m in formatted_entries)
         formatted_entries = [m + [' ' * len(m[0])] * (max_lines_in_row - len(m)) for i, m in enumerate(formatted_entries)]
         transposed_entries = list(zip_longest(*formatted_entries, fillvalue=' ' * max(max_width_per_col)))
 
         for j, transposed_line in enumerate(transposed_entries):
-            line = '  '.join(transposed_line)
+            line = (spacer).join(transposed_line)
             if j == 0:
                 line = indent[1:]+'[' + line + (']' if len(transposed_entries) == 1 else '')
             elif j == len(transposed_entries) - 1:
                 line = indent + line + ']'
             else:
                 line = indent + line + ' '
             formatted_rows.append(line)
     return formatted_rows
 
 def format_1d_as_row(array_1d, column_limit=200, wrap_text=False):
-    max_lines = max(len(process_line(str(line), column_limit, wrap_text)) for line in array_1d)
-    max_width = min(max(max(len(str(line)) for line in str(element).split('\n')) for element in array_1d), column_limit)
-    formatted_entries = [format_entry(entry, max_lines, max_width, wrap_text) for entry in array_1d]
-
-    # Transpose to align multiline entries
-    transposed_entries = list(zip_longest(*formatted_entries, fillvalue=' ' * max_width))
-
-    formatted_rows = ['  '.join(line) for line in transposed_entries]
-    return '[ ' + ('\n' + ' ').join(formatted_rows) + ' ]'
+    formatted_rows = format_2d(array_1d.reshape(1, -1), column_limit, wrap_text)
+    return formatted_rows[0]
 
 def format_1d(array_1d, column_limit=200, wrap_text=False):
     # Treat the 1D array as a 2D array with a single column
     return [m[1:-1] if len(m) >= 2 else m for m in format_2d(array_1d.reshape(-1, 1), column_limit, wrap_text)]
 
 def tensor_str_formatter(cls, array: np.ndarray, indent: str = " ") -> str:
     max_width = ctx.max_width
@@ -116,13 +110,13 @@
         if len(str(array)) > 100:
             formatted_lines = format_1d(array, max_width, wrap_text)
             return '[' + ('\n' + indent).join(formatted_lines) + ']'
         else:
             return format_1d_as_row(array, max_width, wrap_text)
     elif array.ndim == 2:
         indent = ' '
-        formatted_lines = format_2d(array, max_width, wrap_text)
+        formatted_lines = format_2d(array, max_width, wrap_text, spacing=3)
         return indent[1:] + '[' + ('\n' + indent).join(formatted_lines) + ']'
     else:
         inner_arrays = [ indent+tensor_str_formatter(cls, sub_array, indent + '  ') for sub_array in array]
         inner_content = (',\n').join(("\n"+indent).join(a.split("\n")) for a in inner_arrays)
         return '[\n' + inner_content + '\n' + indent[:-2] + ']'
```

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/langtorch_default_parser.py` & `LangTorch-1.0.4/src/langtorch/grammars/langtorch_default_parser.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/pandoc.py` & `LangTorch-1.0.4/src/langtorch/grammars/pandoc.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/parsers.py` & `LangTorch-1.0.4/src/langtorch/grammars/parsers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/text_content_ast.py` & `LangTorch-1.0.4/src/langtorch/grammars/text_content_ast.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/grammars/utils.py` & `LangTorch-1.0.4/src/langtorch/grammars/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/main.py` & `LangTorch-1.0.4/src/langtorch/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,15 @@
 import numpy as np
 import torch
 from langtorch import TextModule
 from langtorch import Chat, ChatML
 
 from langtorch import TextTensor, TextModule, OpenAI
 import torch
-# Without any additional classes we can implement a retriever and RAG module
 
-print(type(TextTensor(["",""]).content))
-
-
-
-quit()
 
 llm = Activation(model="gpt-3.5-turbo", T=0.9, tools=[{"type": "function",
                   "function": {
                     "name": "get_current_weather",
                     "description": "Get the current weather in a given location",
                     "parameters": {
                       "type": "object",
@@ -38,15 +32,15 @@
                           "enum": ["celsius", "fahrenheit"]
                         }
                       },
                       "required": ["location"]
                     }}}], tool_choice="auto")
 
 
-print(llm(TextTensor("What is the current weather in San Francisco?")).item().items())
+# print(llm(TextTensor("What is the current weather in San Francisco?")).item().items())
 # Outputs: [('assistant', ('tool_call', '{"id": "call_6bII1dQHLYWiar5W1eSRDCQu", "type": "function", "function": {"name": "get_current_weather", "arguments": "{\\"location\\":\\"San Francisco\\"}"}}'))]
 
 class ChatML(Chat):
     language = 'chatml'
     allowed_keys = ["user", "assistant", "system"]
 
     def __str__(self):
@@ -58,34 +52,18 @@
     ("system", "Hello!"),
     ("assistant", "Hi! How can I help you today?"),
     ("user", "Tell me about {thing}."),
     ("system", "Hello!"),
     ("assistant", "Hi! How can I help you today?"),
     ("user", "Tell me about {thing}.")
 )
-# Use iloc to make sure you format the right message
-input = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
-for i, m in enumerate([chat_template]):
-    if "system" in m.keys():
-        _ = m.loc["system"].values()[-1]
-        print("sys", _)
-        m = m.loc[["user", "assistant"]]
-    if np.all([key in ["user", "assistant"] for key in m.keys()]):
-        input[i] = [(k, str(Text(v, parse=False))) for k, v in m.items()]
-        print('>', input[i])
-    elif "user" not in m.keys() or "assistant" not in m.keys():
-        # NOT STRICT
-        input[i] = [("user", str(m))]
-    else:
-        raise ValueError(
-            f"Invalid input to OpenAI Chat. Ambigous input: some but not all items in TextTensor entries have keys 'user' or 'assistant'. Change the input into a valid chat, or the input was a single user message remove these keys or use entry.add_key_('user'): \nentry.items()=={m.items()}")
 
-quit()
 # In this case there are no other "thing" values so we could've also used
-chat_template *= {"thing": "the weather"}
+print(TextTensor(["170*32", "123*45/10", "2**10*5"]))
+quit()
 from langtorch import OpenAI
 
 ensemble_llm = OpenAI("gpt-3.5-turbo",
                       system_message="You are a rewriting bot that answers only with the revised text",
                       T=1.1,  # High temperature to sample diverse completions
                       n=5)  # 5 completions for each entry
 paragraphs = Text.from_file("./conf/paper.md").loc["Para"].to_tensor()[:15]
```

### Comparing `LangTorch-1.0.3/src/langtorch/main2.py` & `LangTorch-1.0.4/src/langtorch/main2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from langtorch import Session
 # paper = Text.from_file("D:\langtorch\src\langtorch\conf\paper.md")
 import os
 import logging
 # logging.basicConfig(level=logging.DEBUG)
 # Example usage
 
+import torch
 
+print(TextTensor([[["Yes"],                       ["Yes"]]]).embed())
+quit()
 with Session("test.yaml") as session:
     os.environ["GROQ_API_KEY"] = "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"
     # llm = Activation(model="llama3-70b-8192", provider="groq", T=1.2, max_tokens=350)
     llm = Activation(model="gpt-4o",  T=0., max_tokens=350)
     # llm = Activation(model="claude-3-opus-20240229", provider="anthropic", max_tokens=10)
     # chat = TextTensor({"user": input()})
     chat = TextTensor({"user": "make ascii art of donald trump"})
```

### Comparing `LangTorch-1.0.3/src/langtorch/methods/chain_of_density.py` & `LangTorch-1.0.4/src/langtorch/methods/chain_of_density.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/methods/chain_of_thought.py` & `LangTorch-1.0.4/src/langtorch/methods/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/methods/embeddings.py` & `LangTorch-1.0.4/src/langtorch/methods/embeddings.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/optim/optimizer.py` & `LangTorch-1.0.4/src/langtorch/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/semalg_utils.py` & `LangTorch-1.0.4/src/langtorch/semalg_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/semantic_algebra.py` & `LangTorch-1.0.4/src/langtorch/semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/session.py` & `LangTorch-1.0.4/src/langtorch/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,22 +217,22 @@
         ids, _ = self.request(provider, type, request_strings, False)
         responses = [self.get_response(id) for id in ids]
         for i, response in enumerate(responses):
             if response is None:
                 raise ValueError(f"Could not find response for {request_strings[i]}")
 
         if type == "embeddings":
-            return torch.vstack(responses).permute((1,0))
+            return torch.vstack(responses)#.permute((1,0))
         else:
             from langtorch import TextTensor
             responses = [
                 [text.add_key("assistant") if len(text.items()) != 0 and text.items()[0][0] != "assistant" else text for
                  text in response] for
                 response in responses]
-            return TextTensor(responses, parse=False).permute((1, 0))
+            return TextTensor(responses, parse=False)#.permute((1, 0))
 
 
     def __setattr__(self, name, value, save=True):
         if name in ["_config", "_tensors", "_session_file", "_overwrite"]:
             super().__setattr__(name, value)
             if name == "_config" and self._path and save:
                 self.save()
```

### Comparing `LangTorch-1.0.3/src/langtorch/tensors/chattensor.py` & `LangTorch-1.0.4/src/langtorch/tensors/chattensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tensors/codetensor.py` & `LangTorch-1.0.4/src/langtorch/tensors/codetensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tensors/markdowntensor.py` & `LangTorch-1.0.4/src/langtorch/tensors/markdowntensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tensors/texttensor.py` & `LangTorch-1.0.4/src/langtorch/tensors/texttensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,27 +144,32 @@
 
 
         def dict_to_tt(cls, d, parse):  # TODO create from dict of tensors
             if not d:
                 return None
 
             def item_to_tt(cls, k, v, parse):
-                content = cls.input_formatter(cls.content_to_object_array(v, parse=parse))
-                content = np.array([(k, v) for v in content.flat], dtype=object).reshape(content.shape)
-                return cls.__new__(cls, content, parse=parse)
-
-            content = item_to_tt(cls, d.items()[0][0], d.items()[0][1], parse=parse)
-            for k, v in d.items()[1:]:
-                content += item_to_tt(cls, k, v, parse=parse)
+                tt = cls.__new__(cls, v, parse=parse)
+                return cls([(k,t) for t in tt.flat], parse=False).reshape(tt.shape)
+
+            items = iter(d.items())
+            first = next(items)
+            content = item_to_tt(cls, first[0], first[1], parse=parse)
+            first_shape = content.shape
+            for k, v in items:
+                content += item_to_tt(cls, k, v, parse=parse).reshape(first_shape)
             return content
 
         def replace_tuple_with_ttype(tpl):
             nonlocal cls
-            return cls._ttype(tpl)
+            return cls._ttype(*tpl)
 
+        # if isinstance(metadata["content"], dict):
+        #     metadata["content"] = dict_to_tt(cls, metadata["content"], parse=parse)
+        # Replace tuples with Text entries
         metadata["content"] = cls.recursive_walk_replace(metadata["content"], tuple, replace_tuple_with_ttype)
         # Set content to be an object array with cls.text_class entries
         metadata["content"] = cls.content_to_object_array(metadata["content"], parse=parse)
         # Apply input formatter
         metadata["content"] = cls.input_formatter(metadata["content"])
 
         tensor = super().__new__(cls, torch.arange(metadata["content"].size, dtype=torch.float32).reshape(
@@ -339,34 +344,42 @@
 
     @classmethod
     def _handle_functions_on_embeddings(self, func: Callable, *args, **kwargs):
         """Substitutes the TextTensor entries with their embeddings and applies the function."""
 
         def apply_to_texttensors(func, args, kwargs):
             args2, kwargs2 = [], {}
+            first = None
             for i, arg in enumerate(args):
                 if isinstance(arg, TextTensor):
                     args2.append(func(arg))
+                    if first is None:
+                        first = arg
                 else:
                     args.append(arg)
             for k, arg in kwargs.items():
                 if isinstance(arg, TextTensor):
                     kwargs2[k] = func(arg)
+                    if first is None:
+                        first = arg
                 else:
                     kwargs2[k] = arg
 
-            return args2, kwargs2
+            return first, args2, kwargs2
 
-        def apply_embed(tensor) -> torch.Tensor:
-            if tensor.embedding is None:
-                tensor.embed()
+        def apply_embed(tensor, model = None) -> torch.Tensor:
+            tensor.embed(model=model)
             assert isinstance(tensor.embedding, torch.Tensor)
             return tensor.embedding
 
-        args, kwargs = apply_to_texttensors(apply_embed, args, kwargs)
+        first, args, kwargs = apply_to_texttensors(lambda t:t, args, kwargs)
+        model = kwargs.pop("model", None)
+        if model is None:
+            model = first.embedding_model
+        first, args, kwargs = apply_to_texttensors(lambda t:apply_embed(t, model), args, kwargs)
 
         if func is torch.cosine_similarity:
             kwargs["dim"] = -1
             # args = [a.reshape(-1) for a in args]
             return torch.cosine_similarity(*args, **kwargs)
 
         return func(*args, **kwargs)
@@ -810,19 +823,24 @@
     def T(self):  # diff!
         return self.__class__(self.content.T, super().mT, parse=False)
 
     @property
     def mT(self):  # diff!
         return self.__class__(self.content.T, super().mT, parse=False)
 
-    def embed(self, model="default", verbose=False):
-        if model == "default":
+    def embed(self, model=None, verbose=False):
+        if model is None:
             model = self._embedding_model
+        else:
+            self.embedding_model = model
         assert model is not None
-        self.embedding = get_embedding(self, model=model, verbose=verbose)
+        if callable(model):
+            self.embedding = model([str(m) for m in self.flat]).reshape(self.shape + (-1,))
+        else:
+            self.embedding = get_embedding(self, model=model, verbose=verbose)
         return self.embedding
 
     def apply(self, func):
         """Applies a function to each entry of self.content."""
         # Ensure the function is callable
         if not callable(func):
             raise ValueError("Provided function is not callable.")
```

### Comparing `LangTorch-1.0.3/src/langtorch/texts/chat.py` & `LangTorch-1.0.4/src/langtorch/texts/chat.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/texts/markdown.py` & `LangTorch-1.0.4/src/langtorch/texts/markdown.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/texts/text.py` & `LangTorch-1.0.4/src/langtorch/texts/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     def to_tensor(self, **kwargs):
         from langtorch import TextTensor
         if not "ttype" in kwargs:
             kwargs["ttype"] = self.__class__
             kwargs["ttype"].language = self.language
         if not "parse" in kwargs:
             kwargs["parse"] = False
-        return TextTensor(self.items(), **kwargs)
+        return TextTensor([(kv,) for kv in self.items()], **kwargs)
 
     @property
     def identity(self):
         return self.__class__()
 
     @property
     def content(self):
@@ -602,56 +602,55 @@
                     return True
                 elif v == k_:
                     result[ind] = (k, v_)
                     formatted_indices.append(i)
                     return True
             return False
 
-        def handle_positional_args(k_, v_, i, result, formatted_indices, indices_to_delete, positional_j):
-            for j, (k, v) in enumerate(content):
-                if v == str(positional_j):
-                    result[j] = (k, v_)
-                    positional_j += 1
-                    formatted_indices.append(j)
-                    return positional_j
-            for j, (k, v) in enumerate(content):
-                if v == "":
-                    result[j] = (k, v_)
-                    formatted_indices.append(j)
-                    if v_ == k:
-                        indices_to_delete.append(j)
-                    return positional_j
-            result.append((k_, v_))
-            return positional_j
-
-        content = self.items()
-        result = content[:]
-        formatted_indices = []
-        indices_to_delete = []
-        positional_j = 0
+        items = self.items()
+        result = items[:]
+        items_other = other.items()
 
-        for i, (k, v) in enumerate(content):
+        for i, (k, v) in enumerate(items):
             if v == "*":
                 if k == "":
                     result = result[:i] + list(other.items()) + result[i + 1:]
                 else:
                     result[i] = (k, other.items())
                 return self.__class__(*result, parse=False)
 
-        for k_, v_ in other.items():
-            if v_ == "*":
-                result = [(k_, [item for i, item in enumerate(result) if i not in indices_to_delete])]
-                indices_to_delete = []
-                formatted_indices = []
-            elif k_ == "":
-                positional_j = handle_positional_args(k_, v_, i, result, formatted_indices, indices_to_delete,
-                                                      positional_j)
-            else:  # Key substitution
+        # if v_ == "*":
+        #     result = [(k_, [item for i, item in enumerate(result) if i not in indices_to_delete])]
+        replacement_map = {}
+        for i, (k, v) in enumerate(items):
+            if isinstance(v, str) and v.isdigit():
+                if int(v)<len(items_other):
+                    replacement_map[i] = int(v)
+        for i, (k, v) in enumerate(items):
+            if isinstance(v, str) and v == "":
+                try:
+                    replacement_map[i] = next(j for j in range(len(items_other)) if j not in replacement_map.values())
+                except StopIteration: # no more items in other
+                    break
+
+        # Replace entries of result according to replacement_map
+        for i, j in replacement_map.items():
+            if items_other[j][0] == "":
+                result[i] = (result[i][0], items_other[j][1])
+            elif result[i][0] == "":
+                result[i] = items_other[j]
+            else:
+                result[i] = (result[i][0], items_other[j])
+
+        formatted_indices = list(replacement_map.keys())
+        indices_to_delete = []
+        for j, (k_, v_) in enumerate(items_other):
+            if j not in replacement_map.values():
                 k_, v_ = flatten_keys(k_, v_)
-                for i, (k, v) in enumerate(content):
+                for i, (k, v) in enumerate(items):
                     if match_mul_rule(k, v, k_, v_, i, result, formatted_indices, indices_to_delete):
                         break
                 else:
                     result.append((k_, v_))
 
         def del_ind(subresult, index):
             if isinstance(subresult, tuple):
```

### Comparing `LangTorch-1.0.3/src/langtorch/tt/functional.py` & `LangTorch-1.0.4/src/langtorch/tt/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 
 
 class MulTextTensor(Function):
     @staticmethod
     def forward(ctx, input1, input2):
         # Store the input for backward computation
         assert isinstance(input1, langtorch.TextTensor) and hasattr(input1, "content"), input1
-        assert isinstance(input2, langtorch.TextTensor) and hasattr(input2, "content"), input2
+        if not isinstance(input2, langtorch.TextTensor):
+            input2 = langtorch.TextTensor([input2] * len(input1.flat), parse=False).reshape(input1.shape)
         ctx.save_for_backward(input1, input2)
 
         # Compute the result using the content attribute's multiplication
         result = input1.__class__(input1.content * input2.content, parse=False)
         return (result)
 
     @staticmethod
```

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_t/distance.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_t/distance.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_t/tokenizer.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_t/tokenizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/activation.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/activation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/assistantmodule.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/assistantmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/codemodule.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/codemodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/conv.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/linear.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/linear.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/loss.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/loss.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/retriever.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/retriever.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/textmodule.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/textmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformers.py` & `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,18 @@
         tokenizer_default_kwargs = {"return_tensors": "pt", "padding": True, "truncation": True}
         # Update tokenizer_kwargs with default values if the value isn't overriden
         tokenizer_kwargs = {**tokenizer_default_kwargs, **tokenizer_kwargs}
         self.tokenizer_kwargs = tokenizer_kwargs
         self.model_kwargs = model_kwargs
 
     def forward(self, input_texttensor: TextTensor, skip_special_tokens=True, **gen_kwargs) -> TextTensor:
-        assert isinstance(input_texttensor, TextTensor)
-        # Convert TextTensor to a list of strings
-        texts = [str(entry) for entry in input_texttensor.flat]
+        input_texttensor = TextTensor(input_texttensor, tokenizer = self.tokenizer, tokenizer_kwargs=self.tokenizer_kwargs)
 
         # Tokenize and generate responses
-        inputs = self.tokenizer(texts, **self.tokenizer_kwargs).to(self.model.device)
+        inputs = input_texttensor.tokenize().to(self.model.device)
         with torch.no_grad():
             outputs = self.model.generate(**inputs, **self.model_kwargs, **gen_kwargs)
 
         # Decode responses and convert to TextTensor
         decoded_texts = [self.tokenizer.decode(output, skip_special_tokens=skip_special_tokens) for output in outputs]
         output = TextTensor([str(text) for text in decoded_texts], parse=False).reshape(input_texttensor.shape)
```

### Comparing `LangTorch-1.0.3/src/langtorch/types.py` & `LangTorch-1.0.4/src/langtorch/types.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/src/langtorch/utils.py` & `LangTorch-1.0.4/src/langtorch/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_activation.py` & `LangTorch-1.0.4/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_autograd.py` & `LangTorch-1.0.4/tests/test_autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_conv.py` & `LangTorch-1.0.4/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_embedding.py` & `LangTorch-1.0.4/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_functional.py` & `LangTorch-1.0.4/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_group_operation.py` & `LangTorch-1.0.4/tests/test_group_operation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_methods.py` & `LangTorch-1.0.4/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_mul.py` & `LangTorch-1.0.4/tests/test_mul.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_optimizer.py` & `LangTorch-1.0.4/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_pandoc.py` & `LangTorch-1.0.4/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_semantic_algebra.py` & `LangTorch-1.0.4/tests/test_semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_session.py` & `LangTorch-1.0.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_session_api.py` & `LangTorch-1.0.4/tests/test_session_api.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_text.py` & `LangTorch-1.0.4/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_texttensor.py` & `LangTorch-1.0.4/tests/test_texttensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_texttensor_constructor.py` & `LangTorch-1.0.4/tests/test_texttensor_constructor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.3/tests/test_visualize.py` & `LangTorch-1.0.4/tests/test_visualize.py`

 * *Files identical despite different names*

