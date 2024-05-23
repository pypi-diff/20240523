# Comparing `tmp/llama_index_llms_ipex_llm-0.1.2.tar.gz` & `tmp/llama_index_llms_ipex_llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ipex_llm-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_llms_ipex_llm-0.1.3.tar", max compression
```

## Comparing `llama_index_llms_ipex_llm-0.1.2.tar` & `llama_index_llms_ipex_llm-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      714 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/README.md
--rw-r--r--   0        0        0       17 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/BUILD
--rw-r--r--   0        0        0       75 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/__init__.py
--rw-r--r--   0        0        0    20955 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/base.py
--rw-r--r--   0        0        0     1642 2024-04-15 18:09:27.821012 llama_index_llms_ipex_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      863 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/BUILD
+-rw-r--r--   0        0        0       75 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/__init__.py
+-rw-r--r--   0        0        0    21197 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/base.py
+-rw-r--r--   0        0        0     2433 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.3/PKG-INFO
```

### Comparing `llama_index_llms_ipex_llm-0.1.2/README.md` & `llama_index_llms_ipex_llm-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 ### On CPU
 
 ```bash
 pip install llama-index-llms-ipex-llm
 ```
 
+### On GPU
+
+```bash
+pip install llama-index-llms-ipex-llm[xpu] --extra-index-url https://pytorch-extension.intel.com/release-whl/stable/xpu/us/
+```
+
 ## Usage
 
 ```python
 from llama_index.llms.ipex_llm import IpexLLM
 ```
 
 ## Examples
```

### Comparing `llama_index_llms_ipex_llm-0.1.2/llama_index/llms/ipex_llm/base.py` & `llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is adapted from
 # https://github.com/run-llama/llama_index/blob/main/llama-index-integrations/
 # llms/llama-index-llms-huggingface/llama_index/llms/huggingface/base.py
 
 import logging
 from threading import Thread
-from typing import Any, Callable, List, Optional, Sequence
+from typing import Any, Callable, List, Optional, Sequence, Literal
 
 import torch
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseGen,
     CompletionResponse,
