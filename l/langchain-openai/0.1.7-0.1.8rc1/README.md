# Comparing `tmp/langchain_openai-0.1.7.tar.gz` & `tmp/langchain_openai-0.1.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.7.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.8rc1.tar", max compression
```

## Comparing `langchain_openai-0.1.7.tar` & `langchain_openai-0.1.8rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/LICENSE
--rw-r--r--   0        0        0     1627 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/README.md
--rw-r--r--   0        0        0      371 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10790 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    47309 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    22520 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24578 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/py.typed
--rw-r--r--   0        0        0     2839 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 langchain_openai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/README.md
+-rw-r--r--   0        0        0      371 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    11220 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    48383 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    24289 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8340 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24651 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2879 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 langchain_openai-0.1.8rc1/PKG-INFO
```

### Comparing `langchain_openai-0.1.7/LICENSE` & `langchain_openai-0.1.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.7/README.md` & `langchain_openai-0.1.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.7/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/chat_models/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import openai
+from langchain_core.language_models.chat_models import LangSmithParams
 from langchain_core.outputs import ChatResult
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 
 from langchain_openai.chat_models.base import BaseChatOpenAI
 
 logger = logging.getLogger(__name__)
@@ -76,15 +77,15 @@
     azure_ad_token: Optional[SecretStr] = None
     """Your Azure Active Directory token.
     
         Automatically inferred from env var `AZURE_OPENAI_AD_TOKEN` if not provided.
         
         For more: 
         https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id.
-    """  # noqa: E501
+    """
     azure_ad_token_provider: Union[Callable[[], str], None] = None
     """A function that returns an Azure Active Directory token.
         
         Will be invoked on every request.
     """
     model_version: str = ""
     """Legacy, for openai<1.0.0 support."""
@@ -173,15 +174,15 @@
                     "`base_url` (or alias `openai_api_base`) should not be. "
                     "If specifying `azure_deployment`/`deployment_name` then use "
                     "`azure_endpoint` instead of `base_url`.\n\n"
                     "For example, you could specify:\n\n"
                     'azure_endpoint="https://xxx.openai.azure.com/", '
                     'azure_deployment="my-deployment"\n\n'
                     "Or you can equivalently specify:\n\n"
-                    'base_url="https://xxx.openai.azure.com/openai/deployments/my-deployment"'  # noqa: E501
+                    'base_url="https://xxx.openai.azure.com/openai/deployments/my-deployment"'
                 )
         client_params = {
             "api_version": values["openai_api_version"],
             "azure_endpoint": values["azure_endpoint"],
             "azure_deployment": values["deployment_name"],
             "api_key": values["openai_api_key"].get_secret_value()
             if values["openai_api_key"]
@@ -224,14 +225,24 @@
     @property
     def lc_attributes(self) -> Dict[str, Any]:
         return {
             "openai_api_type": self.openai_api_type,
             "openai_api_version": self.openai_api_version,
         }
 
+    def _get_ls_params(
+        self, stop: Optional[List[str]] = None, **kwargs: Any
+    ) -> LangSmithParams:
+        """Get the parameters used to invoke the model."""
+        params = super()._get_ls_params(stop=stop, **kwargs)
+        params["ls_provider"] = "azure"
+        if self.deployment_name:
+            params["ls_model_name"] = self.deployment_name
+        return params
+
     def _create_chat_result(
         self, response: Union[dict, openai.BaseModel]
     ) -> ChatResult:
         if not isinstance(response, dict):
             response = response.model_dump()
         for res in response["choices"]:
             if res.get("finish_reason", None) == "content_filter":
```

### Comparing `langchain_openai-0.1.7/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/chat_models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
+    LangSmithParams,
     agenerate_from_stream,
     generate_from_stream,
 )
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
@@ -543,25 +544,31 @@
         # Sometimes the AI Model calling will get error, we should raise it.
         # Otherwise, the next code 'choices.extend(response["choices"])'
         # will throw a "TypeError: 'NoneType' object is not iterable" error
         # to mask the true error. Because 'response["choices"]' is None.
         if response.get("error"):
             raise ValueError(response.get("error"))
 
+        token_usage = response.get("usage", {})
         for res in response["choices"]:
             message = _convert_dict_to_message(res["message"])
+            if token_usage and isinstance(message, AIMessage):
+                message.usage_metadata = {
+                    "input_tokens": token_usage.get("prompt_tokens", 0),
+                    "output_tokens": token_usage.get("completion_tokens", 0),
+                    "total_tokens": token_usage.get("total_tokens", 0),
+                }
             generation_info = dict(finish_reason=res.get("finish_reason"))
             if "logprobs" in res:
                 generation_info["logprobs"] = res["logprobs"]
             gen = ChatGeneration(
                 message=message,
                 generation_info=generation_info,
             )
             generations.append(gen)
-        token_usage = response.get("usage", {})
         llm_output = {
             "token_usage": token_usage,
             "model_name": self.model_name,
             "system_fingerprint": response.get("system_fingerprint", ""),
         }
         return ChatResult(generations=generations, llm_output=llm_output)
 
@@ -635,14 +642,31 @@
         return {
             "model": self.model_name,
             **super()._get_invocation_params(stop=stop),
             **self._default_params,
             **kwargs,
         }
 
+    def _get_ls_params(
+        self, stop: Optional[List[str]] = None, **kwargs: Any
+    ) -> LangSmithParams:
+        """Get standard params for tracing."""
+        params = self._get_invocation_params(stop=stop, **kwargs)
+        ls_params = LangSmithParams(
+            ls_provider="openai",
+            ls_model_name=self.model_name,
+            ls_model_type="chat",
+            ls_temperature=params.get("temperature", self.temperature),
+        )
+        if ls_max_tokens := params.get("max_tokens", self.max_tokens):
+            ls_params["ls_max_tokens"] = ls_max_tokens
+        if ls_stop := stop or params.get("stop", None):
+            ls_params["ls_stop"] = ls_stop
+        return ls_params
+
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "openai-chat"
 
     def _get_encoding_model(self) -> Tuple[str, tiktoken.Encoding]:
         if self.tiktoken_model_name is not None:
```

### Comparing `langchain_openai-0.1.7/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/embeddings/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     azure_ad_token: Optional[SecretStr] = None
     """Your Azure Active Directory token.
 
         Automatically inferred from env var `AZURE_OPENAI_AD_TOKEN` if not provided.
 
         For more:
         https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id.
