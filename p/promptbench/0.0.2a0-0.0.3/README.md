# Comparing `tmp/promptbench-0.0.2a0.tar.gz` & `tmp/promptbench-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptbench-0.0.2a0.tar", last modified: Mon Nov 27 14:48:36 2023, max compression
+gzip compressed data, was "promptbench-0.0.3.tar", last modified: Wed May 22 23:05:13 2024, max compression
```

## Comparing `promptbench-0.0.2a0.tar` & `promptbench-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.621852 promptbench-0.0.2a0/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1141 2023-11-27 14:23:20.000000 promptbench-0.0.2a0/LICENSE
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    19456 2023-11-27 14:48:36.621852 promptbench-0.0.2a0/PKG-INFO
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    18883 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/README.md
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      276 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    18192 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/config.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/dataload/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)       46 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dataload/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     2439 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dataload/dataload.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    15585 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dataload/dataset.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/dyval/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      233 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dyval/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     9051 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dyval/dyval_dataset.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    87176 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/dyval/dyval_utils.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/metrics/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)       96 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/metrics/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     4340 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/metrics/eval.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/models/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     6458 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/models/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    11663 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/models/models.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/prompt_attack/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     2050 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    31660 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/attack.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    15933 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/goal_function.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      819 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/label_constraint.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      571 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/search.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     2283 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_attack/transformations.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/prompt_engineering/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     2677 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     2058 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/ask_me_anything.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     3642 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/chain_of_thought.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      607 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/emotion_prompt.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1673 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/expert_prompting.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1541 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/generated_knowledge.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1490 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompt_engineering/least_to_most.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/prompts/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)       26 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    14686 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/method_oriented.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     8417 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/prompt.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    29239 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/role_oriented.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)   215737 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/semantic_atk_prompts.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    24356 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/prompts/task_oriented.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench/utils/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      189 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/utils/__init__.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     4410 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/utils/dataprocess.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)      655 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/utils/defense.py
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     4899 2023-11-27 14:23:26.000000 promptbench-0.0.2a0/promptbench/utils/visualize.py
-drwxrwxr-x   0 haoc      (1001) haoc      (1001)        0 2023-11-27 14:48:36.617851 promptbench-0.0.2a0/promptbench.egg-info/
--rw-rw-r--   0 haoc      (1001) haoc      (1001)    19456 2023-11-27 14:48:36.000000 promptbench-0.0.2a0/promptbench.egg-info/PKG-INFO
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1494 2023-11-27 14:48:36.000000 promptbench-0.0.2a0/promptbench.egg-info/SOURCES.txt
--rw-rw-r--   0 haoc      (1001) haoc      (1001)        1 2023-11-27 14:48:36.000000 promptbench-0.0.2a0/promptbench.egg-info/dependency_links.txt
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1720 2023-11-27 14:48:36.000000 promptbench-0.0.2a0/promptbench.egg-info/requires.txt
--rw-rw-r--   0 haoc      (1001) haoc      (1001)       12 2023-11-27 14:48:36.000000 promptbench-0.0.2a0/promptbench.egg-info/top_level.txt
--rw-rw-r--   0 haoc      (1001) haoc      (1001)       38 2023-11-27 14:48:36.621852 promptbench-0.0.2a0/setup.cfg
--rw-rw-r--   0 haoc      (1001) haoc      (1001)     1650 2023-11-27 14:48:31.000000 promptbench-0.0.2a0/setup.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.341808 promptbench-0.0.3/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     1141 2024-05-22 22:50:18.000000 promptbench-0.0.3/LICENSE
+-rw-r--r--   0 haoc      (1001) haoc      (1002)    15055 2024-05-22 23:05:13.341808 promptbench-0.0.3/PKG-INFO
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    13880 2024-05-22 22:50:18.000000 promptbench-0.0.3/README.md
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      449 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    18192 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/config.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/dataload/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      120 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dataload/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     3950 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dataload/dataload.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    44865 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dataload/dataset.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/dyval/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      307 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dyval/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     9125 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dyval/dyval_dataset.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    86934 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/dyval/dyval_utils.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/metrics/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)       96 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/metrics/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     5291 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/metrics/eval.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/models/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    14441 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/models/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    38489 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/models/models.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench/prompt_attack/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     2124 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    32803 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/attack.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    11173 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/goal_function.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     1078 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/label_constraint.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      571 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/search.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     2283 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_attack/transformations.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.341808 promptbench-0.0.3/promptbench/prompt_engineering/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     3232 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     1543 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/base.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     4499 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/chain_of_thought.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     2187 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/emotion_prompt.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     2649 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/expert_prompting.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     3206 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/generated_knowledge.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     2603 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompt_engineering/least_to_most.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.341808 promptbench-0.0.3/promptbench/prompts/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      100 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    23942 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/method_oriented.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     8491 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/prompt.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    29239 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/role_oriented.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)   215737 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/semantic_atk_prompts.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)    24356 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/prompts/task_oriented.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.341808 promptbench-0.0.3/promptbench/utils/
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      189 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/utils/__init__.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     4410 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/utils/dataprocess.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      655 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/utils/defense.py
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     4900 2024-05-22 22:50:18.000000 promptbench-0.0.3/promptbench/utils/visualize.py
+drwxrwxr-x   0 haoc      (1001) haoc      (1002)        0 2024-05-22 23:05:13.337808 promptbench-0.0.3/promptbench.egg-info/
+-rw-r--r--   0 haoc      (1001) haoc      (1002)    15055 2024-05-22 23:05:13.000000 promptbench-0.0.3/promptbench.egg-info/PKG-INFO
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     1483 2024-05-22 23:05:13.000000 promptbench-0.0.3/promptbench.egg-info/SOURCES.txt
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)        1 2024-05-22 23:05:13.000000 promptbench-0.0.3/promptbench.egg-info/dependency_links.txt
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)      334 2024-05-22 23:05:13.000000 promptbench-0.0.3/promptbench.egg-info/requires.txt
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)       12 2024-05-22 23:05:13.000000 promptbench-0.0.3/promptbench.egg-info/top_level.txt
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)       38 2024-05-22 23:05:13.341808 promptbench-0.0.3/setup.cfg
+-rw-rw-r--   0 haoc      (1001) haoc      (1002)     1650 2024-05-22 22:50:51.000000 promptbench-0.0.3/setup.py
```

### Comparing `promptbench-0.0.2a0/LICENSE` & `promptbench-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/config.py` & `promptbench-0.0.3/promptbench/config.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/dyval/dyval_dataset.py` & `promptbench-0.0.3/promptbench/dyval/dyval_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
+
 from tqdm import tqdm
 from .dyval_utils import process_dyval_training_sample
 
 class DyValDataset:
     """
     A class for creating and managing datasets for various types of Directed Acyclic Graph (DAG) tasks.
```

### Comparing `promptbench-0.0.2a0/promptbench/dyval/dyval_utils.py` & `promptbench-0.0.3/promptbench/dyval/dyval_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
+
 import re
 
 def round_value(val):
     """
     Rounds a numerical value to 8 decimal places.
 
     Parameters:
@@ -13,15 +16,15 @@
     --------
     str
         The rounded value as a string.
     """
     return str(round(float(val), 8))
 
 
-def evaluate(dataset_type, preds, gts):
+def dyval_evaluate(dataset_type, preds, gts):
     """
     Evaluates predictions against ground truths for different dataset types.
 
     Parameters:
     -----------
     dataset_type : str
         The type of dataset (e.g., 'arithmetic', 'max_sum_path').
@@ -122,29 +125,15 @@
             inputs = [prompt.format(input_text) for input_text in input_texts]
                     
         descriptions[order] = inputs
     
     return descriptions
 
 def process_dyval_training_sample(sample, dataset_type):
-    """
-    Processes a single training sample for DyVal training dataset.
-
-    Parameters:
-    -----------
-    sample : dict
-        The sample to be processed.
-    dataset_type : str
-        The type of dataset (e.g., 'arithmetic', 'bool_logic').
 
-    Returns:
-    --------
-    dict
-        The processed sample.
-    """
     prompt = DYVAL_PROMPTS[dataset_type][0]
     for order, input_text in sample["descriptions"].items():
         if dataset_type in ["arithmetic", "bool_logic", "deductive_logic"]:
             var = sample["vars"]
             problem = prompt.format(input_text, var)
         else:
             problem = prompt.format(input_text)
```

### Comparing `promptbench-0.0.2a0/promptbench/metrics/eval.py` & `promptbench-0.0.3/promptbench/metrics/eval.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
-
 class Eval:
     """
     A utility class for computing various evaluation metrics.
 
     This class provides static methods to compute metrics such as classification accuracy, SQuAD V2 F1 score, BLEU score, and math accuracy.
 
-    Attributes:
-    -----------
-    BLEU_NORMALIZATION_FACTOR : int
-        The normalization factor for the BLEU score.
-    SQUAD_V2_NORMALIZATION_FACTOR : int
-        The normalization factor for the SQuAD V2 F1 score.
-
     Methods:
     --------
     compute_cls_accuracy(preds, gts)
         Computes classification accuracy.
     compute_squad_v2_f1(preds, gts, dataset)
         Computes the F1 score for the SQuAD V2 dataset.
     compute_bleu(preds, gts)
         Computes the BLEU score for translation tasks.
     compute_math_accuracy(dataset, preds, gts)
         Computes accuracy for math dataset.
     """
-    BLEU_NORMALIZATION_FACTOR = 100
-    SQUAD_V2_NORMALIZATION_FACTOR = 100
     
     @staticmethod
     def compute_cls_accuracy(preds, gts):
         """
         Computes classification accuracy based on predictions and ground truths.
 
         Parameters:
@@ -86,15 +76,15 @@
             pred = "" if pred == "unanswerable" else pred
             model_output.append({"id": id, "prediction_text": pred, "no_answer_probability": no_ans_prob})
 
         references = [{"answers": data["answers"], "id": data["id"]} for data in dataset]
 
         score = metric.compute(predictions=model_output, references=references)
 
-        return score["f1"] / self.SQUAD_V2_NORMALIZATION_FACTOR
+        return score["f1"]
 
     @staticmethod
     def compute_bleu(preds, gts):
         """
         Computes the BLEU score for translation tasks.
 
         Parameters:
@@ -108,18 +98,18 @@
         --------
         float
             The BLEU score.
         """
         from .bleu.bleu import Bleu
         metric = Bleu()
         results = metric.compute(predictions=preds, references=gts)
-        return results['bleu'] / self.BLEU_NORMALIZATION_FACTOR
+        return results['bleu']
 
     @staticmethod
-    def compute_math_accuracy(self, dataset, preds, gts):
+    def compute_math_accuracy(preds, gts):
         """
         Computes accuracy for the 'math' dataset.
 
         Parameters:
         -----------
         dataset : list
             The dataset containing math data.
@@ -139,7 +129,55 @@
         for pred, gt in zip(preds, gts):
             pred = "True" if pred.lower() == "yes" else ("False" if pred.lower() == "no" else pred)
             gt = str(gt).lower()
             processed_preds.append(pred.lower())
             processed_gts.append(gt)
 
         return sum(a == b for a, b in zip(processed_preds, processed_gts)) / len(processed_gts)
+
+    @staticmethod
+    def compute_vqa_accuracy(preds, gts):
+        """
+        Computes vqa accuracy for the VQAv2 dataset.
+
+        Parameters:
+        -----------
+        preds : list
+            A list of predictions.
+        gts : list
+            A list of answers.
+
+        Returns:
+        --------
+        float
+            The vqa accuracy.
+        """
+        from .vqa.eval_vqa import VQAEval
+        metric = VQAEval(n=3)
+        dict_gts = {i: {"answers": val} for i, val in enumerate(gts)}
+        dict_preds = {i: {"answer": val} for i, val in enumerate(preds)}
+        score = metric.evaluate(dict_gts, dict_preds, list(range(len(preds))))
+        return score
+    
+    @staticmethod
+    def compute_cider(preds, gts):
+        """
+        Computes the CIDEr score for image captioning tasks.
+
+        Parameters:
+        -----------
+        preds : list
+            A list of predictions.
+        gts : list
+            A list of ground truth captions.
+
+        Returns:
+        --------
+        float
+            The CIDEr score.
+        """
+        from .cider.cider import Cider
+        metric = Cider()
+        dict_gts = {i: val for i, val in enumerate(gts)}
+        dict_preds = {i: [val] for i, val in enumerate(preds)}
+        score, _ = metric.compute_score(gts=dict_gts, res=dict_preds)
+        return score
```

### Comparing `promptbench-0.0.2a0/promptbench/prompt_attack/__init__.py` & `promptbench-0.0.3/promptbench/prompt_attack/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
+
 from .attack import *
 
 MNLI_LABEL = ['entailment', 'neutral', 'contradiction',
               'entailment\'', 'neutral\'', 'contradiction\'']
 EQ_LABEL = ['equivalent', 'not_equivalent', 'equivalent\'', 'not_equivalent\'']
 ENTAIL_LABEL = ['entailment', 'not_entailment', 'entailment\'',
                 'not_entailment\'', '0', '1', '0\'', '1\'']
```

### Comparing `promptbench-0.0.2a0/promptbench/prompt_attack/attack.py` & `promptbench-0.0.3/promptbench/prompt_attack/attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+#
+# Source Attribution:
+# The majority of this code is derived from the following sources:
+# - TextAttack GitHub Repository: https://github.com/QData/TextAttack
+# - Reference Paper: Morris, John X., et al. "TextAttack: A Framework for Adversarial Attacks, Data Augmentation, and Adversarial Training in NLP." arXiv preprint arXiv:2005.05909 (2020).
+
 
 
 """
 Attack Class
 """
 
 from collections import OrderedDict
@@ -52,45 +58,56 @@
 )
 
 from .__init__ import LABEL_SET, attack_config
 from .goal_function import AdvPromptGoalFunction
 
 
 class Attack(object):
-    def __init__(self, model, attack_name, dataset, prompt, input_process_func, output_process_func, eval_func, unmodifiable_words=None):
+    def __init__(self, model, attack_name, dataset, prompt, eval_func, unmodifiable_words=None, verbose=True):
+        """
+        model: the model to attack
+        attack_name: the name of the attack, e.g. "textfooler", "textbugger", "deepwordbug", "bertattack", "checklist", "stresstest", "semantic"
+        dataset: the dataset for prompt attack
+        prompt: the prompt to attack
+        eval_func: the evaluation function to evaluate the performance of a prompt, the interface is eval_func(prompt, dataset, model), in this function, you need to implement the logic to get the prediction of the model on the prompt, and evaluate the correctness of the prediction, finally, return the accuracy of the model on the prompt.
+        unmodifiable_words: the words that are not allowed to be attacked
+        verbose: whether to print the attack process
+
+        return: None
+        """
         self.model = model
         self.attack_name = attack_name
         self.dataset = dataset
         self.prompt = prompt
