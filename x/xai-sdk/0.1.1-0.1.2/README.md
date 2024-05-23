# Comparing `tmp/xai_sdk-0.1.1.tar.gz` & `tmp/xai_sdk-0.1.2.tar.gz`

## Comparing `xai_sdk-0.1.1.tar` & `xai_sdk-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/Makefile
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/create_bindings.sh
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/__about__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/__init__.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/chat.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/client.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/files.py
--rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/grok.py
--rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/ide.py
--rw-r--r--   0        0        0    14274 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/sampler.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/compat/__init__.py
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/compat/chat.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/compat/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/__init__.py
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2.py
--rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2.pyi
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2_grpc.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2.pyi
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2_grpc.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2.pyi
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2_grpc.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2.pyi
--rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2_grpc.py
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2.pyi
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2_grpc.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2.pyi
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/x_entities_pb2.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/x_entities_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/x_entities_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/src/xai_sdk/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/README.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/Makefile
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/create_bindings.sh
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/__about__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/__init__.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/chat.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/client.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/files.py
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/grok.py
+-rw-r--r--   0        0        0    17025 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/ide.py
+-rw-r--r--   0        0        0    13895 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/sampler.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/__init__.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/chat.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/__init__.py
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.py
+-rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.pyi
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2_grpc.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.pyi
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.pyi
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2_grpc.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.pyi
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2_grpc.py
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.pyi
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2_grpc.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.pyi
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/PKG-INFO
```

### Comparing `xai_sdk-0.1.1/Makefile` & `xai_sdk-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/create_bindings.sh` & `xai_sdk-0.1.2/create_bindings.sh`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/__init__.py` & `xai_sdk-0.1.2/src/xai_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/chat.py` & `xai_sdk-0.1.2/src/xai_sdk/chat.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/client.py` & `xai_sdk-0.1.2/src/xai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/files.py` & `xai_sdk-0.1.2/src/xai_sdk/files.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/grok.py` & `xai_sdk-0.1.2/src/xai_sdk/grok.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/ide.py` & `xai_sdk-0.1.2/src/xai_sdk/ide.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from . import sampler
 
 _USER = 1
 _MODEL = 2
 
 
 # The client used by the ide.
-_CLIENT: _client.Client | None = None
+_CLIENT: Union[_client.Client, None] = None
 
 
 def set_client(client: _client.Client):
     """Sets the client use by the IDE SDK."""
     global _CLIENT
     _CLIENT = client
 
@@ -33,15 +33,15 @@
     """Returns the client used by the IDE."""
     global _CLIENT
     if _CLIENT is None:
         _CLIENT = _client.Client()
     return _CLIENT
 
 
-async def user_input(text: str) -> str | None:
+async def user_input(text: str) -> Optional[str]:
     """Asks the user to enter a string.
 
     Args:
         text: The prompt presented to the user.
 
     Returns:
         A string if the user actually entered some text and `None` if the input is empty.
```