-    """  # noqa: E501
+    """
     azure_ad_token_provider: Union[Callable[[], str], None] = None
     """A function that returns an Azure Active Directory token.
 
         Will be invoked on every request.
     """
     openai_api_version: Optional[str] = Field(default=None, alias="api_version")
     """Automatically inferred from env var `OPENAI_API_VERSION` if not provided."""
```

### Comparing `langchain_openai-0.1.7/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/embeddings/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,75 @@
     get_from_dict_or_env,
     get_pydantic_field_names,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def _process_batched_chunked_embeddings(
+    num_texts: int,
+    tokens: List[Union[List[int], str]],
+    batched_embeddings: List[List[float]],
+    indices: List[int],
+    skip_empty: bool,
+) -> List[Optional[List[float]]]:
+    # for each text, this is the list of embeddings (list of list of floats)
+    # corresponding to the chunks of the text
+    results: List[List[List[float]]] = [[] for _ in range(num_texts)]
+
+    # for each text, this is the token length of each chunk
+    # for transformers tokenization, this is the string length
+    # for tiktoken, this is the number of tokens
+    num_tokens_in_batch: List[List[int]] = [[] for _ in range(num_texts)]
+
+    for i in range(len(indices)):
+        if skip_empty and len(batched_embeddings[i]) == 1:
+            continue
+        results[indices[i]].append(batched_embeddings[i])
+        num_tokens_in_batch[indices[i]].append(len(tokens[i]))
+
+    # for each text, this is the final embedding
+    embeddings: List[Optional[List[float]]] = []
+    for i in range(num_texts):
+        # an embedding for each chunk
+        _result: List[List[float]] = results[i]
+
+        if len(_result) == 0:
+            # this will be populated with the embedding of an empty string
+            # in the sync or async code calling this
+            embeddings.append(None)
+            continue
+
+        elif len(_result) == 1:
+            # if only one embedding was produced, use it
+            embeddings.append(_result[0])
+            continue
+
+        else:
+            # else we need to weighted average
+            # should be same as
+            # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
+            total_weight = sum(num_tokens_in_batch[i])
+            average = [
+                sum(
+                    val * weight
+                    for val, weight in zip(embedding, num_tokens_in_batch[i])
+                )
+                / total_weight
+                for embedding in zip(*_result)
+            ]
+
+            # should be same as
+            # embeddings.append((average / np.linalg.norm(average)).tolist())
+            magnitude = sum(val**2 for val in average) ** 0.5
+            embeddings.append([val / magnitude for val in average])
+
+    return embeddings
+
+
 class OpenAIEmbeddings(BaseModel, Embeddings):
     """OpenAI embedding models.
 
     To use, you should have the
     environment variable ``OPENAI_API_KEY`` set with your API key or pass it
     as a named parameter to the constructor.
 
@@ -244,17 +305,37 @@
         params: Dict = {"model": self.model, **self.model_kwargs}
         if self.dimensions is not None:
             params["dimensions"] = self.dimensions
         return params
 
     def _tokenize(
         self, texts: List[str], chunk_size: int
-    ) -> Tuple[Iterable[int], List[List[float]], List[int]]:
-        tokens = []
-        indices = []
+    ) -> Tuple[Iterable[int], List[Union[List[int], str]], List[int]]:
+        """
+        Take the input `texts` and `chunk_size` and return 3 iterables as a tuple:
+
+        We have `batches`, where batches are sets of individual texts
+        we want responses from the openai api. The length of a single batch is
+        `chunk_size` texts.
+
+        Each individual text is also split into multiple texts based on the
+        `embedding_ctx_length` parameter (based on number of tokens).
+
+        This function returns a 3-tuple of the following:
+
+        _iter: An iterable of the starting index in `tokens` for each *batch*
+        tokens: A list of tokenized texts, where each text has already been split
+            into sub-texts based on the `embedding_ctx_length` parameter. In the
+            case of tiktoken, this is a list of token arrays. In the case of
+            HuggingFace transformers, this is a list of strings.
+        indices: An iterable of the same length as `tokens` that maps each token-array
+            to the index of the original text in `texts`.
+        """
+        tokens: List[Union[List[int], str]] = []
+        indices: List[int] = []
         model_name = self.tiktoken_model_name or self.model
 
         # If tiktoken flag set to False
         if not self.tiktoken_enabled:
             try:
                 from transformers import AutoTokenizer
             except ImportError:
@@ -265,22 +346,24 @@
                 )
 
             tokenizer = AutoTokenizer.from_pretrained(
                 pretrained_model_name_or_path=model_name
             )
             for i, text in enumerate(texts):
                 # Tokenize the text using HuggingFace transformers
-                tokenized = tokenizer.encode(text, add_special_tokens=False)
+                tokenized: List[int] = tokenizer.encode(text, add_special_tokens=False)
 
                 # Split tokens into chunks respecting the embedding_ctx_length
                 for j in range(0, len(tokenized), self.embedding_ctx_length):
-                    token_chunk = tokenized[j : j + self.embedding_ctx_length]
+                    token_chunk: List[int] = tokenized[
+                        j : j + self.embedding_ctx_length
+                    ]
 
                     # Convert token IDs back to a string
-                    chunk_text = tokenizer.decode(token_chunk)
+                    chunk_text: str = tokenizer.decode(token_chunk)
                     tokens.append(chunk_text)
                     indices.append(i)
         else:
             try:
                 encoding = tiktoken.encoding_for_model(model_name)
             except KeyError:
                 encoding = tiktoken.get_encoding("cl100k_base")
@@ -347,51 +430,31 @@
             response = self.client.create(
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
             if not isinstance(response, dict):
                 response = response.model_dump()
             batched_embeddings.extend(r["embedding"] for r in response["data"])
 
-        results: List[List[List[float]]] = [[] for _ in range(len(texts))]
-        num_tokens_in_batch: List[List[int]] = [[] for _ in range(len(texts))]
-        for i in range(len(indices)):
-            if self.skip_empty and len(batched_embeddings[i]) == 1:
-                continue
-            results[indices[i]].append(batched_embeddings[i])
-            num_tokens_in_batch[indices[i]].append(len(tokens[i]))
-
-        embeddings: List[List[float]] = [[] for _ in range(len(texts))]
-        for i in range(len(texts)):
-            _result = results[i]
-            if len(_result) == 0:
+        embeddings = _process_batched_chunked_embeddings(
+            len(texts), tokens, batched_embeddings, indices, self.skip_empty
+        )
+        _cached_empty_embedding: Optional[List[float]] = None
+
+        def empty_embedding() -> List[float]:
+            nonlocal _cached_empty_embedding
+            if _cached_empty_embedding is None:
                 average_embedded = self.client.create(
                     input="", **self._invocation_params
                 )
                 if not isinstance(average_embedded, dict):
                     average_embedded = average_embedded.model_dump()
-                average = average_embedded["data"][0]["embedding"]
-            else:
-                # should be same as
-                # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
-                total_weight = sum(num_tokens_in_batch[i])
-                average = [
-                    sum(
-                        val * weight
-                        for val, weight in zip(embedding, num_tokens_in_batch[i])
-                    )
-                    / total_weight
-                    for embedding in zip(*_result)
-                ]
+                _cached_empty_embedding = average_embedded["data"][0]["embedding"]
+            return _cached_empty_embedding
 
-            # should be same as
-            #  embeddings[i] = (average / np.linalg.norm(average)).tolist()
-            magnitude = sum(val**2 for val in average) ** 0.5
-            embeddings[i] = [val / magnitude for val in average]
-
-        return embeddings
+        return [e if e is not None else empty_embedding() for e in embeddings]
 
     # please refer to
     # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
     async def _aget_len_safe_embeddings(
         self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
     ) -> List[List[float]]:
         """
