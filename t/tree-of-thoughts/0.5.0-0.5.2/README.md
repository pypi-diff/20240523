# Comparing `tmp/tree_of_thoughts-0.5.0.tar.gz` & `tmp/tree_of_thoughts-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_of_thoughts-0.5.0.tar", max compression
+gzip compressed data, was "tree_of_thoughts-0.5.2.tar", max compression
```

## Comparing `tree_of_thoughts-0.5.0.tar` & `tree_of_thoughts-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.0/LICENSE
--rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.0/README.md
--rw-r--r--   0        0        0     1247 2024-05-23 00:55:59.753124 tree_of_thoughts-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      356 2024-05-23 00:55:53.906281 tree_of_thoughts-0.5.0/tree_of_thoughts/__init__.py
--rw-r--r--   0        0        0     8174 2024-05-23 01:05:50.310188 tree_of_thoughts-0.5.0/tree_of_thoughts/tot_agent.py
--rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.0/tree_of_thoughts/tree_of_thoughts.py
--rw-r--r--   0        0        0    10211 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.2/LICENSE
+-rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.2/README.md
+-rw-r--r--   0        0        0     1247 2024-05-23 01:08:26.862049 tree_of_thoughts-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      356 2024-05-23 00:55:53.906281 tree_of_thoughts-0.5.2/tree_of_thoughts/__init__.py
+-rw-r--r--   0        0        0     8559 2024-05-23 01:09:11.423960 tree_of_thoughts-0.5.2/tree_of_thoughts/tot_agent.py
+-rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.2/tree_of_thoughts/tree_of_thoughts.py
+-rw-r--r--   0        0        0    10211 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.2/PKG-INFO
```

### Comparing `tree_of_thoughts-0.5.0/LICENSE` & `tree_of_thoughts-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.0/README.md` & `tree_of_thoughts-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.0/pyproject.toml` & `tree_of_thoughts-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tree-of-thoughts"
-version = "0.5.0"
+version = "0.5.2"
 description = "Tree of Thoughts - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # Assuming you have a README.md file
 homepage = "https://github.com/kyegomez/tree-of-thoughts"
 keywords = ["artificial intelligence", "deep learning", "optimizers", "Prompt Engineering"]
 classifiers = [
```

### Comparing `tree_of_thoughts-0.5.0/tree_of_thoughts/tot_agent.py` & `tree_of_thoughts-0.5.2/tree_of_thoughts/tot_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 import logging
 from swarms import Agent
+from pydantic import BaseModel, Field
+from typing import List, Dict
 
 # Logging
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 logger = logging.getLogger(__name__)
 
 
+class TreeOfThoughtsResponseFormat(BaseModel):
+    response: str = Field(
+        ..., description="Response from the model", example="Observation:xxxx"
+    )
+    evaluation: float = Field(
+        ..., description="Evaluation of the response", example=0.5
+    )
+
+
+
 class ToTAgent:
     """
 
     OpenAI Language Model API Wrapper
 
     Args:
         agent (Agent): Agent class from swarms
@@ -58,29 +70,25 @@
         self.ReAct_prompt = ""
         if enable_react:
             self.react_prompt = (
                 "Write down your observations in format 'Observation:xxxx',"
                 " then write down your thoughts in format 'Thoughts:xxxx'."
             )
 
-    def run(self, task: str):
+    def run(self, task: str, *args, **kwargs):
         """Generate text from prompt using"""
         if self.use_chat_api:
             thoughts = []
             for _ in range(self.k):
-                response = self.agent(task)
+                response = self.agent.run(task, *args, **kwargs)
                 thoughts += [response]
             return thoughts
 
     def generate_thoughts(
-        self,
-        state,
-        k: int = None,
-        initial_prompt: str = None,
-        rejected_solutions: list = None,
+        self, state, k: int = None, initial_prompt: str = None, rejected_solutions: list = None
     ):
         """
         Generate thoughts from state using OpenAI API
 
         Args:
             state (str or list): State of reasoning
             k (int): Number of thoughts to generate
@@ -157,15 +165,17 @@
                     {state_text}\n       
                     If the solutions is not directly concretely making fast progress in achieving the goal, give it a lower score.
                     Evaluate all solutions AS A FLOAT BETWEEN 0 and 1:\n,  DO NOT RETURN ANYTHING ELSE
                 """
 
                 response = self.agent(prompt)
                 try:
-                    value_text = self.run(response)
+                    value_text = self.run(
+                        response
+                    )
                     # print(f'state: {value_text}')
                     value = float(value_text)
                     print(f"Evaluated Thought Value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
```

### Comparing `tree_of_thoughts-0.5.0/tree_of_thoughts/tree_of_thoughts.py` & `tree_of_thoughts-0.5.2/tree_of_thoughts/tree_of_thoughts.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.0/PKG-INFO` & `tree_of_thoughts-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.5.0
+Version: 0.5.2
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

