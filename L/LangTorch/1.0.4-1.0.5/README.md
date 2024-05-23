# Comparing `tmp/LangTorch-1.0.4.tar.gz` & `tmp/LangTorch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LangTorch-1.0.4.tar", last modified: Thu May 23 14:47:44 2024, max compression
+gzip compressed data, was "LangTorch-1.0.5.tar", last modified: Thu May 23 21:42:53 2024, max compression
```

## Comparing `LangTorch-1.0.4.tar` & `LangTorch-1.0.5.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.046865 LangTorch-1.0.4/
--rw-rw-rw-   0        0        0     6673 2024-05-23 14:47:44.045863 LangTorch-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5968 2024-04-14 08:46:21.000000 LangTorch-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 14:47:44.046865 LangTorch-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1467 2024-05-23 14:47:37.000000 LangTorch-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.938871 LangTorch-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.954867 LangTorch-1.0.4/src/LangTorch.egg-info/
--rw-rw-rw-   0        0        0     6673 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3458 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 14:47:43.000000 LangTorch-1.0.4/src/LangTorch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.966867 LangTorch-1.0.4/src/langtorch/
--rw-rw-rw-   0        0        0     9127 2024-05-17 09:29:22.000000 LangTorch-1.0.4/src/langtorch/_VariableFunctions.py
--rw-rw-rw-   0        0        0      597 2024-05-17 13:20:07.000000 LangTorch-1.0.4/src/langtorch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.978026 LangTorch-1.0.4/src/langtorch/api/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.4/src/langtorch/api/TODO_anthropic_parallel_processor.py
--rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/api/TODO_assistant.py
--rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/api/TODO_gcp_parallel_processor.py
--rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/api/__init__.py
--rw-rw-rw-   0        0        0     1111 2024-05-17 01:10:31.000000 LangTorch-1.0.4/src/langtorch/api/api_threading.py
--rw-rw-rw-   0        0        0    13895 2024-05-23 10:29:24.000000 LangTorch-1.0.4/src/langtorch/api/call.py
--rw-rw-rw-   0        0        0        0 2024-05-16 22:19:27.000000 LangTorch-1.0.4/src/langtorch/api/groq.py
--rw-rw-rw-   0        0        0     6810 2024-05-17 01:30:15.000000 LangTorch-1.0.4/src/langtorch/api/openai.py
--rw-rw-rw-   0        0        0     9982 2024-05-17 20:16:36.000000 LangTorch-1.0.4/src/langtorch/api/parallel_processor_utils.py
--rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/api/tools.py
--rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/api/utils.py
--rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.4/src/langtorch/autograd.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.980580 LangTorch-1.0.4/src/langtorch/conf/
--rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.4/src/langtorch/conf/__init__.py
--rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/conf/new_session_template.yaml
--rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.4/src/langtorch/conf/overrides.yaml
--rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.4/src/langtorch/decorators.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.987451 LangTorch-1.0.4/src/langtorch/grammars/
--rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.4/src/langtorch/grammars/__init__.py
--rw-rw-rw-   0        0        0     5425 2024-05-23 03:22:00.000000 LangTorch-1.0.4/src/langtorch/grammars/formatters.py
--rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/grammars/langtorch_default_parser.py
--rw-rw-rw-   0        0        0     5359 2024-05-17 03:05:19.000000 LangTorch-1.0.4/src/langtorch/grammars/pandoc.py
--rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/grammars/parsers.py
--rw-rw-rw-   0        0        0     6102 2024-05-17 02:21:53.000000 LangTorch-1.0.4/src/langtorch/grammars/text_content_ast.py
--rw-rw-rw-   0        0        0     2343 2024-05-17 03:11:04.000000 LangTorch-1.0.4/src/langtorch/grammars/utils.py
--rw-rw-rw-   0        0        0     7065 2024-05-23 03:19:29.000000 LangTorch-1.0.4/src/langtorch/main.py
--rw-rw-rw-   0        0        0     2408 2024-05-23 10:25:58.000000 LangTorch-1.0.4/src/langtorch/main2.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.991449 LangTorch-1.0.4/src/langtorch/methods/
--rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.4/src/langtorch/methods/__init__.py
--rw-rw-rw-   0        0        0     2704 2024-05-17 09:31:29.000000 LangTorch-1.0.4/src/langtorch/methods/chain_of_density.py
--rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.4/src/langtorch/methods/chain_of_thought.py
--rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/methods/embeddings.py
--rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.4/src/langtorch/methods/prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.992450 LangTorch-1.0.4/src/langtorch/optim/
--rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.4/src/langtorch/optim/__init__.py
--rw-rw-rw-   0        0        0     2189 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/optim/optimizer.py
--rw-rw-rw-   0        0        0      574 2024-05-17 09:32:04.000000 LangTorch-1.0.4/src/langtorch/semalg_utils.py
--rw-rw-rw-   0        0        0     4639 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/semantic_algebra.py
--rw-rw-rw-   0        0        0    13202 2024-05-23 10:27:01.000000 LangTorch-1.0.4/src/langtorch/session.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:43.998457 LangTorch-1.0.4/src/langtorch/tensors/
--rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.4/src/langtorch/tensors/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.4/src/langtorch/tensors/chattensor.py
--rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.4/src/langtorch/tensors/codetensor.py
--rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.4/src/langtorch/tensors/langtorchtensor.py
--rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.4/src/langtorch/tensors/markdowntensor.py
--rw-rw-rw-   0        0        0    43291 2024-05-23 07:39:05.000000 LangTorch-1.0.4/src/langtorch/tensors/texttensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.006485 LangTorch-1.0.4/src/langtorch/texts/
--rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.4/src/langtorch/texts/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-05-15 02:21:06.000000 LangTorch-1.0.4/src/langtorch/texts/chat.py
--rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.4/src/langtorch/texts/code.py
--rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.4/src/langtorch/texts/markdown.py
--rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/texts/markup.py
--rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/texts/string.py
--rw-rw-rw-   0        0        0    36660 2024-05-23 10:35:29.000000 LangTorch-1.0.4/src/langtorch/texts/text.py
--rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.4/src/langtorch/texts/thread.py
--rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.4/src/langtorch/torch_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.007483 LangTorch-1.0.4/src/langtorch/tt/
--rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/__init__.py
--rw-rw-rw-   0        0        0    30677 2024-05-23 01:51:12.000000 LangTorch-1.0.4/src/langtorch/tt/functional.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.009582 LangTorch-1.0.4/src/langtorch/tt/modules/
--rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.4/src/langtorch/tt/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.011103 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.4/src/langtorch/tt/modules/from_t/transformers_automodel.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.014092 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/__init__.py
--rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/distance.py
--rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/embedding.py
--rw-rw-rw-   0        0        0     1312 2024-05-17 09:29:49.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_t/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.028614 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/
--rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/__init__.py
--rw-rw-rw-   0        0        0    22439 2024-05-17 05:36:08.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/activation.py
--rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/assistantmodule.py
--rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/chatmodule.py
--rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/codemodule.py
--rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/conv.py
--rw-rw-rw-   0        0        0     1623 2024-05-17 18:27:32.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/linear.py
--rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/loss.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/pooling.py
--rw-rw-rw-   0        0        0      883 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/retriever.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/rnn.py
--rw-rw-rw-   0        0        0     7195 2024-05-17 18:27:32.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/textmodule.py
--rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformer.py
--rw-rw-rw-   0        0        0     1942 2024-05-23 01:25:33.000000 LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformers.py
--rw-rw-rw-   0        0        0     1268 2024-05-17 09:34:15.000000 LangTorch-1.0.4/src/langtorch/types.py
--rw-rw-rw-   0        0        0     8335 2024-05-17 09:34:19.000000 LangTorch-1.0.4/src/langtorch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:47:44.045863 LangTorch-1.0.4/tests/
--rw-rw-rw-   0        0        0      845 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_activation.py
--rw-rw-rw-   0        0        0     1358 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_autograd.py
--rw-rw-rw-   0        0        0     6419 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_conv.py
--rw-rw-rw-   0        0        0      292 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_dspy.py
--rw-rw-rw-   0        0        0     2487 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_embedding.py
--rw-rw-rw-   0        0        0     4094 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_functional.py
--rw-rw-rw-   0        0        0     6075 2024-03-30 15:39:03.000000 LangTorch-1.0.4/tests/test_group_operation.py
--rw-rw-rw-   0        0        0      489 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_import.py
--rw-rw-rw-   0        0        0      433 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_markdown.py
--rw-rw-rw-   0        0        0     1056 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_methods.py
--rw-rw-rw-   0        0        0     6393 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_mul.py
--rw-rw-rw-   0        0        0     2274 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_optimizer.py
--rw-rw-rw-   0        0        0     5417 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_pandoc.py
--rw-rw-rw-   0        0        0     1994 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_semantic_algebra.py
--rw-rw-rw-   0        0        0     4400 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_session.py
--rw-rw-rw-   0        0        0     1397 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_session_api.py
--rw-rw-rw-   0        0        0     1764 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_text.py
--rw-rw-rw-   0        0        0     3935 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_texttensor.py
--rw-rw-rw-   0        0        0      727 2024-05-17 09:28:38.000000 LangTorch-1.0.4/tests/test_texttensor_constructor.py
--rw-rw-rw-   0        0        0      938 2024-05-17 09:26:53.000000 LangTorch-1.0.4/tests/test_visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.670842 LangTorch-1.0.5/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 21:42:53.670842 LangTorch-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5968 2024-04-14 08:46:21.000000 LangTorch-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:42:53.671842 LangTorch-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2024-05-23 20:42:25.000000 LangTorch-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.518623 LangTorch-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.539675 LangTorch-1.0.5/src/LangTorch.egg-info/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 21:42:53.000000 LangTorch-1.0.5/src/LangTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3491 2024-05-23 21:42:53.000000 LangTorch-1.0.5/src/LangTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:42:53.000000 LangTorch-1.0.5/src/LangTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-23 21:42:53.000000 LangTorch-1.0.5/src/LangTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 21:42:53.000000 LangTorch-1.0.5/src/LangTorch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.556686 LangTorch-1.0.5/src/langtorch/
+-rw-rw-rw-   0        0        0     9127 2024-05-17 09:29:22.000000 LangTorch-1.0.5/src/langtorch/_VariableFunctions.py
+-rw-rw-rw-   0        0        0      597 2024-05-17 13:20:07.000000 LangTorch-1.0.5/src/langtorch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.569780 LangTorch-1.0.5/src/langtorch/api/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.5/src/langtorch/api/TODO_anthropic_parallel_processor.py
+-rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.5/src/langtorch/api/TODO_assistant.py
+-rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.5/src/langtorch/api/TODO_gcp_parallel_processor.py
+-rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/api/__init__.py
+-rw-rw-rw-   0        0        0     1111 2024-05-17 01:10:31.000000 LangTorch-1.0.5/src/langtorch/api/api_threading.py
+-rw-rw-rw-   0        0        0    13895 2024-05-23 10:29:24.000000 LangTorch-1.0.5/src/langtorch/api/call.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 22:19:27.000000 LangTorch-1.0.5/src/langtorch/api/groq.py
+-rw-rw-rw-   0        0        0     6810 2024-05-17 01:30:15.000000 LangTorch-1.0.5/src/langtorch/api/openai.py
+-rw-rw-rw-   0        0        0     9982 2024-05-17 20:16:36.000000 LangTorch-1.0.5/src/langtorch/api/parallel_processor_utils.py
+-rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.5/src/langtorch/api/tools.py
+-rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.5/src/langtorch/api/utils.py
+-rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.5/src/langtorch/autograd.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.575777 LangTorch-1.0.5/src/langtorch/conf/
+-rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.5/src/langtorch/conf/__init__.py
+-rw-rw-rw-   0        0        0     2784 2024-05-17 04:56:42.000000 LangTorch-1.0.5/src/langtorch/conf/defaults.yaml
+-rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.5/src/langtorch/conf/new_session_template.yaml
+-rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.5/src/langtorch/conf/overrides.yaml
+-rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.5/src/langtorch/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.585776 LangTorch-1.0.5/src/langtorch/grammars/
+-rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.5/src/langtorch/grammars/__init__.py
+-rw-rw-rw-   0        0        0     5425 2024-05-23 03:22:00.000000 LangTorch-1.0.5/src/langtorch/grammars/formatters.py
+-rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.5/src/langtorch/grammars/langtorch_default_parser.py
+-rw-rw-rw-   0        0        0     5359 2024-05-17 03:05:19.000000 LangTorch-1.0.5/src/langtorch/grammars/pandoc.py
+-rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.5/src/langtorch/grammars/parsers.py
+-rw-rw-rw-   0        0        0     6102 2024-05-17 02:21:53.000000 LangTorch-1.0.5/src/langtorch/grammars/text_content_ast.py
+-rw-rw-rw-   0        0        0     2343 2024-05-17 03:11:04.000000 LangTorch-1.0.5/src/langtorch/grammars/utils.py
+-rw-rw-rw-   0        0        0     7065 2024-05-23 03:19:29.000000 LangTorch-1.0.5/src/langtorch/main.py
+-rw-rw-rw-   0        0        0     2408 2024-05-23 10:25:58.000000 LangTorch-1.0.5/src/langtorch/main2.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.591775 LangTorch-1.0.5/src/langtorch/methods/
+-rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.5/src/langtorch/methods/__init__.py
+-rw-rw-rw-   0        0        0     2704 2024-05-17 09:31:29.000000 LangTorch-1.0.5/src/langtorch/methods/chain_of_density.py
+-rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.5/src/langtorch/methods/chain_of_thought.py
+-rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/methods/embeddings.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.5/src/langtorch/methods/prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.593889 LangTorch-1.0.5/src/langtorch/optim/
+-rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.5/src/langtorch/optim/__init__.py
+-rw-rw-rw-   0        0        0     2189 2024-05-17 09:34:15.000000 LangTorch-1.0.5/src/langtorch/optim/optimizer.py
+-rw-rw-rw-   0        0        0      574 2024-05-17 09:32:04.000000 LangTorch-1.0.5/src/langtorch/semalg_utils.py
+-rw-rw-rw-   0        0        0     4639 2024-05-17 09:34:15.000000 LangTorch-1.0.5/src/langtorch/semantic_algebra.py
+-rw-rw-rw-   0        0        0    13202 2024-05-23 10:27:01.000000 LangTorch-1.0.5/src/langtorch/session.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.604889 LangTorch-1.0.5/src/langtorch/tensors/
+-rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.5/src/langtorch/tensors/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.5/src/langtorch/tensors/chattensor.py
+-rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.5/src/langtorch/tensors/codetensor.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.5/src/langtorch/tensors/langtorchtensor.py
+-rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.5/src/langtorch/tensors/markdowntensor.py
+-rw-rw-rw-   0        0        0    43291 2024-05-23 07:39:05.000000 LangTorch-1.0.5/src/langtorch/tensors/texttensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.618068 LangTorch-1.0.5/src/langtorch/texts/
+-rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.5/src/langtorch/texts/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-05-15 02:21:06.000000 LangTorch-1.0.5/src/langtorch/texts/chat.py
+-rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.5/src/langtorch/texts/code.py
+-rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.5/src/langtorch/texts/markdown.py
+-rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/texts/markup.py
+-rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/texts/string.py
+-rw-rw-rw-   0        0        0    36660 2024-05-23 10:35:29.000000 LangTorch-1.0.5/src/langtorch/texts/text.py
+-rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.5/src/langtorch/texts/thread.py
+-rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.5/src/langtorch/torch_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.620073 LangTorch-1.0.5/src/langtorch/tt/
+-rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.5/src/langtorch/tt/__init__.py
+-rw-rw-rw-   0        0        0    30677 2024-05-23 01:51:12.000000 LangTorch-1.0.5/src/langtorch/tt/functional.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.621068 LangTorch-1.0.5/src/langtorch/tt/modules/
+-rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.5/src/langtorch/tt/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.623078 LangTorch-1.0.5/src/langtorch/tt/modules/from_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.5/src/langtorch/tt/modules/from_t/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.5/src/langtorch/tt/modules/from_t/transformers_automodel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.626073 LangTorch-1.0.5/src/langtorch/tt/modules/to_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_t/__init__.py
+-rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_t/distance.py
+-rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_t/embedding.py
+-rw-rw-rw-   0        0        0     1312 2024-05-17 09:29:49.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_t/tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.644441 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/
+-rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/__init__.py
+-rw-rw-rw-   0        0        0    22439 2024-05-17 05:36:08.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/activation.py
+-rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/assistantmodule.py
+-rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/chatmodule.py
+-rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/codemodule.py
+-rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/conv.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 18:27:32.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/linear.py
+-rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/loss.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/pooling.py
+-rw-rw-rw-   0        0        0      883 2024-05-17 09:34:15.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/retriever.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/rnn.py
+-rw-rw-rw-   0        0        0     7195 2024-05-17 18:27:32.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/textmodule.py
+-rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/transformer.py
+-rw-rw-rw-   0        0        0     1942 2024-05-23 01:25:33.000000 LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/transformers.py
+-rw-rw-rw-   0        0        0     1268 2024-05-17 09:34:15.000000 LangTorch-1.0.5/src/langtorch/types.py
+-rw-rw-rw-   0        0        0     8335 2024-05-17 09:34:19.000000 LangTorch-1.0.5/src/langtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:42:53.669840 LangTorch-1.0.5/tests/
+-rw-rw-rw-   0        0        0      845 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_activation.py
+-rw-rw-rw-   0        0        0     1358 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_autograd.py
+-rw-rw-rw-   0        0        0     6419 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_conv.py
+-rw-rw-rw-   0        0        0      292 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_dspy.py
+-rw-rw-rw-   0        0        0     2487 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_embedding.py
+-rw-rw-rw-   0        0        0     4094 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6075 2024-03-30 15:39:03.000000 LangTorch-1.0.5/tests/test_group_operation.py
+-rw-rw-rw-   0        0        0      489 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_import.py
+-rw-rw-rw-   0        0        0      433 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_markdown.py
+-rw-rw-rw-   0        0        0     1056 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_methods.py
+-rw-rw-rw-   0        0        0     6393 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_mul.py
+-rw-rw-rw-   0        0        0     2274 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_optimizer.py
+-rw-rw-rw-   0        0        0     5417 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_pandoc.py
+-rw-rw-rw-   0        0        0     1994 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_semantic_algebra.py
+-rw-rw-rw-   0        0        0     4400 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_session.py
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_session_api.py
+-rw-rw-rw-   0        0        0     1764 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_text.py
+-rw-rw-rw-   0        0        0     3935 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_texttensor.py
+-rw-rw-rw-   0        0        0      727 2024-05-17 09:28:38.000000 LangTorch-1.0.5/tests/test_texttensor_constructor.py
+-rw-rw-rw-   0        0        0      938 2024-05-17 09:26:53.000000 LangTorch-1.0.5/tests/test_visualize.py
```

### Comparing `LangTorch-1.0.4/PKG-INFO` & `LangTorch-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.4
+Version: 1.0.5
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LangTorch-1.0.4/README.md` & `LangTorch-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/setup.py` & `LangTorch-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LangTorch",
-    version="1.0.4",
+    version="1.0.5",
     description="Framework for intuitive LLM application development with tensors.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Adam Sobieszek",
     author_email="contact@langtorch.org",
     url="https://github.com/AdamSobieszek/LangTorch",
     packages=find_packages(where="src"),
