# Comparing `tmp/easytl-0.4.0a2.tar.gz` & `tmp/easytl-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.4.0a2.tar", last modified: Mon May 20 06:31:54 2024, max compression
+gzip compressed data, was "easytl-0.4.0a3.tar", last modified: Thu May 23 01:24:54 2024, max compression
```

## Comparing `easytl-0.4.0a2.tar` & `easytl-0.4.0a3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.410033 easytl-0.4.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.406033 easytl-0.4.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.406033 easytl-0.4.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-20 06:30:09.000000 easytl-0.4.0a2/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-20 06:30:09.000000 easytl-0.4.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-20 06:30:09.000000 easytl-0.4.0a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-20 06:31:54.410033 easytl-0.4.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-20 06:30:09.000000 easytl-0.4.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-20 06:30:09.000000 easytl-0.4.0a2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 06:30:09.000000 easytl-0.4.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:31:54.410033 easytl-0.4.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.406033 easytl-0.4.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.410033 easytl-0.4.0a2/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/anthropic_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    94108 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    37175 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-20 06:30:09.000000 easytl-0.4.0a2/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.410033 easytl-0.4.0a2/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-20 06:31:54.000000 easytl-0.4.0a2/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-20 06:31:54.000000 easytl-0.4.0a2/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:31:54.000000 easytl-0.4.0a2/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 06:31:54.000000 easytl-0.4.0a2/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 06:31:54.000000 easytl-0.4.0a2/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:31:54.410033 easytl-0.4.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-20 06:30:09.000000 easytl-0.4.0a2/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-20 06:30:09.000000 easytl-0.4.0a2/tests/passing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-20 06:30:09.000000 easytl-0.4.0a2/tests/simple_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-23 01:23:17.000000 easytl-0.4.0a3/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-23 01:23:17.000000 easytl-0.4.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-23 01:23:17.000000 easytl-0.4.0a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-23 01:24:54.253780 easytl-0.4.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-23 01:23:17.000000 easytl-0.4.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-23 01:23:17.000000 easytl-0.4.0a3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 01:23:17.000000 easytl-0.4.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:24:54.253780 easytl-0.4.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.249780 easytl-0.4.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/anthropic_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96843 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39556 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 01:23:17.000000 easytl-0.4.0a3/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 01:24:54.000000 easytl-0.4.0a3/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:24:54.253780 easytl-0.4.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 01:23:17.000000 easytl-0.4.0a3/tests/simple_test.py
```

### Comparing `easytl-0.4.0a2/.github/workflows/workflow.yml` & `easytl-0.4.0a3/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/.gitignore` & `easytl-0.4.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/LICENSE.md` & `easytl-0.4.0a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/PKG-INFO` & `easytl-0.4.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.4.0a2/README.md` & `easytl-0.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/pyproject.toml` & `easytl-0.4.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "backoff==2.2.1",
     "tiktoken==0.6.0",
     "google-cloud-translate==3.15.3",
     "anthropic==0.26.0"
 ]
 
 name = "easytl"
