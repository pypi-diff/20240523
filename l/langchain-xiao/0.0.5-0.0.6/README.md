# Comparing `tmp/langchain_xiao-0.0.5.tar.gz` & `tmp/langchain_xiao-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_xiao-0.0.5.tar", last modified: Wed May 22 12:47:28 2024, max compression
+gzip compressed data, was "langchain_xiao-0.0.6.tar", last modified: Wed May 22 14:34:01 2024, max compression
```

## Comparing `langchain_xiao-0.0.5.tar` & `langchain_xiao-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.807890 langchain_xiao-0.0.5/
--rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.5/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      949 2024-05-22 12:47:28.806889 langchain_xiao-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.684379 langchain_xiao-0.0.5/langchain_xiao/
--rw-rw-rw-   0        0        0       23 2024-05-22 12:45:04.000000 langchain_xiao-0.0.5/langchain_xiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.749889 langchain_xiao-0.0.5/langchain_xiao/chat_models/
--rw-rw-rw-   0        0        0      136 2024-05-22 12:26:31.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/__init__.py
--rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/baichuan.py
--rw-rw-rw-   0        0        0     5452 2024-05-16 06:55:37.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/cyou.py
--rw-rw-rw-   0        0        0     9747 2024-05-22 12:40:27.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/hunyuan.py
--rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/llamacpp.py
--rw-rw-rw-   0        0        0     1255 2024-05-22 12:27:18.000000 langchain_xiao-0.0.5/langchain_xiao/chat_models/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.751890 langchain_xiao-0.0.5/langchain_xiao/embeddings/
--rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/embeddings/__init__.py
--rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/embeddings/fastllm.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.791890 langchain_xiao-0.0.5/langchain_xiao/llms/
--rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/llms/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/llms/gpt4all.py
--rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/langchain_xiao/llms/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.798890 langchain_xiao-0.0.5/langchain_xiao/retrievers/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.799890 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/
--rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/__init__.py
--rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.805889 langchain_xiao-0.0.5/langchain_xiao.egg-info/
--rw-rw-rw-   0        0        0      949 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 12:47:28.000000 langchain_xiao-0.0.5/langchain_xiao.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 12:47:28.807890 langchain_xiao-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 12:47:28.804890 langchain_xiao-0.0.5/tests/
--rw-rw-rw-   0        0        0     1255 2024-05-22 12:38:55.000000 langchain_xiao-0.0.5/tests/chat_models_utils.py
--rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/fastllm_embeddings.py
--rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/fastllm_rerank.py
--rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.5/tests/llms_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.959576 langchain_xiao-0.0.6/
+-rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      949 2024-05-22 14:34:01.958575 langchain_xiao-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.932575 langchain_xiao-0.0.6/langchain_xiao/
+-rw-rw-rw-   0        0        0       23 2024-05-22 14:30:26.000000 langchain_xiao-0.0.6/langchain_xiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.944575 langchain_xiao-0.0.6/langchain_xiao/chat_models/
+-rw-rw-rw-   0        0        0      172 2024-05-22 14:03:20.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/__init__.py
+-rw-rw-rw-   0        0        0     3121 2024-05-22 14:28:21.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/baichuan.py
+-rw-rw-rw-   0        0        0     5452 2024-05-16 06:55:37.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/cyou.py
+-rw-rw-rw-   0        0        0     9939 2024-05-22 14:01:09.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/hunyuan.py
+-rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/llamacpp.py
+-rw-rw-rw-   0        0        0     1166 2024-05-22 14:00:38.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/tongyi.py
+-rw-rw-rw-   0        0        0     1194 2024-05-22 14:02:48.000000 langchain_xiao-0.0.6/langchain_xiao/chat_models/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.946575 langchain_xiao-0.0.6/langchain_xiao/embeddings/
+-rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/embeddings/fastllm.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.949575 langchain_xiao-0.0.6/langchain_xiao/llms/
+-rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/llms/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/llms/gpt4all.py
+-rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.6/langchain_xiao/llms/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.950575 langchain_xiao-0.0.6/langchain_xiao/retrievers/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.952576 langchain_xiao-0.0.6/langchain_xiao/retrievers/document_compressors/
+-rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/retrievers/document_compressors/__init__.py
+-rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.6/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.957576 langchain_xiao-0.0.6/langchain_xiao.egg-info/
+-rw-rw-rw-   0        0        0      949 2024-05-22 14:34:01.000000 langchain_xiao-0.0.6/langchain_xiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      967 2024-05-22 14:34:01.000000 langchain_xiao-0.0.6/langchain_xiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:34:01.000000 langchain_xiao-0.0.6/langchain_xiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-22 14:34:01.000000 langchain_xiao-0.0.6/langchain_xiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 14:34:01.000000 langchain_xiao-0.0.6/langchain_xiao.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:34:01.959576 langchain_xiao-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 14:34:01.956576 langchain_xiao-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1527 2024-05-22 14:29:58.000000 langchain_xiao-0.0.6/tests/chat_models_utils.py
+-rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.6/tests/fastllm_embeddings.py
+-rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.6/tests/fastllm_rerank.py
+-rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.6/tests/llms_utils.py
```

### Comparing `langchain_xiao-0.0.5/.gitignore` & `langchain_xiao-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/LICENSE` & `langchain_xiao-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/PKG-INFO` & `langchain_xiao-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.5
+Version: 0.0.6
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.5/langchain_xiao/chat_models/baichuan.py` & `langchain_xiao-0.0.6/langchain_xiao/llms/gpt4all.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from typing import List, Optional, Any, Iterator
+from functools import partial
+from typing import Optional, List, Any
 