@@ -419,48 +482,31 @@
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
 
             if not isinstance(response, dict):
                 response = response.model_dump()
             batched_embeddings.extend(r["embedding"] for r in response["data"])
 
-        results: List[List[List[float]]] = [[] for _ in range(len(texts))]
-        num_tokens_in_batch: List[List[int]] = [[] for _ in range(len(texts))]
-        for i in range(len(indices)):
-            results[indices[i]].append(batched_embeddings[i])
-            num_tokens_in_batch[indices[i]].append(len(tokens[i]))
-
-        embeddings: List[List[float]] = [[] for _ in range(len(texts))]
-        for i in range(len(texts)):
-            _result = results[i]
-            if len(_result) == 0:
+        embeddings = _process_batched_chunked_embeddings(
+            len(texts), tokens, batched_embeddings, indices, self.skip_empty
+        )
+        _cached_empty_embedding: Optional[List[float]] = None
+
+        async def empty_embedding() -> List[float]:
+            nonlocal _cached_empty_embedding
+            if _cached_empty_embedding is None:
                 average_embedded = await self.async_client.create(
                     input="", **self._invocation_params
                 )
                 if not isinstance(average_embedded, dict):
                     average_embedded = average_embedded.model_dump()
-                average = average_embedded["data"][0]["embedding"]
-            else:
-                # should be same as
-                # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
-                total_weight = sum(num_tokens_in_batch[i])
-                average = [
-                    sum(
-                        val * weight
-                        for val, weight in zip(embedding, num_tokens_in_batch[i])
-                    )
-                    / total_weight
-                    for embedding in zip(*_result)
-                ]
-            # should be same as
-            # embeddings[i] = (average / np.linalg.norm(average)).tolist()
-            magnitude = sum(val**2 for val in average) ** 0.5
-            embeddings[i] = [val / magnitude for val in average]
+                _cached_empty_embedding = average_embedded["data"][0]["embedding"]
+            return _cached_empty_embedding
 