@@ -90,15 +90,15 @@
         default=DEFAULT_HUGGINGFACE_MODEL,
         description=(
             "The name of the tokenizer to use from HuggingFace. "
             "Unused if `tokenizer` is passed in directly."
         ),
     )
     device_map: str = Field(
-        default="auto", description="The device_map to use. Defaults to 'auto'."
+        default="cpu", description="The device_map to use. Defaults to 'cpu'."
     )
     stopping_ids: List[int] = Field(
         default_factory=list,
         description=(
             "The stopping ids to use. "
             "Generation stops when these token IDs are predicted."
         ),
@@ -141,15 +141,15 @@
         max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
         tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
         model_name: str = DEFAULT_HUGGINGFACE_MODEL,
         load_in_4bit: Optional[bool] = True,
         load_in_low_bit: Optional[str] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
-        device_map: Optional[str] = "auto",
+        device_map: Literal["cpu", "xpu"] = "cpu",
         stopping_ids: Optional[List[int]] = None,
         tokenizer_kwargs: Optional[dict] = None,
         tokenizer_outputs_to_remove: Optional[list] = None,
         model_kwargs: Optional[dict] = None,
         generate_kwargs: Optional[dict] = None,
         is_chat_model: Optional[bool] = False,
         callback_manager: Optional[CallbackManager] = None,
@@ -167,15 +167,15 @@
             max_new_tokens: The maximum number of tokens to generate.
             tokenizer_name: The name of the tokenizer to use from HuggingFace.
                         Unused if `tokenizer` is passed in directly.
             model_name: The model name to use from HuggingFace.
                         Unused if `model` is passed in directly.
             model: The HuggingFace model.
             tokenizer: The tokenizer.
-            device_map: The device_map to use. Defaults to 'auto'.
+            device_map: The device_map to use. Defaults to 'cpu'.
             stopping_ids: The stopping ids to use.
                         Generation stops when these token IDs are predicted.
             tokenizer_kwargs: The kwargs to pass to the tokenizer.
             tokenizer_outputs_to_remove: The outputs to remove from the tokenizer.
                         Sometimes huggingface tokenizers return extra inputs that cause errors.
             model_kwargs: The kwargs to pass to the model during initialization.
             generate_kwargs: The kwargs to pass to the model during generation.
@@ -193,15 +193,19 @@
 
         if model:
             self._model = model
         else:
             self._model = self._load_model(
                 low_bit_model, load_in_4bit, load_in_low_bit, model_name, model_kwargs
             )
-
+        if device_map not in ["cpu", "xpu"]:
+            raise ValueError(
+                "IpexLLM currently only supports device to be 'cpu' or 'xpu', "
+                f"but you have: {device_map}."
+            )
         if "xpu" in device_map:
             self._model = self._model.to(device_map)
 
         # check context_window
         config_dict = self._model.config.to_dict()
         model_context_window = int(
             config_dict.get("max_position_embeddings", context_window)
@@ -284,15 +288,15 @@
         max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
         tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
         model_name: str = DEFAULT_HUGGINGFACE_MODEL,
         load_in_4bit: Optional[bool] = True,
         load_in_low_bit: Optional[str] = None,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
-        device_map: Optional[str] = "auto",
+        device_map: Literal["cpu", "xpu"] = "cpu",
         stopping_ids: Optional[List[int]] = None,
         tokenizer_kwargs: Optional[dict] = None,
         tokenizer_outputs_to_remove: Optional[list] = None,
         model_kwargs: Optional[dict] = None,
         generate_kwargs: Optional[dict] = None,
         is_chat_model: Optional[bool] = False,
         callback_manager: Optional[CallbackManager] = None,
@@ -330,15 +334,15 @@
         cls,
         context_window: int = DEFAULT_CONTEXT_WINDOW,
         max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
         tokenizer_name: str = DEFAULT_HUGGINGFACE_MODEL,
         model_name: str = DEFAULT_HUGGINGFACE_MODEL,
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
-        device_map: Optional[str] = "auto",
+        device_map: Literal["cpu", "xpu"] = "cpu",
         stopping_ids: Optional[List[int]] = None,
         tokenizer_kwargs: Optional[dict] = None,
         tokenizer_outputs_to_remove: Optional[list] = None,
         model_kwargs: Optional[dict] = None,
         generate_kwargs: Optional[dict] = None,
         is_chat_model: Optional[bool] = False,
         callback_manager: Optional[CallbackManager] = None,
```

### Comparing `llama_index_llms_ipex_llm-0.1.2/pyproject.toml` & `llama_index_llms_ipex_llm-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -26,21 +26,28 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ipex-llm integration"
 license = "MIT"
 name = "llama-index-llms-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.0"
-torch = "<2.2.0"
-ipex-llm = {allow-prereleases = true, extras = ["all"], version = "*"}
+ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240514"}
+torch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.0a0"}
+torchvision = {optional = true, source = "ipex-xpu-src-us", version = "0.16.0a0"}
+intel_extension_for_pytorch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.10+xpu"}
+bigdl-core-xe-21 = {optional = true, version = "*"}
+bigdl-core-xe-esimd-21 = {optional = true, version = "*"}
+
+[tool.poetry.extras]
+xpu = ["bigdl-core-xe-21", "bigdl-core-xe-esimd-21", "intel_extension_for_pytorch", "torch", "torchvision"]
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
@@ -52,7 +59,17 @@
 tree-sitter-languages = "^1.8.0"
 types-Deprecated = ">=0.1.0"
 types-PyYAML = "^6.0.12.12"
 types-protobuf = "^4.24.0.4"
 types-redis = "4.5.5.0"
 types-requests = "2.28.11.8"  # TODO: unpin when mypy>0.991
 types-setuptools = "67.1.0.0"
+
+[[tool.poetry.source]]
+name = "ipex-xpu-src-us"
+priority = "explicit"
+url = "https://pytorch-extension.intel.com/release-whl/stable/xpu/us/"
+
+[[tool.poetry.source]]
+name = "ipex-xpu-src-cn"
+priority = "supplemental"
+url = "https://pytorch-extension.intel.com/release-whl/stable/xpu/cn/"
```

### Comparing `llama_index_llms_ipex_llm-0.1.2/PKG-INFO` & `llama_index_llms_ipex_llm-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ipex-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index llms ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ipex-llm[all]
+Provides-Extra: xpu
+Requires-Dist: bigdl-core-xe-21 ; extra == "xpu"
+Requires-Dist: bigdl-core-xe-esimd-21 ; extra == "xpu"
+Requires-Dist: intel_extension_for_pytorch (==2.1.10+xpu) ; extra == "xpu"
+Requires-Dist: ipex-llm[llama-index] (>=2.1.0b20240514)
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
-Requires-Dist: torch (<2.2.0)
+Requires-Dist: torch (==2.1.0a0) ; extra == "xpu"
+Requires-Dist: torchvision (==0.16.0a0) ; extra == "xpu"
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: IPEX-LLM
 
 [IPEX-LLM](https://github.com/intel-analytics/ipex-llm) is a PyTorch library for running LLM on Intel CPU and GPU (e.g., local PC with iGPU, discrete GPU such as Arc, Flex and Max) with very low latency. This module enables the use of LLMs optimized with `ipex-llm` in LlamaIndex pipelines.
 
 ## Installation
 
 ### On CPU
 
 ```bash
 pip install llama-index-llms-ipex-llm
 ```
 
+### On GPU
+
+```bash
+pip install llama-index-llms-ipex-llm[xpu] --extra-index-url https://pytorch-extension.intel.com/release-whl/stable/xpu/us/
+```
+
 ## Usage
 
 ```python
 from llama_index.llms.ipex_llm import IpexLLM
 ```
 
 ## Examples
```

