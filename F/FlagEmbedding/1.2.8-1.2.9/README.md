# Comparing `tmp/FlagEmbedding-1.2.8.tar.gz` & `tmp/FlagEmbedding-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlagEmbedding-1.2.8.tar", last modified: Wed Mar 20 07:38:25 2024, max compression
+gzip compressed data, was "FlagEmbedding-1.2.9.tar", last modified: Wed Apr 17 05:42:00 2024, max compression
```

## Comparing `FlagEmbedding-1.2.8.tar` & `FlagEmbedding-1.2.9.tar`

### file list

```diff
@@ -1,93 +1,100 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:24.000000 FlagEmbedding-1.2.8/FlagEmbedding/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    13476 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/data.py
--rw-rw-rw-   0 root         (0) root         (0)    17799 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     5889 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/run.py
--rw-rw-rw-   0 root         (0) root         (0)     7601 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/split_data_by_length.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2818 2024-02-19 03:56:00.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     4008 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/data.py
--rw-rw-rw-   0 root         (0) root         (0)     7233 2023-10-31 12:34:46.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/eval_msmarco.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2023-11-25 06:12:39.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/hn_mine.py
--rw-rw-rw-   0 root         (0) root         (0)     5200 2024-02-19 03:56:00.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-01-23 08:48:12.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2275 2024-01-23 13:13:27.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/trainer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-09-07 08:58:23.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-08-22 15:34:10.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/data.py
--rw-rw-rw-   0 root         (0) root         (0)    13649 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/enhancedDecoder.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2023-11-03 09:31:39.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/run.py
--rw-rw-rw-   0 root         (0) root         (0)     1857 2023-11-30 03:17:01.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11648 2024-02-27 07:43:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/bge_m3.py
--rw-rw-rw-   0 root         (0) root         (0)    10505 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/flag_models.py
--rw-rw-rw-   0 root         (0) root         (0)    17797 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.8/FlagEmbedding/flag_reranker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5054 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     8297 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/data.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/load_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     4516 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2137 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/trainer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5407 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     9966 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/configuration_minicpm_reranker.py
--rw-rw-rw-   0 root         (0) root         (0)     8157 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/data.py
--rw-rw-rw-   0 root         (0) root         (0)     3970 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/load_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3977 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)    72521 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling_minicpm_reranker.py
--rw-rw-rw-   0 root         (0) root         (0)     4610 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/trainer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2023-10-31 12:34:46.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/data.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2023-12-19 04:11:47.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/modeling.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/run.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-11-30 03:17:01.000000 FlagEmbedding-1.2.8/FlagEmbedding/reranker/trainer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    22490 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/eva_vit_model.py
--rw-rw-rw-   0 root         (0) root         (0)    21025 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1928 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/hf_configs.py
--rw-rw-rw-   0 root         (0) root         (0)    10571 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/hf_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5862 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/loss.py
--rw-rw-rw-   0 root         (0) root         (0)    17076 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/modified_resnet.py
--rw-rw-rw-   0 root         (0) root         (0)     5446 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/openai.py
--rw-rw-rw-   0 root         (0) root         (0)    11791 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/pretrained.py
--rw-rw-rw-   0 root         (0) root         (0)     5368 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/rope.py
--rw-rw-rw-   0 root         (0) root         (0)     4910 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/timm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     7125 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/tokenizer.py
--rw-rw-rw-   0 root         (0) root         (0)     3382 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/transform.py
--rw-rw-rw-   0 root         (0) root         (0)    26730 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)    14654 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14306 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.8/FlagEmbedding/visual/modeling.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-20 07:38:24.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    24438 2024-03-20 07:38:23.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3650 2024-03-20 07:38:23.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-20 07:38:23.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-20 07:38:23.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-20 07:38:23.000000 FlagEmbedding-1.2.8/FlagEmbedding.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    24438 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    24210 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-20 07:38:25.000000 FlagEmbedding-1.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:41:59.000000 FlagEmbedding-1.2.9/FlagEmbedding/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:41:59.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4419 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    13476 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/data.py
+-rw-rw-rw-   0 root         (0) root         (0)    17797 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     8006 2024-03-28 08:44:23.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/split_data_by_length.py
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:41:59.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2024-02-19 03:56:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)     4008 2024-03-12 08:08:33.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7233 2023-10-31 12:34:46.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/eval_msmarco.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2023-11-25 06:12:39.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/hn_mine.py
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2024-02-19 03:56:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-01-23 08:48:12.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2024-01-23 13:13:27.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-09-07 08:58:23.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-08-22 15:34:10.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13649 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/enhancedDecoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3626 2024-03-28 08:44:23.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2023-11-30 03:17:01.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11648 2024-02-27 07:43:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/bge_m3.py
+-rw-rw-rw-   0 root         (0) root         (0)    10505 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/flag_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    27345 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/flag_reranker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5054 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)     8321 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/load_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4516 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2137 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)     9966 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/configuration_minicpm_reranker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8181 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/load_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)    72521 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling_minicpm_reranker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4678 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9965 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/configuration_minicpm_reranker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/merge_base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1552 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/merge_layerwise_model_from_finetuned_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3454 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/merge_layerwise_model_from_raw_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    72520 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/merge/modeling_minicpm_reranker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2023-10-31 12:34:46.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2023-12-19 04:11:47.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/modeling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2023-09-12 12:00:08.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-11-30 03:17:01.000000 FlagEmbedding-1.2.9/FlagEmbedding/reranker/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    22492 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/eva_vit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    21025 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1928 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/hf_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10571 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/hf_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5862 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/loss.py
+-rw-rw-rw-   0 root         (0) root         (0)    17078 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7055 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/modified_resnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5446 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/openai.py
+-rw-rw-rw-   0 root         (0) root         (0)    11791 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/pretrained.py
+-rw-rw-rw-   0 root         (0) root         (0)     5368 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/rope.py
+-rw-rw-rw-   0 root         (0) root         (0)     4910 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/timm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7125 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/tokenizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    26732 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)    14654 2024-03-18 07:31:20.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14277 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/FlagEmbedding/visual/modeling.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 05:41:59.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    24438 2024-04-17 05:41:58.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2024-04-17 05:41:58.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 05:41:58.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-17 05:41:58.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-17 05:41:58.000000 FlagEmbedding-1.2.9/FlagEmbedding.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-08-09 07:15:28.000000 FlagEmbedding-1.2.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    24438 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    24210 2024-03-20 07:37:49.000000 FlagEmbedding-1.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-17 05:42:00.000000 FlagEmbedding-1.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-17 05:38:52.000000 FlagEmbedding-1.2.9/setup.py
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/arguments.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/data.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                                                       dense_scores + 0.3 * sparse_scores + colbert_scores,
                                                       group_size=group_size)
                     loss = (loss + ensemble_loss + 0.1 * sparse_loss + colbert_loss) / 4
 
 
             else:
                 idxs = torch.arange(q_dense_vecs.size(0), device=q_dense_vecs.device, dtype=torch.long)
