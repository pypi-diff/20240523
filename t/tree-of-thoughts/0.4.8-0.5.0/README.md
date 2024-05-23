# Comparing `tmp/tree_of_thoughts-0.4.8.tar.gz` & `tmp/tree_of_thoughts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_of_thoughts-0.4.8.tar", max compression
+gzip compressed data, was "tree_of_thoughts-0.5.0.tar", max compression
```

## Comparing `tree_of_thoughts-0.4.8.tar` & `tree_of_thoughts-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11343 2023-11-19 09:51:07.502043 tree_of_thoughts-0.4.8/LICENSE
--rw-r--r--   0        0        0     6833 2024-02-23 19:33:32.053708 tree_of_thoughts-0.4.8/README.md
--rw-r--r--   0        0        0     1246 2024-02-24 08:11:45.058940 tree_of_thoughts-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      354 2024-02-23 19:18:36.492143 tree_of_thoughts-0.4.8/tree_of_thoughts/__init__.py
--rw-r--r--   0        0        0     8174 2024-02-23 19:30:18.311121 tree_of_thoughts-0.4.8/tree_of_thoughts/tot_agent.py
--rw-r--r--   0        0        0    23710 2024-02-24 07:53:48.736156 tree_of_thoughts-0.4.8/tree_of_thoughts/treeofthoughts.py
--rw-r--r--   0        0        0     7712 1970-01-01 00:00:00.000000 tree_of_thoughts-0.4.8/setup.py
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 tree_of_thoughts-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.0/README.md
+-rw-r--r--   0        0        0     1247 2024-05-23 00:55:59.753124 tree_of_thoughts-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      356 2024-05-23 00:55:53.906281 tree_of_thoughts-0.5.0/tree_of_thoughts/__init__.py
+-rw-r--r--   0        0        0     8174 2024-05-23 01:05:50.310188 tree_of_thoughts-0.5.0/tree_of_thoughts/tot_agent.py
+-rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.0/tree_of_thoughts/tree_of_thoughts.py
+-rw-r--r--   0        0        0    10211 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.0/PKG-INFO
```

### Comparing `tree_of_thoughts-0.4.8/LICENSE` & `tree_of_thoughts-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.4.8/README.md` & `tree_of_thoughts-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Multi-Modality](imags/agorabanner.png)](https://discord.gg/qUtxnK2NMf)
+[![Multi-Modality](images/agorabanner.png)](https://discord.gg/qUtxnK2NMf)
 
 ![Tree of Thoughts Banner](images/treeofthoughts.png)
 
 ![Discord](https://img.shields.io/discord/999382051935506503)
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
 [![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 [![Facebook](https://img.shields.io/badge/Share-Facebook-blue?style=social&logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
@@ -175,17 +175,41 @@
 )
 
 print(f"Solution: {solution}")
 
 ```
 
 ### Basic Prompts
-- Copy and paste this into your llm!
+```txt
+
+Imagine three different experts are answering this question. All experts will write down 1 step of their thinking, then share it with the group. Then all experts will go on to the next step, etc. If any expert realises they're wrong at any point then they leave. The question is...
+
+
+
+################ 2nd ################
+
+Simulate three brilliant, logical experts collaboratively answering a question. Each one verbosely explains their thought process in real-time, considering the prior explanations of others and openly acknowledging mistakes. At each step, whenever possible, each expert refines and builds upon the thoughts of others, acknowledging their contributions. They continue until there is a definitive answer to the question. For clarity, your entire response should be in a markdown table. The question is...
+
+
+################ ################
+
+Imagine three highly intelligent experts working together to answer a question. They will follow a tree of thoughts approach, where each expert shares their thought process step by step. They will consider the input from others, refine their thoughts, and build upon the group's collective knowledge. If an expert realizes their thought is incorrect, they will acknowledge it and withdraw from the discussion. Continue this process until a definitive answer is reached. Present the entire response in a markdown table. The question is...
+
+
+################ 2nd ################
+
+Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...
+################ 2nd ################
+
+
+Envision a group of three experts working in unison to tackle a question by employing a tree of thoughts strategy. Each expert will thoroughly explain their line of thinking at every step, while also considering the insights provided by their peers. They will openly recognize any mistakes and build upon the group's shared understanding. This iterative process will continue until a definitive solution is reached. Structure the entire response as a markdown table. The question is...
+
+
+################ 2nd ################
 
-```
 "Three experts with exceptional logical thinking skills are collaboratively answering a question using the tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The task is:
 ```
 
 
 
 # Acknowledgements
```

### Comparing `tree_of_thoughts-0.4.8/pyproject.toml` & `tree_of_thoughts-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tree-of-thoughts"
-version = "0.4.8"
+version = "0.5.0"
 description = "Tree of Thoughts - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # Assuming you have a README.md file
 homepage = "https://github.com/kyegomez/tree-of-thoughts"
 keywords = ["artificial intelligence", "deep learning", "optimizers", "Prompt Engineering"]
 classifiers = [
@@ -12,15 +12,15 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.10"
 transformers = "*"
 swarms = "*"
 numpy = "*"
 queue = "*"
```

### Comparing `tree_of_thoughts-0.4.8/tree_of_thoughts/tot_agent.py` & `tree_of_thoughts-0.5.0/tree_of_thoughts/tot_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,19 @@
             thoughts = []
             for _ in range(self.k):
                 response = self.agent(task)
                 thoughts += [response]
             return thoughts
 
     def generate_thoughts(
-        self, state, k, initial_prompt, rejected_solutions=None
+        self,
+        state,
+        k: int = None,
+        initial_prompt: str = None,
+        rejected_solutions: list = None,
     ):
         """
         Generate thoughts from state using OpenAI API
 
         Args:
             state (str or list): State of reasoning
             k (int): Number of thoughts to generate
@@ -90,18 +94,20 @@
 
         """
         if type(state) == str:
             state_text = state
         else:
             state_text = "\n".join(state)
         print("New state generating thought:", state, "\n\n")
-        prompt = f"""Y
-        ou're an TreeofThoughts, an superintelligent AI model devoted to helping Humans by any means necessary. You're purpose is to generate a series of solutions to comply with the user's instructions, you must generate solutions on the basis of determining the most reliable solution in the shortest amount of time, while taking rejected solutions into account and learning from them. 
-        Considering the reasoning provided:\n\n
-        ###'{state_text}'\n\n###
+        prompt = f"""
+        You're TreeofThoughts, an superintelligent AI model devoted to helping Humans by any means necessary. 
+        You're purpose is to generate a series of solutions to comply with the user's instructions, you must generate solutions on the basis of determining the most reliable solution in the shortest amount of time, while taking rejected solutions into account and learning from them. 
+        Considering the reasoning provided:
+        
+        \n\n###'{state_text}'\n\n###
         Devise the best possible solution for the task: {initial_prompt}, Here are evaluated solutions that were rejected: 
         ###{rejected_solutions}###, 
         complete the {initial_prompt} without making the same mistakes you did with the evaluated rejected solutions. Be simple. Be direct. Provide intuitive solutions as soon as you think of them."""
 
         prompt += self.react_prompt
         thoughts = self.run(prompt)
         return thoughts
@@ -151,17 +157,15 @@
                     {state_text}\n       
                     If the solutions is not directly concretely making fast progress in achieving the goal, give it a lower score.
                     Evaluate all solutions AS A FLOAT BETWEEN 0 and 1:\n,  DO NOT RETURN ANYTHING ELSE
                 """
 
                 response = self.agent(prompt)
                 try:
-                    value_text = self.openai_choice2text_handler(
-                        response.choices[0]
-                    )
+                    value_text = self.run(response)
                     # print(f'state: {value_text}')
                     value = float(value_text)
                     print(f"Evaluated Thought Value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
```

### Comparing `tree_of_thoughts-0.4.8/tree_of_thoughts/treeofthoughts.py` & `tree_of_thoughts-0.5.0/tree_of_thoughts/tree_of_thoughts.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.4.8/PKG-INFO` & `tree_of_thoughts-0.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.4.8
+Version: 0.5.0
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: numpy
 Requires-Dist: queue
 Requires-Dist: swarms
 Requires-Dist: transformers
 Description-Content-Type: text/markdown
 
-[![Multi-Modality](imags/agorabanner.png)](https://discord.gg/qUtxnK2NMf)
+[![Multi-Modality](images/agorabanner.png)](https://discord.gg/qUtxnK2NMf)
 
 ![Tree of Thoughts Banner](images/treeofthoughts.png)
 
 ![Discord](https://img.shields.io/discord/999382051935506503)
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
 [![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 [![Facebook](https://img.shields.io/badge/Share-Facebook-blue?style=social&logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
@@ -203,17 +200,41 @@
 )
 
 print(f"Solution: {solution}")
 
 ```
 
 ### Basic Prompts
-- Copy and paste this into your llm!
+```txt
+
+Imagine three different experts are answering this question. All experts will write down 1 step of their thinking, then share it with the group. Then all experts will go on to the next step, etc. If any expert realises they're wrong at any point then they leave. The question is...
+
+
+
+################ 2nd ################
+
+Simulate three brilliant, logical experts collaboratively answering a question. Each one verbosely explains their thought process in real-time, considering the prior explanations of others and openly acknowledging mistakes. At each step, whenever possible, each expert refines and builds upon the thoughts of others, acknowledging their contributions. They continue until there is a definitive answer to the question. For clarity, your entire response should be in a markdown table. The question is...
+
+
+################ ################
+
+Imagine three highly intelligent experts working together to answer a question. They will follow a tree of thoughts approach, where each expert shares their thought process step by step. They will consider the input from others, refine their thoughts, and build upon the group's collective knowledge. If an expert realizes their thought is incorrect, they will acknowledge it and withdraw from the discussion. Continue this process until a definitive answer is reached. Present the entire response in a markdown table. The question is...
+
+
+################ 2nd ################
+
+Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...
+################ 2nd ################
+
+
+Envision a group of three experts working in unison to tackle a question by employing a tree of thoughts strategy. Each expert will thoroughly explain their line of thinking at every step, while also considering the insights provided by their peers. They will openly recognize any mistakes and build upon the group's shared understanding. This iterative process will continue until a definitive solution is reached. Structure the entire response as a markdown table. The question is...
+
+
+################ 2nd ################
 
-```
 "Three experts with exceptional logical thinking skills are collaboratively answering a question using the tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The task is:
 ```
 
 
 
 # Acknowledgements
```