-from langchain_community.chat_models.baichuan import ChatBaichuan
+from langchain_community.llms import GPT4All
 from langchain_core.callbacks import CallbackManagerForLLMRun
-from langchain_core.messages import BaseMessage
-from langchain_core.outputs import ChatGenerationChunk
 
+from langchain_community.llms.utils import enforce_stop_tokens
 
-class MyChatBaichuan(ChatBaichuan):
-    def _stream(
+
+class MyGPT4All(GPT4All):
+    def _call(
         self,
-        messages: List[BaseMessage],
+        prompt: str,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
-    ) -> Iterator[ChatGenerationChunk]:
-        # 调用stream和astream时，必须手动在kwargs里添加上stream=True才行
-        kwargs.update({"stream": True})
-        return super()._stream(messages, **kwargs)
+    ) -> str:
+        text_callback = None
+        if run_manager:
+            text_callback = partial(run_manager.on_llm_new_token, verbose=self.verbose)
+        text = ""
+        params = {**self._default_params(), **kwargs}
+        with self.client.chat_session():    # 新增行，解决输出异常
+            for token in self.client.generate(prompt, **params):
+                if text_callback:
+                    text_callback(token)
+                text += token
+        if stop is not None:
+            text = enforce_stop_tokens(text, stop)
+        return text
```

### Comparing `langchain_xiao-0.0.5/langchain_xiao/chat_models/cyou.py` & `langchain_xiao-0.0.6/langchain_xiao/chat_models/cyou.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/langchain_xiao/chat_models/hunyuan.py` & `langchain_xiao-0.0.6/langchain_xiao/chat_models/hunyuan.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,25 @@
 def _create_chat_result(response) -> ChatResult:
     generations = []
     for choice in response.Choices:
         message = _convert_dict_to_message(choice.Message)
         generations.append(ChatGeneration(message=message))
 
     token_usage = response.Usage
-    llm_output = {"token_usage": token_usage}
+    llm_output = {
+        "token_usage": {
+            "prompt_tokens": token_usage.PromptTokens,
+            "completion_tokens": token_usage.CompletionTokens,
+            "total_tokens": token_usage.TotalTokens
+        }
+    }
     return ChatResult(generations=generations, llm_output=llm_output)
 
 