### Comparing `xai_sdk-0.1.1/src/xai_sdk/sampler.py` & `xai_sdk-0.1.2/src/xai_sdk/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
             compression,
         )
 
         return [Token.from_proto(token) for token in tokens]
 
     async def sample(
         self,
-        prompt: Union[str, Sequence[int], Sequence["Token"]],
         *,
+        prompt: Union[str, Sequence[int], Sequence["Token"]],
         inputs: Sequence[Union[str, int, bytes]] = (),
         model_name: str = "",
         max_len: int = 256,
         temperature: float = 0.7,
         nucleus_p: float = 0.95,
         stop_tokens: Optional[list[str]] = None,
         stop_strings: Optional[list[str]] = None,
@@ -87,18 +87,18 @@
         allowed_tokens: Optional[Sequence[Union[int, str]]] = None,
         disallowed_tokens: Optional[Sequence[Union[int, str]]] = None,
         augment_tokens: bool = True,
     ) -> AsyncGenerator["Token", None]:
         """Generates a model response by continuing `prompt`.
 
         Args:
-            prompt: [Deprecated, use inputs instead] Prompt to continue. This can either be a string, a sequence of
-                token IDs, or a sequence of `Token` instances.
-            inputs: Multimodal input of the model. This can be a sequence of strings, token IDs, image in bytes or
-                base64 encoded string.
+            prompt: [Deprecated, use inputs instead] Prompt to continue. This can either be a
+                string, a sequence of token IDs, or a sequence of `Token` instances.
+            inputs: Multimodal input of the model. This can be a sequence of strings, token IDs,
+                image in bytes or base64 encoded string.
             model_name: Name of the model to sample from. Leave empty to sample from the default
                 model.
             max_len: Maximum number of tokens to generate.
             temperature: Temperature of the final softmax operation. The lower the temperature, the
                 lower the variance of the token distribution. In the limit, the distribution
                 collapses onto the single token with the highest probability.
             nucleus_p: Threshold of the Top-P sampling technique: We rank all tokens by their
@@ -171,19 +171,18 @@
                 elif isinstance(element, list):
                     converted_inputs.append(PromptInput(token_ids=TokenIds(tokens=element)))
                 elif isinstance(element, bytes):
                     converted_inputs.append(PromptInput(image_bytes=element))
                 else:
                     logging.error("Invalid input type %s.", type(element))
         else:
-            token_ids = await self._prompt_to_token_ids(prompt, model_name)
-            converted_inputs = (PromptInput(token_ids=TokenIds(tokens=token_ids)),)
+            converted_inputs.append(_prompt_to_input(prompt))
 
         request = sampler_public_pb2.SampleTokensRequest(
-            prompt=token_ids,
+            inputs=converted_inputs,
             settings=sampler_public_pb2.SampleSettings(
                 max_len=max_len or 0,
                 temperature=temperature,
                 nucleus_p=nucleus_p,
                 stop_tokens=stop_tokens or [],
                 stop_strings=stop_strings or [],
                 rng_seed=rng_seed,
@@ -202,51 +201,14 @@
                 if token_counter % 10 == 0:
                     logging.debug("Sampled %d tokens", token_counter)
                 yield Token.from_proto(token.token)
             elif token.HasField("budget"):
                 # The sample request also sends the current token budget information.
                 log_budget_update(token.budget)
 
-    async def _prompt_to_token_ids(
-        self, prompt: Union[str, Sequence[int], Sequence["Token"]], model_name: str
-    ) -> list[int]:
-        """Converts a prompt to a list of token IDs.
-
-        Args:
-            prompt: The prompt, which can take one of three formats: A raw string, a sequence of
-                integers (which are assumed to be token IDs), or a sequence of `Token` instances.
-            model_name: Name of the model to use if we have to call the tokenizer.
-
-        Returns:
-            List of token IDs.
-
-        Raises:
-            ValueError: If the prompt's type doesn't conform to our assumptions.
-        """
-        assert prompt, "Prompt must not be empty."
-
-        if isinstance(prompt, str):
-            # The prompt is a raw string, tokenize it and extract the token IDs.
-            tokens = await self.tokenize(prompt, model_name)
-            return [t.token_id for t in tokens]
-        elif isinstance(prompt, Sequence):
-            # Check the type of the first item in the list and assume all items are of the same
-            # type.
-            if isinstance(prompt[0], int):
-                # The prompt is already in the form of a list of integers. Nothing to do here.
-                return list(prompt)
-            elif isinstance(prompt[0], Token):
-                # Extract the token IDs from the sequence of token instances.
-                return [t.token_id for t in prompt]
-
-        raise ValueError(
-            f"Prompt must be either a string, a list of token IDs, or a sequence of "
-            f"Token instance. Given prompt was neither. Prompt: {prompt}"
-        )
-
 
 @dataclasses.dataclass(frozen=True)
 class Token:
     """A token is an element of our vocabulary that has a unique index and string representation.
 
     A token can either be sampled from a model or provided by the user (i.e. prompted). If the token
     comes from the mode, we may have additional metadata such as its sampling probability, the
