# Comparing `tmp/continuous_eval-0.3.8.tar.gz` & `tmp/continuous_eval-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuous_eval-0.3.8.tar", max compression
+gzip compressed data, was "continuous_eval-0.3.9.tar", max compression
```

## Comparing `continuous_eval-0.3.8.tar` & `continuous_eval-0.3.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.8/LICENSE
--rw-r--r--   0        0        0     9731 2024-05-19 17:18:08.444721 continuous_eval-0.3.8/README.md
--rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.8/continuous_eval/__init__.py
--rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.8/continuous_eval/classifiers/__init__.py
--rw-r--r--   0        0        0     3071 2024-05-16 15:09:47.554528 continuous_eval-0.3.8/continuous_eval/classifiers/ensemble.py
--rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.8/continuous_eval/classifiers/utils.py
--rw-r--r--   0        0        0     3014 2024-05-19 17:18:08.445148 continuous_eval-0.3.8/continuous_eval/data_downloader.py
--rw-r--r--   0        0        0     3740 2024-05-16 15:14:21.930240 continuous_eval-0.3.8/continuous_eval/datatypes.py
--rw-r--r--   0        0        0      308 2024-05-19 17:18:08.445480 continuous_eval-0.3.8/continuous_eval/eval/__init__.py
--rw-r--r--   0        0        0     6829 2024-05-19 17:18:08.445900 continuous_eval-0.3.8/continuous_eval/eval/dataset.py
--rw-r--r--   0        0        0     3238 2024-05-19 17:18:08.446195 continuous_eval-0.3.8/continuous_eval/eval/logger.py
--rw-r--r--   0        0        0     1637 2024-05-19 17:18:08.446528 continuous_eval-0.3.8/continuous_eval/eval/modules.py
--rw-r--r--   0        0        0     4539 2024-05-17 18:58:11.809843 continuous_eval-0.3.8/continuous_eval/eval/pipeline.py
--rw-r--r--   0        0        0     5883 2024-05-19 17:18:08.447080 continuous_eval-0.3.8/continuous_eval/eval/result_types.py
--rw-r--r--   0        0        0     3609 2024-05-19 17:18:08.447290 continuous_eval-0.3.8/continuous_eval/eval/runner.py
--rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.8/continuous_eval/eval/tests.py
--rw-r--r--   0        0        0      288 2024-05-19 17:18:08.447591 continuous_eval-0.3.8/continuous_eval/eval/types.py
--rw-r--r--   0        0        0     1107 2024-05-18 03:37:31.360398 continuous_eval-0.3.8/continuous_eval/eval/utils.py
--rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.8/continuous_eval/generators/__init__.py
--rw-r--r--   0        0        0    12878 2024-05-19 17:18:08.447912 continuous_eval-0.3.8/continuous_eval/generators/simple.py
--rw-r--r--   0        0        0    10016 2024-04-30 03:48:52.158450 continuous_eval-0.3.8/continuous_eval/llm_factory.py
--rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.8/continuous_eval/llms/__init__.py
--rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.8/continuous_eval/llms/bedrock.py
--rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.8/continuous_eval/metrics/__init__.py
--rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.8/continuous_eval/metrics/_utils/simple_tokenizer.py
--rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.8/continuous_eval/metrics/base.py
--rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.8/continuous_eval/metrics/classification/__init__.py
--rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.8/continuous_eval/metrics/classification/classification.py
--rw-r--r--   0        0        0      111 2024-03-08 07:02:54.302236 continuous_eval-0.3.8/continuous_eval/metrics/code/python/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-08 08:55:45.681607 continuous_eval-0.3.8/continuous_eval/metrics/code/python/code_deterministic_metrics.py
--rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/__init__.py
--rw-r--r--   0        0        0     3769 2024-05-16 15:14:21.925777 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/bert.py
--rw-r--r--   0        0        0     2945 2024-05-16 15:14:21.919758 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/custom.py
--rw-r--r--   0        0        0     4814 2024-05-18 03:37:32.100141 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/deterministic.py
--rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/llm_based.py
--rw-r--r--   0        0        0     5770 2024-05-16 15:14:21.670171 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/semantic.py
--rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.8/continuous_eval/metrics/generation/text/utils.py
--rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/__init__.py
--rw-r--r--   0        0        0     6541 2024-04-05 23:59:38.533703 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/llm_based.py
--rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/matching_strategy.py
--rw-r--r--   0        0        0     2470 2024-04-02 16:24:12.028818 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/precision_recall_f1.py
--rw-r--r--   0        0        0     3394 2024-04-02 16:24:12.029049 continuous_eval-0.3.8/continuous_eval/metrics/retrieval/ranked.py
--rw-r--r--   0        0        0     1867 2024-05-19 17:18:08.448171 continuous_eval-0.3.8/continuous_eval/metrics/tools/match.py
--rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.8/continuous_eval/utils/telemetry.py
--rw-r--r--   0        0        0     1671 2024-05-19 17:18:08.456046 continuous_eval-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    11364 1970-01-01 00:00:00.000000 continuous_eval-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.9/LICENSE
+-rw-r--r--   0        0        0     9765 2024-05-21 14:55:57.525589 continuous_eval-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.9/continuous_eval/__init__.py
+-rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.9/continuous_eval/classifiers/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-16 15:09:47.554528 continuous_eval-0.3.9/continuous_eval/classifiers/ensemble.py
+-rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.9/continuous_eval/classifiers/utils.py
+-rw-r--r--   0        0        0     3014 2024-05-19 17:18:08.445148 continuous_eval-0.3.9/continuous_eval/data_downloader.py
+-rw-r--r--   0        0        0     3740 2024-05-16 15:14:21.930240 continuous_eval-0.3.9/continuous_eval/datatypes.py
+-rw-r--r--   0        0        0      308 2024-05-19 17:18:08.445480 continuous_eval-0.3.9/continuous_eval/eval/__init__.py
+-rw-r--r--   0        0        0     6829 2024-05-19 17:18:08.445900 continuous_eval-0.3.9/continuous_eval/eval/dataset.py
+-rw-r--r--   0        0        0     3238 2024-05-19 17:18:08.446195 continuous_eval-0.3.9/continuous_eval/eval/logger.py
+-rw-r--r--   0        0        0     1637 2024-05-19 17:18:08.446528 continuous_eval-0.3.9/continuous_eval/eval/modules.py
+-rw-r--r--   0        0        0     4539 2024-05-17 18:58:11.809843 continuous_eval-0.3.9/continuous_eval/eval/pipeline.py
+-rw-r--r--   0        0        0     5883 2024-05-19 17:18:08.447080 continuous_eval-0.3.9/continuous_eval/eval/result_types.py
+-rw-r--r--   0        0        0     3609 2024-05-19 17:18:08.447290 continuous_eval-0.3.9/continuous_eval/eval/runner.py
+-rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.9/continuous_eval/eval/tests.py
+-rw-r--r--   0        0        0      288 2024-05-19 17:18:08.447591 continuous_eval-0.3.9/continuous_eval/eval/types.py
+-rw-r--r--   0        0        0     1107 2024-05-18 03:37:31.360398 continuous_eval-0.3.9/continuous_eval/eval/utils.py
+-rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.9/continuous_eval/generators/__init__.py
+-rw-r--r--   0        0        0    12878 2024-05-19 17:18:08.447912 continuous_eval-0.3.9/continuous_eval/generators/simple.py
+-rw-r--r--   0        0        0    10016 2024-04-30 03:48:52.158450 continuous_eval-0.3.9/continuous_eval/llm_factory.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.9/continuous_eval/llms/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.9/continuous_eval/llms/bedrock.py
+-rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.9/continuous_eval/metrics/__init__.py
+-rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.9/continuous_eval/metrics/_utils/simple_tokenizer.py
+-rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.9/continuous_eval/metrics/base.py
+-rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.9/continuous_eval/metrics/classification/__init__.py
+-rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.9/continuous_eval/metrics/classification/classification.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:45:43.595374 continuous_eval-0.3.9/continuous_eval/metrics/code/__init__.py
+-rw-r--r--   0        0        0    11701 2024-05-21 14:55:57.527248 continuous_eval-0.3.9/continuous_eval/metrics/code/python/code_deterministic_metrics.py
+-rw-r--r--   0        0        0     5127 2024-05-22 20:07:07.109742 continuous_eval-0.3.9/continuous_eval/metrics/code/sql/deterministic.py
+-rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/__init__.py
+-rw-r--r--   0        0        0     3769 2024-05-16 15:14:21.925777 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/bert.py
+-rw-r--r--   0        0        0     2945 2024-05-16 15:14:21.919758 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/custom.py
+-rw-r--r--   0        0        0     4814 2024-05-18 03:37:32.100141 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/deterministic.py
+-rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/llm_based.py
+-rw-r--r--   0        0        0     5770 2024-05-16 15:14:21.670171 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/semantic.py
+-rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.9/continuous_eval/metrics/generation/text/utils.py
+-rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.9/continuous_eval/metrics/retrieval/__init__.py
+-rw-r--r--   0        0        0     6541 2024-04-05 23:59:38.533703 continuous_eval-0.3.9/continuous_eval/metrics/retrieval/llm_based.py
+-rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.9/continuous_eval/metrics/retrieval/matching_strategy.py
+-rw-r--r--   0        0        0     2470 2024-04-02 16:24:12.028818 continuous_eval-0.3.9/continuous_eval/metrics/retrieval/precision_recall_f1.py
+-rw-r--r--   0        0        0     3394 2024-04-02 16:24:12.029049 continuous_eval-0.3.9/continuous_eval/metrics/retrieval/ranked.py
+-rw-r--r--   0        0        0     1867 2024-05-19 17:18:08.448171 continuous_eval-0.3.9/continuous_eval/metrics/tools/match.py
+-rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.9/continuous_eval/utils/telemetry.py
+-rw-r--r--   0        0        0     1743 2024-05-22 19:57:25.275186 continuous_eval-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 continuous_eval-0.3.9/PKG-INFO
```

### Comparing `continuous_eval-0.3.8/LICENSE` & `continuous_eval-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/README.md` & `continuous_eval-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         <td rowspan="1">Classification</td>
         <td>Deterministic</td>
         <td>ClassificationAccuracy</td>
     </tr>
     <tr>
         <td rowspan="2">Code Generation</td>
         <td>Deterministic</td>