@@ -34,11 +34,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="LangTorch, PyTorch, LLM, Language Models, Chat, Chains",
     package_data={
-        'langtorch': ['cong/defaults.yaml', 'conf/new_session_template.yaml','conf/overrides.yaml', 'methods/prompts.yaml'],
+        'langtorch': ['conf/defaults.yaml', 'conf/new_session_template.yaml','conf/overrides.yaml', 'methods/prompts.yaml'],
     },
     include_package_data=True,
 )
```

### Comparing `LangTorch-1.0.4/src/LangTorch.egg-info/PKG-INFO` & `LangTorch-1.0.5/src/LangTorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.4
+Version: 1.0.5
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LangTorch-1.0.4/src/LangTorch.egg-info/SOURCES.txt` & `LangTorch-1.0.5/src/LangTorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/langtorch/api/call.py
 src/langtorch/api/groq.py
 src/langtorch/api/openai.py
 src/langtorch/api/parallel_processor_utils.py
 src/langtorch/api/tools.py
 src/langtorch/api/utils.py
 src/langtorch/conf/__init__.py
+src/langtorch/conf/defaults.yaml
 src/langtorch/conf/new_session_template.yaml
 src/langtorch/conf/overrides.yaml
 src/langtorch/grammars/__init__.py
 src/langtorch/grammars/formatters.py
 src/langtorch/grammars/langtorch_default_parser.py
 src/langtorch/grammars/pandoc.py
 src/langtorch/grammars/parsers.py