@@ -304,7 +266,42 @@
     """Converts the argument to an `InputToken` proto."""
     if isinstance(token, int):
         return sampler_public_pb2.InputToken(token_id=token)
     elif isinstance(token, str):
         return sampler_public_pb2.InputToken(string_token=token)
     else:
         raise ValueError(f"Invalid token type {type(token)}.")
+
+
+def _prompt_to_input(
+    prompt: Union[str, Sequence[int], Sequence["Token"]]) -> PromptInput:
+    """Converts a prompt to a PromptInput proto.
+
+    Args:
+        prompt: The prompt, which can take one of three formats: A raw string, a sequence of
+            integers (which are assumed to be token IDs), or a sequence of `Token` instances.
+
+    Returns:
+        List of token IDs.
+
+    Raises:
+        ValueError: If the prompt's type doesn't conform to our assumptions.
+    """
+    assert prompt, "Prompt must not be empty."
+
+    if isinstance(prompt, str):
+        # The prompt is a raw string.
+        return PromptInput(text=prompt)
+    elif isinstance(prompt, Sequence):
+        # Check the type of the first item in the list and assume all items are of the same
+        # type.
+        if isinstance(prompt[0], int):
+            # The prompt is in the form of a list of integers.
+            return PromptInput(token_ids=TokenIds(tokens=prompt))
+        elif isinstance(prompt[0], Token):
+            # Extract the token IDs from the sequence of token instances.
+            return PromptInput(token_ids=TokenIds(tokens=[t.token_id for t in prompt]))
+
+    raise ValueError(
+        f"Prompt must be either a string, a list of token IDs, or a sequence of "
+        f"Token instance. Given prompt was neither. Prompt: {prompt}"
+    )
```

### Comparing `xai_sdk-0.1.1/src/xai_sdk/compat/chat.py` & `xai_sdk-0.1.2/src/xai_sdk/compat/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         tools: Any = None,
         top_p: Optional[float] = None,
         user: Optional[str] = None,
         extra_headers: Any = None,
         extra_query: Any = None,
         extra_body: Any = None,
         timeout: Optional[float] = None,
