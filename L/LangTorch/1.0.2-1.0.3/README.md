# Comparing `tmp/LangTorch-1.0.2.tar.gz` & `tmp/LangTorch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LangTorch-1.0.2.tar", last modified: Sat Apr 13 15:18:19 2024, max compression
+gzip compressed data, was "LangTorch-1.0.3.tar", last modified: Thu May 23 01:20:11 2024, max compression
```

## Comparing `LangTorch-1.0.2.tar` & `LangTorch-1.0.3.tar`

### file list

```diff
@@ -1,100 +1,123 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.519626 LangTorch-1.0.2/
--rw-rw-rw-   0        0        0     6463 2024-04-13 15:18:19.518628 LangTorch-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5758 2024-03-31 16:29:32.000000 LangTorch-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 15:18:19.519626 LangTorch-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1499 2024-04-13 15:18:01.000000 LangTorch-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.418653 LangTorch-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.467954 LangTorch-1.0.2/src/LangTorch.egg-info/
--rw-rw-rw-   0        0        0     6463 2024-04-13 15:18:19.000000 LangTorch-1.0.2/src/LangTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2950 2024-04-13 15:18:19.000000 LangTorch-1.0.2/src/LangTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 15:18:19.000000 LangTorch-1.0.2/src/LangTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2024-04-13 15:18:19.000000 LangTorch-1.0.2/src/LangTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-13 15:18:19.000000 LangTorch-1.0.2/src/LangTorch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.478437 LangTorch-1.0.2/src/langtorch/
--rw-rw-rw-   0        0        0     9127 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/_VariableFunctions.py
--rw-rw-rw-   0        0        0      483 2024-03-06 17:07:38.000000 LangTorch-1.0.2/src/langtorch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.484935 LangTorch-1.0.2/src/langtorch/api/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.2/src/langtorch/api/TODO_anthropic_parallel_processor.py
--rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/api/TODO_assistant.py
--rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.2/src/langtorch/api/TODO_gcp_parallel_processor.py
--rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/api/__init__.py
--rw-rw-rw-   0        0        0     1107 2024-01-14 23:17:01.000000 LangTorch-1.0.2/src/langtorch/api/api_threading.py
--rw-rw-rw-   0        0        0    12599 2024-04-05 11:21:04.000000 LangTorch-1.0.2/src/langtorch/api/call.py
--rw-rw-rw-   0        0        0    10822 2024-03-23 23:19:27.000000 LangTorch-1.0.2/src/langtorch/api/openai_parallel_processor.py
--rw-rw-rw-   0        0        0     9670 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/api/parallel_processor_utils.py
--rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/api/tools.py
--rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.2/src/langtorch/api/utils.py
--rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.2/src/langtorch/autograd.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.486935 LangTorch-1.0.2/src/langtorch/conf/
--rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.2/src/langtorch/conf/__init__.py
--rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.2/src/langtorch/conf/new_session_template.yaml
--rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.2/src/langtorch/conf/overrides.yaml
--rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.2/src/langtorch/decorators.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.489935 LangTorch-1.0.2/src/langtorch/grammars/
--rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.2/src/langtorch/grammars/__init__.py
--rw-rw-rw-   0        0        0     4522 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/grammars/formatters.py
--rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/grammars/langtorch_default_parser.py
--rw-rw-rw-   0        0        0     5186 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/grammars/pandoc.py
--rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/grammars/parsers.py
--rw-rw-rw-   0        0        0     6102 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/grammars/text_content_ast.py
--rw-rw-rw-   0        0        0     2269 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/grammars/utils.py
--rw-rw-rw-   0        0        0     8111 2024-04-13 15:18:01.000000 LangTorch-1.0.2/src/langtorch/main.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.495450 LangTorch-1.0.2/src/langtorch/methods/
--rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.2/src/langtorch/methods/__init__.py
--rw-rw-rw-   0        0        0     2704 2024-03-31 16:48:02.000000 LangTorch-1.0.2/src/langtorch/methods/chain_of_density.py
--rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.2/src/langtorch/methods/chain_of_thought.py
--rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/methods/embeddings.py
--rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.2/src/langtorch/methods/prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.495450 LangTorch-1.0.2/src/langtorch/optim/
--rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.2/src/langtorch/optim/__init__.py
--rw-rw-rw-   0        0        0     2199 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/optim/optimizer.py
--rw-rw-rw-   0        0        0      574 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/semalg_utils.py
--rw-rw-rw-   0        0        0     4639 2024-04-13 15:14:32.000000 LangTorch-1.0.2/src/langtorch/semantic_algebra.py
--rw-rw-rw-   0        0        0    15346 2024-04-05 11:21:12.000000 LangTorch-1.0.2/src/langtorch/session.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.499449 LangTorch-1.0.2/src/langtorch/tensors/
--rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.2/src/langtorch/tensors/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.2/src/langtorch/tensors/chattensor.py
--rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.2/src/langtorch/tensors/codetensor.py
--rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.2/src/langtorch/tensors/langtorchtensor.py
--rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.2/src/langtorch/tensors/markdowntensor.py
--rw-rw-rw-   0        0        0    37217 2024-04-13 15:15:57.000000 LangTorch-1.0.2/src/langtorch/tensors/texttensor.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.504339 LangTorch-1.0.2/src/langtorch/texts/
--rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.2/src/langtorch/texts/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/texts/chat.py
--rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.2/src/langtorch/texts/code.py
--rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/texts/markdown.py
--rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/texts/markup.py
--rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/texts/string.py
--rw-rw-rw-   0        0        0    36118 2024-04-07 13:08:34.000000 LangTorch-1.0.2/src/langtorch/texts/text.py
--rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.2/src/langtorch/texts/thread.py
--rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.2/src/langtorch/torch_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.504339 LangTorch-1.0.2/src/langtorch/tt/
--rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.2/src/langtorch/tt/__init__.py
--rw-rw-rw-   0        0        0    30603 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/functional.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.505338 LangTorch-1.0.2/src/langtorch/tt/modules/
--rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.2/src/langtorch/tt/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.506337 LangTorch-1.0.2/src/langtorch/tt/modules/from_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.2/src/langtorch/tt/modules/from_t/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.2/src/langtorch/tt/modules/from_t/transformers_automodel.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.509338 LangTorch-1.0.2/src/langtorch/tt/modules/to_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_t/__init__.py
--rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_t/distance.py
--rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_t/embedding.py
--rw-rw-rw-   0        0        0     1312 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_t/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:18:19.517627 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/
--rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/__init__.py
--rw-rw-rw-   0        0        0    22263 2024-04-09 18:19:04.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/activation.py
--rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/assistantmodule.py
--rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/chatmodule.py
--rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/codemodule.py
--rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/conv.py
--rw-rw-rw-   0        0        0     1623 2024-03-14 00:05:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/linear.py
--rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/loss.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/pooling.py
--rw-rw-rw-   0        0        0      883 2024-03-31 16:49:04.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/retriever.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/rnn.py
--rw-rw-rw-   0        0        0     7201 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/textmodule.py
--rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/transformer.py
--rw-rw-rw-   0        0        0     2009 2024-03-31 08:18:44.000000 LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/transformers.py
--rw-rw-rw-   0        0        0     1270 2024-02-28 12:31:38.000000 LangTorch-1.0.2/src/langtorch/types.py
--rw-rw-rw-   0        0        0     8337 2024-03-27 03:29:29.000000 LangTorch-1.0.2/src/langtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.572054 LangTorch-1.0.3/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 01:20:11.570875 LangTorch-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5968 2024-04-14 08:46:21.000000 LangTorch-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:20:11.572054 LangTorch-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2024-05-23 01:19:40.000000 LangTorch-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.491490 LangTorch-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.508915 LangTorch-1.0.3/src/LangTorch.egg-info/
+-rw-rw-rw-   0        0        0     6673 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3458 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 01:20:11.000000 LangTorch-1.0.3/src/LangTorch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.517924 LangTorch-1.0.3/src/langtorch/
+-rw-rw-rw-   0        0        0     9127 2024-05-17 09:29:22.000000 LangTorch-1.0.3/src/langtorch/_VariableFunctions.py
+-rw-rw-rw-   0        0        0      597 2024-05-17 13:20:07.000000 LangTorch-1.0.3/src/langtorch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.525426 LangTorch-1.0.3/src/langtorch/api/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.3/src/langtorch/api/TODO_anthropic_parallel_processor.py
+-rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/api/TODO_assistant.py
+-rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/api/TODO_gcp_parallel_processor.py
+-rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/api/__init__.py
+-rw-rw-rw-   0        0        0     1111 2024-05-17 01:10:31.000000 LangTorch-1.0.3/src/langtorch/api/api_threading.py
+-rw-rw-rw-   0        0        0    13887 2024-05-17 19:49:39.000000 LangTorch-1.0.3/src/langtorch/api/call.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 22:19:27.000000 LangTorch-1.0.3/src/langtorch/api/groq.py
+-rw-rw-rw-   0        0        0     6810 2024-05-17 01:30:15.000000 LangTorch-1.0.3/src/langtorch/api/openai.py
+-rw-rw-rw-   0        0        0     9982 2024-05-17 20:16:36.000000 LangTorch-1.0.3/src/langtorch/api/parallel_processor_utils.py
+-rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/api/tools.py
+-rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/api/utils.py
+-rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.3/src/langtorch/autograd.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.527428 LangTorch-1.0.3/src/langtorch/conf/
+-rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.3/src/langtorch/conf/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/conf/new_session_template.yaml
+-rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.3/src/langtorch/conf/overrides.yaml
+-rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.3/src/langtorch/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.530572 LangTorch-1.0.3/src/langtorch/grammars/
+-rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.3/src/langtorch/grammars/__init__.py
+-rw-rw-rw-   0        0        0     5850 2024-05-17 10:46:51.000000 LangTorch-1.0.3/src/langtorch/grammars/formatters.py
+-rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/grammars/langtorch_default_parser.py
+-rw-rw-rw-   0        0        0     5359 2024-05-17 03:05:19.000000 LangTorch-1.0.3/src/langtorch/grammars/pandoc.py
+-rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/grammars/parsers.py
+-rw-rw-rw-   0        0        0     6102 2024-05-17 02:21:53.000000 LangTorch-1.0.3/src/langtorch/grammars/text_content_ast.py
+-rw-rw-rw-   0        0        0     2343 2024-05-17 03:11:04.000000 LangTorch-1.0.3/src/langtorch/grammars/utils.py
+-rw-rw-rw-   0        0        0     8093 2024-05-22 23:57:17.000000 LangTorch-1.0.3/src/langtorch/main.py
+-rw-rw-rw-   0        0        0     2315 2024-05-22 23:41:02.000000 LangTorch-1.0.3/src/langtorch/main2.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.534572 LangTorch-1.0.3/src/langtorch/methods/
+-rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.3/src/langtorch/methods/__init__.py
+-rw-rw-rw-   0        0        0     2704 2024-05-17 09:31:29.000000 LangTorch-1.0.3/src/langtorch/methods/chain_of_density.py
+-rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.3/src/langtorch/methods/chain_of_thought.py
+-rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/methods/embeddings.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.3/src/langtorch/methods/prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.535571 LangTorch-1.0.3/src/langtorch/optim/
+-rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.3/src/langtorch/optim/__init__.py
+-rw-rw-rw-   0        0        0     2189 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/optim/optimizer.py
+-rw-rw-rw-   0        0        0      574 2024-05-17 09:32:04.000000 LangTorch-1.0.3/src/langtorch/semalg_utils.py
+-rw-rw-rw-   0        0        0     4639 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/semantic_algebra.py
+-rw-rw-rw-   0        0        0    13200 2024-05-18 10:39:50.000000 LangTorch-1.0.3/src/langtorch/session.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.537869 LangTorch-1.0.3/src/langtorch/tensors/
+-rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.3/src/langtorch/tensors/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.3/src/langtorch/tensors/chattensor.py
+-rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.3/src/langtorch/tensors/codetensor.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.3/src/langtorch/tensors/langtorchtensor.py
+-rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.3/src/langtorch/tensors/markdowntensor.py
+-rw-rw-rw-   0        0        0    42547 2024-05-23 00:01:23.000000 LangTorch-1.0.3/src/langtorch/tensors/texttensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.542867 LangTorch-1.0.3/src/langtorch/texts/
+-rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.3/src/langtorch/texts/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-05-15 02:21:06.000000 LangTorch-1.0.3/src/langtorch/texts/chat.py
+-rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.3/src/langtorch/texts/code.py
+-rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.3/src/langtorch/texts/markdown.py
+-rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/texts/markup.py
+-rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/texts/string.py
+-rw-rw-rw-   0        0        0    36694 2024-05-23 00:04:36.000000 LangTorch-1.0.3/src/langtorch/texts/text.py
+-rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.3/src/langtorch/texts/thread.py
+-rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.3/src/langtorch/torch_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.543867 LangTorch-1.0.3/src/langtorch/tt/
+-rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/__init__.py
+-rw-rw-rw-   0        0        0    30608 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/functional.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.543867 LangTorch-1.0.3/src/langtorch/tt/modules/
+-rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.3/src/langtorch/tt/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.544882 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.3/src/langtorch/tt/modules/from_t/transformers_automodel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.547908 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/__init__.py
+-rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/distance.py
+-rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/embedding.py
+-rw-rw-rw-   0        0        0     1312 2024-05-17 09:29:49.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_t/tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.556509 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/
+-rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/__init__.py
+-rw-rw-rw-   0        0        0    22439 2024-05-17 05:36:08.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/activation.py
+-rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/assistantmodule.py
+-rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/chatmodule.py
+-rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/codemodule.py
+-rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/conv.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 18:27:32.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/linear.py
+-rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/loss.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/pooling.py
+-rw-rw-rw-   0        0        0      883 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/retriever.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/rnn.py
+-rw-rw-rw-   0        0        0     7195 2024-05-17 18:27:32.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/textmodule.py
+-rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformer.py
+-rw-rw-rw-   0        0        0     2009 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformers.py
+-rw-rw-rw-   0        0        0     1268 2024-05-17 09:34:15.000000 LangTorch-1.0.3/src/langtorch/types.py
+-rw-rw-rw-   0        0        0     8335 2024-05-17 09:34:19.000000 LangTorch-1.0.3/src/langtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:20:11.570875 LangTorch-1.0.3/tests/
+-rw-rw-rw-   0        0        0      845 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_activation.py
+-rw-rw-rw-   0        0        0     1358 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_autograd.py
+-rw-rw-rw-   0        0        0     6419 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_conv.py
+-rw-rw-rw-   0        0        0      292 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_dspy.py
+-rw-rw-rw-   0        0        0     2487 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_embedding.py
+-rw-rw-rw-   0        0        0     4094 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6075 2024-03-30 15:39:03.000000 LangTorch-1.0.3/tests/test_group_operation.py
+-rw-rw-rw-   0        0        0      489 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_import.py
+-rw-rw-rw-   0        0        0      433 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_markdown.py
+-rw-rw-rw-   0        0        0     1056 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_methods.py
+-rw-rw-rw-   0        0        0     6393 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_mul.py
+-rw-rw-rw-   0        0        0     2274 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_optimizer.py
+-rw-rw-rw-   0        0        0     5417 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_pandoc.py
+-rw-rw-rw-   0        0        0     1994 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_semantic_algebra.py
+-rw-rw-rw-   0        0        0     4400 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_session.py
+-rw-rw-rw-   0        0        0     1397 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_session_api.py
+-rw-rw-rw-   0        0        0     1764 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_text.py
+-rw-rw-rw-   0        0        0     3935 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_texttensor.py
+-rw-rw-rw-   0        0        0      727 2024-05-17 09:28:38.000000 LangTorch-1.0.3/tests/test_texttensor_constructor.py
+-rw-rw-rw-   0        0        0      938 2024-05-17 09:26:53.000000 LangTorch-1.0.3/tests/test_visualize.py
```

### Comparing `LangTorch-1.0.2/PKG-INFO` & `LangTorch-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
+<p align="center">
+<img align="center" src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;">
+</p>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
+**Quickstart Tutorial:**  [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg">](https://colab.research.google.com/github/AdamSobieszek/langtorch/blob/main/quickstart.ipynb)
+
+---
 
 LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
 
 While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
-> Powered by **TextTensors** â€” "torch Tensors but with text data as entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+> Powered by **TextTensors** â€” "torch Tensors but with text data entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
@@ -94,17 +99,17 @@
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
     TextModule("Calculate the described quantity: {}"),
     OpenAI("gpt-4", T=0)
 )