```

### Comparing `LangTorch-1.0.4/src/langtorch/_VariableFunctions.py` & `LangTorch-1.0.5/src/langtorch/_VariableFunctions.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/__init__.py` & `LangTorch-1.0.5/src/langtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/TODO_assistant.py` & `LangTorch-1.0.5/src/langtorch/api/TODO_assistant.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/TODO_gcp_parallel_processor.py` & `LangTorch-1.0.5/src/langtorch/api/TODO_gcp_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/api_threading.py` & `LangTorch-1.0.5/src/langtorch/api/api_threading.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/call.py` & `LangTorch-1.0.5/src/langtorch/api/call.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/openai.py` & `LangTorch-1.0.5/src/langtorch/api/openai.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/parallel_processor_utils.py` & `LangTorch-1.0.5/src/langtorch/api/parallel_processor_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/tools.py` & `LangTorch-1.0.5/src/langtorch/api/tools.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/api/utils.py` & `LangTorch-1.0.5/src/langtorch/api/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/autograd.py` & `LangTorch-1.0.5/src/langtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/conf/__init__.py` & `LangTorch-1.0.5/src/langtorch/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/decorators.py` & `LangTorch-1.0.5/src/langtorch/decorators.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/formatters.py` & `LangTorch-1.0.5/src/langtorch/grammars/formatters.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/langtorch_default_parser.py` & `LangTorch-1.0.5/src/langtorch/grammars/langtorch_default_parser.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/pandoc.py` & `LangTorch-1.0.5/src/langtorch/grammars/pandoc.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/parsers.py` & `LangTorch-1.0.5/src/langtorch/grammars/parsers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/text_content_ast.py` & `LangTorch-1.0.5/src/langtorch/grammars/text_content_ast.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/grammars/utils.py` & `LangTorch-1.0.5/src/langtorch/grammars/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/main.py` & `LangTorch-1.0.5/src/langtorch/main.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/main2.py` & `LangTorch-1.0.5/src/langtorch/main2.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/methods/chain_of_density.py` & `LangTorch-1.0.5/src/langtorch/methods/chain_of_density.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/methods/chain_of_thought.py` & `LangTorch-1.0.5/src/langtorch/methods/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/methods/embeddings.py` & `LangTorch-1.0.5/src/langtorch/methods/embeddings.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/optim/optimizer.py` & `LangTorch-1.0.5/src/langtorch/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/semalg_utils.py` & `LangTorch-1.0.5/src/langtorch/semalg_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/semantic_algebra.py` & `LangTorch-1.0.5/src/langtorch/semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/session.py` & `LangTorch-1.0.5/src/langtorch/session.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tensors/chattensor.py` & `LangTorch-1.0.5/src/langtorch/tensors/chattensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tensors/codetensor.py` & `LangTorch-1.0.5/src/langtorch/tensors/codetensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tensors/markdowntensor.py` & `LangTorch-1.0.5/src/langtorch/tensors/markdowntensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tensors/texttensor.py` & `LangTorch-1.0.5/src/langtorch/tensors/texttensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/texts/chat.py` & `LangTorch-1.0.5/src/langtorch/texts/chat.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/texts/markdown.py` & `LangTorch-1.0.5/src/langtorch/texts/markdown.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/texts/text.py` & `LangTorch-1.0.5/src/langtorch/texts/text.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/functional.py` & `LangTorch-1.0.5/src/langtorch/tt/functional.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_t/distance.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_t/distance.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_t/tokenizer.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_t/tokenizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/activation.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/activation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/assistantmodule.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/assistantmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/codemodule.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/codemodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/conv.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/linear.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/linear.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/loss.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/loss.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/retriever.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/retriever.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/textmodule.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/textmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/tt/modules/to_tt/transformers.py` & `LangTorch-1.0.5/src/langtorch/tt/modules/to_tt/transformers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/types.py` & `LangTorch-1.0.5/src/langtorch/types.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/src/langtorch/utils.py` & `LangTorch-1.0.5/src/langtorch/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_activation.py` & `LangTorch-1.0.5/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_autograd.py` & `LangTorch-1.0.5/tests/test_autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_conv.py` & `LangTorch-1.0.5/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_embedding.py` & `LangTorch-1.0.5/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_functional.py` & `LangTorch-1.0.5/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_group_operation.py` & `LangTorch-1.0.5/tests/test_group_operation.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_methods.py` & `LangTorch-1.0.5/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_mul.py` & `LangTorch-1.0.5/tests/test_mul.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_optimizer.py` & `LangTorch-1.0.5/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_pandoc.py` & `LangTorch-1.0.5/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_semantic_algebra.py` & `LangTorch-1.0.5/tests/test_semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_session.py` & `LangTorch-1.0.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_session_api.py` & `LangTorch-1.0.5/tests/test_session_api.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_text.py` & `LangTorch-1.0.5/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_texttensor.py` & `LangTorch-1.0.5/tests/test_texttensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_texttensor_constructor.py` & `LangTorch-1.0.5/tests/test_texttensor_constructor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.4/tests/test_visualize.py` & `LangTorch-1.0.5/tests/test_visualize.py`

 * *Files identical despite different names*