-        <td>CodeStringMatch, PythonASTSimilarity</td>
+        <td>CodeStringMatch, PythonASTSimilarity, SQLSyntaxMatch, SQLASTSimilarity</td>
     </tr>
     <tr>
         <td>LLM-based</td>
         <td>LLMBasedCodeGeneration</td>
     </tr>
     <tr>
         <td>Agent Tools</td>
```

#### html2text {}

```diff
@@ -38,15 +38,16 @@
                 Deterministic DeterministicFaithfulness,
                               FleschKincaidReadability
 Text Generation Semantic      DebertaAnswerScores, BertAnswerRelevance,
                               BertAnswerSimilarity
                 LLM-based     LLMBasedFaithfulness, LLMBasedAnswerCorrectness,
                               LLMBasedAnswerRelevance, LLMBasedStyleConsistency
 Classification  Deterministic ClassificationAccuracy
-Code Generation Deterministic CodeStringMatch, PythonASTSimilarity
+                Deterministic CodeStringMatch, PythonASTSimilarity,
+Code Generation               SQLSyntaxMatch, SQLASTSimilarity
                 LLM-based     LLMBasedCodeGeneration
 Agent Tools     Deterministic ToolSelectionAccuracy
 Custom                        Define your own metrics
 To define your own metrics, you only need to extend the [Metric]
 (continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the
 `__call__` method. Optional methods are `batch` (if it is possible to implement
 optimizations for batch processing) and `aggregate` (to aggregate metrics
```

### Comparing `continuous_eval-0.3.8/continuous_eval/classifiers/ensemble.py` & `continuous_eval-0.3.9/continuous_eval/classifiers/ensemble.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/classifiers/utils.py` & `continuous_eval-0.3.9/continuous_eval/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/data_downloader.py` & `continuous_eval-0.3.9/continuous_eval/data_downloader.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/datatypes.py` & `continuous_eval-0.3.9/continuous_eval/datatypes.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/dataset.py` & `continuous_eval-0.3.9/continuous_eval/eval/dataset.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/logger.py` & `continuous_eval-0.3.9/continuous_eval/eval/logger.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/modules.py` & `continuous_eval-0.3.9/continuous_eval/eval/modules.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/pipeline.py` & `continuous_eval-0.3.9/continuous_eval/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/result_types.py` & `continuous_eval-0.3.9/continuous_eval/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/runner.py` & `continuous_eval-0.3.9/continuous_eval/eval/runner.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/tests.py` & `continuous_eval-0.3.9/continuous_eval/eval/tests.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/eval/utils.py` & `continuous_eval-0.3.9/continuous_eval/eval/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/generators/simple.py` & `continuous_eval-0.3.9/continuous_eval/generators/simple.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/llm_factory.py` & `continuous_eval-0.3.9/continuous_eval/llm_factory.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/llms/bedrock.py` & `continuous_eval-0.3.9/continuous_eval/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/_utils/simple_tokenizer.py` & `continuous_eval-0.3.9/continuous_eval/metrics/_utils/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/base.py` & `continuous_eval-0.3.9/continuous_eval/metrics/base.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/classification/classification.py` & `continuous_eval-0.3.9/continuous_eval/metrics/classification/classification.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/code/python/code_deterministic_metrics.py` & `continuous_eval-0.3.9/continuous_eval/metrics/code/python/code_deterministic_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import ast
 from typing import List, Union
 
 from munkres import Munkres
+from sqlglot import diff, parse_one
+from sqlglot.diff import Keep
 from thefuzz import fuzz
 
 from continuous_eval.metrics.base import Metric
 
 
 class CodeStringMatch(Metric):
     def __call__(self, answer: str, ground_truth_answers: List[str]):
```

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/__init__.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/__init__.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/bert.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/bert.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/custom.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/custom.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/deterministic.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/deterministic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/llm_based.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/semantic.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/semantic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/generation/text/utils.py` & `continuous_eval-0.3.9/continuous_eval/metrics/generation/text/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/llm_based.py` & `continuous_eval-0.3.9/continuous_eval/metrics/retrieval/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/matching_strategy.py` & `continuous_eval-0.3.9/continuous_eval/metrics/retrieval/matching_strategy.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/precision_recall_f1.py` & `continuous_eval-0.3.9/continuous_eval/metrics/retrieval/precision_recall_f1.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/retrieval/ranked.py` & `continuous_eval-0.3.9/continuous_eval/metrics/retrieval/ranked.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/metrics/tools/match.py` & `continuous_eval-0.3.9/continuous_eval/metrics/tools/match.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/continuous_eval/utils/telemetry.py` & `continuous_eval-0.3.9/continuous_eval/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.8/pyproject.toml` & `continuous_eval-0.3.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "continuous-eval"
-version = "0.3.8"
+version = "0.3.9"
 description = "Open-Source Evaluation for GenAI Application Pipelines."
 authors = ["Yi Zhang <yi@relari.ai>", "Pasquale Antonante <pasquale@relari.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "continuous_eval"}]
 
 [tool.poetry.dependencies]
@@ -22,14 +22,15 @@
 pyyaml = "^6.0.1"
 appdirs = "^1.4.4"
 munkres = "^1.1.4"
 thefuzz = "^0.22.1"
 sentencepiece = "^0.2.0"
 tenacity = "^8.2.3"
 
+sqlglot = {version = "^23.17.0", optional = true}
 langchain-community = {version = "^0.0.29", optional = true}
 cohere = {version = "^4.54", optional = true}
 boto3 = {version = "^1.34.70", optional = true}
 google-generativeai = {version = "^0.3.1", optional = true}
 anthropic = {version = "^0.7.7", optional = true}
 
 [tool.poetry.group.semantic]
@@ -55,14 +56,15 @@
 
 [tool.poetry.extras]
 langchain = ["langchain-community"]
 anthropic = ["anthropic"]
 bedrock = ["boto3"]
 gemini = ["google-generativeai"]
 cohere = ["cohere"]
+sqlglot = ["sqlglot"]
 
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `continuous_eval-0.3.8/PKG-INFO` & `continuous_eval-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuous-eval
-Version: 0.3.8
+Version: 0.3.9
 Summary: Open-Source Evaluation for GenAI Application Pipelines.
 License: Apache-2.0
 Author: Yi Zhang
 Author-email: yi@relari.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: anthropic
 Provides-Extra: bedrock
 Provides-Extra: cohere
 Provides-Extra: gemini
 Provides-Extra: langchain
+Provides-Extra: sqlglot
 Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra == "anthropic"
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: boto3 (>=1.34.70,<2.0.0) ; extra == "bedrock"
 Requires-Dist: cohere (>=4.54,<5.0) ; extra == "cohere"
 Requires-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra == "gemini"
 Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0)
 Requires-Dist: langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain"
@@ -30,14 +31,15 @@
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: protobuf (>=4.23.4,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
+Requires-Dist: sqlglot (>=23.17.0,<24.0.0) ; extra == "sqlglot"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: thefuzz (>=0.22.1,<0.23.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h3 align="center">
   <img
@@ -159,15 +161,15 @@
         <td rowspan="1">Classification</td>
         <td>Deterministic</td>
         <td>ClassificationAccuracy</td>
     </tr>
     <tr>
         <td rowspan="2">Code Generation</td>
         <td>Deterministic</td>
-        <td>CodeStringMatch, PythonASTSimilarity</td>
+        <td>CodeStringMatch, PythonASTSimilarity, SQLSyntaxMatch, SQLASTSimilarity</td>
     </tr>
     <tr>
         <td>LLM-based</td>
         <td>LLMBasedCodeGeneration</td>
     </tr>
     <tr>
         <td>Agent Tools</td>
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.8 Summary: Open-Source
+Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.9 Summary: Open-Source
 Evaluation for GenAI Application Pipelines. License: Apache-2.0 Author: Yi
 Zhang Author-email: yi@relari.ai Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: anthropic Provides-Extra: bedrock
 Provides-Extra: cohere Provides-Extra: gemini Provides-Extra: langchain
-Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra == "anthropic" Requires-Dist:
-appdirs (>=1.4.4,<2.0.0) Requires-Dist: boto3 (>=1.34.70,<2.0.0) ; extra ==
-"bedrock" Requires-Dist: cohere (>=4.54,<5.0) ; extra == "cohere" Requires-
-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra == "gemini" Requires-Dist:
-imbalanced-learn (>=0.11.0,<0.12.0) Requires-Dist: langchain-community
-(>=0.0.29,<0.0.30) ; extra == "langchain" Requires-Dist: mapie (>=0.7.0,<0.8.0)
-Requires-Dist: munkres (>=1.1.4,<2.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: openai (>=1.3.7,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0)
-Requires-Dist: protobuf (>=4.23.4,<5.0.0) Requires-Dist: python-dotenv
-(>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: rouge (>=1.0.1,<2.0.0) Requires-Dist:
-sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Description-Content-Type: text/markdown
+Provides-Extra: sqlglot Requires-Dist: anthropic (>=0.7.7,<0.8.0) ; extra ==
+"anthropic" Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: boto3
+(>=1.34.70,<2.0.0) ; extra == "bedrock" Requires-Dist: cohere (>=4.54,<5.0) ;
+extra == "cohere" Requires-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra
+== "gemini" Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0) Requires-Dist:
+langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain" Requires-Dist:
+mapie (>=0.7.0,<0.8.0) Requires-Dist: munkres (>=1.1.4,<2.0.0) Requires-Dist:
+nltk (>=3.8.1,<4.0.0) Requires-Dist: openai (>=1.3.7,<2.0.0) Requires-Dist:
+pandas (>=2.1.4,<3.0.0) Requires-Dist: protobuf (>=4.23.4,<5.0.0) Requires-
+Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: rouge (>=1.0.1,<2.0.0)
+Requires-Dist: sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: sqlglot
+(>=23.17.0,<24.0.0) ; extra == "sqlglot" Requires-Dist: tenacity
+(>=8.2.3,<9.0.0) Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist: tqdm
+(>=4.66.1,<5.0.0) Description-Content-Type: text/markdown
                ******** [[ddooccss//ppuubblliicc//ccoonnttiinnuuoouuss--eevvaall--llooggoo..ppnngg]] ********
    _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_]_(_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_G_i_t_H_u_b_._c_o_m_/
   _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_r_e_l_e_a_s_e_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
    _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_) _!_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_N_a_e_r_e_e_n_/_b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/
    _b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_) ![https://
      pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/
@@ -60,15 +61,16 @@
                 Deterministic DeterministicFaithfulness,
                               FleschKincaidReadability
 Text Generation Semantic      DebertaAnswerScores, BertAnswerRelevance,
                               BertAnswerSimilarity
                 LLM-based     LLMBasedFaithfulness, LLMBasedAnswerCorrectness,
                               LLMBasedAnswerRelevance, LLMBasedStyleConsistency
 Classification  Deterministic ClassificationAccuracy
-Code Generation Deterministic CodeStringMatch, PythonASTSimilarity
+                Deterministic CodeStringMatch, PythonASTSimilarity,
+Code Generation               SQLSyntaxMatch, SQLASTSimilarity
                 LLM-based     LLMBasedCodeGeneration
 Agent Tools     Deterministic ToolSelectionAccuracy
 Custom                        Define your own metrics
 To define your own metrics, you only need to extend the [Metric]
 (continuous_eval/metrics/base.py#L23C7-L23C13) class implementing the
 `__call__` method. Optional methods are `batch` (if it is possible to implement
 optimizations for batch processing) and `aggregate` (to aggregate metrics
```

