# Comparing `tmp/amazon_bedrock_haystack-0.7.1.tar.gz` & `tmp/amazon_bedrock_haystack-0.8.0.tar.gz`

## Comparing `amazon_bedrock_haystack-0.7.1.tar` & `amazon_bedrock_haystack-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/examples/chatgenerator_example.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/examples/embedders_generator_with_rag_example.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/pydoc/config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/errors.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    13329 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
--rw-r--r--   0        0        0    23013 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_chat_generator.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_document_embedder.py
--rw-r--r--   0        0        0    41832 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_generator.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/README.md
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/examples/chatgenerator_example.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/examples/embedders_generator_with_rag_example.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/pydoc/config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/common/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/common/amazon_bedrock/errors.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/common/amazon_bedrock/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
+-rwxr-xr-x   0        0        0    12729 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
+-rwxr-xr-x   0        0        0     8621 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0    13329 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
+-rw-r--r--   0        0        0    23012 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/test_chat_generator.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0    41832 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/test_generator.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/README.md
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.8.0/PKG-INFO
```

### Comparing `amazon_bedrock_haystack-0.7.1/examples/chatgenerator_example.py` & `amazon_bedrock_haystack-0.8.0/examples/chatgenerator_example.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/examples/embedders_generator_with_rag_example.py` & `amazon_bedrock_haystack-0.8.0/examples/embedders_generator_with_rag_example.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/pydoc/config.yml` & `amazon_bedrock_haystack-0.8.0/pydoc/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Amazon Bedrock integration for Haystack
   category_slug: integrations-api
   title: Amazon Bedrock
   slug: integrations-amazon-bedrock
   order: 9
   markdown:
     descriptive_class_title: false
```

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/errors.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/common/amazon_bedrock/errors.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/utils.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/common/amazon_bedrock/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,20 @@
     AmazonBedrockConfigurationError,
     AmazonBedrockInferenceError,
 )
 from haystack_integrations.common.amazon_bedrock.utils import get_aws_session
 
 logger = logging.getLogger(__name__)
 
-SUPPORTED_EMBEDDING_MODELS = ["amazon.titan-embed-text-v1", "cohere.embed-english-v3", "cohere.embed-multilingual-v3"]
+SUPPORTED_EMBEDDING_MODELS = [
+    "amazon.titan-embed-text-v1",
+    "cohere.embed-english-v3",
+    "cohere.embed-multilingual-v3",
+    "amazon.titan-embed-text-v2:0",
+]
 
 
 @component
 class AmazonBedrockDocumentEmbedder:
     """
     A component for computing Document embeddings using Amazon Bedrock.
     The embedding of each Document is stored in the `embedding` field of the Document.
@@ -47,15 +52,20 @@
 
     # [0.002, 0.032, 0.504, ...]
     ```
     """
 
     def __init__(
         self,
-        model: Literal["amazon.titan-embed-text-v1", "cohere.embed-english-v3", "cohere.embed-multilingual-v3"],
+        model: Literal[
+            "amazon.titan-embed-text-v1",
+            "cohere.embed-english-v3",
+            "cohere.embed-multilingual-v3",
+            "amazon.titan-embed-text-v2:0",
+        ],
         aws_access_key_id: Optional[Secret] = Secret.from_env_var("AWS_ACCESS_KEY_ID", strict=False),  # noqa: B008
         aws_secret_access_key: Optional[Secret] = Secret.from_env_var(  # noqa: B008
             "AWS_SECRET_ACCESS_KEY", strict=False
         ),
         aws_session_token: Optional[Secret] = Secret.from_env_var("AWS_SESSION_TOKEN", strict=False),  # noqa: B008
         aws_region_name: Optional[Secret] = Secret.from_env_var("AWS_DEFAULT_REGION", strict=False),  # noqa: B008
         aws_profile_name: Optional[Secret] = Secret.from_env_var("AWS_PROFILE", strict=False),  # noqa: B008
```

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,20 @@
     AmazonBedrockConfigurationError,
     AmazonBedrockInferenceError,
 )
 from haystack_integrations.common.amazon_bedrock.utils import get_aws_session
 
 logger = logging.getLogger(__name__)
 
-SUPPORTED_EMBEDDING_MODELS = ["amazon.titan-embed-text-v1", "cohere.embed-english-v3", "cohere.embed-multilingual-v3"]
+SUPPORTED_EMBEDDING_MODELS = [
+    "amazon.titan-embed-text-v1",
+    "cohere.embed-english-v3",
+    "cohere.embed-multilingual-v3",
+    "amazon.titan-embed-text-v2:0",
+]
 
 
 @component
 class AmazonBedrockTextEmbedder:
     """
     A component for embedding strings using Amazon Bedrock.
 