-    ) -> ChatCompletion | Generator[ChatCompletionChunk, None, None]:
+    ) -> Union[ChatCompletion, Generator[ChatCompletionChunk, None, None]]:
         """Creates a new chat completion by calling the API.
 
         Args:
             messages: List of messages that have been exchanged in the conversation (i.e. the
                 message history).
             model: ID of the model to sample from. If empty/not provided, the default model will be
                 used.
```

### Comparing `xai_sdk-0.1.1/src/xai_sdk/compat/client.py` & `xai_sdk-0.1.2/src/xai_sdk/compat/client.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/chat_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/compat_chat_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/files_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/prod_search_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/sampler_public_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,38 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from .google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from . import chat_pb2 as chat__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14stateless_chat.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\"\xb0\x02\n\x15StatelessConversation\x12!\n\x19stateless_conversation_id\x18\x05 \x01(\t\x12\x30\n\tresponses\x18\x01 \x03(\x0b\x32\x1d.prompt_ide.StatelessResponse\x12\x1a\n\x12system_prompt_name\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x1f\n\x17\x65xpose_username_to_grok\x18\x06 \x01(\x08\x12\x16\n\x0e\x64isable_search\x18\x07 \x01(\x08\x12\x1f\n\x17\x65nable_image_generation\x18\x08 \x01(\x08\x12\x12\n\nmodel_name\x18\t \x01(\t\x12\x18\n\x10x_posts_as_field\x18\n \x01(\x08\"\x99\x02\n\x11StatelessResponse\x12\x34\n\x06sender\x18\x01 \x01(\x0e\x32$.prompt_ide.StatelessResponse.Sender\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05query\x18\x03 \x01(\t\x12\x12\n\nquery_type\x18\x05 \x01(\t\x12:\n\x10image_attachment\x18\x06 \x01(\x0b\x32\x1b.prompt_ide.ImageAttachmentH\x00\x88\x01\x01\x12\x12\n\nx_post_ids\x18\x07 \x03(\t\"/\n\x06Sender\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05HUMAN\x10\x01\x12\r\n\tASSISTANT\x10\x02\x42\x13\n\x11_image_attachmentJ\x04\x08\x04\x10\x05\"<\n\x0fImageAttachment\x12\x13\n\x0bimage_bytes\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\":\n DeleteLoggedConversationsRequest\x12\x16\n\x0e\x61\x63\x63ounting_key\x18\x01 \x01(\t2\xa8\x03\n\rStatelessChat\x12\x7f\n\x0b\x41\x64\x64Response\x12!.prompt_ide.StatelessConversation\x1a\x1d.prompt_ide.StatelessResponse\",\x82\xd3\xe4\x93\x02&\"!/rest/stateless-chat/add-response:\x01*0\x01\x12\x7f\n\x0fLogForDebugging\x12!.prompt_ide.StatelessConversation\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+\"&/rest/stateless-chat/log-for-debugging:\x01*\x12\x94\x01\n\x19\x44\x65leteLoggedConversations\x12,.prompt_ide.DeleteLoggedConversationsRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+*)/rest/stateless-chat/logged-conversationsB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14stateless_chat.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\nchat.proto\"\xeb\x02\n\x15StatelessConversation\x12!\n\x19stateless_conversation_id\x18\x05 \x01(\t\x12\x30\n\tresponses\x18\x01 \x03(\x0b\x32\x1d.prompt_ide.StatelessResponse\x12\x1a\n\x12system_prompt_name\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x1f\n\x17\x65xpose_username_to_grok\x18\x06 \x01(\x08\x12\x16\n\x0e\x64isable_search\x18\x07 \x01(\x08\x12\x1f\n\x17\x65nable_image_generation\x18\x08 \x01(\x08\x12\x12\n\nmodel_name\x18\t \x01(\t\x12\x18\n\x10x_posts_as_field\x18\n \x01(\x08\x12\x39\n\x12\x61\x64\x64itional_options\x18\x0b \x01(\x0b\x32\x1d.prompt_ide.AdditionalOptions\"\xca\x02\n\x11StatelessResponse\x12\x34\n\x06sender\x18\x01 \x01(\x0e\x32$.prompt_ide.StatelessResponse.Sender\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05query\x18\x03 \x01(\t\x12\x12\n\nquery_type\x18\x05 \x01(\t\x12:\n\x10image_attachment\x18\x06 \x01(\x0b\x32\x1b.prompt_ide.ImageAttachmentH\x00\x88\x01\x01\x12\x12\n\nx_post_ids\x18\x07 \x03(\t\x12/\n\tdebug_log\x18\x08 \x01(\x0b\x32\x1c.prompt_ide.ResponseDebugLog\"/\n\x06Sender\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05HUMAN\x10\x01\x12\r\n\tASSISTANT\x10\x02\x42\x13\n\x11_image_attachmentJ\x04\x08\x04\x10\x05\"<\n\x0fImageAttachment\x12\x13\n\x0bimage_bytes\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\":\n DeleteLoggedConversationsRequest\x12\x16\n\x0e\x61\x63\x63ounting_key\x18\x01 \x01(\t2\xa8\x03\n\rStatelessChat\x12\x7f\n\x0b\x41\x64\x64Response\x12!.prompt_ide.StatelessConversation\x1a\x1d.prompt_ide.StatelessResponse\",\x82\xd3\xe4\x93\x02&\"!/rest/stateless-chat/add-response:\x01*0\x01\x12\x7f\n\x0fLogForDebugging\x12!.prompt_ide.StatelessConversation\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+\"&/rest/stateless-chat/log-for-debugging:\x01*\x12\x94\x01\n\x19\x44\x65leteLoggedConversations\x12,.prompt_ide.DeleteLoggedConversationsRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+*)/rest/stateless-chat/logged-conversationsB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stateless_chat_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
   _STATELESSCHAT.methods_by_name['AddResponse']._options = None
   _STATELESSCHAT.methods_by_name['AddResponse']._serialized_options = b'\202\323\344\223\002&\"!/rest/stateless-chat/add-response:\001*'
   _STATELESSCHAT.methods_by_name['LogForDebugging']._options = None
   _STATELESSCHAT.methods_by_name['LogForDebugging']._serialized_options = b'\202\323\344\223\002+\"&/rest/stateless-chat/log-for-debugging:\001*'
   _STATELESSCHAT.methods_by_name['DeleteLoggedConversations']._options = None
   _STATELESSCHAT.methods_by_name['DeleteLoggedConversations']._serialized_options = b'\202\323\344\223\002+*)/rest/stateless-chat/logged-conversations'
-  _globals['_STATELESSCONVERSATION']._serialized_start=96
-  _globals['_STATELESSCONVERSATION']._serialized_end=400
-  _globals['_STATELESSRESPONSE']._serialized_start=403
-  _globals['_STATELESSRESPONSE']._serialized_end=684
-  _globals['_STATELESSRESPONSE_SENDER']._serialized_start=610
-  _globals['_STATELESSRESPONSE_SENDER']._serialized_end=657
-  _globals['_IMAGEATTACHMENT']._serialized_start=686
-  _globals['_IMAGEATTACHMENT']._serialized_end=746
-  _globals['_DELETELOGGEDCONVERSATIONSREQUEST']._serialized_start=748
-  _globals['_DELETELOGGEDCONVERSATIONSREQUEST']._serialized_end=806
-  _globals['_STATELESSCHAT']._serialized_start=809
-  _globals['_STATELESSCHAT']._serialized_end=1233
+  _globals['_STATELESSCONVERSATION']._serialized_start=108
+  _globals['_STATELESSCONVERSATION']._serialized_end=471
+  _globals['_STATELESSRESPONSE']._serialized_start=474
+  _globals['_STATELESSRESPONSE']._serialized_end=804
+  _globals['_STATELESSRESPONSE_SENDER']._serialized_start=730
+  _globals['_STATELESSRESPONSE_SENDER']._serialized_end=777
+  _globals['_IMAGEATTACHMENT']._serialized_start=806
+  _globals['_IMAGEATTACHMENT']._serialized_end=866
+  _globals['_DELETELOGGEDCONVERSATIONSREQUEST']._serialized_start=868
+  _globals['_DELETELOGGEDCONVERSATIONSREQUEST']._serialized_end=926
+  _globals['_STATELESSCHAT']._serialized_start=929
+  _globals['_STATELESSCHAT']._serialized_end=1353
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 from .google.api import annotations_pb2 as _annotations_pb2
 from google.protobuf import empty_pb2 as _empty_pb2
+from . import chat_pb2 as _chat_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class StatelessConversation(_message.Message):
-    __slots__ = ["stateless_conversation_id", "responses", "system_prompt_name", "name", "username", "expose_username_to_grok", "disable_search", "enable_image_generation", "model_name", "x_posts_as_field"]
+    __slots__ = ["stateless_conversation_id", "responses", "system_prompt_name", "name", "username", "expose_username_to_grok", "disable_search", "enable_image_generation", "model_name", "x_posts_as_field", "additional_options"]
     STATELESS_CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     RESPONSES_FIELD_NUMBER: _ClassVar[int]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     USERNAME_FIELD_NUMBER: _ClassVar[int]
     EXPOSE_USERNAME_TO_GROK_FIELD_NUMBER: _ClassVar[int]
     DISABLE_SEARCH_FIELD_NUMBER: _ClassVar[int]
     ENABLE_IMAGE_GENERATION_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     X_POSTS_AS_FIELD_FIELD_NUMBER: _ClassVar[int]
+    ADDITIONAL_OPTIONS_FIELD_NUMBER: _ClassVar[int]
     stateless_conversation_id: str
     responses: _containers.RepeatedCompositeFieldContainer[StatelessResponse]
     system_prompt_name: str
     name: str
     username: str
     expose_username_to_grok: bool
     disable_search: bool
     enable_image_generation: bool
     model_name: str
     x_posts_as_field: bool
-    def __init__(self, stateless_conversation_id: _Optional[str] = ..., responses: _Optional[_Iterable[_Union[StatelessResponse, _Mapping]]] = ..., system_prompt_name: _Optional[str] = ..., name: _Optional[str] = ..., username: _Optional[str] = ..., expose_username_to_grok: bool = ..., disable_search: bool = ..., enable_image_generation: bool = ..., model_name: _Optional[str] = ..., x_posts_as_field: bool = ...) -> None: ...
+    additional_options: _chat_pb2.AdditionalOptions
+    def __init__(self, stateless_conversation_id: _Optional[str] = ..., responses: _Optional[_Iterable[_Union[StatelessResponse, _Mapping]]] = ..., system_prompt_name: _Optional[str] = ..., name: _Optional[str] = ..., username: _Optional[str] = ..., expose_username_to_grok: bool = ..., disable_search: bool = ..., enable_image_generation: bool = ..., model_name: _Optional[str] = ..., x_posts_as_field: bool = ..., additional_options: _Optional[_Union[_chat_pb2.AdditionalOptions, _Mapping]] = ...) -> None: ...
 
 class StatelessResponse(_message.Message):
-    __slots__ = ["sender", "message", "query", "query_type", "image_attachment", "x_post_ids"]
+    __slots__ = ["sender", "message", "query", "query_type", "image_attachment", "x_post_ids", "debug_log"]
     class Sender(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
         UNKNOWN: _ClassVar[StatelessResponse.Sender]
         HUMAN: _ClassVar[StatelessResponse.Sender]
         ASSISTANT: _ClassVar[StatelessResponse.Sender]
     UNKNOWN: StatelessResponse.Sender
     HUMAN: StatelessResponse.Sender
     ASSISTANT: StatelessResponse.Sender
     SENDER_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     QUERY_TYPE_FIELD_NUMBER: _ClassVar[int]
     IMAGE_ATTACHMENT_FIELD_NUMBER: _ClassVar[int]
     X_POST_IDS_FIELD_NUMBER: _ClassVar[int]
+    DEBUG_LOG_FIELD_NUMBER: _ClassVar[int]
     sender: StatelessResponse.Sender
     message: str
     query: str
     query_type: str
     image_attachment: ImageAttachment
     x_post_ids: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, sender: _Optional[_Union[StatelessResponse.Sender, str]] = ..., message: _Optional[str] = ..., query: _Optional[str] = ..., query_type: _Optional[str] = ..., image_attachment: _Optional[_Union[ImageAttachment, _Mapping]] = ..., x_post_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+    debug_log: _chat_pb2.ResponseDebugLog
+    def __init__(self, sender: _Optional[_Union[StatelessResponse.Sender, str]] = ..., message: _Optional[str] = ..., query: _Optional[str] = ..., query_type: _Optional[str] = ..., image_attachment: _Optional[_Union[ImageAttachment, _Mapping]] = ..., x_post_ids: _Optional[_Iterable[str]] = ..., debug_log: _Optional[_Union[_chat_pb2.ResponseDebugLog, _Mapping]] = ...) -> None: ...
 
 class ImageAttachment(_message.Message):
     __slots__ = ["image_bytes", "content_type"]
     IMAGE_BYTES_FIELD_NUMBER: _ClassVar[int]
     CONTENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     image_bytes: bytes
     content_type: str
```

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/stateless_chat_pb2_grpc.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/x_entities_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/x_entities_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/google/api/annotations_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/google/api/http_pb2.py` & `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/src/xai_sdk/proto/google/api/http_pb2.pyi` & `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/.gitignore` & `xai_sdk-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/LICENSE.txt` & `xai_sdk-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/pyproject.toml` & `xai_sdk-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.1/PKG-INFO` & `xai_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xai-sdk
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: Documentation, https://x.ai/api/sdk.html
 Author-email: Toby Pohlen <pohlen@x.ai>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