-
-input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
-output_tensor = chain(input_tensor)
+	
+	input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
+	output_tensor = chain(input_tensor)
 ```
 
 
 
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
```

### Comparing `LangTorch-1.0.2/README.md` & `LangTorch-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
+<p align="center">
+<img align="center" src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;">
+</p>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
+**Quickstart Tutorial:**  [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg">](https://colab.research.google.com/github/AdamSobieszek/langtorch/blob/main/quickstart.ipynb)
+
+---
 
 LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
 
 While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
-> Powered by **TextTensors** — "torch Tensors but with text data as entries" — offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+> Powered by **TextTensors** — "torch Tensors but with text data entries" — offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
@@ -77,17 +82,17 @@
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
     TextModule("Calculate the described quantity: {}"),
     OpenAI("gpt-4", T=0)
 )
-
-input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
-output_tensor = chain(input_tensor)
+	
+	input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
+	output_tensor = chain(input_tensor)
 ```
 
 
 
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
```

### Comparing `LangTorch-1.0.2/setup.py` & `LangTorch-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LangTorch",
-    version="1.0.2",
+    version="1.0.3",
     description="Framework for intuitive LLM application development with tensors.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Adam Sobieszek",
     author_email="contact@langtorch.org",
     url="https://github.com/AdamSobieszek/LangTorch",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "numpy",
-        "torch>=2.0.0",
+        "torch >= 2.1.0",
         "aiohttp",
         "nest_asyncio",
         "openai>=1.2.4",
         "tiktoken",
         "pandas",
         "retry",
         "pyparsing",
         "pypandoc",
         "transformers",
-        "peft",
         'omegaconf',
         'hydra-core',
-        'h5py',
         "markdown-it-py"
     ],
     python_requires='>=3.8',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
```

### Comparing `LangTorch-1.0.2/src/LangTorch.egg-info/PKG-INFO` & `LangTorch-1.0.3/src/LangTorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
+<p align="center">
+<img align="center" src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;">
+</p>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
+**Quickstart Tutorial:**  [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg">](https://colab.research.google.com/github/AdamSobieszek/langtorch/blob/main/quickstart.ipynb)
+
+---
 
 LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
 
 While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
-> Powered by **TextTensors** â€” "torch Tensors but with text data as entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+> Powered by **TextTensors** â€” "torch Tensors but with text data entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
@@ -94,17 +99,17 @@
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
     TextModule("Calculate the described quantity: {}"),
     OpenAI("gpt-4", T=0)
 )
-
-input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
-output_tensor = chain(input_tensor)
+	
+	input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
+	output_tensor = chain(input_tensor)
 ```
 
 
 
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
```

### Comparing `LangTorch-1.0.2/src/LangTorch.egg-info/SOURCES.txt` & `LangTorch-1.0.3/src/LangTorch.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 src/LangTorch.egg-info/requires.txt
 src/LangTorch.egg-info/top_level.txt
 src/langtorch/_VariableFunctions.py
 src/langtorch/__init__.py
 src/langtorch/autograd.py
 src/langtorch/decorators.py
 src/langtorch/main.py
+src/langtorch/main2.py
 src/langtorch/semalg_utils.py
 src/langtorch/semantic_algebra.py
 src/langtorch/session.py
 src/langtorch/torch_utils.py
 src/langtorch/types.py
 src/langtorch/utils.py
 src/langtorch/api/TODO_anthropic_parallel_processor.py
 src/langtorch/api/TODO_assistant.py
 src/langtorch/api/TODO_gcp_parallel_processor.py
 src/langtorch/api/__init__.py
 src/langtorch/api/api_threading.py
 src/langtorch/api/call.py
-src/langtorch/api/openai_parallel_processor.py
+src/langtorch/api/groq.py
+src/langtorch/api/openai.py
 src/langtorch/api/parallel_processor_utils.py
 src/langtorch/api/tools.py
 src/langtorch/api/utils.py
 src/langtorch/conf/__init__.py
 src/langtorch/conf/new_session_template.yaml
 src/langtorch/conf/overrides.yaml
 src/langtorch/grammars/__init__.py
@@ -75,8 +77,28 @@
 src/langtorch/tt/modules/to_tt/linear.py
 src/langtorch/tt/modules/to_tt/loss.py
 src/langtorch/tt/modules/to_tt/pooling.py
 src/langtorch/tt/modules/to_tt/retriever.py
 src/langtorch/tt/modules/to_tt/rnn.py
 src/langtorch/tt/modules/to_tt/textmodule.py
 src/langtorch/tt/modules/to_tt/transformer.py
-src/langtorch/tt/modules/to_tt/transformers.py
+src/langtorch/tt/modules/to_tt/transformers.py
+tests/test_activation.py
+tests/test_autograd.py
+tests/test_conv.py
+tests/test_dspy.py
+tests/test_embedding.py
+tests/test_functional.py
+tests/test_group_operation.py
+tests/test_import.py
+tests/test_markdown.py
+tests/test_methods.py
+tests/test_mul.py
+tests/test_optimizer.py
+tests/test_pandoc.py
+tests/test_semantic_algebra.py
+tests/test_session.py
+tests/test_session_api.py
+tests/test_text.py
+tests/test_texttensor.py
+tests/test_texttensor_constructor.py
+tests/test_visualize.py
```

### Comparing `LangTorch-1.0.2/src/langtorch/_VariableFunctions.py` & `LangTorch-1.0.3/src/langtorch/_VariableFunctions.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/api/TODO_assistant.py` & `LangTorch-1.0.3/src/langtorch/api/TODO_assistant.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/api/TODO_gcp_parallel_processor.py` & `LangTorch-1.0.3/src/langtorch/api/TODO_gcp_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/api/call.py` & `LangTorch-1.0.3/src/langtorch/api/call.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,93 +127,104 @@
                     tools[i] = json.loads(tool)
                 except json.JSONDecodeError as e:
                     raise ValueError(f"Tool {tool} is not a valid JSON string object.") from e
             if not "type" in tools[i]:
                 tools[i] = {"type": "function", "function": tools[i]}
 
     params = {"temperature": temperature,
-              "top_p": top_p,
-              "n": n,
-              "stop": stop,
-              "max_tokens": max_tokens,
-              "presence_penalty": presence_penalty,
-              "frequency_penalty": frequency_penalty,
-              "tools": tools,
-              "tool_choice": tool_choice}
+                  "top_p": top_p,
+                  "n": n,
+                  "stop": stop,
+                  "max_tokens": max_tokens,
+                  "presence_penalty": presence_penalty,
+                  "frequency_penalty": frequency_penalty,
+                  "tools": tools,
+                  "tool_choice": tool_choice}
 
     default_values = {"temperature": 1, "top_p": 1, "n": 1, "stop": None, "max_tokens": None, "presence_penalty": 0,
                       "frequency_penalty": 0, "tools": None, "tool_choice": "none"}
 
     jobs = [{"model": model,
-             "messages": [{"role": "system", "content": system_message},
-                          {"role": "user", "content": prompt}] if isinstance(prompt, str) else
-             [{"role": "system", "content": system_message}] + [{"role": r, "content": c} for r, c in prompt],
+             "messages": ([{"role": "system", "content": system_message}] if system_message else [])+([{"role": "user", "content": prompt}] if isinstance(prompt, str) else
+             [{"role": r, "content": c} for r, c in prompt]),
              **{param: value for param, value in params.items() if value != default_values[param]}}
             for prompt, system_message in zip(prompts, system_messages)]
     return [json.dumps(job, ensure_ascii=False) for job in jobs]
 
 