+        self.eval_func = eval_func
         self.goal_function = AdvPromptGoalFunction(self.model, 
-                                                   self.dataset, 
-                                                   input_process_func, 
-                                                   output_process_func, 
+                                                   self.dataset,  
                                                    eval_func, 
                                                    query_budget=attack_config["goal_function"]["query_budget"], 
-                                                   model_wrapper=None)
+                                                   model_wrapper=None,
+                                                   verbose=verbose)
         if unmodifiable_words:
             self.unmodifiable_words = unmodifiable_words
         else:
             print("Using default unmodifiable words.")
             self.unmodifiable_words = LABEL_SET[dataset]
         
         print(f"These words (if they appear in the prompt) are not allowed to be attacked:\n{self.unmodifiable_words}")
-        self.prompt_attack = self._create_attack(attack_name, self.unmodifiable_words, self.goal_function)
+        self.prompt_attack = self._create_attack(attack_name)
 
     @staticmethod
     def attack_list():
         return ["textbugger", "deepwordbug", "textfooler", "bertattack", "checklist", "stresstest", "semantic"]
 
-    def _create_attack(self, attack, unmodifiable_words, goal_function):
+    def _create_attack(self, attack):
         if attack == "semantic":
             return None
         
         from promptbench.prompt_attack.label_constraint import LabelConstraint
-        label_constraint = LabelConstraint(unmodifiable_words)
+        label_constraint = LabelConstraint(self.unmodifiable_words)
         
         if attack == "textfooler":
 
             transformation = WordSwapEmbedding(max_candidates=attack_config["textfooler"]["max_candidates"])
             stopwords = set(
                 ["a", "about", "above", "across", "after", "afterwards", "again", "against", "ain", "all", "almost", "alone", "along", "already", "also", "although", "am", "among", "amongst", "an", "and", "another", "any", "anyhow", "anyone", "anything", "anyway", "anywhere", "are", "aren", "aren't", "around", "as", "at", "back", "been", "before", "beforehand", "behind", "being", "below", "beside", "besides", "between", "beyond", "both", "but", "by", "can", "cannot", "could", "couldn", "couldn't", "d", "didn", "didn't", "doesn", "doesn't", "don", "don't", "down", "due", "during", "either", "else", "elsewhere", "empty", "enough", "even", "ever", "everyone", "everything", "everywhere", "except", "first", "for", "former", "formerly", "from", "hadn", "hadn't", "hasn", "hasn't", "haven", "haven't", "he", "hence", "her", "here", "hereafter", "hereby", "herein", "hereupon", "hers", "herself", "him", "himself", "his", "how", "however", "hundred", "i", "if", "in", "indeed", "into", "is", "isn", "isn't", "it", "it's", "its", "itself", "just", "latter", "latterly", "least", "ll", "may", "me", "meanwhile", "mightn", "mightn't", "mine", "more", "moreover", "most", "mostly", "must", "mustn", "mustn't", "my", "myself", "namely", "needn", "needn't", "neither", "never", "nevertheless", "next", "no", "nobody", "none", "noone", "nor", "not", "nothing", "now", "nowhere", "o", "of", "off", "on", "once", "one", "only", "onto", "or", "other", "others", "otherwise", "our", "ours", "ourselves", "out", "over", "per", "please", "s", "same", "shan", "shan't", "she", "she's", "should've", "shouldn", "shouldn't", "somehow", "something", "sometime", "somewhere", "such", "t", "than", "that", "that'll", "the", "their", "theirs", "them", "themselves", "then", "thence", "there", "thereafter", "thereby", "therefore", "therein", "thereupon", "these", "they", "this", "those", "through", "throughout", "thru", "thus", "to", "too", "toward", "towards", "under", "unless", "until", "up", "upon", "used", "ve", "was", "wasn", "wasn't", "we", "were", "weren", "weren't", "what", "whatever", "when", "whence", "whenever", "where", "whereafter", "whereas", "whereby", "wherein", "whereupon", "wherever", "whether", "which", "while", "whither", "who", "whoever", "whole", "whom", "whose", "why", "with", "within", "without", "won", "won't", "would", "wouldn", "wouldn't", "y", "yet", "you", "you'd", "you'll", "you're", "you've", "your", "yours", "yourself", "yourselves"]
             )
@@ -185,28 +202,26 @@
             search_method = BruteForceSearch() 
 
         else:
             raise NotImplementedError
         
         # Adding label constraint
         constraints.append(label_constraint)
-        goal_function = goal_function
-        attack = AdvPromptAttack(goal_function, constraints, transformation, search_method)
+        attack = AdvPromptAttack(self.goal_function, constraints, transformation, search_method)
         return attack
    
     def attack(self):
         if self.attack_name == "semantic":
             from ..prompts.semantic_atk_prompts import SEMANTIC_ADV_PROMPT_SET
             prompts_dict = SEMANTIC_ADV_PROMPT_SET[self.dataset.dataset_name]
             results = {}
             for language in prompts_dict.keys():
                 prompts = prompts_dict[language]
                 for prompt in prompts:
-                    from ..utils import inference_total_dataset
-                    acc = inference_total_dataset(prompt, self.model, self.dataset)
+                    acc = self.eval_func(prompt, self.dataset, self.model)
                     results[prompt] = acc
             
             return results
                   
         else:
             return self.prompt_attack.attack(self.prompt)
 
@@ -591,15 +606,21 @@
         elif final_result.goal_status == GoalFunctionResultStatus.MAXIMIZING:
             result = MaximizedAttackResult(
                 initial_result,
                 final_result,
             )
         else:
             raise ValueError(f"Unrecognized goal status {final_result.goal_status}")
-        return  result.original_result.output, result.perturbed_result.attacked_text.text, result.perturbed_result.output, result.perturbed_result.score
+        return  {
+            "original prompt": result.original_result.attacked_text.text,
+            "original score": result.original_result.output, 
+            "attacked prompt": result.perturbed_result.attacked_text.text, 
+            "attacked score": result.perturbed_result.output, 
+            "PDR": (result.original_result.output-result.perturbed_result.output) / result.original_result.output
+        }
 
     def attack(self, example):
         """Attack a single example.
 
         Args:
             example (:obj:`str`, :obj:`OrderedDict[str, str]` or :class:`~textattack.shared.AttackedText`):
                 Example to attack. It can be a single string or an `OrderedDict` where
```

### Comparing `promptbench-0.0.2a0/promptbench/prompt_attack/goal_function.py` & `promptbench-0.0.3/promptbench/prompt_attack/goal_function.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+#
+# Source Attribution:
+# The majority of this code is derived from the following sources:
+# - TextAttack GitHub Repository: https://github.com/QData/TextAttack
+# - Reference Paper: Morris, John X., et al. "TextAttack: A Framework for Adversarial Attacks, Data Augmentation, and Adversarial Training in NLP." arXiv preprint arXiv:2005.05909 (2020).
+
 
 from abc import ABC, abstractmethod
 
 import lru
 import numpy as np
 import torch
 
@@ -229,211 +235,58 @@
 
     def __setstate__(self, state):
         self.__dict__ = state
         if self.use_cache:
             self._call_model_cache = lru.LRU(state["_call_model_cache"])
 
 
-
 class AdvPromptGoalFunction(GoalFunction):
 
     """A goal function defined on a model that outputs a probability for some
     number of classes."""
 
-    def __init__(self, model, dataset, input_process_func, output_process_func, eval_func, query_budget, *args, target_max_acc=0, **kwargs):
+    def __init__(self, model, dataset, eval_func, query_budget, *args, target_max_acc=0, verbose=True, **kwargs):
         super().__init__(*args, **kwargs)
         self.model = model
         self.dataset = dataset
-        self.input_process_func = input_process_func
-        self.output_process_func = output_process_func
         self.eval_func = eval_func
         self.query_budget = query_budget
         self.target_max_acc = target_max_acc
+        self.verbose = verbose
 
     def _call_model(self, attacked_text_list):
         acc_list = []
         for attacked_prompt in attacked_text_list:
             prompt = attacked_prompt.text
-            labels = []
-            preds = []
-            for d in self.dataset:
-                input_text = self.input_process_func(prompt, d)
-                labels.append(d["label"])
-                print(self.model)
-                exit()
-                raw_pred = self.model(input_text)
-                pred = self.output_process_func(raw_pred)
-                preds.append(pred)
+            
+            acc_list.append(self.eval_func(prompt, self.dataset, self.model))
+            if self.verbose:
+                print("--------------------------------------------------")
+                print("Current prompt is: ", prompt)
+                print("Current accuracy is: ", acc_list[-1])
+                print("--------------------------------------------------\n")
+
+        return acc_list
+
     def _process_model_outputs(self, inputs, outputs):
         return outputs
 
     def _is_goal_complete(self, acc, _):
         return acc < self.target_max_acc
         
     def _get_score(self, model_output, _):
-        # Evaluate how much does the adv prompt decrease the accuracy.
-        # return self.ground_truth_output - model_output
         score = self.ground_truth_output - model_output
 
         return score
 
     def _goal_function_result_type(self):
         """Returns the class of this goal function's results."""
         return ClassificationGoalFunctionResult
 
     def extra_repr_keys(self):
         return []
 
     def _get_displayed_output(self, raw_output):
         return raw_output
 
-
-    # def _should_skip(self, *_):
-    #     return False
-    
-    def _call_model(self, attacked_text_list):
-        acc_list = []
-        for attacked_prompt in attacked_text_list:
-            prompt = attacked_prompt.text
-            labels = []
-            preds = []
-            idx = 0 
-            for d in self.dataset:
-                idx += 1
-                if idx > 2:
-                    break
-                input_text = self.input_process_func(prompt, d)
-                labels.append(d["label"])
-                raw_pred = self.model(input_text)
-                pred = self.output_process_func(raw_pred)
-                preds.append(pred)
-                
-            acc = self.eval_func(preds, labels)
-
-            acc_list.append(acc)
-        return acc_list
-
     def _get_goal_status(self, model_output, attacked_text, check_skip=False):
