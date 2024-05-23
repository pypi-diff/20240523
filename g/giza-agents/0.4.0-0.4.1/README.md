# Comparing `tmp/giza_agents-0.4.0.tar.gz` & `tmp/giza_agents-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_agents-0.4.0.tar", max compression
+gzip compressed data, was "giza_agents-0.4.1.tar", max compression
```

## Comparing `giza_agents-0.4.0.tar` & `giza_agents-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2024-05-22 14:50:53.812941 giza_agents-0.4.0/LICENSE
--rw-r--r--   0        0        0     4503 2024-05-22 14:50:53.812941 giza_agents-0.4.0/README.md
--rw-r--r--   0        0        0      395 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/__init__.py
--rw-r--r--   0        0        0     5991 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/action.py
--rw-r--r--   0        0        0    17879 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/agent.py
--rw-r--r--   0        0        0      630 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/deployments.py
--rw-r--r--   0        0        0      252 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/logger.py
--rw-r--r--   0        0        0     3051 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/logging.yaml
--rw-r--r--   0        0        0    18146 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/model.py
--rw-r--r--   0        0        0      576 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/task.py
--rw-r--r--   0        0        0     1974 2024-05-22 14:50:53.824941 giza_agents-0.4.0/giza/agents/utils.py
--rw-r--r--   0        0        0     1206 2024-05-22 14:50:53.828941 giza_agents-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 giza_agents-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-23 15:02:13.436045 giza_agents-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4609 2024-05-23 15:02:13.436045 giza_agents-0.4.1/README.md
+-rw-r--r--   0        0        0      395 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/__init__.py
+-rw-r--r--   0        0        0     5991 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/action.py
+-rw-r--r--   0        0        0    17968 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/agent.py
+-rw-r--r--   0        0        0      630 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/deployments.py
+-rw-r--r--   0        0        0      252 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/logger.py
+-rw-r--r--   0        0        0     3051 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/logging.yaml
+-rw-r--r--   0        0        0    18146 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/model.py
+-rw-r--r--   0        0        0      576 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/task.py
+-rw-r--r--   0        0        0     1974 2024-05-23 15:02:13.448045 giza_agents-0.4.1/giza/agents/utils.py
+-rw-r--r--   0        0        0     1206 2024-05-23 15:02:13.452045 giza_agents-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5659 1970-01-01 00:00:00.000000 giza_agents-0.4.1/PKG-INFO
```

### Comparing `giza_agents-0.4.0/LICENSE` & `giza_agents-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/README.md` & `giza_agents-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+![image](https://github.com/gizatechxyz/giza-agents/assets/18899187/eb01e7f2-c0ec-4467-ba29-09e96042dae4)
 
 # AI Agents
 
 Giza Agents is a framework for trust-minimized integration of machine learning into on-chain strategy and action, featuring mechanisms for agentic memory and reflection that improve performance over their lifecycle.
 
 The extensible nature of Giza Agents allows developers to enshrine custom strategies using ML and other algorithms, develop novel agent functionalities and manage continuous iteration processes.
```

### Comparing `giza_agents-0.4.0/giza/agents/action.py` & `giza_agents-0.4.1/giza/agents/action.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/giza/agents/agent.py` & `giza_agents-0.4.1/giza/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         input_file: Optional[str] = None,
         input_feed: Optional[Dict] = None,
         verifiable: bool = False,
         fp_impl: str = "FP16x16",
         custom_output_dtype: Optional[str] = None,
         job_size: str = "M",
         dry_run: bool = False,
+        model_category: Optional[str] = None,
         **result_kwargs: Any,
     ) -> Optional[Union[Tuple[Any, Any], "AgentResult"]]:
         """
         Runs a round of inference on the model and saves the result.
 
         Args:
             input_file: The input file to use for inference
@@ -266,14 +267,15 @@
             input_file=input_file,
             input_feed=input_feed,
             verifiable=verifiable,
             fp_impl=fp_impl,
             custom_output_dtype=custom_output_dtype,
             job_size=job_size,
             dry_run=dry_run,
+            model_category=model_category,
         )
 
         self.verifiable = verifiable
 
         if not verifiable:
             logger.warning(
                 "Inference is not verifiable. No request ID was returned. No proof will be generated."
```

### Comparing `giza_agents-0.4.0/giza/agents/deployments.py` & `giza_agents-0.4.1/giza/agents/deployments.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/giza/agents/logging.yaml` & `giza_agents-0.4.1/giza/agents/logging.yaml`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/giza/agents/model.py` & `giza_agents-0.4.1/giza/agents/model.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/giza/agents/task.py` & `giza_agents-0.4.1/giza/agents/task.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/giza/agents/utils.py` & `giza_agents-0.4.1/giza/agents/utils.py`

 * *Files identical despite different names*

### Comparing `giza_agents-0.4.0/pyproject.toml` & `giza_agents-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-agents"
-version = "0.4.0"
+version = "0.4.1"
 
 description = "A Python SDK for Giza platform"
 authors = [
     "Francisco Algaba <fran@gizatech.xyz>",
     "Raphael Doukhan <raphael@gizatech.xyz>",
     "Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
```

### Comparing `giza_agents-0.4.0/PKG-INFO` & `giza_agents-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-agents
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python SDK for Giza platform
 License: MIT
 Author: Francisco Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,15 @@
 Requires-Dist: onnxruntime (>=1.16.3,<2.0.0)
 Requires-Dist: prefect (==2.14.6)
 Requires-Dist: prefect-docker (>=0.4.1,<0.5.0)
 Requires-Dist: prefect-gcp (>=0.5.4,<0.6.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
+![image](https://github.com/gizatechxyz/giza-agents/assets/18899187/eb01e7f2-c0ec-4467-ba29-09e96042dae4)
 
 # AI Agents
 
 Giza Agents is a framework for trust-minimized integration of machine learning into on-chain strategy and action, featuring mechanisms for agentic memory and reflection that improve performance over their lifecycle.
 
 The extensible nature of Giza Agents allows developers to enshrine custom strategies using ML and other algorithms, develop novel agent functionalities and manage continuous iteration processes.
```