-class ChatHunyuan(BaseChatModel):
+class MyChatHunyuan(BaseChatModel):
     """Tencent Hunyuan chat models API by Tencent.
 
     For more information, see https://cloud.tencent.com/document/product/1729
     """
 
     @property
     def lc_secrets(self) -> Dict[str, str]:
```

### Comparing `langchain_xiao-0.0.5/langchain_xiao/chat_models/llamacpp.py` & `langchain_xiao-0.0.6/langchain_xiao/chat_models/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/langchain_xiao/chat_models/utils.py` & `langchain_xiao-0.0.6/langchain_xiao/chat_models/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from typing import Any
 
 from langchain_core.language_models import BaseChatModel
 
 
 XIAO_CHAT_MODELS = [
     "ChatLlamaCpp",
+    "MyChatTongyi",
     "MyChatBaichuan",
-    "ChatHunyuan",
+    "MyChatHunyuan",
     "ChatCyou"
 ]
 
 
 def get_chat_model(instance_type: str, **model_kwargs: Any) -> BaseChatModel:
     if instance_type == "ChatOpenAI":
         try:
@@ -19,22 +20,20 @@
         except ImportError:
             raise ImportError(
                 "Could not import langchain_openai python package. "
                 "Please install it with `pip install langchain_openai`."
             )
         model = ChatOpenAI(**model_kwargs)
 
-    elif instance_type == "ChatTongyi":
-        from langchain_community.chat_models import ChatTongyi
-        model = ChatTongyi(**model_kwargs)
-        model.model_name = model_kwargs["model_name"]
-
     else:
         if instance_type in XIAO_CHAT_MODELS:
             chat_models_module = importlib.import_module("langchain_xiao.chat_models")
         else:
             chat_models_module = importlib.import_module("langchain_community.chat_models")
 
         ChatModel = getattr(chat_models_module, instance_type)
         model = ChatModel(**model_kwargs)
 
+        if instance_type in ["ChatTongyi", "MyChatTongyi"]:
+            model.model_name = model_kwargs["model_name"]
+
     return model
```

### Comparing `langchain_xiao-0.0.5/langchain_xiao/embeddings/fastllm.py` & `langchain_xiao-0.0.6/langchain_xiao/embeddings/fastllm.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/langchain_xiao/llms/utils.py` & `langchain_xiao-0.0.6/langchain_xiao/llms/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py` & `langchain_xiao-0.0.6/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/langchain_xiao.egg-info/PKG-INFO` & `langchain_xiao-0.0.6/langchain_xiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.5
+Version: 0.0.6
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.5/langchain_xiao.egg-info/SOURCES.txt` & `langchain_xiao-0.0.6/langchain_xiao.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 langchain_xiao.egg-info/requires.txt
 langchain_xiao.egg-info/top_level.txt
 langchain_xiao/chat_models/__init__.py
 langchain_xiao/chat_models/baichuan.py
 langchain_xiao/chat_models/cyou.py
 langchain_xiao/chat_models/hunyuan.py
 langchain_xiao/chat_models/llamacpp.py
+langchain_xiao/chat_models/tongyi.py
 langchain_xiao/chat_models/utils.py
 langchain_xiao/embeddings/__init__.py
 langchain_xiao/embeddings/fastllm.py
 langchain_xiao/llms/__init__.py
 langchain_xiao/llms/gpt4all.py
 langchain_xiao/llms/utils.py
 langchain_xiao/retrievers/__init__.py
```

### Comparing `langchain_xiao-0.0.5/pyproject.toml` & `langchain_xiao-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.5/tests/fastllm_rerank.py` & `langchain_xiao-0.0.6/tests/fastllm_rerank.py`

 * *Files identical despite different names*