-        return embeddings
+        return [e if e is not None else await empty_embedding() for e in embeddings]
 
     def embed_documents(
         self, texts: List[str], chunk_size: Optional[int] = 0
     ) -> List[List[float]]:
         """Call out to OpenAI's embedding endpoint for embedding search docs.
 
         Args:
```

### Comparing `langchain_openai-0.1.7/langchain_openai/llms/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/llms/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     azure_ad_token: Optional[SecretStr] = None
     """Your Azure Active Directory token.
 
         Automatically inferred from env var `AZURE_OPENAI_AD_TOKEN` if not provided.
 
         For more: 
         https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id.
-    """  # noqa: E501
+    """
     azure_ad_token_provider: Union[Callable[[], str], None] = None
     """A function that returns an Azure Active Directory token.
 
         Will be invoked on every request.
     """
     openai_api_type: str = ""
     """Legacy, for openai<1.0.0 support."""
```

### Comparing `langchain_openai-0.1.7/langchain_openai/llms/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/llms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,14 +533,16 @@
 
         Example:
             .. code-block:: python
 
                 max_tokens = openai.modelname_to_contextsize("gpt-3.5-turbo-instruct")
         """
         model_token_mapping = {
+            "gpt-4o": 128_000,
+            "gpt-4o-2024-05-13": 128_000,
             "gpt-4": 8192,
             "gpt-4-0314": 8192,
             "gpt-4-0613": 8192,
             "gpt-4-32k": 32768,
             "gpt-4-32k-0314": 32768,
             "gpt-4-32k-0613": 32768,
             "gpt-3.5-turbo": 4096,
```

### Comparing `langchain_openai-0.1.7/pyproject.toml` & `langchain_openai-0.1.8rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.7"
+version = "0.1.8rc1"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.1.46,<0.3"
+langchain-core = {version =">=0.2.2rc1,<0.3", allow-prereleases=true}
 openai = "^1.24.0"
 tiktoken = ">=0.7,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_openai-0.1.7/PKG-INFO` & `langchain_openai-0.1.8rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.7
+Version: 0.1.8rc1
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.46,<0.3)
+Requires-Dist: langchain-core (>=0.2.2rc1,<0.3)
 Requires-Dist: openai (>=1.24.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.7,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