-version = "v0.4.0-alpha-2"
+version = "v0.4.0-alpha-3"
 authors = [
   { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easytl-0.4.0a2/src/easytl/__init__.py` & `easytl-0.4.0a3/src/easytl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "EasyTL",
     "Language", "SplitSentences", "Formality", "GlossaryInfo", "TextResult",
     "Message", "SystemTranslationMessage", "ModelTranslationMessage",
     "ChatCompletion",
     "GenerateContentResponse", "AsyncGenerateContentResponse", "GenerationConfig",
     "AnthropicMessage","AnthropicTextBlock", "AnthropicToolsBetaMessage", "AnthropicToolUseBlock",
     "NOT_GIVEN","NotGiven",
-    "MODEL_COSTS", "ALLOWED_GEMINI_MODELS", "ALLOWED_OPENAI_MODELS", "ALLOWED_ANTHROPIC_MODELS", "VALID_JSON_OPENAI_MODELS", "VALID_JSON_GEMINI_MODELS", "VALID_JSON_ANTHROPIC_MODELS",
+    "MODEL_COSTS", "ALLOWED_GEMINI_MODELS", "ALLOWED_OPENAI_MODELS", "ALLOWED_ANTHROPIC_MODELS", "VALID_JSON_OPENAI_MODELS", "VALID_JSON_GEMINI_MODELS", "VALID_JSON_ANTHROPIC_MODELS", "MODEL_MAX_TOKENS",
     "DeepLException",
     "GoogleAPIError",
     "OpenAIError",
     "AnthropicError",
     "OpenAIAPIError", "OpenAIConflictError", "OpenAINotFoundError", "OpenAIAPIStatusError", "OpenAIRateLimitError", "OpenAIAPITimeoutError", "OpenAIBadRequestError", "OpenAIAPIConnectionError", "OpenAIAuthenticationError", "OpenAIInternalServerError", "OpenAIPermissionDeniedError", "OpenAIUnprocessableEntityError", "OpenAIAPIResponseValidationError",
     "DeepLAuthorizationException", "DeepLQuotaExceededException", "DeepLConnectionException", "DeepLTooManyRequestsException", "DeepLDocumentNotReadyException", "DeepLGlossaryNotFoundException", "DeepLDocumentTranslationException",
     "GoogleAuthError", "GoogleDefaultCredentialsError",
```

### Comparing `easytl-0.4.0a2/src/easytl/anthropic_service.py` & `easytl-0.4.0a3/src/easytl/anthropic_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/classes.py` & `easytl-0.4.0a3/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/decorators.py` & `easytl-0.4.0a3/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/deepl_service.py` & `easytl-0.4.0a3/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/easytl.py` & `easytl-0.4.0a3/src/easytl/easytl.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .openai_service import OpenAIService
 from .googletl_service import GoogleTLService
 from .anthropic_service import AnthropicService
 
 from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion, AnthropicMessage, AnthropicToolsBetaMessage, AnthropicTextBlock, AnthropicToolUseBlock
 from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException, AnthropicError
 
-from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings
+from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings, _validate_text_length
 
 class EasyTL:
 
     """
     
     EasyTL global client, used to interact with Translation APIs.
 
@@ -583,15 +583,15 @@
 ##-------------------start-of-gemini_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def gemini_translate(text:typing.Union[str, typing.Iterable[str]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
-                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                        response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                         response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                         translation_delay:float | None = None,
                         translation_instructions:str | None = None,
                         model:str="gemini-pro",
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
@@ -611,44 +611,46 @@
         It is not known whether Gemini has backoff retrying implemented. Assume it does not exist. 
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a GenerateContentResponse object, 'json' returns a json-parseable string.
-        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a GenerateContentResponse object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, a GenerateContentResponse object, but with the content as a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json' or 'json_raw'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
-        model (string) : The model to use. 
+        model (string) : The model to use. (E.g. 'gemini-pro' or 'gemini-pro-1.5-latest')
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
-        stop_sequences (list or None) : The sequences to stop at.
+        stop_sequences (list or None) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
         result (string or list - string or GenerateContentResponse or list - GenerateContentResponse) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
+        _validate_text_length(text, model, service="gemini")
+
         response_schema = _validate_response_schema(response_schema)
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("gemini")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
@@ -667,37 +669,37 @@
             GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
         
         if(isinstance(text, str)):
             _result = GeminiService._translate_text(text)
             
             assert not isinstance(_result, list) and hasattr(_result, "text"), EasyTLException("Malformed response received. Please try again.")
             
-            result = _result if response_type == "raw" else _result.text
+            result = _result if response_type in ["raw", "raw_json"] else _result.text
 
         elif(_is_iterable_of_strings(text)):
             
             _results = [GeminiService._translate_text(t) for t in text]
 
             assert isinstance(_results, list) and all([hasattr(_r, "text") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
 
-            result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
+            result = [_r.text for _r in _results] if response_type in ["text","json"] else _results # type: ignore
             
         else:
             raise InvalidTextInputException("text must be a string or an iterable of strings.")
         
         return result
 
 ##-------------------start-of-gemini_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def gemini_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
-                                    response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                    response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                     response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                                     semaphore:int | None = None,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | None = None,
                                     model:str="gemini-pro",
                                     temperature:float=0.5,
                                     top_p:float=0.9,
@@ -721,45 +723,47 @@
         It is not known whether Gemini has backoff retrying implemented. Assume it does not exist.
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a AsyncGenerateContentResponse object, 'json' returns a json-parseable string.
-        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AsyncGenerateContentResponse object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, an AsyncGenerateContentResponse object, but with the content as a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json' or 'json_raw'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
         semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models. For Gemini, it is recommend to use translation_delay along with the semaphore to prevent rate limiting.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
-        model (string) : The model to use.
+        model (string) : The model to use. (E.g. 'gemini-pro' or 'gemini-pro-1.5-latest')
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
-        stop_sequences (list or None) : The sequences to stop at.
+        stop_sequences (list or None) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
         result (string or list - string or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AsyncGenerateContentResponse objects if the response type is 'raw' and input was an iterable, a AsyncGenerateContentResponse object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
+        _validate_text_length(text, model, service="gemini")
+
         response_schema = _validate_response_schema(response_schema)
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("gemini")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
@@ -776,35 +780,35 @@
             
             ## Done afterwards, cause default translation instructions can change based on set_attributes()
             GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
             
         if(isinstance(text, str)):
             _result = await GeminiService._translate_text_async(text)
 
-            result = _result if response_type == "raw" else _result.text
+            result = _result if response_type in ["raw", "raw_json"] else _result.text
             
         elif(_is_iterable_of_strings(text)):
             _tasks = [GeminiService._translate_text_async(_t) for _t in text]
             _results = await asyncio.gather(*_tasks)
 
-            result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
+            result = [_r.text for _r in _results] if response_type in ["text","json"] else _results # type: ignore
 
         else:
             raise InvalidTextInputException("text must be a string or an iterable of strings.")
         
         return result
             
 ##-------------------start-of-openai_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def openai_translate(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
-                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                        response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                         translation_delay:float | None = None,
                         translation_instructions:str | SystemTranslationMessage | None = None,
                         model:str="gpt-4",
                         temperature:float=0.3,
                         top_p:float=1.0,
                         stop:typing.List[str] | None=None,
                         max_tokens:int | None=None,
@@ -823,41 +827,44 @@
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, a ChatCompletion object, but with the content as a json-parseable string.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
+        model (string) : The model to use. (E.g. 'gpt-4', 'gpt-3.5-turbo-0125', 'gpt-4o', etc.)
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
-        stop (list or None) : The sequences to stop at.
+        stop (list or None) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_tokens (int or None) : The maximum number of tokens to output.
-        presence_penalty (float) : The presence penalty to use.
-        frequency_penalty (float) : The frequency penalty to use.
+        presence_penalty (float) : The presence penalty to use. This penalizes the model from repeating the same content in the output. Shouldn't be messed with for translation.
+        frequency_penalty (float) : The frequency penalty to use. This penalizes the model from using the same words too frequently in the output. Shouldn't be messed with for translation.
 
         Returns:
         result (string or list - string or ChatCompletion or list - ChatCompletion) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
+        _validate_text_length(text, model, service="openai")
+
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("openai")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
         
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
                                         top_p=top_p,
                                         n=1,
@@ -885,15 +892,15 @@
         
         for _text, _translation_instructions in translation_batches:
 
             _result = OpenAIService._translate_text(_translation_instructions, _text)
 
             assert not isinstance(_result, list) and hasattr(_result, "choices"), EasyTLException("Malformed response received. Please try again.")
 
-            translation = _result if response_type == "raw" else _result.choices[0].message.content
+            translation = _result if response_type in ["raw", "raw_json"] else _result.choices[0].message.content
             
             translations.append(translation)
         
         ## If originally a single text was provided, return a single translation instead of a list
         result = translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
         
         return result
@@ -901,15 +908,15 @@
 ##-------------------start-of-openai_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def openai_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
-                                    response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                    response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                     semaphore:int | None = None,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | SystemTranslationMessage | None = None,
                                     model:str="gpt-4",
                                     temperature:float=0.3,
                                     top_p:float=1.0,
                                     stop:typing.List[str] | None=None,
@@ -930,43 +937,45 @@
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, a ChatCompletion object, but with the content as a json-parseable string.
         semaphore (int) : The number of concurrent requests to make. Default is 5.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
-        model (string) : The model to use.
+        model (string) : The model to use. (E.g. 'gpt-4', 'gpt-3.5-turbo-0125', 'gpt-4o', etc.)
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
-        stop (list or None) : The sequences to stop at.
+        stop (list or None) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_tokens (int or None) : The maximum number of tokens to output.
-        presence_penalty (float) : The presence penalty to use.
-        frequency_penalty (float) : The frequency penalty to use.
+        presence_penalty (float) : The presence penalty to use. This penalizes the model from repeating the same content in the output. Shouldn't be messed with for translation.
+        frequency_penalty (float) : The frequency penalty to use. This penalizes the model from using the same words too frequently in the output. Shouldn't be messed with for translation.
 
         Returns:
         result (string or list - string or ChatCompletion or list - ChatCompletion) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise.
         
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_openai_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "openai")
 
         _validate_stop_sequences(stop)
 
+        _validate_text_length(text, model, service="openai")
+
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("openai")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
 
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
                                         top_p=top_p,
                                         n=1,
@@ -998,28 +1007,28 @@
 
         _results = await asyncio.gather(*_translation_tasks)
 
         _results:typing.List[ChatCompletion] = _results
 
         assert all([hasattr(_r, "choices") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
 
-        translation = _results if response_type == "raw" else [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
+        translation = _results if response_type in ["raw","raw_json"] else [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
 
         result = translation if isinstance(text, typing.Iterable) and not isinstance(text, str) else translation[0]
 
         return result
     
 ##-------------------start-of-anthropic_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def anthropic_translate(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                             override_previous_settings:bool = True,
                             decorator:typing.Callable | None = None,
                             logging_directory:str | None = None,
-                            response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                            response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                             response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                             translation_delay:float | None = None,
                             translation_instructions:str | None = None,
                             model:str="claude-3-haiku-20240307",
                             temperature:float | NotGiven = NOT_GIVEN,
                             top_p:float | NotGiven = NOT_GIVEN,
                             top_k:int | NotGiven = NOT_GIVEN,
@@ -1043,44 +1052,46 @@
         Anthropic's JSON response is quite unsophisticated and also in Beta, it costs a lot of extra tokens to return a json response. It's also inconsistent. Be careful when using it.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Anthropic translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, Anthropic will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. Anthropic's API is unsophisticated in this regard, it costs a lot of extra tokens to return a json response.
-        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json. 
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, an AnthropicMessage object, but with the content as a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json' or 'json_raw'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json. 
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
-        model (string) : The model to use.
+        model (string) : The model to use. (E.g. 'claude-3-haiku-20240307', 'claude-3-sonnet-20240229' or 'claude-3-opus-20240229')
         temperature (float or NotGiven) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float or NotGiven) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int or NotGiven) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
-        stop_sequences (list or NotGiven) : The sequences to stop at.
+        stop_sequences (list or NotGiven) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_output_tokens (int or NotGiven) : The maximum number of tokens to output.
 
         Returns:
         result (string or list - string or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_anthropic_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "anthropic")
 
         _validate_stop_sequences(stop_sequences)
 
+        _validate_text_length(text, model, service="anthropic")
+
         response_schema = _validate_response_schema(response_schema)
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("anthropic")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
 
         if(override_previous_settings == True):
             AnthropicService._set_attributes(model=model,
                                             system=translation_instructions,
                                             temperature=temperature,
                                             top_p=top_p,
                                             top_k=top_k,
@@ -1105,15 +1116,15 @@
 
         for _text in _translation_batches:
 
             _result = AnthropicService._translate_text(AnthropicService._system, _text)
 
             assert not isinstance(_result, list) and hasattr(_result, "content"), EasyTLException("Malformed response received. Please try again.")
 
-            if(response_type == "raw"):
+            if(response_type in ["raw", "raw_json"]):
                 translation = _result
 
             ## response structure is different for beta
             elif(isinstance(_result, AnthropicToolsBetaMessage)):
                 content = _result.content
 
                 if(isinstance(content[0], AnthropicTextBlock)):
@@ -1135,15 +1146,15 @@
 ##-------------------start-of-anthropic_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def anthropic_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                         override_previous_settings:bool = True,
                                         decorator:typing.Callable | None = None,
                                         logging_directory:str | None = None,
-                                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                        response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                         response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                                         semaphore:int | None = None,
                                         translation_delay:float | None = None,
                                         translation_instructions:str | None = None,
                                         model:str="claude-3-haiku-20240307",
                                         temperature:float | NotGiven = NOT_GIVEN,
                                         top_p:float | NotGiven = NOT_GIVEN,
@@ -1170,45 +1181,47 @@
         Anthropic's JSON response is quite unsophisticated and also in Beta, it costs a lot of extra tokens to return a json response. It's also inconsistent. Be careful when using it.
 
         Parameters:
         text (string | ModelTranslationMessage or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Anthropic translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, Anthropic will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
-        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. Anthropic's API is unsophisticated in this regard, it costs a lot of extra tokens to return a json response.
-        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
+        response_type (literal["text", "raw", "json", "raw_json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. 'raw_json' returns the raw response, an AnthropicMessage object, but with the content as a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json' or 'json_raw'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
         semaphore (int) : The number of concurrent requests to make. Default is 5.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
-        model (string) : The model to use.
+        model (string) : The model to use. (E.g. 'claude-3-haiku-20240307', 'claude-3-sonnet-20240229' or 'claude-3-opus-20240229')
         temperature (float or NotGiven) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float or NotGiven) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int or NotGiven) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
-        stop_sequences (list or NotGiven) : The sequences to stop at.
+        stop_sequences (list or NotGiven) : String sequences that will cause the model to stop translating if encountered, generally useless.
         max_output_tokens (int or NotGiven) : The maximum number of tokens to output.
 
         Returns:
         result (string or list - string or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+        assert response_type in ["text", "raw", "json", "raw_json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw', 'json' or 'raw_json'.")
 
         _settings = _return_curated_anthropic_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "anthropic")
 
         _validate_stop_sequences(stop_sequences)
 
+        _validate_text_length(text, model, service="anthropic")
+
         response_schema = _validate_response_schema(response_schema)
 
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("anthropic")
 
-        json_mode = True if response_type == "json" else False
+        json_mode = True if response_type in ["json", "raw_json"] else False
 
         if(override_previous_settings == True):
             AnthropicService._set_attributes(model=model,
                                             system=translation_instructions,
                                             temperature=temperature,
                                             top_p=top_p,
                                             top_k=top_k,
@@ -1237,15 +1250,15 @@
 
         _results = await asyncio.gather(*_translations_tasks)
 
         _results:typing.List[AnthropicMessage | AnthropicToolsBetaMessage] = _results
 
         assert all([hasattr(_r, "content") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
 
-        if(response_type == "raw"):
+        if(response_type in ["raw", "raw_json"]):
             translations = _results
 
         ## response structure is different for beta
         elif(isinstance(_results[0], AnthropicToolsBetaMessage)):
             translations = [result.content[0].input if isinstance(result.content[0], AnthropicToolUseBlock) else result.content[0].text for result in _results]
         
         elif(isinstance(_results[0], AnthropicMessage)):
```

### Comparing `easytl-0.4.0a2/src/easytl/exceptions.py` & `easytl-0.4.0a3/src/easytl/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,8 +129,27 @@
         """
 
         Parameters:
         message (string) : The message to display when the exception is raised.
 
         """
 
+        self.message = message
+
+class TooManyInputTokensException(EasyTLException):
+
+    """
+
+    TooManyInputTokensException is an exception that is raised when the input text contains too many tokens to be accepted by the API
+
+    """
+
+    def __init__(self, message:str) -> None:
+
+        """
+
+        Parameters:
+        message (string) : The message to display when the exception is raised.
+
+        """
+
         self.message = message
```

### Comparing `easytl-0.4.0a2/src/easytl/gemini_service.py` & `easytl-0.4.0a3/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/googletl_service.py` & `easytl-0.4.0a3/src/easytl/googletl_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         except Exception as _e:
 
             return _validity, _e
         
 ##-------------------start-of-_calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
-    @_redefine_client_decorator
     def _calculate_cost(text:str | typing.Iterable) -> typing.Tuple[int, float, str]:
 
         """
 
         Calculates the cost of the translation.
 
         Parameters:
```

### Comparing `easytl-0.4.0a2/src/easytl/openai_service.py` & `easytl-0.4.0a3/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/src/easytl/util.py` & `easytl-0.4.0a3/src/easytl/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 ## third-party libraries
 import tiktoken
 import backoff
 
 ## custom modules
 import google.generativeai as genai
 
-from .exceptions import InvalidEasyTLSettingsException, GoogleAPIError
-from .classes import NotGiven, NOT_GIVEN
+from .exceptions import InvalidEasyTLSettingsException, GoogleAPIError, TooManyInputTokensException
+from .classes import NotGiven, NOT_GIVEN, ModelTranslationMessage
 
 ##-------------------start-of-_return_curated_anthropic_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _return_curated_anthropic_settings(local_settings:dict[str, typing.Any]) -> dict:
 
     """
 
@@ -137,23 +137,84 @@
             return response_schema
         
         except (TypeError, OverflowError):
             raise InvalidEasyTLSettingsException("Invalid response_schema. Must be a valid JSON object or None.")
 
     raise InvalidEasyTLSettingsException("Invalid response_schema. Must be a valid JSON, a valid JSON string, or None.")
 
+
+##-------------------start-of-validate_text_length()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _validate_text_length(text:str | typing.Iterable[str] | ModelTranslationMessage | typing.Iterable[ModelTranslationMessage] , model:str, service:str) -> None:
+
+    """
+
+    Validates the length of the input text.
+
+    Parameters:
+    text (string | typing.Iterable[string]) : The text to validate the length of.
+    model (string) : The model to validate the text length for.
+    service (string) : The service to validate the text length for.
+
+    """
+
+    try:
+
+        if(isinstance(text, ModelTranslationMessage)):
+            text = str(text)
+
+        text = _convert_iterable_to_str(text) 
+
+        if(service == "openai"):
+            _encoding = tiktoken.encoding_for_model(model)
+            _num_tokens = len(_encoding.encode(text))
+
+            _max_tokens_allowed = MODEL_MAX_TOKENS.get(model, {}).get("max_input_tokens")
+
+            ## silently return if the model is not in the list of models with a max token limit
+            if(not _max_tokens_allowed):
+                return
+
+            ## we can do a hard error with openai since we can accurately count tokens
+            if(_num_tokens > _max_tokens_allowed):
+                raise TooManyInputTokensException(f"Input text exceeds the maximum token limit of {model}.")
+            
+        else:
+            _num_tokens = _gemini_count_tokens(text, model)
+
+            _max_tokens_allowed = MODEL_MAX_TOKENS.get(model, {}).get("max_input_tokens")
+
+            ## silently return if the model is not in the list of models with a max token limit
+            if(not _max_tokens_allowed):
+                return
+
+            ## we can't accurately count tokens with gemini/anthropic, so we'll just do a warning
+            if(_num_tokens > _max_tokens_allowed):
+                logging.warning(f"Input text may exceed the maximum token limit of {model}.")
+
+    except TooManyInputTokensException:
+        raise
+
+    ## soft error, pretty sure this thing will break randomly
+    except Exception as e:
+        logging.error(f"Error validating text length: {str(e)}")
+
 ##-------------------start-of-_string_to_bool()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _string_to_bool(string:str) -> bool:
 
     return string.lower() in ['true', '1', 'yes', 'y', 't']
 
 ##-------------------start-of-_convert_iterable_to_str()-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _convert_iterable_to_str(iterable:typing.Iterable) -> str:
+
+    if(isinstance(iterable, str)):
+        return iterable
+
     return "".join(map(str, iterable))
 
 ##-------------------start-of-is_iterable_of_strings()-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _is_iterable_of_strings(value):
 
     if(isinstance(value, str)):
```

### Comparing `easytl-0.4.0a2/src/easytl.egg-info/PKG-INFO` & `easytl-0.4.0a3/src/easytl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.4.0a2/src/easytl.egg-info/SOURCES.txt` & `easytl-0.4.0a3/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/tests/issue_template.py` & `easytl-0.4.0a3/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/tests/passing.py` & `easytl-0.4.0a3/tests/passing.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0a2/tests/simple_test.py` & `easytl-0.4.0a3/tests/simple_test.py`

 * *Files identical despite different names*