@@ -40,15 +45,20 @@
 
     # {'embedding': [0.002, 0.032, 0.504, ...]}
     ```
     """
 
     def __init__(
         self,
-        model: Literal["amazon.titan-embed-text-v1", "cohere.embed-english-v3", "cohere.embed-multilingual-v3"],
+        model: Literal[
+            "amazon.titan-embed-text-v1",
+            "cohere.embed-english-v3",
+            "cohere.embed-multilingual-v3",
+            "amazon.titan-embed-text-v2:0",
+        ],
         aws_access_key_id: Optional[Secret] = Secret.from_env_var("AWS_ACCESS_KEY_ID", strict=False),  # noqa: B008
         aws_secret_access_key: Optional[Secret] = Secret.from_env_var(  # noqa: B008
             "AWS_SECRET_ACCESS_KEY", strict=False
         ),
         aws_session_token: Optional[Secret] = Secret.from_env_var("AWS_SESSION_TOKEN", strict=False),  # noqa: B008
         aws_region_name: Optional[Secret] = Secret.from_env_var("AWS_DEFAULT_REGION", strict=False),  # noqa: B008
         aws_profile_name: Optional[Secret] = Secret.from_env_var("AWS_PROFILE", strict=False),  # noqa: B008
```

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/generator.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
         # Use `mistralai/Mistral-7B-v0.1` as tokenizer, all mistral models likely use the same tokenizer
         # a) we should get good estimates for the prompt length
         # b) we can use apply_chat_template with the template above to delineate ChatMessages
         tokenizer: PreTrainedTokenizer = AutoTokenizer.from_pretrained("mistralai/Mistral-7B-Instruct-v0.1")
         self.prompt_handler = DefaultPromptHandler(
             tokenizer=tokenizer,
             model_max_length=model_max_length,
-            max_length=self.generation_kwargs.get("max_gen_len") or 512,
+            max_length=self.generation_kwargs.get("max_tokens") or 512,
         )
 
     def prepare_body(self, messages: List[ChatMessage], **inference_kwargs) -> Dict[str, Any]:
         """
         Prepares the body for the Mistral request.
 
         :param messages: The chat messages to package into the request.
```

### Comparing `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py` & `amazon_bedrock_haystack-0.8.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/tests/conftest.py` & `amazon_bedrock_haystack-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/tests/test_chat_generator.py` & `amazon_bedrock_haystack-0.8.0/tests/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/tests/test_document_embedder.py` & `amazon_bedrock_haystack-0.8.0/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/tests/test_generator.py` & `amazon_bedrock_haystack-0.8.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/tests/test_text_embedder.py` & `amazon_bedrock_haystack-0.8.0/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/.gitignore` & `amazon_bedrock_haystack-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/LICENSE.txt` & `amazon_bedrock_haystack-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/README.md` & `amazon_bedrock_haystack-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/pyproject.toml` & `amazon_bedrock_haystack-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.1/PKG-INFO` & `amazon_bedrock_haystack-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amazon-bedrock-haystack
-Version: 0.7.1
+Version: 0.8.0
 Summary: An integration of Amazon Bedrock as an AmazonBedrockGenerator component.
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