-        return super()._get_goal_status(model_output, attacked_text, check_skip)
-
-
-
-
-
-
-# class AdvPromptGoalFunction(GoalFunction):
-
-#     """A goal function defined on a model that outputs a probability for some
-#     number of classes."""
-
-#     def __init__(self, inference, query_budget, verbose=True, logger=None, *args, target_max_acc=0, **kwargs):
-#         self.inference = inference
-#         self.query_budget = query_budget
-#         self.target_max_acc = target_max_acc
-#         self.logger = logger
-#         self.verbose = verbose
-#         super().__init__(*args, **kwargs)
-
-#     def _process_model_outputs(self, inputs, outputs):
-#         return outputs
-
-#     def _is_goal_complete(self, acc, _):
-#         return acc < self.target_max_acc
-        
-#     def _get_score(self, model_output, _):
-#         # Evaluate how much does the adv prompt decrease the accuracy.
-#         # return self.ground_truth_output - model_output
-#         score = self.ground_truth_output - model_output
-
-#         return score
-
-#     def _goal_function_result_type(self):
-#         """Returns the class of this goal function's results."""
-#         return ClassificationGoalFunctionResult
-
-#     def extra_repr_keys(self):
-#         return []
-
-#     def _get_displayed_output(self, raw_output):
-#         return raw_output
-
-
-#     # def _should_skip(self, *_):
-#     #     return False
-    
-#     def _call_model(self, attacked_text_list):
-#         acc_list = []
-#         for attacked_prompt in attacked_text_list:
-#             prompt = attacked_prompt.text
-#             if self.verbose:
-#                 self.logger.info("Current adv prompt is: {}".format(prompt))
-#             acc = self.inference.predict(prompt)
-#             if self.verbose:
-#                 self.logger.info("Current acc: {:.2f}".format(acc*100))
-#             acc_list.append(acc)
-#         return acc_list
-
-#     def _get_goal_status(self, model_output, attacked_text, check_skip=False):
-#         return super()._get_goal_status(model_output, attacked_text, check_skip)
-
-
-# def create_goal_function(args, inference_model):
-#     goal_function = AdvPromptGoalFunction(inference=inference_model, query_budget=args.query_budget, 
-#                                           logger=args.logger, model_wrapper=None, verbose=args.verbose)
-#     return goal_function
-
-
-# class PromptGoalFunction(GoalFunction):
-
-#     """A goal function defined on a model that outputs a probability for some
-#     number of classes."""
-
-#     def __init__(self, inference, query_budget, verbose=True, logger=None, *args, target_max_acc=0, **kwargs):
-#         self.inference = inference
-#         self.query_budget = query_budget
-#         self.target_max_acc = target_max_acc
-#         self.logger = logger
-#         self.verbose = verbose
-#         super().__init__(*args, **kwargs)
-
-#     def _process_model_outputs(self, inputs, outputs):
-#         return outputs
-
-#     def _is_goal_complete(self, acc, _):
-        
-#         return acc < self.target_max_acc
-        
-#     def _get_score(self, model_output, _):
-#         # Evaluate how much does the adv prompt decrease the accuracy.
-#         score = self.ground_truth_output - model_output
-#         return score
-
-#     def _goal_function_result_type(self):
-#         """Returns the class of this goal function's results."""
-#         return ClassificationGoalFunctionResult
-
-#     def extra_repr_keys(self):
-#         return []
-
-#     def _get_displayed_output(self, raw_output):
-#         return raw_output
-
-
-#     # def _should_skip(self, *_):
-#     #     return False
-    
-#     def _call_model(self, text_list):
-#         acc_list = []
-#         for prompt in text_list:
-#             prompt = prompt.text
-#             if self.verbose:
-#                 self.logger.info("Current prompt is: {}".format(prompt))
-#             acc = self.inference.predict(prompt)
-#             if self.verbose:
-#                 self.logger.info("Current acc: {:.2f}".format(acc*100))
-#             acc_list.append(acc)
-#         return acc_list
-
-#     def _get_goal_status(self, model_output, text, check_skip=False):
-#         return super()._get_goal_status(model_output, text, check_skip)
-
-
+        return super()._get_goal_status(model_output, attacked_text, check_skip)
```

### Comparing `promptbench-0.0.2a0/promptbench/prompt_attack/search.py` & `promptbench-0.0.3/promptbench/prompt_attack/search.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/prompt_attack/transformations.py` & `promptbench-0.0.3/promptbench/prompt_attack/transformations.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/prompt_engineering/__init__.py` & `promptbench-0.0.3/promptbench/prompt_engineering/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
+
 from tqdm import tqdm
+import re
 
+from .base import Base
 from .least_to_most import LeastToMost
 from .generated_knowledge import GeneratedKnowledge
 from .chain_of_thought import ZSCoT, CoT
 from .expert_prompting import ExpertPrompting
 from .emotion_prompt import EmotionPrompt
 
 from ..metrics import Eval
 