-def chat(prompts, system_messages, model="gpt-3.5-turbo", cache=True, api_key=None, verbose=False, as_str=False,
+def chat(prompts, system_messages, model="gpt-3.5-turbo", provider = "openai", cache=True, api_key=None, verbose=False, as_str=False,
          **kwargs):
     """
     Processes a list of chat prompts in parallel, saving the results to a specified file.
 
     Parameters:
         prompts (List[str] or List[Tuple[str,str]] or str): List or single prompt or list of (role, prompt) pairs to send to the model.
         system_messages (List[str] or str): List or single system message to guide the model's behavior.
         model (str, optional): Model name to use. Default is "gpt-3.5-turbo-0613".
+        provider (str, optional):  The provider to use. Default is "openai".
         cache (bool, optional): If True, reuse previous call results.
         api_key (str, optional): API key for authentication. If None, uses environment variable.
         verbose (bool, optional): If True, enables detailed logging. Default is True.
         as_str (bool, optional): If True, returns only the model's message as string, otherwise returns the entire response object. Default is False.
         **kwargs: Additional parameters  of the api request.
 
     Returns:
         Union[Coroutine, openai.ChatCompletion, str]: Coroutine object representing the asynchronous execution of the API requests if save_filepath is provided. Otherwise, returns the chat response object, or a string if as_str is True.
     """
 
-    session = Session()
     if "T" in kwargs:
         kwargs["temperature"] = kwargs["T"]
     if not isinstance(system_messages, list): system_messages = [system_messages]
     if not isinstance(prompts, list):
         prompts = [prompts]
     if len(system_messages) == 1:
         system_messages = system_messages * len(prompts)
     request_strings = chat_strings(prompts, system_messages, model, **kwargs)
 
+    session = Session()
+    provider_to_request_url = {"openai":"https://api.openai.com/v1/chat/completions",
+                                               "anthropic":"https://api.anthropic.com/v1/messages",
+                                               "groq":"https://api.groq.com/openai/v1/chat/completions"}
+    assert provider in provider_to_request_url, f"Provider {provider} not in available providers"
     if api_key is None:
         try:
-            api_key = os.environ["OPENAI_API_KEY"]
+            api_key = os.environ[f"{provider.upper()}_API_KEY"]
         except KeyError as e:
-            raise KeyError('No OpenAI API key. Set os.environ["OPENAI_API_KEY"] = YOUR KEY') from e
-    ids, uncached_request_strings = session.request("openai", "chat", request_strings, cache)
+            raise KeyError(f'No {provider} API key. Set os.environ["{provider.upper()}_API_KEY"] = YOUR KEY') from e
+    provider_to_request_header = {"openai": {"Authorization": f"Bearer {api_key}"},
+                 "anthropic": {"x-api-key:": f"{os.environ['ANTHROPIC_API_KEY']}",
+                               "anthropic-version": "2023-06-01",
+                               "Content-Type": "application/json"},
+                                                  "groq": {"Authorization": f"Bearer {api_key}"},}
+    request_header = provider_to_request_header[provider]
+    ids, uncached_request_strings = session.request(provider, "chat", request_strings, cache)
+
+    with Session(session.path) as session:
+        if request_strings:
+            job = execute_api_requests_in_parallel(
+                ids=ids,
+                request_strings=uncached_request_strings,
+                request_url=provider_to_request_url[provider],
+                request_header=request_header,
+                logging_level=logging.INFO if verbose else logging.ERROR,
+                max_requests_per_minute=200 if "gpt-4" in request_strings[0] else 3_500 * 0.5,
+                max_tokens_per_minute=40_000 * 0.5 if "gpt-4" in request_strings[0] else 90_000 * 0.5,
+            )
 
-    if request_strings:
-        job = execute_api_requests_in_parallel(
-            ids=ids,
-            request_strings=uncached_request_strings,
-            request_url="https://api.openai.com/v1/chat/completions",
-            api_key=api_key,
-            logging_level=logging.INFO if verbose else logging.ERROR,
-            max_requests_per_minute=200 if "gpt-4" in request_strings[0] else 3_500 * 0.5,
-            max_tokens_per_minute=40_000 * 0.5 if "gpt-4" in request_strings[0] else 90_000 * 0.5,
-        )
-
-        try:
-            loop = asyncio.get_event_loop()
-            loop.run_until_complete(job)
-        except RuntimeError as E1:
             try:
-                asyncio.run(job)
-            except RuntimeError as E2:
-                raise RuntimeError(
-                    f"Asyncio get current event loop failed with {E1}. Tried to fall back on new event loop with asyncio.run(job) but failed with error: {E2}.\nThis indicates error with the API code or provider and could be hard to fix.")
+                loop = asyncio.get_event_loop()
+                loop.run_until_complete(job)
+            except RuntimeError as E1:
+                try:
+                    asyncio.run(job)
+                except RuntimeError as E2:
+                    raise RuntimeError(
+                        f"Asyncio get current event loop failed with {E1}. Tried to fall back on new event loop with asyncio.run(job) but failed with error: {E2}.\nThis indicates error with the API code or provider and could be hard to fix.")
 
-    return session.completions("chat", "openai", request_strings)
+        return session.completions("chat", provider, request_strings)
 
 
 def get_embedding(texts, model="text-embedding-3-small", cache=True, as_np=False, api_key=None, verbose=False):
     """
     Retrieves embeddings for the given texts from the OpenAI API and saves the results in a file.
 
     Parameters:
@@ -226,44 +237,47 @@
     Returns:
         dict: The embeddings from the saved results file, loaded as a Python dictionary.
     """
     from langtorch import TextTensor
     session = Session()
 
     if api_key is None:
+
         try:
             api_key = os.environ["OPENAI_API_KEY"]
         except KeyError:
             raise KeyError('No OpenAI API key. Set os.environ["OPENAI_API_KEY"] = YOUR KEY')
     if isinstance(texts, str): texts = [str(texts)]
     if isinstance(texts, TextTensor):
         shape = texts.content.shape
         texts = [str(m) for m in texts.content.flat]
     else:
         shape = (len(texts),)
     request_strings = [json.dumps({"model": model, "input": str(x).strip() + "\n"}, ensure_ascii=False) for x in texts]
 
     ids, uncached_request_strings = session.request("openai", "embeddings", request_strings, cache)
+    request_header = {"Authorization": f"Bearer {api_key}"}
 
     # Execute API requests in parallel and save to session
-    job = execute_api_requests_in_parallel(
-        ids=ids,
-        request_strings=uncached_request_strings,
-        request_url="https://api.openai.com/v1/embeddings",
-        api_key=api_key,
-        max_requests_per_minute=3_000 * 0.5,
-        max_tokens_per_minute=250_000 * 0.5,
-        token_encoding_name="cl100k_base",
-        max_attempts=3,
-        logging_level=logging.INFO if verbose else logging.ERROR,
-    )
-
-    try:
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(job)
-    except Exception as E:
-        asyncio.run(job)
+    with Session(session.path) as session:
+        job = execute_api_requests_in_parallel(
+            ids=ids,
+            request_strings=uncached_request_strings,
+            request_url="https://api.openai.com/v1/embeddings",
+            request_header=request_header,
+            max_requests_per_minute=3_000 * 0.5,
+            max_tokens_per_minute=250_000 * 0.5,
+            token_encoding_name="cl100k_base",
+            max_attempts=3,
+            logging_level=logging.INFO if verbose else logging.ERROR,
+        )
+
+        try:
+            loop = asyncio.get_event_loop()
+            loop.run_until_complete(job)
+        except Exception as E:
+            asyncio.run(job)
 
-    return session.completions("embeddings", "openai", request_strings).reshape(shape + (-1,))
+        return session.completions("embeddings", "openai", request_strings).reshape(shape + (-1,))
 
 
 embed = get_embedding  ## Alternative function name
```

### Comparing `LangTorch-1.0.2/src/langtorch/api/parallel_processor_utils.py` & `LangTorch-1.0.3/src/langtorch/api/parallel_processor_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import logging  # for logging rate limit warnings and other messages
 import re  # for matching endpoint from request URL
 import time  # for sleeping after rate limit is hit
 from abc import ABC, abstractmethod  # for abstract APIRequest class
 from dataclasses import dataclass  # for storing API inputs, outputs, and metadata
 
 import aiohttp  # for making API calls concurrently
+from aiohttp import ClientConnectorError
 import tiktoken  # for counting tokens
 
 from ..session import ctx as langtorch_session
 
 
 # dataclasses
 
@@ -73,36 +74,38 @@
         logging.info(f"Starting request #{self.task_id}")
         error = None
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post(
                         url=request_url, headers=request_header, json=self.request_json
                 ) as response:
-                    response = await response.json()
+                    response = await response.json(content_type='application/json')
             if "error" in response:
-                logging.warning(
+                logging.debug(
                     f"Request {self.task_id} failed with error {response['error']}"
                 )
                 status_tracker.num_api_errors += 1
                 error = response
                 if "Rate limit" in response["error"].get("message", ""):
                     status_tracker.time_of_last_rate_limit_error = time.time()
                     status_tracker.num_rate_limit_errors += 1
                     status_tracker.num_api_errors -= 1  # rate limit errors are counted separately
-
+        except ClientConnectorError as e:
+            raise e  # Re-raise a connection error
         except Exception as e:  # catching naked exceptions is bad practice, but in this case we'll log & save them
             logging.warning(f"Request {self.task_id} failed with Exception {e}")
             status_tracker.num_other_errors += 1
             error = e
         if error:
             self.result.append(error)
             if self.attempts_left:
                 retry_queue.put_nowait(self)
             else:
-                logging.error(f"Request {self.request_json} failed after all attempts. Saving errors: {self.result}")
+                errors = '\n'.join(list(set([str(r['error']) for r in self.result])))
+                logging.error(f"Request {self.request_json} failed after all attempts. Encountered errors: {errors}")
 
                 try:  # error catching to deal with session errors
                     langtorch_session.add_response(self.id, response)
                 except Exception as e:
                     logging.warning(f"Failed to add {self.task_id} API ERROR response, caused by {e}")
                 status_tracker.num_tasks_in_progress -= 1
                 status_tracker.num_tasks_failed += 1
@@ -114,16 +117,20 @@
             status_tracker.num_tasks_in_progress -= 1
             status_tracker.num_tasks_succeeded += 1
             logging.debug(f"Request {self.task_id} saved to responses")
 
 
 def api_endpoint_from_url(request_url):
     """Extract the API endpoint from the request URL."""
+
     match = re.search('^https://[^/]+/v\\d+/(.+)$', request_url)
-    return match[1]
+    if match is None:
+        return None
+    else:
+        return match[1]
 
 
 def append_to_jsonl(data, filename: str) -> None:
     """Append a json payload to the end of a jsonl file."""
     json_string = json.dumps(data, ensure_ascii=False)
     with open(filename, "a", encoding="utf-8") as f:
         f.write(json_string + "\n")
```

### Comparing `LangTorch-1.0.2/src/langtorch/api/tools.py` & `LangTorch-1.0.3/src/langtorch/api/tools.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/api/utils.py` & `LangTorch-1.0.3/src/langtorch/api/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/autograd.py` & `LangTorch-1.0.3/src/langtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/conf/__init__.py` & `LangTorch-1.0.3/src/langtorch/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/decorators.py` & `LangTorch-1.0.3/src/langtorch/decorators.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/grammars/langtorch_default_parser.py` & `LangTorch-1.0.3/src/langtorch/grammars/langtorch_default_parser.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/grammars/pandoc.py` & `LangTorch-1.0.3/src/langtorch/grammars/pandoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         list: The modified list of Pandoc tuples.
     """
     if isinstance(pandoc_tuples, str):
         return pandoc_tuples
     elif isinstance(pandoc_tuples, tuple):
         if pandoc_tuples[0] == 'Str':
             return pandoc_tuples[1]
+        elif len(pandoc_tuples) == 2:
+            return (pandoc_tuples[0], join_str_types(pandoc_tuples[1]))
     elif len(pandoc_tuples) == 1:
         return join_str_types(pandoc_tuples[0])
     elif all(isinstance(x, str) for x in pandoc_tuples):
         return "".join(pandoc_tuples)
     result = []
     temp_str = ""
 
@@ -84,35 +86,36 @@
                 result.append(temp_str)
                 temp_str = ""
                 result.append(item)
         else:
             if temp_str:
                 result.append(temp_str)
                 temp_str = ""
-
             result.append(item)
     if temp_str:
         result.append(temp_str)
     return result
 
 
 def pandoc_dict_to_tuple(d):
     if isinstance(d, list):
-        return join_str_types([pandoc_dict_to_tuple(x) for x in d])
+        r = [pandoc_dict_to_tuple(x) for x in d]
+        return join_str_types(r)
     if isinstance(d, dict):
         if "c" not in d:
             return (d["t"], "")
         if isinstance(d["c"], str):
             return (d["t"], d["c"])
         else:
             # Identify Header size
             if len(d["c"]) == 3 and isinstance(d["c"][0], int):
                 d["t"] += str(d["c"][0])
             return (d["t"], pandoc_dict_to_tuple(d["c"]))
-
+    # if isinstance(d, str):
+    #     return d
 
 def pandoc_to_ast(input_string: str, input_format: str) -> str:
     """
     Converts a given string into a Pandoc AST JSON format.
 
     Args:
         input_string (str): The input string to be converted.
```

### Comparing `LangTorch-1.0.2/src/langtorch/grammars/parsers.py` & `LangTorch-1.0.3/src/langtorch/grammars/parsers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/grammars/text_content_ast.py` & `LangTorch-1.0.3/src/langtorch/grammars/text_content_ast.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/grammars/utils.py` & `LangTorch-1.0.3/src/langtorch/grammars/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union, Tuple, List
-
+import logging
 
 def block_to_markdown(cls, entry: Union[str, Tuple[str, Union[str, List]]]) -> str:
     newline = '\n'
 
     key_to_md = {
         "Header": "# ",
         'Header1': '# ',
@@ -25,22 +25,22 @@
     if isinstance(entry, str) and not hasattr(entry, "content"):
         return entry
     if isinstance(entry, tuple) and len(entry) == 2 and isinstance(entry[0], str) and isinstance(entry[1], str):
         return f"{key_to_md.get(entry[0], '')}{entry[1]}"
 
     # Recursive cases
     if isinstance(entry, tuple) and len(entry) == 2 and isinstance(entry[0], str) and isinstance(entry[1],
-                                                                                                 list):
+                                                                                                 (list, tuple)):
         # Special case for code blocks
         if entry[0] == 'code':
             return f"{key_to_md.get(entry[0], '')}\n{entry[1]}\n{key_to_md.get(entry[0], '')}"
-        elif entry[0] in ['BulletList', 'OrderedList']:
+        elif entry[0] in ['BulletList', 'OrderedList', 'BlockQuote']:
             # Handling of list items
             if isinstance(entry[1], tuple):
-                entry[1] = [entry[1]]
+                entry = (entry[0],[entry[1]])
             result = ""
             for i, child in enumerate(entry[1]):
                 if isinstance(child, str):
                     child = ('', child)
                 if result:
                     result += newline
                 if entry[0] == 'OrderedList':
@@ -50,8 +50,9 @@
             return result
         else:
             return f"{key_to_md.get(entry[0], '')}{newline.join([block_to_markdown(cls, child) for child in entry[1]])}"
 
     if isinstance(entry, list):
         return newline.join([block_to_markdown(cls, child) for child in entry])
 
-    return "Markdown parsing error, convert to Text first."
+    logging.warning(f"Markdown parsing error for entry: {entry}")
+    return f"{entry}"
```

### Comparing `LangTorch-1.0.2/src/langtorch/main.py` & `LangTorch-1.0.3/src/langtorch/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from langtorch import TextModule
 from langtorch import Chat, ChatML
 
 from langtorch import TextTensor, TextModule, OpenAI
 import torch
 # Without any additional classes we can implement a retriever and RAG module
 
-print(TextTensor([*range(9)]).reshape(3,3).sum(0, sep=", "))
+print(type(TextTensor(["",""]).content))
+
 
 
 quit()
 
 llm = Activation(model="gpt-3.5-turbo", T=0.9, tools=[{"type": "function",
                   "function": {
                     "name": "get_current_weather",
```

### Comparing `LangTorch-1.0.2/src/langtorch/methods/chain_of_density.py` & `LangTorch-1.0.3/src/langtorch/methods/chain_of_density.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/methods/chain_of_thought.py` & `LangTorch-1.0.3/src/langtorch/methods/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/methods/embeddings.py` & `LangTorch-1.0.3/src/langtorch/methods/embeddings.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/optim/optimizer.py` & `LangTorch-1.0.3/src/langtorch/optim/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
             for param in group['params']:
-                if not isinstance(param, TextTensor):
+                if not isinstance(param, ):
                     raise ValueError("Optimizer parameters must be of type TextTensor")
                 if param.grad is None:
                     continue
                 grad = param.grad
                 # Perform the optimization step to update 'param.data'
                 # This is where the custom optimization logic would go
                 # For demonstration, let's just subtract a fraction of the gradient
```

### Comparing `LangTorch-1.0.2/src/langtorch/semalg_utils.py` & `LangTorch-1.0.3/src/langtorch/semalg_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/semantic_algebra.py` & `LangTorch-1.0.3/src/langtorch/semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/session.py` & `LangTorch-1.0.3/src/langtorch/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import base64
+import contextlib
 import contextvars
-import datetime
 import hashlib
 import logging
 import os
 from collections import OrderedDict
-
-import h5py
-# time the execution
+from dataclasses import dataclass  # for storing API metadata
 import torch
 import yaml
-from omegaconf import OmegaConf
-from omegaconf.errors import UnsupportedValueType
-from dataclasses import dataclass  # for storing API metadata
+from omegaconf import OmegaConf, UnsupportedValueType
 
 from .conf import cfg_yaml_aliases
 
-
 class SingletonMeta(type):
     # This dict holds a single instance of a given singleton class, indexed by the class itself
     _instance = contextvars.ContextVar('ctx',
                                        default={})
 
     def __call__(cls, *args, **kwargs):
         instances = cls._instance.get()  # Get the dict of single instances
@@ -44,318 +39,297 @@
     num_tasks_failed: int = 0
     num_rate_limit_errors: int = 0
     num_api_errors: int = 0  # excluding rate limit errors, counted above
     num_other_errors: int = 0
     time_of_last_rate_limit_error: int = 0  # used to cool off after hitting rate limits
 
 
+class SingletonMeta(type):
+    _instance = contextvars.ContextVar('ctx', default={})
+
+    def __call__(cls, *args, **kwargs):
+        instances = cls._instance.get()  # Get the dict of single instances
+        if cls not in instances:  # Add new
+            instance = super().__call__(*args, **kwargs)
+            instances[cls] = instance
+            cls._instance.set(instances)
+        else:
+            if args or kwargs:  # Reload existing
+                instances[cls] = instances[cls].load(*args, **kwargs)
+        return instances[cls]
+
+
+@dataclass
+class StatusTracker:
+    num_tasks_started: int = 0
+    num_tasks_in_progress: int = 0  # script ends when this reaches 0
+    num_tasks_succeeded: int = 0
+    num_tasks_failed: int = 0
+    num_rate_limit_errors: int = 0
+    num_api_errors: int = 0  # excluding rate limit errors, counted above
+    num_other_errors: int = 0
+    time_of_last_rate_limit_error: int = 0  # used to cool off after hitting rate limits
+
+
 class Session(metaclass=SingletonMeta):
     """A context manager for saving and loading session data: tensors, api calls, configuration and caching"""
     default_config = os.path.join(os.path.dirname(os.path.abspath(__file__)), "conf/defaults.yaml")
     session_file_template = os.path.join(os.path.dirname(os.path.abspath(__file__)), "conf/new_session_template.yaml")
 
-    def __init__(self, session_file=None, cache_file=None, new_session_file=False):
+    def __init__(self, path=None, overwrite_existing=False):
         self._tensors = dict()
         self._requests = dict()
         self._responses = dict()
-        self._overwrite = new_session_file
-        self._session_file = session_file
-        self._cache_file = None if cache_file is None else cache_file if "." in cache_file else cache_file + ".hdf5"
-        self.load(session_file, cache_file, new_session_file)
-        self.status_tracker = StatusTracker()
-        assert self.tensor_savepath is not None
-
-    def load(self, path=None, cache=None, new_session_file=False):
-        """Called to set or change the path and load or reload the config"""
-        _config = OmegaConf.load(self.default_config)
-        _config["tensors"] = getattr(_config, "tensors", [])
-
-        self._session_file = path if path else self._session_file
-        self._cache_file = cache if cache else self._cache_file
-
-        if self._cache_file and os.path.exists(self._cache_file):
-            import numpy as np
-            with h5py.File(self._cache_file, 'r') as f:
-                for key in f.keys():
-                    if key not in self._responses:
-                        dataset = f[key]
-                        self._responses[key] = [m.decode('utf-8') for m in
-                                                dataset[:]] if dataset.dtype == np.object_ else torch.from_numpy(
-                            dataset[:])
-
-        if self._session_file and os.path.exists(self._session_file) and not new_session_file:
-            try:
-                _config = OmegaConf.merge(_config, OmegaConf.load(self._session_file))
-            except Exception as e:
-                print(f"Error loading session from {self._session_file}: {e}")
-
-        if not getattr(_config, "tensor_savepath", None):
-            _config.tensor_savepath = "" if self._session_file is None else os.path.join(
-                os.path.dirname(os.path.abspath(self._session_file)), "saved_tensors.pt")
-
-        if _config.tensor_savepath and os.path.exists(_config.tensor_savepath):
-            self._tensors = torch.load(_config.tensor_savepath)
+        self._overwrite = overwrite_existing
+        self._path = path if path is None else  f"{os.path.splitext(path)[0]}.yaml"
+        self._cache_file = None
+        self.load(path, overwrite_existing)
+        self._status_tracker = StatusTracker()
 
-        self._config = _config
+    def load(self, path=None, overwrite_existing=False):
+        try:
+            self._config = OmegaConf.load(self.default_config)
+            if path:
+                self._path = path
+            if self._path and not overwrite_existing:
+                session_config = OmegaConf.load(path)
+                self._config = OmegaConf.merge(self._config, session_config)
+
+                self._config.cache_file = f"{os.path.splitext(self._path)[0]}.pt"
+                self._cache_file = self._config.cache_file
+            if self._cache_file and os.path.exists(self._cache_file):
+                cache = torch.load(self._cache_file)
+                if "tensors" in cache:
+                    self._tensors = cache.pop("tensors")
+                if "responses" in cache:
+                    self._responses = cache.pop("responses")
+                for k, v in cache.items():
+                    setattr(self, k, v)
+        except Exception as e:
+            logging.error(f"Error loading session configuration: {e}")
+            self._config = OmegaConf.load(self.session_file_template)
         return self
 
+    def save(self, path=None):
+        if path is None:
+            path = self._path
+
+        tensors_metadata = self._config.pop('tensors', [])
+
+        underscore_attrs = OrderedDict((k, v) for k, v in self._config.items() if k.startswith('_'))
+        for k in underscore_attrs.keys():
+            self._config.pop(k, None)
+
+        self._config.tensors = tensors_metadata
+
+        for k, v in underscore_attrs.items():
+            self._config[k] = v
+
+        with open(self._path, 'w', encoding="utf-8") as f:
+            OmegaConf.save(self._config, f, resolve=True)
+
+        # Save the tensor cache
+        if self._cache_file:
+            torch.save({
+                'tensors': self._tensors,
+                'responses': self._responses
+            }, self._cache_file)
+
+    def __setattr__(self, name, value, save=True):
+        if name in ["_config", "_tensors", "_session_file", "_overwrite"]:
+            super().__setattr__(name, value)
+            if name == "_config" and self._path and save:
+                self.save()
+        elif name.startswith('_'):
+            super().__setattr__(name, value)
+        else:
+            if isinstance(value, torch.Tensor):
+                self._tensors[name] = value
+            else:
+                try:
+                    self._config[name] = value
+                    if name in self._tensors:
+                        print(f"Saving non-tensor with the same name as a saved tensor {name}, the tensor will be unobtainable (but remains saved)")
+                except UnsupportedValueType as e:
+                    raise UnsupportedValueType("Session can only hold primitive types and TextTenor objects.") from e
+            if self._path and save:
+                self.save()
+
+
+
     @property
     def path(self):
-        return self._session_file
+        return self._path
 
     def reload(self):
-        """Called to ensure config is up-to-date"""
         return self.load()
 
     def request(self, provider, type, request_strings, cache=True):
-        """Query the session for cached result or add new requests"""
-
         def append_spaces_to_duplicates(strings):
             occurrence_dict = {}
             result = []
 
             for s in strings:
                 count = occurrence_dict.get(s, 0)
                 occurrence_dict[s] = count + 1
                 result.append(s + " " * count)
 
             return result
 
-        # Generate unique hashes from the request strings
         strings = [provider + type + s for s in request_strings]
         strings = append_spaces_to_duplicates(strings)
         assert len(strings) == len(set(strings)), "Duplicate requests found"
         ids = [self.get_hash(s) for s in strings]
 
-        # for id, request in zip(ids, request_strings):
-        #     if not '"user"' in request and not '"assistant"' in request and id not in self._responses:
-        #         from langtorch import Text
-        #         logging.debug(f"Activation got request without a 'user' or 'assistant' message: {request}\nEmpty response set by default")
-        #         self._responses[id]  = [Text()]
         if cache:
-            ids, request_strings = [id for id in ids if not id in self._responses], [request for id, request in
+            criterion = lambda id: id not in self._responses or any([isinstance(r,dict) for r in self._responses[id]])
+            ids, request_strings = [id for id in ids if criterion(id)], [request for id, request in
                                                                                      zip(ids, request_strings) if
-                                                                                     not id in self._responses]
-
+                                                                                     criterion(id)]
         for id, request in zip(ids, request_strings):
             self._requests[id] = request
         return ids, request_strings
 
     def get_response(self, id):
-        """Retrieve a cached response"""
         return self._responses[id] if id in self._responses else None
 
     def add_response(self, id, response):
-        """Append an api response payload to response list."""
         if "error" in response:
             from langtorch import Text
             response = [Text(response["error"], parse=False)]
         elif "data" in response:
             response = torch.tensor(response["data"][0]["embedding"])
-            if self._cache_file:
-                self._append_tensor_to_cache(id, response)
+            result_dict = {id: response}
+            self._tensors.update(result_dict)
         elif "choices" in response:
             from langtorch import Text
             response = [Text.from_messages(m['message'], parse=False) for m in response["choices"]]
-            if self._cache_file:
-                self._append_chat_to_cache(id, response)
         else:
             raise ValueError(f"Invalid response: {response}")
         self._responses.update({id: response})
 
-    def _append_tensor_to_cache(self, key, tensor_data):
-        with h5py.File(self._cache_file, 'a') as f:
-            if key in f:
-                del f[key]  # Delete the existing dataset
-            f.create_dataset(key, data=tensor_data.numpy())
-        ### Alternative, slower implementation with torch.save
-        #     import torch
-        #     result_dict = dict([*zip(inputs, embeddings)])
-        #     if self.tensor_savepath:
-        #         if not os.path.exists(self.tensor_savepath):
-        #             torch.save(result_dict, self.tensor_savepath)
-        #         else:
-        #             tensors = torch.load(self.tensor_savepath)
-        #             assert isinstance(tensors, dict)
-        #             tensors.update(result_dict)
-        #             torch.save(tensors, self.tensor_savepath)
-        #     else:
-        #         self._tensors.update(result_dict)
-        # self.save()
-
-    def _append_chat_to_cache(self, key, texts: list):
-        assert isinstance(texts, list)
-        with h5py.File(self._cache_file, 'a') as f:
-            if key in f:
-                del f[key]  # Delete the existing dataset
-            dt = h5py.string_dtype(encoding='utf-8')
-            f.create_dataset(key, (len(texts),), dtype=dt)
-            for i, text in enumerate(texts):
-                f[key][i] = str(text)
-
     def prompts(self, ids):
         return [self._requests[id] if id in self._requests else None for id in ids]
 
     def completions(self, type, provider, request_strings):
         if len(request_strings) == 0:
             return []
 
         ids, _ = self.request(provider, type, request_strings, False)
         responses = [self.get_response(id) for id in ids]
         for i, response in enumerate(responses):
             if response is None:
                 raise ValueError(f"Could not find response for {request_strings[i]}")
 
         if type == "embeddings":
-            return torch.vstack(responses)
+            return torch.vstack(responses).permute((1,0))
         else:
             from langtorch import TextTensor
             responses = [
                 [text.add_key("assistant") if len(text.items()) != 0 and text.items()[0][0] != "assistant" else text for
                  text in response] for
                 response in responses]
-            return TextTensor(responses, parse=False)
-
-    def save(self, path=None):
-        """Save the current configuration to a file"""
-        if path is None:
-            path = self._session_file
-        if path is None:
-            raise ValueError("No session file path provided")
-        # Decompose the current configuration
-        tensor_savepath = self._config.pop('tensor_savepath', None)
-        tensors_metadata = self._config.pop('tensors', [])
-
-        # Filter attributes starting with an underscore
-        underscore_attrs = OrderedDict((k, v) for k, v in self._config.items() if k.startswith('_'))
-        for k in underscore_attrs.keys():
-            self._config.pop(k, None)
-
-        self._config['tensor_savepath'] = tensor_savepath
-        self._config.tensors = tensors_metadata
-
-        # Merge underscore attributes at the end
-        for k, v in underscore_attrs.items():
-            self._config[k] = v
+            return TextTensor(responses, parse=False).permute((1, 0))
 
-        with open(self._session_file, 'w', encoding="utf-8") as f:
-            OmegaConf.save(self._config, f, resolve=True)
 
     def __setattr__(self, name, value, save=True):
         if name in ["_config", "_tensors", "_session_file", "_overwrite"]:
-            # Use the base class's __setattr__ to prevent recursive calls
             super().__setattr__(name, value)
-            if name == "_config" and self._session_file and save:
+            if name == "_config" and self._path and save:
                 self.save()
         elif name.startswith('_'):
-            # Set the attribute directly
             super().__setattr__(name, value)
         else:
             if isinstance(value, torch.Tensor):
-                tensor_savepath = self._config.tensor_savepath
-                tensors_metadata = self._config.pop('tensors', [])
-                timestamp = datetime.datetime.now().isoformat()
-                if not os.path.exists(tensor_savepath):
-                    tensors = torch.load(tensor_savepath)
-                    tensors[name] = value
-                    torch.save(tensors, tensor_savepath)
-                else:
-                    torch.save({name: value}, tensor_savepath)
-
-                metadata = {
-                    "id": name,
-                    "object": str(type(value)),
-                    "created": timestamp,
-                    "shape": tuple(value.shape)
-                }
-                if name in [m["id"] for m in tensors_metadata]:
-                    tensors_metadata = [m for m in tensors_metadata if m["id"] != name]
-                self._config["tensors"] = list(tensors_metadata) + [metadata]
+                self._tensors[name] = value
             else:
                 try:
                     self._config[name] = value
-                    if name in [m["id"] for m in self._config["tensors"]]:
-                        print(
-                            f"Saving non-tensor with the same name as a saved tensor {name}, the tensor will be unobtainable (but remains saved)")
-                except UnsupportedValueType:
-                    raise UnsupportedValueType("Session can only hold primitive types and TextTenor objects.")
-            if self._session_file and save:
+                    if name in self._tensors:
+                        print(f"Saving non-tensor with the same name as a saved tensor {name}, the tensor will be unobtainable (but remains saved)")
+                except UnsupportedValueType as e:
+                    raise UnsupportedValueType("Session can only hold primitive types and TextTenor objects.") from e
+            if self._path and save:
                 self.save()
 
     @property
     def tensors(self):
-        if self.tensor_savepath:
-            tensors = torch.load(self._config["tensor_savepath"])
-        else:
-            tensors = self._tensors
-        return tensors
+        return self._tensors
+
+    @property
+    def config(self):
+        return self._config
+
+    @property
+    def cfg(self):
+        return self._config
 
     def __getattr__(self, name):
         if name in ["_config", "_session_file", "_cache_file", "_tensors", "_overwrite"]:
             return super().__getattribute__(name)
-        try:
-            # This block of code seems intended to ensure that 'tensors' attribute exists
-            # and initializes it if it doesn't, which should probably be handled elsewhere.
-            _ = (self._config.tensors)
-        except Exception:
-            self.tensors = []
-
-        # If the attribute name corresponds to an id in the tensors list, return that tensors
-        if not hasattr(self._config, name) and name in [m["id"] for m in self._config["tensors"]]:
-            return self.tensors[name]
 
-        # Return the attribute from the configuration
+        if not hasattr(self._config, name) and name in self._tensors:
+            return self._tensors[name]
+
         try:
-            attr = self._config[name]
+            if hasattr(self._config, name):
+                attr = self._config[name]
+            elif hasattr(self._config.cfg, name):
+                attr = self._config.cfg[name]
+            elif hasattr(self._config.methods, name):
+                attr = self._config.methods[name]
+            else:
+                raise KeyError()
         except KeyError as e:
             logging.warning(f"getattr {name}, but session attributes are: {self._config.keys()}")
 
-            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'") from e
-
+            raise AttributeError(f"'{type(self).__name__}' has no attribute '{name}'") from e
         return attr
 
     def get_hash(self, *args):
-        """
-        Generates hash converted to base64 from a list of string requests.
-        This serves as a unique ID for an api request for caching purposes.
-
-        :return: A base64 SHA-256 hash
-        """
         combined_string = ''.join(map(str, args))
-        # Generate a SHA-256 hash
         hex_string = hashlib.sha256(combined_string.encode()).hexdigest()[0:32]
-        # Convert to base 64
         base64_encoded = base64.b64encode(bytes.fromhex(hex_string))
         return base64_encoded.decode('utf-8').replace("/", "_")
 
     @classmethod
     def create_aliases(cls, aliases):
         for alias, path in aliases.items():
             def create_property(path):
                 def property_func(self):
                     return getattr(self, path)
-
                 return property(property_func)
-
             setattr(cls, alias, create_property(path))
 
     def __getitem__(self, entry):
         return self.__getattr__(entry)
 
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
     def __str__(self):
-        return "---   Session Config   ---\n" + yaml.dump(
-            OmegaConf.to_object(self._config)) + "---   --------------   ---\n"
+        return "---   Session Config   ---\n" + yaml.dump(OmegaConf.to_object(self._config)) + "---   --------------   ---\n"
+
+    def __repr__(self):
+        return self.__str__()
 
     def _delete(self):
-        # Cleanup: remove the session file
-        os.remove(self._session_file)
+        os.remove(self._path)
         Session.current_session.set({})
 
     def get_tensor_metadata(self):
         raise NotImplementedError
 
+    # Make Session a context manager
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self._path:  # Save to file if a path is set
+            self.save()
+        # If any exception occurs, you can handle it here.
+        if exc_type is not None and not exc_type is SystemExit:
+            logging.error(f"An error occurred: {exc_val.__class__}")
+        return False  # False means don't suppress exceptions
 
 ctx = Session()
 ctx.create_aliases(cfg_yaml_aliases)
```

### Comparing `LangTorch-1.0.2/src/langtorch/tensors/chattensor.py` & `LangTorch-1.0.3/src/langtorch/tensors/chattensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tensors/codetensor.py` & `LangTorch-1.0.3/src/langtorch/tensors/codetensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tensors/markdowntensor.py` & `LangTorch-1.0.3/src/langtorch/tensors/markdowntensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tensors/texttensor.py` & `LangTorch-1.0.3/src/langtorch/tensors/texttensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             pass
 
     arr = np.array(arr, dtype=object)
     text_arr = [ttype(a, **kwargs) for a in arr.flat]
     text_arr = np.array(text_arr, dtype=object).reshape(arr.shape if shape is None else shape)
     return text_arr
 
+from typing import Any, Callable
+
 
 class TextTensor(torch.Tensor, metaclass=_ParameterMeta):
     """
     TextTensor is a specialized subclass of torch.Tensor designed for handling and manipulating textual data within the LangTorch framework. Each entry in a TextTensor is a structured Text object, enabling complex text operations and transformations, including natural language processing tasks and interaction with large language models (LLMs).
 
     TextTensor supports standard tensor operations adapted for text, such as concatenation and reshaping, alongside unique text-specific operations like prompt formatting through multiplication. It seamlessly integrates with PyTorch, allowing developers to leverage familiar tensor operations while working with textual data.
 
@@ -82,51 +84,88 @@
         - Incorrect usage of keys or mismatched shapes during operations may lead to unexpected results.
     """
 
     _ttype = Text  # The class of a Tensor entry, replaced in subclasses. May in the future move this logic to the metaclass
     _embedding_model = "text-embedding-3-small"  # TextTensor to Tensor with an embedding model
     _tokenizer = None  # TextTensor to Tensor with a transformer tokenizer
     _embedding, _tokens = None, None
-    _tokenizer_default_kwargs = {"return_tensors": "pt", "padding": True, "truncation": True}
+    _tokenizer_kwargs = {"return_tensors": "pt", "padding": True, "truncation": True}
     parse = 'auto'
+    is_gradient = False
+    is_param = False
 
     @classmethod
     def input_formatter(cls, content):
         # Default implementation, to be overridden by subclasses if needed
         return content
 
     @classmethod
     def linter(cls, tensor):
         # Default implementation, ensures correct class of Tensor content entries
         tensor.content = chararray_to_TextArray(tensor.content, cls._ttype)
         return tensor
 
-    def __new__(cls, content="", parse=True, metadata=None, requires_grad: bool = False,
-                is_gradient: bool = False, is_param: bool = False, **kwargs):
+    @classmethod
+    def recursive_walk_replace(cls, obj: Any, target_class: type, func: Callable[[Any], Any]) -> Any:
+        """
+        Recursively walks through any iterable structure, finds all instances of target_class,
+        and replaces them with the result of func applied to them.
+
+        :param obj: The object to walk through.
+        :param target_class: The class to look for in the structure.
+        :param func: The function to apply to instances of target_class.
+        :return: A new object with the replacements made.
+        """
+        if isinstance(obj, target_class):
+            return func(obj)
+        elif isinstance(obj, dict):
+            return {k: cls.recursive_walk_replace(v, target_class, func) for k, v in obj.items()}
+        elif isinstance(obj, (list, set)):
+            cls2 = type(obj)
+            return cls2(cls.recursive_walk_replace(item, target_class, func) for item in obj)
+        elif isinstance(obj, tuple):
+            return func(obj)  # Directly replace tuple with _ttype
+        else:
+            return obj
+
+    def __new__(cls, content="", parse=True, metadata=None,
+                ttype: Text = None,
+                embedding_model: Union[str, Callable] = None,
+                tokenizer: Union[str, Callable] = None,
+                tokenizer_kwargs: dict = None,
+                requires_grad: bool = False,
+                is_gradient: bool = False,
+                is_param: bool = False, **kwargs):
         embedding = None
         if metadata is None:
             metadata = dict()
         for attr in ["content", "embedding"]:
             if not attr in metadata:
                 metadata[attr] = eval(attr)
 
-        def dict_to_tt(cls, d, parse): # TODO create from dict of tensors
+
+        def dict_to_tt(cls, d, parse):  # TODO create from dict of tensors
             if not d:
                 return None
-            def item_to_tt(cls, k,v, parse):
-                content = cls.input_formatter(cls.content_to_object_array(v,  parse=parse))
+
+            def item_to_tt(cls, k, v, parse):
+                content = cls.input_formatter(cls.content_to_object_array(v, parse=parse))
                 content = np.array([(k, v) for v in content.flat], dtype=object).reshape(content.shape)
                 return cls.__new__(cls, content, parse=parse)
 
             content = item_to_tt(cls, d.items()[0][0], d.items()[0][1], parse=parse)
             for k, v in d.items()[1:]:
                 content += item_to_tt(cls, k, v, parse=parse)
             return content
 
-        
+        def replace_tuple_with_ttype(tpl):
+            nonlocal cls
+            return cls._ttype(tpl)
+
+        metadata["content"] = cls.recursive_walk_replace(metadata["content"], tuple, replace_tuple_with_ttype)
         # Set content to be an object array with cls.text_class entries
         metadata["content"] = cls.content_to_object_array(metadata["content"], parse=parse)
         # Apply input formatter
         metadata["content"] = cls.input_formatter(metadata["content"])
 
         tensor = super().__new__(cls, torch.arange(metadata["content"].size, dtype=torch.float32).reshape(
             metadata["content"].shape), **kwargs)
@@ -135,14 +174,23 @@
         tensor._is_param = is_param
         tensor.requires_grad = requires_grad or is_param
         tensor._is_gradient = is_gradient
         assert tensor._content is not None
 
         # Apply linter
         tensor = cls.linter(tensor)
+        if ttype is not None:
+            tensor.ttype = ttype
+        if embedding_model is not None:
+            tensor.embedding_model = embedding_model
+        if tokenizer is not None:
+            tensor.tokenizer = tokenizer
+        if tokenizer_kwargs is not None:
+            tensor._tokenizer_kwargs = tokenizer_kwargs
+
         return tensor
 
     def __init__(self, *args, **kwargs):
         super().__init__()
 
     def __hash__(self):
         return id(self)
@@ -150,24 +198,33 @@
     @classmethod
     def content_to_object_array(cls, input, **kwargs):
         try:
             return input.content if isinstance(input, TextTensor) \
                 else np.array(input, dtype=object) if isinstance(input, Text) \
                 else chararray_to_TextArray(input, cls._ttype, **kwargs)
         except Exception as e:
-            raise ValueError(f"Could not convert input to TextTensor content. Failed to convert input to an array:\n{e}")
+            raise ValueError(
+                f"Could not convert input to TextTensor content. Failed to convert input to an array:\n{e}")
 
     @property
     def content(self):
         return self._content
 
     @content.setter
     def content(self, content):
         self._content = TextTensor.content_to_object_array(content)
         assert self._content is not None
+    @property
+    def embedding_model(self):
+        return self._embedding_model
+
+    @embedding_model.setter
+    def embedding_model(self, embedding_model):
+        self._embedding_model = embedding_model
+        assert self._content is not None
 
     @property
     def embedding(self):
         return self._embedding
 
     @embedding.setter
     def embedding(self, embedding: Union[torch.Tensor, List[float], np.ndarray, tuple]):
@@ -212,39 +269,52 @@
     @tokenizer.setter
     def tokenizer(self, tokenizer):
         if isinstance(tokenizer, str):
             from transformers import AutoTokenizer
             self._tokenizer = AutoTokenizer.from_pretrained(tokenizer)
         self._tokenizer = tokenizer
 
+    @property
+    def tokenizer_kwargs(self):
+        return self._tokenizer_kwargs
+
+    @tokenizer_kwargs.setter
+    def tokenizer_kwargs(self, tokenizer_kwargs):
+        self._tokenizer_kwargs = dict(tokenizer_kwargs)
+
     def tokenize(self, tokenizer=None, **kwargs):
         if tokenizer is not None:
             self.tokenizer = tokenizer
         assert self.tokenizer is not None
-        kwargs = {**self._tokenizer_default_kwargs, **kwargs}
+        kwargs = {**self._tokenizer_kwargs, **kwargs}
         self.tokens = self.tokenizer([str(m) for m in self.content.flat], **kwargs)
+        return self.tokens
 
     @property
     def ttype(self):
         return self._ttype
 
-    @tokens.setter
+    @ttype.setter
     def ttype(self, text_class):
-        if isinstance(text_class, Text):
+        if issubclass(text_class, Text):
             self._ttype = text_class
         else:
             if callable(text_class):
                 raise ValueError("ttype must be a subclass of Text or its name as a string")
             text_class = str(text_class)
             assert text_class in dir(langtorch.texts), f"Text class {text_class} not found in langtorch.texts"
 
             self._ttype = getattr(langtorch.texts, text_class)
+        self.content = np.array([self._ttype(t) for t in self.content.flat], dtype=object).reshape(self.content.shape)
+        # iter over multidimensional self._content
+        for index, text_entry in np.ndenumerate(self._content):
+            self._content[index].language = self._ttype.language
 
     functions_on_texts = [torch.cat, torch.concat, torch.concatenate, torch.vstack, torch.stack, torch.hstack,
-                          torch.squeeze, torch.unsqueeze, torch.reshape, torch.swapaxes, torch.sum]
+                          torch.squeeze, torch.unsqueeze, torch.reshape, torch.swapaxes, torch.sum, torch.nonzero]
     functions_on_embeddings = [torch.mean, torch.cosine_similarity]
     functions_on_tokens = []
 
     @classmethod
     def __torch_function__(cls, func: Callable, types: Iterable, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
@@ -302,14 +372,62 @@
         return func(*args, **kwargs)
 
     @classmethod
     def _handle_functions_on_tokens(self, func: Callable, *args, **kwargs):
         # Fallback if the function is not recognized
         raise NotImplementedError("This torch function has no langtorch equivalent yet")
 
+    @property
+    def loc(self):
+        """
+        Provides key-based indexing for TextTensor, leveraging the `loc` method of the Text entries.
+        You can access and manipulate sub-elements of the TextTensor based on keys.
+        """
+
+        class LocIndexer:
+            def __init__(self, tensor):
+                self.tensor = tensor
+
+            def __getitem__(self, key):
+                result = [text.loc[key] for text in self.tensor.content.flat]
+                shape = self.tensor.content.shape
+                return TextTensor(np.array(result, dtype=object).reshape(shape), parse=False)
+
+            def __setitem__(self, key, value):
+                if not isinstance(value, np.ndarray):
+                    value = np.array(value, dtype=object).reshape(self.tensor.content.shape)
+                for index, text_entry in np.ndenumerate(self.tensor.content):
+                    text_entry.loc[key] = value[index]
+
+        return LocIndexer(self)
+
+    @property
+    def iloc(self):
+        """
+        Provides index-based indexing for TextTensor, leveraging the `iloc` method of the Text entries.
+        You can access and manipulate sub-elements of the TextTensor based on indices.
+        """
+
+        class IlocIndexer:
+            def __init__(self, tensor):
+                self.tensor = tensor
+
+            def __getitem__(self, index):
+                result = [text.iloc[index] for text in self.tensor.content.flat]
+                shape = self.tensor.content.shape
+                return TextTensor(np.array(result, dtype=object).reshape(shape), parse=False)
+
+            def __setitem__(self, index, value):
+                if not isinstance(value, np.ndarray):
+                    value = np.array(value, dtype=object).reshape(self.tensor.content.shape)
+                for idx, text_entry in np.ndenumerate(self.tensor.content):
+                    text_entry.iloc[index] = value[idx]
+
+        return IlocIndexer(self)
+
     def detach(self) -> 'TextTensor':
         with torch.no_grad():
             detached_tensor = self.clone()
 
         detached_tensor._is_param = False
         detached_tensor.requires_grad_(False)
         return detached_tensor
@@ -323,18 +441,16 @@
             self.tokens = self.tokens.to(device, *args, **kwargs)
         return self
 
     def numpy(self):
         return np.array([str(c) for c in self.content.flat]).reshape(self.content.shape)
 
     @classmethod
-    def from_file(cls, path, encoding="utf-8", **kwargs):
-        with open(path, encoding=encoding) as f:
-            content = f.read()
-        return cls(content, **kwargs)
+    def from_file(cls, path, encoding="utf-8", parse: Union[bool, str] = True, **kwargs):
+        return cls._ttype.from_file(path, encoding=encoding, parse=parse).to_tensor(**kwargs)
 
     @classmethod
     def from_df(cls, df: 'DataFrame', **kwargs) -> 'TextTensor':
         text_list = []
         if not "parse" in kwargs:
             kwargs["parse"] = False
 
@@ -427,15 +543,15 @@
                 setattr(self, attr, metadata.pop(attr))
 
         for attr in attrs:
             metadata[attr] = getattr(self, "_" + attr)
 
         self._metadata = metadata
 
-    def metadata_index(self, index):
+    def getitem_over_metadata(self, index):
         """Pick out entries of metadata with the provided index. Usually used to transfer metadata to a sub-tensors."""
 
         index = utils.positive_indices(index, self.content.shape)
         index = index[0] if len(index) == 1 else index
 
         if len(self.content.shape) == 0:  # and (index == slice(None, None, None))
             return self.metadata_apply(lambda v: v, lambda v: v, lambda v: v)
@@ -480,15 +596,15 @@
         if f_scalar:
             for k in scalar_attributes:
                 metadata[k] = f_scalar(metadata[k], *args, **kwargs)
 
         return metadata
 
     def __repr__(self):
-        return str(self.sum().content)
+        return self.__str__()
 
     def __str__(self):
         return self.str_formatter(self)
 
     def inspect(self):
         details = np.vectorize(lambda x: x.inspect())(self.content)
         return details
@@ -498,20 +614,22 @@
         return self.__class__(metadata=new_dict, parse=False)
 
     clone = copy  # Alias
 
     def __eq__(self, other):
         return self.content == other.content if isinstance(other, TextTensor) else self.content == other
 
+    def __ne__(self, other):
+        return ~self.__eq__(other)
     def sum(self, dim: Union[int, List[int]] = None, keepdim: bool = False, sep: str = "") -> 'TextTensor':
         """Reduces the input tensor over the specified dimensions, optionally keeping dimensions."""
         if len(self.shape) == 0:
             return self
 
-        if dim is None:
+        if dim is None and not sep:
             dim = list(range(len(self.shape)))
             connecting_char = ([" "] + ["\n" * (i + 1) for i in range(len(self.content.shape) - 1)])[::-1]
         else:
             if isinstance(dim, int):
                 dim = [dim]
             connecting_char = [sep] * len(dim)
         for d in dim:
@@ -522,16 +640,16 @@
         for d, char in zip(sorted(dim)[::-1], connecting_char):
             result = result.join_with(char, dim=d)
             if keepdim:
                 result = result.unsqueeze(d)
 
         return result
 
-    def join_with(self, delimiter=" ", dim=None):
-        return JoinTextTensor.apply(self, delimiter, dim)
+    def join_with(self, sep=" ", dim=None):
+        return JoinTextTensor.apply(self, sep, dim)
 
     join = join_with  # Alias
 
     def format(self, **kwargs):
         """
         Return a formatted version of self, using substitutions from kwargs.
         The substitutions are identified by braces ('{' and '}').
@@ -583,15 +701,15 @@
             self.content.shape)
 
     def __getattr__(self, name):
         try:
             metadata = object.__getattribute__(self, "_metadata")
         except AttributeError:
             raise AttributeError(
-                "Got a TextTensor without content. TextTensor was likely passed outside of langtorch, e.g. to an unsupported torch function that expects torch.Tensor")
+                "Got a TextTensor without content. TextTensor was likely passed outside of langtorch, e.g. to an unsupported torch function that expects a torch.Tensor")
         if name in ["_content", "content"] or name in metadata:
             if name in metadata:
                 return metadata[name]
             try:
                 return object.__getattribute__(self, name)
             except AttributeError:
                 return None
@@ -624,20 +742,28 @@
                     index = index.indices
                 else:
                     raise ValueError(
                         "Trying to index with an unsupported torch.return_types object. Please use an index compatible with numpy indexing.")
             if isinstance(index, torch.Tensor):
                 index = index.cpu().detach().numpy()
             _ = self.content[index]
-        except IndexError as E:
-            if ("out of bounds" in str(E)) or ("out of range" in str(E)):
-                raise IndexError(f"Index {index} out of bounds for TextTensor of shape {self.content.shape}")
+        except IndexError as e:
+            if ("out of bounds" in str(e)) or ("out of range" in str(e)):
+                raise IndexError(f"Index {index} out of bounds for TextTensor of shape {self.content.shape}") from e
             else:
-                raise E
-        return self.__class__(metadata=self.metadata_index(index), parse=False)
+                raise e
+        return self.__class__(metadata=self.getitem_over_metadata(index),
+                            ttype=self.ttype,
+                            embedding_model=self.embedding_model,
+                            tokenizer=self.tokenizer,
+                            tokenizer_kwargs=self.tokenizer_kwargs,
+                            requires_grad=self.requires_grad,
+                            is_gradient=self.is_gradient,
+                            is_param=self.is_param,
+                            parse=False)
 
     def __setitem__(self, index, value):
         """
         Sets the item at the specified index to value. If embeddings are present, they are invalidated for the modified entries.
 
         Parameters:
         - index: The index or indices specifying where to update the tensor.
```

### Comparing `LangTorch-1.0.2/src/langtorch/texts/chat.py` & `LangTorch-1.0.3/src/langtorch/texts/chat.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/texts/markdown.py` & `LangTorch-1.0.3/src/langtorch/texts/markdown.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/texts/text.py` & `LangTorch-1.0.3/src/langtorch/texts/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         content = [c if c is not None else cls.identity for c in (list(substrings) + list(named_substrings.items()))]
         # cast TextTensors to strings
         for i in range(len(content)):
             if is_TextTensor(content[i]):
                 content[i] = content[i].sum().item()
                 assert isinstance(content[i], str) or (0 < len(content[i]) <= 2)
         # returns the final content tuple
-        parser = "langtorch-f-string" if parse is True else parse
+        parser = "langtorch-f-string" if parse is True else (False if parse is None else parse)
         content = cls._parse_content(content, parser=parser)
 
         assert cls._is_valid_tree(content, is_tuple=True), f"Creating Text with an invalid content tree: {content}"
 
         instance = super().__new__(cls, cls.str_formatter(content))
         instance._content = content
         instance.language = language
@@ -140,15 +140,15 @@
         Returns:
             (str): A string representation of the instance.
         """
         return cls.formatters[language](instance)
 
     def __str__(self):
         s = self.__class__.str_formatter(self, self.language)
-        return s if s else "\u200B"  # Zero width space to fix errors with printing arrays of empty Texts
+        return s
 
     @classmethod
     def from_messages(cls, *messages, **kwargs):
         """Text from a list of dicts with keys 'role' and 'content'"""
         if len(messages) == 0:
             return cls()
         if all(isinstance(m, list) for m in messages):
@@ -210,19 +210,26 @@
         bottom_line = bottom_line.rstrip('|')
 
         # Print the formatted lines
         print(top_line)
         print(bottom_line)
 
     def __repr__(self):
-        return self.__str__()
+        s = self.__class__.str_formatter(self, self.language)
+        return s if s else "\u200b"  # Zero width space to fix errors with printing arrays of empty Texts
+
 
-    def to_tensor(self):
+    def to_tensor(self, **kwargs):
         from langtorch import TextTensor
-        return TextTensor(self.content)
+        if not "ttype" in kwargs:
+            kwargs["ttype"] = self.__class__
+            kwargs["ttype"].language = self.language
+        if not "parse" in kwargs:
+            kwargs["parse"] = False
+        return TextTensor(self.items(), **kwargs)
 
     @property
     def identity(self):
         return self.__class__()
 
     @property
     def content(self):
@@ -460,15 +467,15 @@
                     """
                     if isinstance(keys, str):
                         keys = [keys]
                     if not isinstance(value, Text):
                         value = Text(value)
 
                     new_tup = []
-                    relevant_items = [(k, v) for k, v in tup if k in keys]
+                    relevant_items = [kv for kv in tup if kv[0] in keys]
                     # Editing case
                     if len(relevant_items) <= len(value.items()):
                         replacement_items = list(value.items()[:len(relevant_items)])
                         append_items = list(value.items()[len(relevant_items):])
                     else:
                         replacement_items = [value.items()] * len(relevant_items)
                         append_items = []
@@ -501,26 +508,35 @@
         from langtorch import TextTensor
         return TextTensor(str(self).split() if sep == "" else str(self).split(sep), parse=False)
 
 
     def __getitem__(self, index):
         if isinstance(index, str):
             return self.loc[index]
-        return self.iloc[index]
+        return str(self)[index]
 
     def __or__(self, other):
         return
 
     def __len__(self):
         return len(str(self.content))
 
+    def __eq__(self, other):
+        if isinstance(other, Text):
+            return self.content == other.content
+        elif isinstance(other,str):
+            s = str(Text(self)).replace("u200b","")
+            return s == other
+        return False
+
     def __iter__(self):
         for s in self.content:
             yield s
 
+
     # def _handle_other(self, other, method):
     #     if isinstance(other, str) and not isinstance(other, Text):
     #         return other
     #     elif isinstance(other, Text):
     #         return other.content
     #     elif is_TextTensor(other):
     #         if len(other.flat) == 1:
@@ -795,34 +811,34 @@
         return bool(re.fullmatch(full_pattern, text))
 
     @classmethod
     def guess_language(cls, text):
         return Text.guess_format(text)
 
     @classmethod
-    def load(cls, path: str, language: str = "str"):
+    def load(cls, path: str, encoding="utf-8", parse: Union[bool, str] = True):
         # Determine the caller's file path
         caller_frame = inspect.currentframe().f_back
         caller_file = inspect.getframeinfo(caller_frame).filename
         caller_dir = os.path.dirname(caller_file)
 
         # Resolve the relative path to an absolute path
         absolute_path = os.path.abspath(os.path.join(caller_dir, path))
 
         # Extract the file extension as the input format
-        if language == "str":
-            input_format = os.path.splitext(absolute_path)[1][1:]
+        if parse is True:
+            language = os.path.splitext(absolute_path)[1][1:]
         else:
-            input_format = language
+            language = parse
 
         # Read the file content
-        with open(absolute_path, 'r', encoding="utf-8") as file:
+        with open(absolute_path, 'r', encoding=encoding) as file:
             input_string = file.read()
 
-        return cls(input_string, language=input_format, parse=input_format)
+        return cls(input_string, parse=language, language=language)
 
     def save(self, path: str) -> None:
         with open(path, 'w', encoding='utf-8') as file:
             file.write(str(self))
 
     from_file = load
     to_file = save
```

### Comparing `LangTorch-1.0.2/src/langtorch/tt/functional.py` & `LangTorch-1.0.3/src/langtorch/tt/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,40 +236,40 @@
     def backward(ctx, grad_output):
         # Add here
         return ...
 
 
 class JoinTextTensor(Function):
     @staticmethod
-    def forward(ctx, input, on="", dim=None):
+    def forward(ctx, input, sep="", dim=None):
         shape = input.content.shape
-        ctx.save_for_backward(input, langtorch.TextTensor(on, parse=False), torch.tensor(shape),
+        ctx.save_for_backward(input, langtorch.TextTensor(sep, parse=False), torch.tensor(shape),
                               torch.tensor(dim if dim is not None else []))
         # Convert the content to a list and join the elements with `on`
         if len(input.shape) == 0: return input
         if dim is not None and len(input.shape) > dim and input.shape[dim] == 1: return input.squeeze(dim=dim)
 
         if dim is None:
             result = input.ttype()
             for i, t in enumerate(input.content.flat):
                 if i != input.content.size - 1:
-                    result += (t + on)
+                    result += (t + sep)
                 else:
                     result += t
             output = input.__class__(result, parse=False)
         else:
             if dim < 0: dim = dim + len(input.shape)
             new_shape = input.shape[:dim] + input.shape[dim + 1:]
 
             for i, tt in enumerate(langtorch.utils.iter_subarrays(input.content, dim)):
 
                 if i == 0:
                     result = tt.reshape(new_shape)
                 else:
-                    result = np.array([m + on + t for m, t in zip(result.flat, tt.flat)], dtype=object).reshape(
+                    result = np.array([m + sep + t for m, t in zip(result.flat, tt.flat)], dtype=object).reshape(
                         new_shape)
             output = input.__class__(result, parse=False)
 
         return output
 
     @staticmethod
     def backward(ctx, grad_output):
@@ -283,15 +283,15 @@
 
 
 class ReshapeTextTensor(Function):
     @staticmethod
     def forward(ctx, input, shape):
         ctx.shape = input.shape
         output = input.__class__(input.content.reshape(*shape), parse=False),
-        # metadata = input.metadax
+        # metadata = input.metadata
         # a_apply(lambda v: v.reshape(*shape), lambda v: v.reshape(*shape, v.shape[-1]))
         # # add metadata
         return output
 
     @staticmethod
     def backward(ctx, grad_output):
         return grad_output.reshape(ctx.shape), None
```

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_t/distance.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_t/distance.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_t/tokenizer.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_t/tokenizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/activation.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/activation.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,60 +28,64 @@
 
 class Activation(TextModule):
     input_class = TextTensor
     output_class = TextTensor
 
     @set_defaults_from_ctx
     def __new__(cls, model: str = "default",
-                system_message: str = "default",
+                system_message: str = None,
+                provider: str = "openai",
                 cache: bool = False,
                 keep_history: bool = False,
                 T: float = 0.8,
                 tools: Optional[List[dict]] = None,
                 key: Optional[str] = None,
                 backward_prompt: Union[str, TextTensor] = "default",
                 *args, **kwargs):
         if any([arg == "default" for arg in [model, system_message]]):
             print(f"model = {model}, system_message = {system_message}")
             raise ValueError(
                 "Activation requires a model and system_message,, but these were not loaded from defaults or passed.")
         if cls is Activation:
             # Return an instance of the OpenAI subclass instead of Activation
             # In the future more subclasses of Activation will be added here
-            return OpenAI(model=model,
-                          system_message=system_message,
-                          cache=cache,
-                          keep_history=keep_history,
-                          T=T,
-                          tools=tools,
-                          key=key,
-                          backward_prompt=backward_prompt,
-                          *args, **kwargs)
+                activation = OpenAI(model=model,
+                              system_message=system_message,
+                              cache=cache,
+                              keep_history=keep_history,
+                              T=T,
+                              tools=tools,
+                              key=key,
+                              backward_prompt=backward_prompt,
+                              *args, **kwargs)
+                activation.provider = provider
+                return activation
         else:
             # If a subclass of Activation is being instantiated, proceed as normal
             return super().__new__(cls)
 
 
 class OpenAI(TextModule):
     input_class = TextTensor
     output_class = TextTensor
+    provider = "openai"
 
     def __init__(self,
                  model: Union[str, TextTensor] = "gpt-3.5-turbo",
                  system_message: Union[
-                     str, TextTensor] = "You are an expert, who answers only with the requested texts. Keep it short.",
+                     str, TextTensor] = None,
                  backward_prompt: Union[str, TextTensor] = "",
                  cache: bool = False,
                  keep_history: bool = False,
                  T: float = 0.8,
                  tools: Optional[List[dict]] = None,
                  parse_output=False,
                  *args, **kwargs):
         super(OpenAI, self).__init__()
-        self.system_message = str(system_message)
+        self.system_message = str(system_message) if system_message is not None else None
         self.model = model
         self.backward_prompt = backward_prompt
         self.keep_history = True if keep_history or kwargs.get('echo', False) else False
         if not 'temperature' in kwargs:
             kwargs['temperature'] = T
         cache = cache | (kwargs['temperature'] == .0)
         self.cache = cache
@@ -98,15 +102,15 @@
         self.parse_output = parse_output
 
     def forward(self, input: TextTensor):
         if isinstance(input, list):
             shape = (-1, self.n) if self.n > 1 else -1
             input = TextTensor(input)
         elif isinstance(input, TextTensor):
-            shape = tuple([m for m in input.shape] + [self.n]) if self.n > 1 else tuple(input.shape)
+            shape = tuple([self.n]+[m for m in input.shape]) if self.n > 1 else tuple(input.shape)
         else:
             raise TypeError("Activation handles only lists and TextTensors")
 
         input = list(input.content.flat)
         system_messages = [self.system_message] * len(input)
 
         # Transform chat input into (role, content) pairs
@@ -123,15 +127,15 @@
                     f"A text without exclusively 'assistant' ot 'user' keys was passed to OpenAI Chat. Assuming the whole Text is one user message: = '{str(m)[:25]}'... ")
             else:
                 raise ValueError(
                     f"Invalid input to OpenAI Chat. Ambiguous input: some but not all items in TextTensor entries have keys 'user' or 'assistant'. Change the input into a valid chat, or the input was a single user message remove these keys or use entry.add_key_('user'): \nentry.items()=={m.items()}")
         logging.debug(f"Chat api input: {input}")
         logging.debug(f"Chat api unique system messages: {set(system_messages)}")
 
-        result = chat(input, system_messages, model=self.model, cache=self.cache, as_str=True, tools=self.tool_jsons,
+        result = chat(input, system_messages, model=self.model, provider=self.provider, cache=self.cache, as_str=True, tools=self.tool_jsons,
                       **self.kwargs)
 
         assert result is not None
         if not self.keep_history:
             return TextTensor(result, parse=self.parse_output).reshape(shape)
         else:
             return input + TextTensor(result, parse=self.parse_output).reshape(shape)
```

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/assistantmodule.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/assistantmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/codemodule.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/codemodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/conv.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/linear.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Shape:
         - Input: :math:`(*, H_{in})` where :math:`*` means any number of
           dimensions including none and :math:`H_{in} = \text{in\_features}`.
         - Output: :math:`(*, H_{out})` where all but the last dimension
           are the same shape as the input and :math:`H_{out} = \text{out\_features}`.
 
     Attributes:
-        weight: the TextTensor to format of shape
+        prompt: the TextTensor to format of shape
             :math:`(\text{out\_features}, \text{in\_features})`. The values are
             initialized from :math:`\mathcal{U}(-\sqrt{k}, \sqrt{k})`, where
             :math:`k = \frac{1}{\text{in\_features}}`
         bias:   the "bias", Text that is added of the module of shape :math:`(\text{out\_features})`.
                 If :attr:`bias` is ``True``, the values are initialized from
                 :math:`\mathcal{U}(-\sqrt{k}, \sqrt{k})` where
                 :math:`k = \frac{1}{\text{in\_features}}`
```

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/loss.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/loss.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/retriever.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/retriever.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/textmodule.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/textmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
            >>> summary = text_module(input_text)
            # summary is a TextTensor with the key "summary" containing the summarized texts.
        """
     input_class = TextTensor
     output_class = TextTensor
 
     def __init__(self,
-                 prompt: Union[str, 'TextTensor', Callable] = [""],
+                 prompt: Union[str, TextTensor, list] = [""],
                  activation=None,
                  key=None,
                  type_checking=False, *args, **kwargs):
         super(TextModule, self).__init__(*args, **kwargs)
 
         if not isinstance(prompt, TextTensor):
             self._prompt = TextTensor(prompt)
```

### Comparing `LangTorch-1.0.2/src/langtorch/tt/modules/to_tt/transformers.py` & `LangTorch-1.0.3/src/langtorch/tt/modules/to_tt/transformers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.2/src/langtorch/types.py` & `LangTorch-1.0.3/src/langtorch/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import torch
 
 import langtorch
 
 # Convenience aliases for common composite types that we need
 # to talk about in LangTorch
 
-_TextTensorOrTensors = Union[langtorch.TextTensor, Sequence[langtorch.TextTensor]]
-_TextTensorOrText = Union[langtorch.TextTensor, str]
+TextTensorOrTensors = Union[langtorch.TextTensor, Sequence[langtorch.TextTensor]]
+TextTensorOrText = Union[langtorch.TextTensor, str]
 
 
 # Storage protocol implemented by ${Type}StorageBase classes, maybe use this interface
 
 class Storage:
     _cdata: int
     device: torch.device
```

### Comparing `LangTorch-1.0.2/src/langtorch/utils.py` & `LangTorch-1.0.3/src/langtorch/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 import torch
 from torch.types import _TensorOrTensors
 
 import langtorch
 from .torch_utils import _OptionalTensor
 
-
 def zeros_like(other, **kwargs):
     size = other.content.size if isinstance(other, langtorch.TextTensor) else other.size
     return langtorch.TextTensor([langtorch.Text()] * size, **kwargs).reshape(other.shape)
 
 
 def zeros(*shape, **kwargs):
     return langtorch.TextTensor(np.char.array(torch.zeros(*shape), unicode=True).join("").astype(dtype="<U"), **kwargs)
```

