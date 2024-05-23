# Comparing `tmp/llama_index_multi_modal_llms_gemini-0.1.6.tar.gz` & `tmp/llama_index_multi_modal_llms_gemini-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_multi_modal_llms_gemini-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_multi_modal_llms_gemini-0.1.7.tar", max compression
```

## Comparing `llama_index_multi_modal_llms_gemini-0.1.6.tar` & `llama_index_multi_modal_llms_gemini-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2024-05-16 18:07:23.410491 llama_index_multi_modal_llms_gemini-0.1.6/README.md
--rw-r--r--   0        0        0      102 2024-05-16 18:07:23.410491 llama_index_multi_modal_llms_gemini-0.1.6/llama_index/multi_modal_llms/gemini/__init__.py
--rw-r--r--   0        0        0     9505 2024-05-16 18:07:23.410491 llama_index_multi_modal_llms_gemini-0.1.6/llama_index/multi_modal_llms/gemini/base.py
--rw-r--r--   0        0        0     1557 2024-05-16 18:07:23.410491 llama_index_multi_modal_llms_gemini-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_gemini-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-05-23 15:04:57.777394 llama_index_multi_modal_llms_gemini-0.1.7/README.md
+-rw-r--r--   0        0        0      102 2024-05-23 15:04:57.777394 llama_index_multi_modal_llms_gemini-0.1.7/llama_index/multi_modal_llms/gemini/__init__.py
+-rw-r--r--   0        0        0     9505 2024-05-23 15:04:57.777394 llama_index_multi_modal_llms_gemini-0.1.7/llama_index/multi_modal_llms/gemini/base.py
+-rw-r--r--   0        0        0     1526 2024-05-23 15:04:57.777394 llama_index_multi_modal_llms_gemini-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_gemini-0.1.7/PKG-INFO
```

### Comparing `llama_index_multi_modal_llms_gemini-0.1.6/llama_index/multi_modal_llms/gemini/base.py` & `llama_index_multi_modal_llms_gemini-0.1.7/llama_index/multi_modal_llms/gemini/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_multi_modal_llms_gemini-0.1.6/pyproject.toml` & `llama_index_multi_modal_llms_gemini-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index multi-modal-llms gemini integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-multi-modal-llms-gemini"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.11.post1"
-llama-index-llms-gemini = "^0.1.7"
+llama-index-llms-gemini = "^0.1.9"
 pillow = "^10.2.0"
-google-generativeai = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_multi_modal_llms_gemini-0.1.6/PKG-INFO` & `llama_index_multi_modal_llms_gemini-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-multi-modal-llms-gemini
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index multi-modal-llms gemini integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
-Requires-Dist: llama-index-llms-gemini (>=0.1.7,<0.2.0)
+Requires-Dist: llama-index-llms-gemini (>=0.1.9,<0.2.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Multi-Modal-Llms Integration: Gemini
```