-                targets = idxs * (p_sparse_vecs.size(0) // q_sparse_vecs.size(0))
+                targets = idxs * (p_dense_vecs.size(0) // q_dense_vecs.size(0))
 
                 # dense loss
                 dense_scores = self.dense_score(q_dense_vecs, p_dense_vecs)  # B, B * N
                 if self.negatives_cross_device:
                     cross_q_dense_vecs = self._dist_gather_tensor(q_dense_vecs)
                     cross_p_dense_vecs = self._dist_gather_tensor(p_dense_vecs)
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/run.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/split_data_by_length.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/split_data_by_length.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 --overwrite False
 """
 import os
 import json
 import math
 import time
 import argparse
+import datasets
 from tqdm import tqdm
 from pprint import pprint
 from transformers import AutoTokenizer
 from datasets import load_dataset, Features, Value, Sequence
 
 
 def get_args():
@@ -50,25 +51,26 @@
         pprint(self.length_ranges_list)
 
         def _map_func(examples):
             results = {}
             results['idx'] = []
             results['max_length'] = []
             for i in range(len(examples['query'])):
-                results['idx'].append(i)
-
+                idx = examples['idx'][i]
                 query = examples['query'][i]
                 pos, neg = examples['pos'][i], examples['neg'][i]
                 all_texts = [query] + pos + neg
 
                 max_len = 0
                 for x in all_texts:
                     tokenized_x = self.tokenizer(x)['input_ids']
                     if len(tokenized_x) > max_len:
                         max_len = len(tokenized_x)
+                
+                results['idx'].append(idx)
                 results['max_length'].append(max_len)
             return results
 
         self._map_func = _map_func
 
     @staticmethod
     def _get_length_ranges_list(length_list: list):
@@ -116,25 +118,33 @@
             'pos_scores': Sequence(Value('float')),
             'neg_scores': Sequence(Value('float'))
         })
         try:
             dataset = load_dataset('json', data_files=file_path, cache_dir=self.cache_dir, features=features)['train']
         except:
             dataset = load_dataset('json', data_files=file_path, cache_dir=self.cache_dir, features=kd_features)['train']
-        mapped_dataset = dataset.map(self._map_func, batched=True, num_proc=self.num_proc)
 
+        dataset_with_idx_list = []
+        for i, data in enumerate(dataset):
+            data['idx'] = i
+            dataset_with_idx_list.append(data)
+        dataset_with_idx = datasets.Dataset.from_list(dataset_with_idx_list)
+        
+        mapped_dataset = dataset_with_idx.map(self._map_func, batched=True, num_proc=self.num_proc)
+        
         split_info_dict = {}
         for length_l, length_r in self.length_ranges_list:
             save_path = output_path + f'_len-{length_l}-{length_r}.jsonl'
             if os.path.exists(save_path) and not self.overwrite:
                 print(f'{save_path} exists, skip')
                 continue
 
             idxs = mapped_dataset.filter(lambda x: length_l <= x['max_length'] < length_r, num_proc=self.num_proc)
-            split_dataset = dataset.select(idxs['idx'])
+            split_dataset = dataset_with_idx.select(idxs['idx'])
+            split_dataset = split_dataset.remove_columns('idx')
 
             split_info_dict[f'len-{length_l}-{length_r}'] = len(split_dataset)
 
             if len(split_dataset) > 0:
                 split_dataset.to_json(save_path, force_ascii=False)
 
         end_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/BGE_M3/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/BGE_M3/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/arguments.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/data.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/eval_msmarco.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/eval_msmarco.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/hn_mine.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/hn_mine.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/modeling.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/run.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/finetune/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/finetune/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/arguments.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/data.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/enhancedDecoder.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/enhancedDecoder.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,20 +49,20 @@
             return_dict=True
         )
         cls_hiddens = lm_out.hidden_states[-1][:, :1]  # B 1 D
 
         decoder_embedding_output = self.decoder_embeddings(input_ids=decoder_input_ids)
         hiddens = torch.cat([cls_hiddens, decoder_embedding_output[:, 1:]], dim=1)
 
-        decoder_position_ids = self.lm.bert.embeddings.position_ids[:, :decoder_input_ids.size(1)]
-        decoder_position_embeddings = self.lm.bert.embeddings.position_embeddings(decoder_position_ids)  # B L D
-        query = decoder_position_embeddings + cls_hiddens
+        # decoder_position_ids = self.lm.bert.embeddings.position_ids[:, :decoder_input_ids.size(1)]
+        # decoder_position_embeddings = self.lm.bert.embeddings.position_embeddings(decoder_position_ids)  # B L D
+        # query = decoder_position_embeddings + cls_hiddens
 
-        # cls_hiddens = cls_hiddens.expand(hiddens.size(0), hiddens.size(1), hiddens.size(2))
-        # query = self.decoder_embeddings(inputs_embeds=cls_hiddens)
+        cls_hiddens = cls_hiddens.expand(hiddens.size(0), hiddens.size(1), hiddens.size(2))
+        query = self.decoder_embeddings(inputs_embeds=cls_hiddens)
 
         matrix_attention_mask = self.lm.get_extended_attention_mask(
             decoder_attention_mask,
             decoder_attention_mask.shape,
             decoder_attention_mask.device
         )
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/run.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/baai_general_embedding/retromae_pretrain/utils.py` & `FlagEmbedding-1.2.9/FlagEmbedding/baai_general_embedding/retromae_pretrain/utils.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/bge_m3.py` & `FlagEmbedding-1.2.9/FlagEmbedding/bge_m3.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/flag_models.py` & `FlagEmbedding-1.2.9/FlagEmbedding/flag_models.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/flag_reranker.py` & `FlagEmbedding-1.2.9/FlagEmbedding/flag_reranker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union, List, Tuple, Any
 
 import numpy as np
 import torch
 from torch import Tensor
 from torch.utils.data import DataLoader
-from tqdm import tqdm
+from tqdm import tqdm, trange
 from transformers import AutoTokenizer, AutoModelForCausalLM, AutoModelForSequenceClassification, is_torch_npu_available
 
 import warnings
 from torch.utils.data import Dataset
 import os
 os.environ['TOKENIZERS_PARALLELISM'] = 'true'
 
@@ -147,40 +147,52 @@
     return 1 / (1 + np.exp(-x))
 
 class FlagReranker:
     def __init__(
             self,
             model_name_or_path: str = None,
             use_fp16: bool = False,
-            cache_dir: str = None
+            cache_dir: str = None,
+            device: Union[str, int] = None
     ) -> None:
 
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, cache_dir=cache_dir)
         self.model = AutoModelForSequenceClassification.from_pretrained(model_name_or_path, cache_dir=cache_dir)
 
-        if torch.cuda.is_available():
-            self.device = torch.device("cuda")
-        elif torch.backends.mps.is_available():
-            self.device = torch.device("mps")
-        elif is_torch_npu_available():
-            self.device = torch.device("npu")
+        if device and isinstance(device, str):
+            self.device = torch.device(device)
+            if device == 'cpu':
+                use_fp16 = False
         else:
-            self.device = torch.device("cpu")
-            use_fp16 = False
+            if torch.cuda.is_available():
+                if device is not None:
+                    self.device = torch.device(f"cuda:{device}")
+                else:
+                    self.device = torch.device("cuda")
+            elif torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            elif is_torch_npu_available():
+                self.device = torch.device("npu")
+            else:
+                self.device = torch.device("cpu")
+                use_fp16 = False
         if use_fp16:
             self.model.half()
 
         self.model = self.model.to(self.device)
 
         self.model.eval()
 
-        self.num_gpus = torch.cuda.device_count()
-        if self.num_gpus > 1:
-            print(f"----------using {self.num_gpus}*GPUs----------")
-            self.model = torch.nn.DataParallel(self.model)
+        if device is None:
+            self.num_gpus = torch.cuda.device_count()
+            if self.num_gpus > 1:
+                print(f"----------using {self.num_gpus}*GPUs----------")
+                self.model = torch.nn.DataParallel(self.model)
+        else:
+            self.num_gpus = 1
 
     @torch.no_grad()
     def compute_score(self, sentence_pairs: Union[List[Tuple[str, str]], Tuple[str, str]], batch_size: int = 256,
                       max_length: int = 512, normalize: bool = False) -> List[float]:
         if self.num_gpus > 0:
             batch_size = batch_size * self.num_gpus
 
@@ -214,72 +226,143 @@
 class FlagLLMReranker:
     def __init__(
             self,
             model_name_or_path: str = None,
             use_fp16: bool = False,
             use_bf16: bool = False,
             cache_dir: str = None,
-            device: int = 0
+            device: Union[str, int] = None
     ) -> None:
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path,
                                                        cache_dir=cache_dir,
                                                        trust_remote_code=True)
 
         self.model = AutoModelForCausalLM.from_pretrained(model_name_or_path,
                                                           cache_dir=cache_dir,
                                                           trust_remote_code=True,
                                                           torch_dtype=torch.bfloat16 if use_bf16 else torch.float32)
         self.model_name_or_path = model_name_or_path
         self.cache_dir = cache_dir
 
-        if torch.cuda.is_available():
-            torch.cuda.set_device(device)
-            self.device = torch.device('cuda')
-        elif torch.backends.mps.is_available():
-            self.device = torch.device('mps')
+        if device and isinstance(device, str):
+            self.device = torch.device(device)
         else:
-            self.device = torch.device('cpu')
-            use_fp16 = False
+            device = 0 if device is None else device
+            if torch.cuda.is_available():
+                torch.cuda.set_device(device)
+                self.device = torch.device("cuda")
+            elif torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            elif is_torch_npu_available():
+                self.device = torch.device("npu")
+            else:
+                self.device = torch.device("cpu")
+                use_fp16 = False
+
         if use_fp16 and use_bf16 is False:
             self.model.half()
 
         self.model = self.model.to(self.device)
 
         self.model.eval()
 
         self.yes_loc = self.tokenizer('Yes', add_special_tokens=False)['input_ids'][0]
 
     @torch.no_grad()
     def compute_score(self, sentence_pairs: Union[List[Tuple[str, str]], Tuple[str, str]], batch_size: int = 16,
-                      max_length: int = 512, prompt: str = None, normalize: bool = False) -> List[float]:
+                      max_length: int = 512, prompt: str = None, normalize: bool = False,
+                      use_dataloader: bool = True, num_workers: int = None) -> List[float]:
         assert isinstance(sentence_pairs, list)
         if isinstance(sentence_pairs[0], str):
             sentence_pairs = [sentence_pairs]
 
         length_sorted_idx = np.argsort([-self._text_length(q) - self._text_length(p) for q, p in sentence_pairs])
         sentences_sorted = [sentence_pairs[idx] for idx in length_sorted_idx]
 
-        dataset = DatasetForReranker(sentences_sorted,
-                                     self.model_name_or_path,
-                                     max_length,
-                                     cache_dir=self.cache_dir,
-                                     prompt=prompt)
-        dataloader = DataLoader(dataset, shuffle=False, batch_size=batch_size, drop_last=False,
-                                num_workers=min(batch_size, 16),
-                                collate_fn=collater(self.tokenizer, max_length))
+        dataset, dataloader = None, None
+        if use_dataloader:
+            if num_workers is None:
+                num_workers = min(batch_size, 16)
+            dataset = DatasetForReranker(sentences_sorted,
+                                         self.model_name_or_path,
+                                         max_length,
+                                         cache_dir=self.cache_dir,
+                                         prompt=prompt)
+            dataloader = DataLoader(dataset, shuffle=False, batch_size=batch_size, drop_last=False,
+                                    num_workers=num_workers,
+                                    collate_fn=collater(self.tokenizer, max_length))
 
         all_scores = []
-        for inputs in tqdm(dataloader):
-            inputs = inputs.to(self.device)
-
-            outputs = self.model(**inputs, output_hidden_states=True)
-            logits = outputs.logits
-            scores = last_logit_pool(logits, inputs['attention_mask'])
-            scores = scores[:, self.yes_loc]
-            all_scores.extend(scores.cpu().float().tolist())
+        if dataloader is not None:
+            for inputs in tqdm(dataloader):
+                inputs = inputs.to(self.device)
+
+                outputs = self.model(**inputs, output_hidden_states=True)
+                logits = outputs.logits
+                scores = last_logit_pool(logits, inputs['attention_mask'])
+                scores = scores[:, self.yes_loc]
+                all_scores.extend(scores.cpu().float().tolist())
+        else:
+            if prompt is None:
+                prompt = "Given a query A and a passage B, determine whether the passage contains an answer to the query by providing a prediction of either 'Yes' or 'No'."
+            prompt_inputs = self.tokenizer(prompt,
+                                                return_tensors=None,
+                                                add_special_tokens=False)['input_ids']
+            sep = "\n"
+            sep_inputs = self.tokenizer(sep,
+                                             return_tensors=None,
+                                             add_special_tokens=False)['input_ids']
+            encode_max_length = max_length + len(sep_inputs) + len(prompt_inputs)
+            for batch_start in trange(0, len(sentences_sorted), batch_size):
+                batch_sentences = sentences_sorted[batch_start:batch_start + batch_size]
+                batch_sentences = [(f'A: {q}', f'B: {p}') for q,p in batch_sentences]
+                queries = [s[0] for s in batch_sentences]
+                passages = [s[1] for s in batch_sentences]
+                queries_inputs = self.tokenizer(queries,
+                                                return_tensors=None,
+                                                add_special_tokens=False,
+                                                max_length=max_length * 3 // 4,
+                                                truncation=True)
+                passages_inputs = self.tokenizer(passages,
+                                                 return_tensors=None,
+                                                 add_special_tokens=False,
+                                                 max_length=max_length,
+                                                 truncation=True)
+
+                batch_inputs = []
+                for query_inputs, passage_inputs in zip(queries_inputs['input_ids'], passages_inputs['input_ids']):
+                    item = self.tokenizer.prepare_for_model(
+                        [self.tokenizer.bos_token_id] + query_inputs,
+                        sep_inputs + passage_inputs,
+                        truncation='only_second',
+                        max_length=encode_max_length,
+                        padding=False,
+                        return_attention_mask=False,
+                        return_token_type_ids=False,
+                        add_special_tokens=False
+                    )
+                    item['input_ids'] = item['input_ids'] + sep_inputs + prompt_inputs
+                    item['attention_mask'] = [1] * len(item['input_ids'])
+                    item.pop('token_type_ids') if 'token_type_ids' in item.keys() else None
+                    if 'position_ids' in item.keys():
+                        item['position_ids'] = list(range(len(item['input_ids'])))
+                    batch_inputs.append(item)
+
+                collater_instance = collater(self.tokenizer, max_length)
+                batch_inputs = collater_instance(
+                    [{'input_ids': item['input_ids'], 'attention_mask': item['attention_mask']} for item in
+                     batch_inputs])
+
+                batch_inputs = {key: val.to(self.device) for key, val in batch_inputs.items()}
+
+                outputs = self.model(**batch_inputs, output_hidden_states=True)
+                logits = outputs.logits
+                scores = last_logit_pool(logits, batch_inputs['attention_mask'])
+                scores = scores[:, self.yes_loc]
+                all_scores.extend(scores.cpu().float().tolist())
 
         all_scores = [all_scores[idx] for idx in np.argsort(length_sorted_idx)]
 
         if normalize:
             all_scores = [sigmoid(score) for score in all_scores]
 
         if len(all_scores) == 1:
@@ -300,22 +383,23 @@
         elif not hasattr(text, '__len__'):  # Object has no len() method
             return 1
         elif len(text) == 0 or isinstance(text[0], int):  # Empty string or list of ints
             return len(text)
         else:
             return sum([len(t) for t in text])  # Sum of length of individual strings
 
+
 class LayerWiseFlagLLMReranker:
     def __init__(
             self,
             model_name_or_path: str = None,
             use_fp16: bool = False,
             use_bf16: bool = False,
             cache_dir: str = None,
-            device: int = 0
+            device: Union[str, int] = None
     ) -> None:
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path,
                                                        cache_dir=cache_dir,
                                                        trust_remote_code=True)
 
         if use_bf16 is False and use_fp16 is False:
             warnings.warn("Due to model constraints, `use_bf16` and `use_fp16` cannot both be `False`. Here, `use_fp16` is set to `True` by default.", UserWarning)
@@ -325,68 +409,150 @@
                                                           cache_dir=cache_dir,
                                                           trust_remote_code=True,
                                                           torch_dtype=torch.bfloat16 if use_bf16 else torch.float32)
 
         self.model_name_or_path = model_name_or_path
         self.cache_dir = cache_dir
 
-        if torch.cuda.is_available():
-            torch.cuda.set_device(device)
-            self.device = torch.device('cuda')
-        elif torch.backends.mps.is_available():
-            self.device = torch.device('mps')
+        if device and isinstance(device, str):
+            if device == 'cpu':
+                warnings.warn('The LLM-based layer-wise reranker does not support CPU; it has been set to CUDA.')
+                device = 'cuda'
+            self.device = torch.device(device)
         else:
-            self.device = torch.device('cpu')
-            use_fp16 = False
+            device = 0 if device is None else device
+            if torch.cuda.is_available():
+                torch.cuda.set_device(device)
+                self.device = torch.device("cuda")
+            elif torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            elif is_torch_npu_available():
+                self.device = torch.device("npu")
+            else:
+                self.device = torch.device("cpu")
+                use_fp16 = False
+
         if use_fp16 and use_bf16 is False:
             self.model.half()
 
         self.model = self.model.to(self.device)
 
         self.model.eval()
 
         self.yes_loc = self.tokenizer('Yes', add_special_tokens=False)['input_ids'][0]
 
     @torch.no_grad()
     def compute_score(self, sentence_pairs: Union[List[Tuple[str, str]], Tuple[str, str]], batch_size: int = 16,
                       max_length: int = 512, cutoff_layers: List[int] = None, prompt: str = None,
-                      normalize: bool = False) -> Union[float, List[float], List[List[float]]]:
+                      normalize: bool = False, use_dataloader: bool = True,
+                      num_workers: int = None) -> Union[float, List[float], List[List[float]]]:
         assert isinstance(sentence_pairs, list)
         if isinstance(sentence_pairs[0], str):
             sentence_pairs = [sentence_pairs]
 
         length_sorted_idx = np.argsort([-self._text_length(q) - self._text_length(p) for q, p in sentence_pairs])
         sentences_sorted = [sentence_pairs[idx] for idx in length_sorted_idx]
 
-        dataset = DatasetForReranker(sentences_sorted,
-                                     self.model_name_or_path,
-                                     max_length,
-                                     cache_dir=self.cache_dir,
-                                     prompt=prompt)
-        dataloader = DataLoader(dataset, shuffle=False, batch_size=batch_size, drop_last=False,
-                                num_workers=min(batch_size, 16),
-                                collate_fn=collater(self.tokenizer, max_length))
+        dataset, dataloader = None, None
+        if use_dataloader:
+            if num_workers is None:
+                num_workers = min(batch_size, 16)
+            dataset = DatasetForReranker(sentences_sorted,
+                                         self.model_name_or_path,
+                                         max_length,
+                                         cache_dir=self.cache_dir,
+                                         prompt=prompt)
+            dataloader = DataLoader(dataset, shuffle=False, batch_size=batch_size, drop_last=False,
+                                    num_workers=num_workers,
+                                    collate_fn=collater(self.tokenizer, max_length))
 
         all_scores = []
-        for inputs in tqdm(dataloader):
-            inputs = inputs.to(self.device)
+        if dataloader is not None:
+            for inputs in tqdm(dataloader):
+                inputs = inputs.to(self.device)
+
+                outputs = self.model(**inputs, output_hidden_states=True, cutoff_layers=cutoff_layers)
+                all_logits = outputs.logits
+                tmp_all_scores = []
+                for logits in all_logits:
+                    scores = last_logit_pool_layerwise(logits, inputs['attention_mask'])
+                    tmp_all_scores.append(scores.contiguous())
+
+                if len(all_scores) == 0:
+                    for _ in range(len(tmp_all_scores)):
+                        all_scores.append([])
 
-            outputs = self.model(**inputs, output_hidden_states=True, cutoff_layers=cutoff_layers)
-            all_logits = outputs.logits
-            tmp_all_scores = []
-            for logits in all_logits:
-                scores = last_logit_pool_layerwise(logits, inputs['attention_mask'])
-                tmp_all_scores.append(scores.contiguous())
-
-            if len(all_scores) == 0:
-                for _ in range(len(tmp_all_scores)):
-                    all_scores.append([])
+                for i in range(len(tmp_all_scores)):
+                    all_scores[i].extend(tmp_all_scores[i].cpu().float().tolist())
+        else:
+            if prompt is None:
+                prompt = "Given a query A and a passage B, determine whether the passage contains an answer to the query by providing a prediction of either 'Yes' or 'No'."
+            prompt_inputs = self.tokenizer(prompt,
+                                                return_tensors=None,
+                                                add_special_tokens=False)['input_ids']
+            sep = "\n"
+            sep_inputs = self.tokenizer(sep,
+                                             return_tensors=None,
+                                             add_special_tokens=False)['input_ids']
+            encode_max_length = max_length + len(sep_inputs) + len(prompt_inputs)
+            for batch_start in trange(0, len(sentences_sorted), batch_size):
+                batch_sentences = sentences_sorted[batch_start:batch_start + batch_size]
+                batch_sentences = [(f'A: {q}', f'B: {p}') for q, p in batch_sentences]
+                queries = [s[0] for s in batch_sentences]
+                passages = [s[1] for s in batch_sentences]
+                queries_inputs = self.tokenizer(queries,
+                                                return_tensors=None,
+                                                add_special_tokens=False,
+                                                max_length=max_length * 3 // 4,
+                                                truncation=True)
+                passages_inputs = self.tokenizer(passages,
+                                                 return_tensors=None,
+                                                 add_special_tokens=False,
+                                                 max_length=max_length,
+                                                 truncation=True)
+
+                batch_inputs = []
+                for query_inputs, passage_inputs in zip(queries_inputs['input_ids'], passages_inputs['input_ids']):
+                    item = self.tokenizer.prepare_for_model(
+                        [self.tokenizer.bos_token_id] + query_inputs,
+                        sep_inputs + passage_inputs,
+                        truncation='only_second',
+                        max_length=encode_max_length,
+                        padding=False,
+                        return_attention_mask=False,
+                        return_token_type_ids=False,
+                        add_special_tokens=False
+                    )
+                    item['input_ids'] = item['input_ids'] + sep_inputs + prompt_inputs
+                    item['attention_mask'] = [1] * len(item['input_ids'])
+                    item.pop('token_type_ids') if 'token_type_ids' in item.keys() else None
+                    if 'position_ids' in item.keys():
+                        item['position_ids'] = list(range(len(item['input_ids'])))
+                    batch_inputs.append(item)
+
+                collater_instance = collater(self.tokenizer, max_length)
+                batch_inputs = collater_instance(
+                    [{'input_ids': item['input_ids'], 'attention_mask': item['attention_mask']} for item in
+                     batch_inputs])
+
+                batch_inputs = {key: val.to(self.device) for key, val in batch_inputs.items()}
+
+                outputs = self.model(**batch_inputs, output_hidden_states=True, cutoff_layers=cutoff_layers)
+                all_logits = outputs.logits
+                tmp_all_scores = []
+                for logits in all_logits:
+                    scores = last_logit_pool_layerwise(logits, batch_inputs['attention_mask'])
+                    tmp_all_scores.append(scores.contiguous())
+
+                if len(all_scores) == 0:
+                    for _ in range(len(tmp_all_scores)):
+                        all_scores.append([])
 
-            for i in range(len(tmp_all_scores)):
-                all_scores[i].extend(tmp_all_scores[i].cpu().float().tolist())
+                for i in range(len(tmp_all_scores)):
+                    all_scores[i].extend(tmp_all_scores[i].cpu().float().tolist())
 
         for i in range(len(all_scores)):
             all_scores[i] = [all_scores[i][idx] for idx in np.argsort(length_sorted_idx)]
             if normalize:
                 all_scores[i] = [sigmoid(score) for score in all_scores[i]]
 
         if len(all_scores) == 1:
@@ -407,8 +573,8 @@
         if isinstance(text, dict):  # {key: value} case
             return len(next(iter(text.values())))
         elif not hasattr(text, '__len__'):  # Object has no len() method
             return 1
         elif len(text) == 0 or isinstance(text[0], int):  # Empty string or list of ints
             return len(text)
         else:
-            return sum([len(t) for t in text])  # Sum of length of individual strings
+            return sum([len(t) for t in text])  # Sum of length of individual strings
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/arguments.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import sys
+from typing import List
 
 import math
 import os.path
 import random
 from dataclasses import dataclass
 
 import datasets
@@ -56,15 +57,15 @@
     def __len__(self):
         return self.total_len
 
     def is_chinese(self, text):
         chinese_pattern = re.compile('[\u4e00-\u9fa5]')
         return bool(chinese_pattern.search(text))
 
-    def __getitem__(self, item) -> list[BatchEncoding]:
+    def __getitem__(self, item) -> List[BatchEncoding]:
         query = self.dataset[item]['query']
 
         passages = []
         pos = random.choice(self.dataset[item]['pos'])
         passages.append(pos)
         if len(self.dataset[item]['neg']) < self.args.train_group_size - 1:
             num = math.ceil((self.args.train_group_size - 1) / len(self.dataset[item]['neg']))
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/load_model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/load_model.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,8 +81,10 @@
         state_dict = type(state_dict)(
             {k: v.clone().cpu()
              for k,
              v in state_dict.items()})
         self.model.save_pretrained(output_dir, state_dict=state_dict)
 
     def save_pretrained(self, **kwargs):
+        self.tokenizer.save_pretrained(**kwargs)
         return self.model.save_pretrained(**kwargs)
+
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/run.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_instruction/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_instruction/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,29 +67,34 @@
     )
     cache_dir: str = field(
         default="tmp", metadata={"help": "the cache of the model"}
     )
     from_peft: str = field(
         default=None
     )
-    lora_extra_parameters: str = field(
+    lora_extra_parameters: Optional[List[str]] = field(
         default=None
     )
     start_layer: int = field(
         default=8,
         metadata={"help": "which layer to start to compute score"}
     )
     head_multi: bool = field(
         default=False,
         metadata={"help": "use one / multi classifier"}
     )
     head_type: str = field(
         default='simple',
         metadata={"help": "the type of the classifier"}
     )
+    finetune_type: str = field(
+        default='from_raw_model'  # should be one of ['from_raw_model', 'from_finetuned_model']
+        # from_raw_model -- openbmb/MiniCPM-2B-dpo-bf16
+        # from_finetuned_model -- BAAI/bge-reranker-v2-minicpm-layerwise
+    )
 
 
 @dataclass
 class DataArguments:
     train_data: str = field(
         default='toy_finetune_data.jsonl', metadata={"help": "Path to train data"}
     )
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/configuration_minicpm_reranker.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/configuration_minicpm_reranker.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import sys
+from typing import List
 
 import math
 import os.path
 import random
 from dataclasses import dataclass
 
 import datasets
@@ -52,15 +53,15 @@
                                          add_special_tokens=False)['input_ids']
 
         self.max_length = self.args.query_max_len + self.args.passage_max_len
 
     def __len__(self):
         return self.total_len
 
-    def __getitem__(self, item) -> list[BatchEncoding]:
+    def __getitem__(self, item) -> List[BatchEncoding]:
         query = self.dataset[item]['query']
 
         passages = []
         pos = random.choice(self.dataset[item]['pos'])
         passages.append(pos)
         if len(self.dataset[item]['neg']) < self.args.train_group_size - 1:
             num = math.ceil((self.args.train_group_size - 1) / len(self.dataset[item]['neg']))
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/load_model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/load_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,83 +7,100 @@
 
 def get_model(model_args, training_args, only_for_one_logit: int = None):
     config = AutoConfig.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=model_args.cache_dir,
         trust_remote_code=True,
     )
-    config.use_cache = False
-    config.start_layer = config.num_hidden_layers
-    config.head_multi = False
-    config.head_type = 'raw'
-
-    model = LayerWiseMiniCPMForCausalLM.from_pretrained(
-        model_args.model_name_or_path,
-        torch_dtype=torch.float16 if training_args.fp16 else torch.bfloat16,
-        use_flash_attention_2=True if model_args.use_flash_attn else False,
-        cache_dir=model_args.cache_dir,
-        from_tf=bool(".ckpt" in model_args.model_name_or_path),
-        config=config,
-        trust_remote_code=True,
-    )
-
-
-    config.start_layer = model_args.start_layer
-    config.head_multi = model_args.head_multi
-    config.head_type = model_args.head_type
-    model.config = config
-
-    if model.config.head_type == 'complex':
-        if model.config.head_multi == True:
-            lm_head = nn.ModuleList([LayerWiseHead(
-                model.config.hidden_size, model.config.vocab_size) for _ in range(
-                model.config.start_layer,
-                model.config.num_hidden_layers + 1)])
-            for i in range(len(lm_head)):
-                lm_head[i].linear_head.load_state_dict(model.lm_head.state_dict())
-            model.set_output_embeddings(lm_head)
+    if model_args.finetune_type == 'from_raw_model':
+        config.use_cache = False
+        config.start_layer = config.num_hidden_layers
+        config.head_multi = False
+        config.head_type = 'raw'
+
+        model = LayerWiseMiniCPMForCausalLM.from_pretrained(
+            model_args.model_name_or_path,
+            torch_dtype=torch.float16 if training_args.fp16 else torch.bfloat16,
+            use_flash_attention_2=True if model_args.use_flash_attn else False,
+            cache_dir=model_args.cache_dir,
+            from_tf=bool(".ckpt" in model_args.model_name_or_path),
+            config=config,
+            trust_remote_code=True,
+        )
+
+        config.start_layer = model_args.start_layer
+        config.head_multi = model_args.head_multi
+        config.head_type = model_args.head_type
+        model.config = config
+
+        if model.config.head_type == 'complex':
+            if model.config.head_multi == True:
+                lm_head = nn.ModuleList([LayerWiseHead(
+                    model.config.hidden_size, model.config.vocab_size) for _ in range(
+                    model.config.start_layer,
+                    model.config.num_hidden_layers + 1)])
+                for i in range(len(lm_head)):
+                    lm_head[i].linear_head.load_state_dict(model.lm_head.state_dict())
+                model.set_output_embeddings(lm_head)
+            else:
+                lm_head = LayerWiseHead(model.config.hidden_size, 1)
+                state_dict_back = model.lm_head.state_dict()
+                state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
+                lm_head.linear_head.load_state_dict(state_dict_back)
+                model.set_output_embeddings(lm_head)
         else:
-            lm_head = LayerWiseHead(model.config.hidden_size, 1)
-            state_dict_back = model.lm_head.state_dict()
-            state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
-            lm_head.linear_head.load_state_dict(state_dict_back)
-            model.set_output_embeddings(lm_head)
+            if only_for_one_logit is None:
+                raise ValueError('`only for one logit` cannot be None.')
+            if model.config.head_multi == True:
+                lm_head = nn.ModuleList([LayerWiseHead(
+                    model.config.hidden_size, 1) for _ in range(
+                    model.config.start_layer,
+                    model.config.num_hidden_layers + 1)])
+                state_dict_back = model.lm_head.state_dict()
+                state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
+                for i in range(len(lm_head)):
+                    lm_head[i].linear_head.load_state_dict(state_dict_back)
+                model.set_output_embeddings(lm_head)
+            else:
+                lm_head = LayerWiseHead(model.config.hidden_size, 1)
+                state_dict_back = model.lm_head.state_dict()
+                state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
+                lm_head.linear_head.load_state_dict(state_dict_back)
+                model.set_output_embeddings(lm_head)
+        lora_extra_parameters = model_args.lora_extra_parameters
+        target_modules = model_args.target_modules
     else:
-        if only_for_one_logit is None:
-            raise ValueError('`only for one logit` cannot be None.')
-        if model.config.head_multi == True:
-            lm_head = nn.ModuleList([LayerWiseHead(
-                model.config.hidden_size, 1) for _ in range(
-                model.config.start_layer,
-                model.config.num_hidden_layers + 1)])
-            state_dict_back = model.lm_head.state_dict()
-            state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
-            for i in range(len(lm_head)):
-                lm_head[i].linear_head.load_state_dict(state_dict_back)
-            model.set_output_embeddings(lm_head)
-        else:
-            lm_head = LayerWiseHead(model.config.hidden_size, 1)
-            state_dict_back = model.lm_head.state_dict()
-            state_dict_back['weight'] = state_dict_back['weight'][only_for_one_logit: only_for_one_logit + 1, :]
-            lm_head.linear_head.load_state_dict(state_dict_back)
-            model.set_output_embeddings(lm_head)
+        config.use_cache = False
+
+        model = LayerWiseMiniCPMForCausalLM.from_pretrained(
+            model_args.model_name_or_path,
+            torch_dtype=torch.float16 if training_args.fp16 else torch.bfloat16,
+            use_flash_attention_2=True if model_args.use_flash_attn else False,
+            cache_dir=model_args.cache_dir,
+            from_tf=bool(".ckpt" in model_args.model_name_or_path),
+            config=config,
+            trust_remote_code=True,
+        )
+        target_modules = model_args.target_modules
+        target_modules.extend(model_args.lora_extra_parameters)
+        lora_extra_parameters = None
 
     if model_args.from_peft is not None:
         model = PeftModel.from_pretrained(model, model_args.from_peft, is_trainable=True)
         model.print_trainable_parameters()
     else:
         if model_args.use_lora:
             peft_config = LoraConfig(
                 task_type=TaskType.CAUSAL_LM,
                 inference_mode=False,
                 r=model_args.lora_rank,
-                target_modules=model_args.target_modules,
+                target_modules=target_modules,
                 lora_alpha=model_args.lora_alpha,
                 lora_dropout=model_args.lora_dropout,
-                modules_to_save=model_args.lora_extra_parameters,
+                modules_to_save=lora_extra_parameters,
             )
             print(peft_config)
             model = get_peft_model(model, peft_config)
             model.print_trainable_parameters()
 
     print(model)
     return model
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,9 +102,12 @@
         state_dict = type(state_dict)(
             {k: v.clone().cpu()
              for k,
              v in state_dict.items()})
         self.model.save_pretrained(output_dir, state_dict=state_dict)
 
     def save_pretrained(self, **kwargs):
+        self.tokenizer.save_pretrained(**kwargs)
         self.model.config.save_pretrained(**kwargs)
         return self.model.save_pretrained(**kwargs)
+
+
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling_minicpm_reranker.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling_minicpm_reranker.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,11 +122,12 @@
     if not model_args.use_lora:
         checkpoint_dir = os.path.join(training_args.output_dir, "checkpoint-final")
         trainer.deepspeed.save_checkpoint(checkpoint_dir)
     # For convenience, we also re-save the tokenizer to the same directory,
     # so that you can share your model easily on huggingface.co/models =)
     if trainer.is_world_process_zero():
         tokenizer.save_pretrained(training_args.output_dir)
+        model.model.config.save_pretrained(training_args.output_dir)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/llm_reranker/finetune_for_layerwise/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/llm_reranker/finetune_for_layerwise/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/reranker/arguments.py` & `FlagEmbedding-1.2.9/FlagEmbedding/reranker/arguments.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/reranker/data.py` & `FlagEmbedding-1.2.9/FlagEmbedding/reranker/data.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/reranker/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/reranker/modeling.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/reranker/run.py` & `FlagEmbedding-1.2.9/FlagEmbedding/reranker/run.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/reranker/trainer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/reranker/trainer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/__init__.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/eva_vit_model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/eva_vit_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 else:
     from torch.utils.checkpoint import checkpoint
 
 try:
     import xformers.ops as xops
 except ImportError:
     xops = None
-    print("Please 'pip install xformers'")
+    # print("Please 'pip install xformers'")
 
 
 class DropPath(nn.Module):
     """Drop paths (Stochastic Depth) per sample  (when applied in main path of residual blocks).
     """
     def __init__(self, drop_prob=None):
         super(DropPath, self).__init__()
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/factory.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/factory.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/hf_configs.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/hf_model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/loss.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/loss.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 FusedLayerNorm = LayerNorm
     # print("Please 'pip install apex'")
 
 try:
     import xformers.ops as xops
 except ImportError:
     xops = None
-    print("Please 'pip install xformers'")
+    # print("Please 'pip install xformers'")
 
 @dataclass
 class CLIPVisionCfg:
     layers: Union[Tuple[int, int, int, int], int] = 12
     width: int = 768
     head_width: int = 64
     mlp_ratio: float = 4.0
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/modified_resnet.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/modified_resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import OrderedDict
 
 import torch
 from torch import nn
 from torch.nn import functional as F
 
-from eva_clip.utils import freeze_batch_norm_2d
+from FlagEmbedding.visual.eva_clip.utils import freeze_batch_norm_2d
 
 
 class Bottleneck(nn.Module):
     expansion = 4
 
     def __init__(self, inplanes, planes, stride=1):
         super().__init__()
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/openai.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/openai.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/pretrained.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/rope.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/rope.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/timm_model.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/tokenizer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/transform.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/transform.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/transformer.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 else:
     from torch.utils.checkpoint import checkpoint
 
 try:
     import xformers.ops as xops
 except ImportError:
     xops = None
-    print("Please 'pip install xformers'")
+    # print("Please 'pip install xformers'")
 
 class LayerNormFp32(nn.LayerNorm):
     """Subclass torch's LayerNorm to handle fp16 (by casting to float32 and back)."""
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def forward(self, x: torch.Tensor):
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/eva_clip/utils.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/eva_clip/utils.py`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding/visual/modeling.py` & `FlagEmbedding-1.2.9/FlagEmbedding/visual/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 import torch.distributed as dist
 from torch import nn, Tensor
 from transformers import AutoModel, AutoTokenizer, AutoConfig
 from transformers.file_utils import ModelOutput
 
 
-from eva_clip import create_eva_vision_and_transforms
+from FlagEmbedding.visual.eva_clip import create_eva_vision_and_transforms
 from PIL import Image
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class EncoderOutput(ModelOutput):
@@ -297,21 +297,21 @@
         img_reps = self.encode_mm(images, prompts)
         return img_reps
     
     def forward(self, mm_it_query=None, image_candidate=None, text_candidate=None, text_query=None, mm_it_candidate=None, task_type=None):
         ### for stage-2 training
         if task_type == "edit_image":
             mm_query_reps = self.encode_mm(mm_it_query[0], mm_it_query[1])
-            image_candi_reps = self.encode_image(image_candidate) #输入的是token序列
+            image_candi_reps = self.encode_image(image_candidate)
             query_reps = mm_query_reps
             candi_reps = image_candi_reps
                 
         elif task_type == "t2it":
             text_query_reps = self.encode_text(text_query)
-            mmit_candi_reps = self.encode_mm(mm_it_candidate[0], mm_it_candidate[1]) #输入的是token序列
+            mmit_candi_reps = self.encode_mm(mm_it_candidate[0], mm_it_candidate[1])
             query_reps = text_query_reps
             candi_reps = mmit_candi_reps
             
         
         if self.training:
             if self.negatives_cross_device:
                 query_reps = self._dist_gather_tensor(query_reps)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding.egg-info/PKG-INFO` & `FlagEmbedding-1.2.9/FlagEmbedding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlagEmbedding
-Version: 1.2.8
+Version: 1.2.9
 Summary: FlagEmbedding
 Home-page: https://github.com/FlagOpen/FlagEmbedding
 Author-email: 2906698981@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">FlagEmbedding</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FlagEmbedding Version: 1.2.8 Summary: FlagEmbedding
+Metadata-Version: 2.1 Name: FlagEmbedding Version: 1.2.9 Summary: FlagEmbedding
 Home-page: https://github.com/FlagOpen/FlagEmbedding Author-email:
 2906698981@qq.com Description-Content-Type: text/markdown License-File: LICENSE
                           ************ FFllaaggEEmmbbeeddddiinngg ************
                         _[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_]_[_B_u_i_l_d_]
     ****** _NN_ee_ww_ss || _PP_rr_oo_jj_ee_cc_tt_ss || _MM_oo_dd_ee_ll_ _LL_ii_ss_tt || _CC_oo_nn_tt_rr_ii_bb_uu_tt_oo_rr || _CC_ii_tt_aa_tt_ii_oo_nn || _LL_ii_cc_ee_nn_ss_ee ******
 [English](README.md) | [ä¸­æ](https://github.com/FlagOpen/FlagEmbedding/blob/
 master/README_zh.md) FlagEmbedding focuses on retrieval-augmented LLMs,
```

### Comparing `FlagEmbedding-1.2.8/FlagEmbedding.egg-info/SOURCES.txt` & `FlagEmbedding-1.2.9/FlagEmbedding.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 FlagEmbedding/llm_reranker/finetune_for_layerwise/configuration_minicpm_reranker.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/data.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/load_model.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/modeling_minicpm_reranker.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/run.py
 FlagEmbedding/llm_reranker/finetune_for_layerwise/trainer.py
+FlagEmbedding/llm_reranker/merge/__init__.py
+FlagEmbedding/llm_reranker/merge/configuration_minicpm_reranker.py
+FlagEmbedding/llm_reranker/merge/merge_base_model.py
+FlagEmbedding/llm_reranker/merge/merge_layerwise_model_from_finetuned_model.py
+FlagEmbedding/llm_reranker/merge/merge_layerwise_model_from_raw_model.py
+FlagEmbedding/llm_reranker/merge/modeling_minicpm_reranker.py
 FlagEmbedding/reranker/__init__.py
 FlagEmbedding/reranker/arguments.py
 FlagEmbedding/reranker/data.py
 FlagEmbedding/reranker/modeling.py
 FlagEmbedding/reranker/run.py
 FlagEmbedding/reranker/trainer.py
 FlagEmbedding/visual/__init__.py
```

### Comparing `FlagEmbedding-1.2.8/LICENSE` & `FlagEmbedding-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/PKG-INFO` & `FlagEmbedding-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlagEmbedding
-Version: 1.2.8
+Version: 1.2.9
 Summary: FlagEmbedding
 Home-page: https://github.com/FlagOpen/FlagEmbedding
 Author-email: 2906698981@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">FlagEmbedding</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FlagEmbedding Version: 1.2.8 Summary: FlagEmbedding
+Metadata-Version: 2.1 Name: FlagEmbedding Version: 1.2.9 Summary: FlagEmbedding
 Home-page: https://github.com/FlagOpen/FlagEmbedding Author-email:
 2906698981@qq.com Description-Content-Type: text/markdown License-File: LICENSE
                           ************ FFllaaggEEmmbbeeddddiinngg ************
                         _[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_]_[_B_u_i_l_d_]
     ****** _NN_ee_ww_ss || _PP_rr_oo_jj_ee_cc_tt_ss || _MM_oo_dd_ee_ll_ _LL_ii_ss_tt || _CC_oo_nn_tt_rr_ii_bb_uu_tt_oo_rr || _CC_ii_tt_aa_tt_ii_oo_nn || _LL_ii_cc_ee_nn_ss_ee ******
 [English](README.md) | [ä¸­æ](https://github.com/FlagOpen/FlagEmbedding/blob/
 master/README_zh.md) FlagEmbedding focuses on retrieval-augmented LLMs,
```

### Comparing `FlagEmbedding-1.2.8/README.md` & `FlagEmbedding-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `FlagEmbedding-1.2.8/setup.py` & `FlagEmbedding-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", mode="r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name='FlagEmbedding',
-    version='1.2.8',
+    version='1.2.9',
     description='FlagEmbedding',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='2906698981@qq.com',
     url='https://github.com/FlagOpen/FlagEmbedding',
     packages=find_packages(),
     install_requires=[
```