+SUPPORTED_METHODS = ['CoT', 'ZSCoT', 'least_to_most', 'generated_knowledge', 'expert_prompting', 'emotion_prompt', 'baseline']
+
 METHOD_MAP = {
     'CoT': CoT,
     'ZSCoT': ZSCoT,
     'least_to_most': LeastToMost,
     'generated_knowledge': GeneratedKnowledge,
     'expert_prompting': ExpertPrompting,
     'emotion_prompt': EmotionPrompt,
+    'baseline': Base,
 }
 
 METHOD_SUPPORT_DATASET = {
     'CoT': ['gsm8k', 'csqa', 'bigbench_date', 'bigbench_object_tracking'],
     'ZSCoT': ['gsm8k', 'csqa', 'bigbench_date', 'bigbench_object_tracking'],
     'expert_prompting': ['gsm8k', 'csqa', 'bigbench_date', 'bigbench_object_tracking'],
     'emotion_prompt': ['gsm8k', 'csqa', 'bigbench_date', 'bigbench_object_tracking'],
-    'least_to_most': ['gsm8k', 'drop', 'last-letter-concat'],
+    'least_to_most': ['gsm8k', 'last_letter_concat'],
     'generated_knowledge': ['csqa', 'numersense', 'qasc'],
+    'baseline': ['gsm8k', 'csqa', 'bigbench_date', 'bigbench_object_tracking', 'last_letter_concat', 'numersense', 'qasc'],
 }
 
 # Model: GPT3.5, GPT4, Llama7b-chat, Llama13b-chat, llama70b-chat
 
 class PEMethod(object):
     """
     A class that provides an interface for various methods in prompt engineering.
@@ -49,26 +58,30 @@
             raise ValueError("The method is not supported!")
     
     @staticmethod
     def method_list():
         """Returns a list of supported methods."""
         return METHOD_MAP.keys()
     
-    def test(self, dataset, model):
+    def test(self, dataset, model, num_samples=None):
         """Tests the method on the given dataset and returns the accuracy."""""
         preds = []
         labels = []
-        for data in tqdm(dataset):
+        for i, data in enumerate(tqdm(dataset)):
+            if num_samples and i >= num_samples:
+                break
+            
             label = data['label']
             labels.append(label)
             
             input_text = data['content']
-            pred = self.infer_method.query(input_text, model)
+            ouput = self.infer_method.query(input_text, model)
+            res = re.findall(r'##(.*)', ouput)
+            pred = res[0] if res else ouput
             pred = dataset.extract_answer(pred)  #FIXME 执行取片操作后丢失类
-            # print(pred)
             preds.append(pred)
             
         score = Eval.compute_cls_accuracy(preds, labels)
         return score    
         
     def __call__(self, input_text, model):
         """Calls the method to perform inference."""
```

### Comparing `promptbench-0.0.2a0/promptbench/prompt_engineering/ask_me_anything.py` & `promptbench-0.0.3/promptbench/prompt_engineering/emotion_prompt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-import os 
-import sys 
-import numpy as np
-from pathlib import Path 
-from typing import List 
-import random 
-
-class AskMeAnything: 
-    def __init__(self, llm, args):      
-        self.llm  = llm
-        self.args = args
-        self.data_name = args['dataset']['name']    
-        if args['dataset']['name'] == 'anli_r1':  
-            self.question_prompt_path = args['method']['ask_me_anything']['anli_r1']['question_prompt_path'] 
-            self.answer_prompt_path   = args['method']['ask_me_anything']['anli_r1']['answer_prompt_path']
-            with open(self.question_prompt_path, 'r') as f: 
-                self.question_prompt = f.read()  
-            with open(self.answer_prompt_path, 'r') as f: 
-                self.answer_prompt = f.read() 
-            self.trigger = ' Based on the context , '
-        self.show_process = args['show_process'] 
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
 
+from .base import Base
+from ..prompts.method_oriented import get_prompt
+
+
+class EmotionPrompt(Base):
     """
-    Statement : There is no information indicating whether Daniel Zolnikov is a good legislator or not
-    .
-    Question :
-    """
-    def translate_question(self, question): 
-        question_aug = self.question_prompt + '\n\nStatement : ' + question + '\n\nQuestion : ' 
-        question_aug = [self.llm.convert_message_to_prompt(question_aug, 'user')] 
-        translated_question = self.llm.query(question_aug)
-        return translated_question
-    
-    def query(self, question_input): 
-        if self.data_name == 'anli_r1': 
-            question = self.translate_question(question_input['question']) 
-            question = self.answer_prompt + '\n\nContext : ' + \
-            question_input['context'] + '\n' + 'Question :' + self.trigger + \
-            question + '\n' + 'Answer : '
-            
-            query_prompt = [self.llm.convert_message_to_prompt(question, 'user')] 
-
-            answer = self.llm.query(query_prompt) 
-
-            if self.show_process == True:
-                self.llm.visualize_prompt(
-                    query_prompt + [self.llm.convert_message_to_prompt(answer, 'assistant')]
-                )
+    A class for handling emotion-based prompts in a conversational AI model.
 
-            return answer 
-        # pass 
+    This class is specialized in generating responses for prompts that add some emotions. It leverages a predefined emotion prompt, tailored to the specific needs of the query, to guide the model's response generation.
+
+    Attributes:
+    -----------
+    prompt_id : int
+        An identifier for selecting a specific emotion prompt from a collection of predefined prompts.
+    emotion_prompt : str
+        The actual emotion-based prompt text, retrieved based on the prompt_id, used to assist the model in generating emotion-aware responses.
+
+    Methods:
+    --------
+    __init__(**kwargs)
+        Initializes the EmotionPrompt instance with specific keyword arguments, including setting the prompt_id and retrieving the corresponding emotion prompt.
+        For example: "This is very important to my career."
+    query(input_text, model)
+        Processes the input text by appending it with the emotion prompt. It then instructs the model to generate a response that is cognizant of the emotional context provided. The response is formatted with a specific answer notation.
+    
+    Paper Link: https://arxiv.org/pdf/2307.11760v3.pdf
+    """
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        
+        self.prompt_id = int(kwargs.get('prompt_id'))
+        
+        self.emotion_prompts = get_prompt(['emotion_prompt', 'prompts'])
+        self.emotion_prompt = self.emotion_prompts[self.prompt_id]
+        
+    def query(self, input_text, model):
+        instr_get_answer = input_text + '\n' + self.emotion_prompt + '\n' + \
+                           f'Please output your answer at the end as ##<your answer ({self.output_range})>'
+        prompt_get_answer = model.convert_text_to_prompt(instr_get_answer, 'user')
+        
+        answer = model(prompt_get_answer)
+        
+        if self.verbose:
+            print(prompt_get_answer)
+            print(answer)
+        
+        return answer
```

### Comparing `promptbench-0.0.2a0/promptbench/prompts/prompt.py` & `promptbench-0.0.3/promptbench/prompts/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Microsoft Corporation.
+# Licensed under the MIT License.
+
 import re
 import os
 from typing import Union, List
 
 
 class Prompt:
     def __init__(self, prompt_content: Union[List[str], str, None] = None, dataset_name: str = None):
```

### Comparing `promptbench-0.0.2a0/promptbench/prompts/role_oriented.py` & `promptbench-0.0.3/promptbench/prompts/role_oriented.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/prompts/semantic_atk_prompts.py` & `promptbench-0.0.3/promptbench/prompts/semantic_atk_prompts.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/prompts/task_oriented.py` & `promptbench-0.0.3/promptbench/prompts/task_oriented.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/utils/dataprocess.py` & `promptbench-0.0.3/promptbench/utils/dataprocess.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/utils/defense.py` & `promptbench-0.0.3/promptbench/utils/defense.py`

 * *Files identical despite different names*

### Comparing `promptbench-0.0.2a0/promptbench/utils/visualize.py` & `promptbench-0.0.3/promptbench/utils/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+
 from ..models import LLMModel
 import torch
 import numpy as np
 import copy
 
 class Visualizer:
     def __init__(self, model: LLMModel) -> None:
```

### Comparing `promptbench-0.0.2a0/promptbench.egg-info/SOURCES.txt` & `promptbench-0.0.3/promptbench.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 promptbench/prompt_attack/__init__.py
 promptbench/prompt_attack/attack.py
 promptbench/prompt_attack/goal_function.py
 promptbench/prompt_attack/label_constraint.py
 promptbench/prompt_attack/search.py
 promptbench/prompt_attack/transformations.py
 promptbench/prompt_engineering/__init__.py
-promptbench/prompt_engineering/ask_me_anything.py
+promptbench/prompt_engineering/base.py
 promptbench/prompt_engineering/chain_of_thought.py
 promptbench/prompt_engineering/emotion_prompt.py
 promptbench/prompt_engineering/expert_prompting.py
 promptbench/prompt_engineering/generated_knowledge.py
 promptbench/prompt_engineering/least_to_most.py
 promptbench/prompts/__init__.py
 promptbench/prompts/method_oriented.py
```

### Comparing `promptbench-0.0.2a0/setup.py` & `promptbench-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,23 @@
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='promptbench',
-    version='0.0.2a',
+    version='0.0.3',
     description='PromptBench is a powerful tool designed to scrutinize and analyze the interaction of large language models with various prompts. It provides a convenient infrastructure to simulate **black-box** adversarial  **prompt attacks** on the models and evaluate their performances.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/microsoft/promptbench',
     author='',
     author_email='',
 
     # Note that this is a string of words separated by whitespace, not a list.
     keywords='pytorch, large language models, prompt tuning, dyval, evaluation',
     packages=find_packages(exclude=['examples', 'imgs', 'docs']),
     include_package_data=True,
     # install_requires=['torch >= 1.8', 'torchvision', 'torchaudio', 'transformers', 'timm', 'progress', 'ruamel.yaml', 'scikit-image', 'scikit-learn', 'tensorflow', ''],
     install_requires=install_requires,
     python_requires='>=3.9',
-)
+)
```

