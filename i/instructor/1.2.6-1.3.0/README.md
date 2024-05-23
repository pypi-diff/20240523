# Comparing `tmp/instructor-1.2.6.tar.gz` & `tmp/instructor-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.6.tar", max compression
+gzip compressed data, was "instructor-1.3.0.tar", max compression
```

## Comparing `instructor-1.2.6.tar` & `instructor-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1066 2024-05-09 04:29:33.847049 instructor-1.2.6/LICENSE
--rw-r--r--   0        0        0     9716 2024-05-09 04:29:33.847049 instructor-1.2.6/README.md
--rw-r--r--   0        0        0     1450 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/cli.py
--rw-r--r--   0        0        0     3865 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/files.py
--rw-r--r--   0        0        0     5441 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/hub.py
--rw-r--r--   0        0        0     8314 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6441 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/cli/usage.py
--rw-r--r--   0        0        0    13256 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client.py
--rw-r--r--   0        0        0     2573 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2419 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_cohere.py
--rw-r--r--   0        0        0     1391 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_groq.py
--rw-r--r--   0        0        0     1727 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/client_mistral.py
--rw-r--r--   0        0        0     9579 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/citation.py
--rw-r--r--   0        0        0     8079 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2169 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2562 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    10922 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1879 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4360 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/exceptions.py
--rw-r--r--   0        0        0     8724 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/mode.py
--rw-r--r--   0        0        0     4969 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/patch.py
--rw-r--r--   0        0        0    13501 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/py.typed
--rw-r--r--   0        0        0     9502 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/retry.py
--rw-r--r--   0        0        0     6507 2024-05-09 04:29:33.923049 instructor-1.2.6/instructor/utils.py
--rw-r--r--   0        0        0     2799 2024-05-09 04:29:33.923049 instructor-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 instructor-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-23 17:26:36.440648 instructor-1.3.0/LICENSE
+-rw-r--r--   0        0        0    11016 2024-05-23 17:26:36.440648 instructor-1.3.0/README.md
+-rw-r--r--   0        0        0     1590 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3865 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/files.py
+-rw-r--r--   0        0        0     5441 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8314 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6889 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/cli/usage.py
+-rw-r--r--   0        0        0    13312 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client.py
+-rw-r--r--   0        0        0     2581 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2427 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client_cohere.py
+-rw-r--r--   0        0        0      756 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client_gemini.py
+-rw-r--r--   0        0        0     1399 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client_groq.py
+-rw-r--r--   0        0        0     1735 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/client_mistral.py
+-rw-r--r--   0        0        0     9579 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     8721 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2168 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2562 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11564 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1879 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4360 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      471 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/exceptions.py
+-rw-r--r--   0        0        0     9843 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/function_calls.py
+-rw-r--r--   0        0        0      878 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/mode.py
+-rw-r--r--   0        0        0     5001 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/patch.py
+-rw-r--r--   0        0        0    15936 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/py.typed
+-rw-r--r--   0        0        0    10007 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/retry.py
+-rw-r--r--   0        0        0     7919 2024-05-23 17:26:36.520649 instructor-1.3.0/instructor/utils.py
+-rw-r--r--   0        0        0     2907 2024-05-23 17:26:36.524649 instructor-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13134 1970-01-01 00:00:00.000000 instructor-1.3.0/PKG-INFO
```

### Comparing `instructor-1.2.6/LICENSE` & `instructor-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/README.md` & `instructor-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Instructor: Structured LLM Outputs
 
 Instructor is a Python library that makes it a breeze to work with structured outputs from large language models (LLMs). Built on top of Pydantic, it provides a simple, transparent, and user-friendly API to manage validation, retries, and streaming responses. Get ready to supercharge your LLM workflows!
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/jxnlco?style=social)](https://twitter.com/jxnlco)
-[![Discord](https://img.shields.io/discord/1192334452110659664?label=discord)](https://discord.gg/CV8sPM5k5Y)
+[![Discord](https://img.shields.io/discord/1192334452110659664?label=discord)](https://discord.gg/bD9YE9JArw)
 [![Downloads](https://img.shields.io/pypi/dm/instructor.svg)](https://pypi.python.org/pypi/instructor)
 
-
 ## Key Features
 
 - **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
 - **Retry Management**: Easily configure the number of retry attempts for your requests
 - **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
 - **Streaming Support**: Work with Lists and Partial responses effortlessly
 - **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
+- **Support in many Languages**: We support many languages including [Python](https://python.useinstructor.com), [TypeScript](https://js.useinstructor.com), [Ruby](https://ruby.useinstructor.com), [Go](https://go.useinstructor.com), and [Elixir](https://hex.pm/packages/instructor)
 
 ## Get Started in Minutes
 
 Install Instructor with a single command:
 
 ```bash
 pip install -U instructor
@@ -121,14 +121,54 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
+### Using Gemini Models
+
+Make sure you [install](https://ai.google.dev/api/python/google/generativeai#setup) the Google AI Python SDK. You should set a `GOOGLE_API_KEY` environment variable with your API key.
+
+```
+pip install google-generativeai
+```
+
+```python
+import instructor
+import google.generativeai as genai
+from pydantic import BaseModel
+
+class User(BaseModel):
+    name: str
+    age: int
+
+# genai.configure(api_key=os.environ["API_KEY"]) # alternative API key configuration
+client = instructor.from_gemini(
+    client=genai.GenerativeModel(
+        model_name="models/gemini-1.5-flash-latest", # model defaults to "gemini-pro"
+    ),
+    mode=instructor.Mode.GEMINI_JSON,
+)
+
+# note that client.chat.completions.create will also work
+resp = client.chat.completions.create(
+    messages=[
+        {
+            "role": "user",
+            "content": "Extract Jason is 25 years old.",
+        }
+    ],
+    response_model=User,
+)
+
+assert isinstance(resp, User)
+assert resp.name == "Jason"
+assert resp.age == 25
+```
 
 ### Using Litellm
 
 ```python
 import instructor
 from litellm import completion
 from pydantic import BaseModel
@@ -247,15 +287,14 @@
     ],
     response_model=User,
 )
 ```
 
 ![with_completion](./docs/blog/posts/img/with_completion.png)
 
-
 ### Streaming Partial Objects: `create_partial`
 
 In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simply the type inference, we've added `create_iterable` and `create_partial` methods as well!
 
 ```python
 import openai
 import instructor
```

### Comparing `instructor-1.2.6/instructor/__init__.py` & `instructor-1.3.0/instructor/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 
 
 if importlib.util.find_spec("anthropic") is not None:
     from .client_anthropic import from_anthropic
 
     __all__ += ["from_anthropic"]
 
+if importlib.util.find_spec("google.generativeai") is not None:
+    from .client_gemini import from_gemini
+
+    __all__ += ["from_gemini"]
+
 if importlib.util.find_spec("groq") is not None:
     from .client_groq import from_groq
 
     __all__ += ["from_groq"]
 
 if importlib.util.find_spec("mistralai") is not None:
     from .client_mistral import from_mistral
```

### Comparing `instructor-1.2.6/instructor/_types/_alias.py` & `instructor-1.3.0/instructor/_types/_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Literal
 
 from typing_extensions import TypeAlias
 
 ModelNames: TypeAlias = Literal[
+    "gpt-4o",
     "gpt-4-0125-preview",
     "gpt-4-turbo-preview",
     "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4",
     "gpt-4-0314",
     "gpt-4-0613",
```

### Comparing `instructor-1.2.6/instructor/cli/cli.py` & `instructor-1.3.0/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/cli/files.py` & `instructor-1.3.0/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/cli/hub.py` & `instructor-1.3.0/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/cli/jobs.py` & `instructor-1.3.0/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/cli/usage.py` & `instructor-1.3.0/instructor/cli/usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,18 @@
         for data in fetched_data:
             all_data.extend(data.get("data", []))
     return all_data
 
 
 # Define the cost per unit for each model
 MODEL_COSTS = {
+    "gpt-4o": {"prompt": 0.005 / 1000, "completion": 0.015 / 1000},
+    "gpt-4o-2024-05-13": {"prompt": 0.005 / 1000, "completion": 0.015 / 1000},
+    "gpt-4-turbo": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
+    "gpt-4-turbo-2024-04-09": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-0125-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-turbo-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-1106-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-vision-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
     "gpt-4-0314": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
     "gpt-4-0613": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
@@ -80,16 +84,20 @@
     if model in MODEL_COSTS:
         return MODEL_COSTS[model]
 
     if model.startswith("gpt-3.5-turbo-16k"):
         return MODEL_COSTS["gpt-3.5-turbo-16k"]
     elif model.startswith("gpt-3.5-turbo"):
         return MODEL_COSTS["gpt-3.5-turbo"]
+    elif model.startswith("gpt-4-turbo"):
+        return MODEL_COSTS["gpt-4-turbo-preview"]
     elif model.startswith("gpt-4-32k"):
         return MODEL_COSTS["gpt-4-32k"]
+    elif model.startswith("gpt-4o"):
+        return MODEL_COSTS["gpt-4o"]
     elif model.startswith("gpt-4"):
         return MODEL_COSTS["gpt-4"]
     else:
         raise ValueError(f"Cost for model {model} not found")
 
 
 def calculate_cost(
@@ -106,19 +114,19 @@
     prompt_cost = cost["prompt"] * n_context_tokens
     completion_cost = cost["completion"] * n_generated_tokens
     return prompt_cost + completion_cost
 
 
 def group_and_sum_by_date_and_snapshot(usage_data: list[dict[str, Any]]) -> Table:
     """Group and sum the usage data by date and snapshot, including costs."""
-    summary: defaultdict[str, defaultdict[str, dict[str, Union[int, float]]]] = (
-        defaultdict(
-            lambda: defaultdict(
-                lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
-            )
+    summary: defaultdict[
+        str, defaultdict[str, dict[str, Union[int, float]]]
+    ] = defaultdict(
+        lambda: defaultdict(
+            lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
         )
     )
 
     for usage in usage_data:
         snapshot_id = usage["snapshot_id"]
         date = datetime.fromtimestamp(usage["aggregation_timestamp"]).strftime(
             "%Y-%m-%d"
```

### Comparing `instructor-1.2.6/instructor/client.py` & `instructor-1.3.0/instructor/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,28 @@
         self: AsyncInstructor,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> Awaitable[T]: ...
+    ) -> Awaitable[T]:
+        ...
 
     @overload
     def create(
         self: Self,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> T: ...
+    ) -> T:
+        ...
 
     # TODO: we should overload a case where response_model is None
     def create(
         self,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
@@ -102,38 +104,38 @@
         self: AsyncInstructor,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> AsyncGenerator[T, None]: ...
+    ) -> AsyncGenerator[T, None]:
+        ...
 
     @overload
     def create_partial(
         self: Self,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> Generator[T, None, None]: ...
+    ) -> Generator[T, None, None]:
+        ...
 
     def create_partial(
         self,
         response_model: type[T],
         messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
     ) -> Generator[T, None, None] | AsyncGenerator[T, None]:
-        assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support partial"
-
         kwargs["stream"] = True
 
         kwargs = self.handle_kwargs(kwargs)
 
         response_model = instructor.Partial[response_model]  # type: ignore
         return self.create_fn(
             messages=messages,
@@ -149,26 +151,28 @@
         self: AsyncInstructor,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> AsyncGenerator[T, None]: ...
+    ) -> AsyncGenerator[T, None]:
+        ...
 
     @overload
     def create_iterable(
         self: Self,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> Generator[T, None, None]: ...
+    ) -> Generator[T, None, None]:
+        ...
 
     def create_iterable(
         self,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
@@ -195,26 +199,28 @@
         self: AsyncInstructor,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> Awaitable[tuple[T, Any]]: ...
+    ) -> Awaitable[tuple[T, Any]]:
+        ...
 
     @overload
     def create_with_completion(
         self: Self,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
-    ) -> tuple[T, Any]: ...
+    ) -> tuple[T, Any]:
+        ...
 
     def create_with_completion(
         self,
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
@@ -307,16 +313,14 @@
         messages: list[ChatCompletionMessageParam],
         response_model: type[T],
         max_retries: int = 3,
         validation_context: dict[str, Any] | None = None,
         strict: bool = True,
         **kwargs: Any,
     ) -> AsyncGenerator[T, None]:
-        assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support iterable"
-
         kwargs = self.handle_kwargs(kwargs)
         kwargs["stream"] = True
         async for item in await self.create_fn(
             response_model=Iterable[response_model],
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
@@ -386,14 +390,19 @@
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.JSON_SCHEMA,
             instructor.Mode.MD_JSON,
         }
 
+    if provider in {Provider.DATABRICKS}:
+        assert mode in {
+            instructor.Mode.MD_JSON
+        }, "Databricks provider only supports `MD_JSON` mode."
+
     if provider in {Provider.OPENAI}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.FUNCTIONS,
             instructor.Mode.PARALLEL_TOOLS,
             instructor.Mode.MD_JSON,
@@ -419,15 +428,16 @@
 
 
 @overload
 def from_litellm(
     completion: Callable[..., Any],
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
-) -> Instructor: ...
+) -> Instructor:
+    ...
 
 
 @overload
 def from_litellm(
     completion: Awaitable[Any],
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
```

### Comparing `instructor-1.2.6/instructor/client_anthropic.py` & `instructor-1.3.0/instructor/client_anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 @overload
 def from_anthropic(
     client: (
         anthropic.Anthropic | anthropic.AnthropicBedrock | anthropic.AnthropicVertex
     ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs: Any,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_anthropic(
     client: (
         anthropic.AsyncAnthropic
         | anthropic.AsyncAnthropicBedrock
         | anthropic.AsyncAnthropicVertex
     ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs: Any,
-) -> instructor.AsyncInstructor: ...
+) -> instructor.AsyncInstructor:
+    ...
 
 
 def from_anthropic(
     client: (
         anthropic.Anthropic
         | anthropic.AsyncAnthropic
         | anthropic.AnthropicBedrock
```

### Comparing `instructor-1.2.6/instructor/client_cohere.py` & `instructor-1.3.0/instructor/client_cohere.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 
 
 @overload
 def from_cohere(
     client: cohere.Client,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_cohere(
     client: cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs: Any,
-) -> instructor.AsyncInstructor: ...
+) -> instructor.AsyncInstructor:
+    ...
 
 
 def from_cohere(
     client: cohere.Client | cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs: Any,
 ):
```

### Comparing `instructor-1.2.6/instructor/client_groq.py` & `instructor-1.3.0/instructor/client_groq.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 
 @overload
 def from_groq(
     client: groq.Groq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_groq(
     client: groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 def from_groq(
     client: groq.Groq | groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
 ) -> instructor.Instructor:
```

### Comparing `instructor-1.2.6/instructor/client_mistral.py` & `instructor-1.3.0/instructor/client_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
 
 @overload
 def from_mistral(
     client: mistralai.client.MistralClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_mistral(
     client: mistralaiasynccli.MistralAsyncClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
     **kwargs: Any,
-) -> instructor.AsyncInstructor: ...
+) -> instructor.AsyncInstructor:
+    ...
 
 
 def from_mistral(
     client: mistralai.client.MistralClient | mistralaiasynccli.MistralAsyncClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
     **kwargs: Any,
 ) -> instructor.Instructor | instructor.AsyncInstructor:
```

### Comparing `instructor-1.2.6/instructor/distil.py` & `instructor-1.3.0/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/dsl/citation.py` & `instructor-1.3.0/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/dsl/iterable.py` & `instructor-1.3.0/instructor/dsl/iterable.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,22 @@
 
     @staticmethod
     def extract_json(
         completion: Iterable[Any], mode: Mode
     ) -> Generator[str, None, None]:
         for chunk in completion:
             try:
-                if chunk.choices:
+                if mode == Mode.ANTHROPIC_JSON:
+                    if json_chunk := chunk.delta.text:
+                        yield json_chunk
+                if mode == Mode.ANTHROPIC_TOOLS:
+                    yield chunk.model_extra.get("delta", "").get("partial_json", "")
+                if mode == Mode.GEMINI_JSON:
+                    yield chunk.text
+                elif chunk.choices:
                     if mode == Mode.FUNCTIONS:
                         if json_chunk := chunk.choices[0].delta.function_call.arguments:
                             yield json_chunk
                     elif mode in {Mode.JSON, Mode.MD_JSON, Mode.JSON_SCHEMA}:
                         if json_chunk := chunk.choices[0].delta.content:
                             yield json_chunk
                     elif mode == Mode.TOOLS:
@@ -98,15 +105,20 @@
 
     @staticmethod
     async def extract_json_async(
         completion: AsyncGenerator[Any, None], mode: Mode
     ) -> AsyncGenerator[str, None]:
         async for chunk in completion:
             try:
-                if chunk.choices:
+                if mode == Mode.ANTHROPIC_JSON:
+                    if json_chunk := chunk.delta.text:
+                        yield json_chunk
+                if mode == Mode.ANTHROPIC_TOOLS:
+                    yield chunk.model_extra.get("delta", "").get("partial_json", "")
+                elif chunk.choices:
                     if mode == Mode.FUNCTIONS:
                         if json_chunk := chunk.choices[0].delta.function_call.arguments:
                             yield json_chunk
                     elif mode in {Mode.JSON, Mode.MD_JSON, Mode.JSON_SCHEMA}:
                         if json_chunk := chunk.choices[0].delta.content:
                             yield json_chunk
                     elif mode == Mode.TOOLS:
```

### Comparing `instructor-1.2.6/instructor/dsl/maybe.py` & `instructor-1.3.0/instructor/dsl/maybe.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     Returns:
         MaybeModel (Type[BaseModel]): A new Pydantic model that includes fields for `result`, `error`, and `message`.
     """
     return create_model(
         f"Maybe{model.__name__}",
         __base__=MaybeBase,
-        reuslts=(
+        result=(
             Optional[model],
             Field(
                 default=None,
                 description="Correctly extracted result from the model, if any, otherwise None",
             ),
         ),
         error=(bool, Field(default=False)),
```

### Comparing `instructor-1.2.6/instructor/dsl/parallel.py` & `instructor-1.3.0/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/dsl/partial.py` & `instructor-1.3.0/instructor/dsl/partial.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,22 @@
 
     @staticmethod
     def extract_json(
         completion: Iterable[Any], mode: Mode
     ) -> Generator[str, None, None]:
         for chunk in completion:
             try:
-                if chunk.choices:
+                if mode == Mode.ANTHROPIC_JSON:
+                    if json_chunk := chunk.delta.text:
+                        yield json_chunk
+                if mode == Mode.ANTHROPIC_TOOLS:
+                    yield chunk.model_extra.get("delta", "").get("partial_json", "")
+                if mode == Mode.GEMINI_JSON:
+                    yield chunk.text
+                elif chunk.choices:
                     if mode == Mode.FUNCTIONS:
                         if json_chunk := chunk.choices[0].delta.function_call.arguments:
                             yield json_chunk
                     elif mode in {Mode.JSON, Mode.MD_JSON, Mode.JSON_SCHEMA}:
                         if json_chunk := chunk.choices[0].delta.content:
                             yield json_chunk
                     elif mode == Mode.TOOLS:
@@ -169,15 +176,20 @@
 
     @staticmethod
     async def extract_json_async(
         completion: AsyncGenerator[Any, None], mode: Mode
     ) -> AsyncGenerator[str, None]:
         async for chunk in completion:
             try:
-                if chunk.choices:
+                if mode == Mode.ANTHROPIC_JSON:
+                    if json_chunk := chunk.delta.text:
+                        yield json_chunk
+                if mode == Mode.ANTHROPIC_TOOLS:
+                    yield chunk.model_extra.get("delta", "").get("partial_json", "")
+                elif chunk.choices:
                     if mode == Mode.FUNCTIONS:
                         if json_chunk := chunk.choices[0].delta.function_call.arguments:
                             yield json_chunk
                     elif mode in {Mode.JSON, Mode.MD_JSON, Mode.JSON_SCHEMA}:
                         if json_chunk := chunk.choices[0].delta.content:
                             yield json_chunk
                     elif mode == Mode.TOOLS:
```

### Comparing `instructor-1.2.6/instructor/dsl/simple_type.py` & `instructor-1.3.0/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/dsl/validators.py` & `instructor-1.3.0/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.6/instructor/function_calls.py` & `instructor-1.3.0/instructor/function_calls.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,16 +101,19 @@
 
         if mode == Mode.ANTHROPIC_JSON:
             return cls.parse_anthropic_json(completion, validation_context, strict)
 
         if mode == Mode.COHERE_TOOLS:
             return cls.parse_cohere_tools(completion, validation_context, strict)
 
+        if mode == Mode.GEMINI_JSON:
+            return cls.parse_gemini_json(completion, validation_context, strict)
+
         if completion.choices[0].finish_reason == "length":
-            raise IncompleteOutputException()
+            raise IncompleteOutputException(last_completion=completion)
 
         if mode == Mode.FUNCTIONS:
             return cls.parse_functions(completion, validation_context, strict)
 
         if mode in {Mode.TOOLS, Mode.MISTRAL_TOOLS}:
             return cls.parse_tools(completion, validation_context, strict)
 
@@ -150,14 +153,40 @@
         extra_text = extract_json_from_codeblock(text)
 
         if strict:
             return cls.model_validate_json(
                 extra_text, context=validation_context, strict=True
             )
         else:
+            # Allow control characters.
+            parsed = json.loads(extra_text, strict=False)
+            # Pydantic non-strict: https://docs.pydantic.dev/latest/concepts/strict_mode/
+            return cls.model_validate(parsed, context=validation_context, strict=False)
+
+    @classmethod
+    def parse_gemini_json(
+        cls: type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[dict[str, Any]] = None,
+        strict: Optional[bool] = None,
+    ) -> BaseModel:
+        try:
+            text = completion.text
+        except ValueError:
+            logger.debug(
+                f"Error response: {completion._result.candidates[0].finish_reason}\n\n{completion_result.candidates[0].safety_ratings}"
+            )
+
+        extra_text = extract_json_from_codeblock(text)
+
+        if strict:
+            return cls.model_validate_json(
+                extra_text, context=validation_context, strict=True
+            )
+        else:
             # Allow control characters.
             parsed = json.loads(extra_text, strict=False)
             # Pydantic non-strict: https://docs.pydantic.dev/latest/concepts/strict_mode/
             return cls.model_validate(parsed, context=validation_context, strict=False)
 
     @classmethod
     def parse_cohere_tools(
```

### Comparing `instructor-1.2.6/instructor/mode.py` & `instructor-1.3.0/instructor/mode.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import enum
 import warnings
 
 
-class Mode(enum.Enum):
+class _WarnOnFunctionsAccessEnumMeta(enum.EnumMeta):
+    def __getattribute__(cls, name):
+        if name == "FUNCTIONS":
+            warnings.warn(
+                "FUNCTIONS is deprecated and will be removed in future versions",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        return super().__getattribute__(name)
+
+
+class Mode(enum.Enum, metaclass=_WarnOnFunctionsAccessEnumMeta):
     """The mode to use for patching the client"""
 
     FUNCTIONS = "function_call"
     PARALLEL_TOOLS = "parallel_tool_call"
     TOOLS = "tool_call"
     MISTRAL_TOOLS = "mistral_tools"
     JSON = "json_mode"
     MD_JSON = "markdown_json_mode"
     JSON_SCHEMA = "json_schema_mode"
     ANTHROPIC_TOOLS = "anthropic_tools"
     ANTHROPIC_JSON = "anthropic_json"
     COHERE_TOOLS = "cohere_tools"
-
-    def __new__(cls, value: str) -> "Mode":
-        member = object.__new__(cls)
-        member._value_ = value
-
-        # Deprecation warning for FUNCTIONS
-        if value == "function_call":
-            warnings.warn(
-                "FUNCTIONS is deprecated and will be removed in future versions",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-        return member
+    GEMINI_JSON = "gemini_json"
```

### Comparing `instructor-1.2.6/instructor/patch.py` & `instructor-1.3.0/instructor/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,54 +31,60 @@
     def __call__(
         self,
         response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model: ...
+    ) -> T_Model:
+        ...
 
 
 class AsyncInstructorChatCompletionCreate(Protocol):
     async def __call__(
         self,
         response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model: ...
+    ) -> T_Model:
+        ...
 
 
 @overload
 def patch(
     client: OpenAI,
     mode: Mode = Mode.TOOLS,
-) -> OpenAI: ...
+) -> OpenAI:
+    ...
 
 
 @overload
 def patch(
     client: AsyncOpenAI,
     mode: Mode = Mode.TOOLS,
-) -> AsyncOpenAI: ...
+) -> AsyncOpenAI:
+    ...
 
 
 @overload
 def patch(
     create: Callable[T_ParamSpec, T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate: ...
+) -> InstructorChatCompletionCreate:
+    ...
 
 
 @overload
 def patch(
     create: Awaitable[T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate: ...
+) -> InstructorChatCompletionCreate:
+    ...
 
 
 def patch(
     client: Union[OpenAI, AsyncOpenAI] = None,
     create: Callable[T_ParamSpec, T_Retval] = None,
     mode: Mode = Mode.TOOLS,
 ) -> Union[OpenAI, AsyncOpenAI]:
```

### Comparing `instructor-1.2.6/instructor/process_response.py` & `instructor-1.3.0/instructor/process_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     Any,
 )
 from collections.abc import Generator
 from typing_extensions import ParamSpec
 
 from instructor.mode import Mode
 
+from .utils import transform_to_gemini_prompt
+
 logger = logging.getLogger("instructor")
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
 T = TypeVar("T")
 
@@ -260,14 +262,19 @@
             elif mode == Mode.MD_JSON:
                 new_kwargs["messages"].append(
                     {
                         "role": "user",
                         "content": "Return the correct JSON response within a ```json codeblock. not the JSON_SCHEMA",
                     },
                 )
+                # For some providers, the messages array must be alternating roles of user and assistant, we must merge
+                # consecutive user messages into a single message
+                new_kwargs["messages"] = merge_consecutive_messages(
+                    new_kwargs["messages"]
+                )
             # check that the first message is a system message
             # if it is not, add a system message to the beginning
             if new_kwargs["messages"][0]["role"] != "system":
                 new_kwargs["messages"].insert(
                     0,
                     {
                         "role": "system",
@@ -276,14 +283,18 @@
                 )
             # if it is, system append the schema to the end
             else:
                 new_kwargs["messages"][0]["content"] += f"\n\n{message}"
         elif mode == Mode.ANTHROPIC_TOOLS:
             tool_descriptions = response_model.anthropic_schema
             new_kwargs["tools"] = [tool_descriptions]
+            new_kwargs["tool_choice"] = {
+                "type": "tool",
+                "name": response_model.__name__,
+            }
 
             system_messages = [
                 m["content"] for m in new_kwargs["messages"] if m["role"] == "system"
             ]
             new_kwargs["system"] = "\n\n".join(system_messages)
             new_kwargs["messages"] = [
                 m for m in new_kwargs["messages"] if m["role"] != "system"
@@ -299,15 +310,17 @@
 
             new_kwargs["system"] = (
                 new_kwargs.get("system", "")
                 + "\n\n"
                 + "\n\n".join(openai_system_messages)
             )
 
-            new_kwargs["system"] += f"""
+            new_kwargs[
+                "system"
+            ] += f"""
             You must only response in JSON format that adheres to the following schema:
 
             <JSON_SCHEMA>
             {json.dumps(response_model.model_json_schema(), indent=2)}
             </JSON_SCHEMA>
             """
             new_kwargs["system"] = dedent(new_kwargs["system"])
@@ -341,14 +354,53 @@
                     {
                         "role": message["role"],
                         "message": message["content"],
                     }
                 )
             new_kwargs["message"] = instruction
             new_kwargs["chat_history"] = chat_history
+        elif mode == Mode.GEMINI_JSON:
+            message = dedent(
+                f"""
+                As a genius expert, your task is to understand the content and provide
+                the parsed objects in json that match the following json_schema:\n
+
+                {json.dumps(response_model.model_json_schema(), indent=2)}
+
+                Make sure to return an instance of the JSON, not the schema itself
+                """
+            )
+            # check that the first message is a system message
+            # if it is not, add a system message to the beginning
+            if new_kwargs["messages"][0]["role"] != "system":
+                new_kwargs["messages"].insert(
+                    0,
+                    {
+                        "role": "system",
+                        "content": message,
+                    },
+                )
+            # if it is, system append the schema to the end
+            else:
+                new_kwargs["messages"][0]["content"] += f"\n\n{message}"
+
+            # default to json response type
+            new_kwargs["generation_config"] = new_kwargs.get(
+                "generation_config", {}
+            ) | {"response_mime_type": "application/json"}
+
+            # minimize gemini safety related errors - model is highly prone to false alarms
+            new_kwargs["safety_settings"] = new_kwargs.get("safety_settings", {}) | {
+                HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
+                HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
+                HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
+            }
+            # gemini has a different prompt format and params from other providers
+            new_kwargs["contents"] = transform_to_gemini_prompt(new_kwargs["messages"])
+            del new_kwargs["messages"]
         else:
             raise ValueError(f"Invalid patch mode: {mode}")
 
     logger.debug(
         f"Instructor Request: {mode.value=}, {response_model=}, {new_kwargs=}",
         extra={
             "mode": mode.value,
```

### Comparing `instructor-1.2.6/instructor/retry.py` & `instructor-1.3.0/instructor/retry.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,22 @@
         return
     if mode == Mode.COHERE_TOOLS:
         yield {
             "role": "user",
             "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
         }
         return
+    if mode == Mode.GEMINI_JSON:
+        yield {
+            "role": "user",
+            "parts": [
+                f"Correct the following JSON response, based on the errors given below:\n\nJSON:\n{response.text}\n\nExceptions:\n{exception}"
+            ],
+        }
+        return
 
     yield dump_message(response.choices[0].message)
     # TODO: Give users more control on configuration
     if mode == Mode.TOOLS:
         for tool_call in response.choices[0].message.tool_calls:
             yield {
                 "role": "tool",
@@ -161,32 +169,35 @@
                         stream=stream,
                         validation_context=validation_context,
                         strict=strict,
                         mode=mode,
                     )
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}")
-                    kwargs["messages"].extend(reask_messages(response, mode, e))
+                    if mode in {Mode.GEMINI_JSON}:
+                        kwargs["contents"].extend(reask_messages(response, mode, e))
+                    else:
+                        kwargs["messages"].extend(reask_messages(response, mode, e))
                     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
                         kwargs["messages"] = merge_consecutive_messages(
                             kwargs["messages"]
                         )
                     raise InstructorRetryException(
                         e,
                         last_completion=response,
                         n_attempts=attempt.retry_state.attempt_number,
-                        messages=kwargs["messages"],
+                        messages=kwargs.get("messages", kwargs.get("contents")),
                         total_usage=total_usage,
                     ) from e
     except RetryError as e:
         raise InstructorRetryException(
             e,
             last_completion=response,
             n_attempts=attempt.retry_state.attempt_number,
-            messages=kwargs["messages"],
+            messages=kwargs.get("messages", kwargs.get("contents")),
             total_usage=total_usage,
         ) from e
 
 
 async def retry_async(
     func: Callable[T_ParamSpec, T_Retval],
     response_model: type[T] | None,
```

### Comparing `instructor-1.2.6/instructor/utils.py` & `instructor-1.3.0/instructor/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
     ANYSCALE = "anyscale"
     TOGETHER = "together"
     GROQ = "groq"
     MISTRAL = "mistral"
     COHERE = "cohere"
+    GEMINI = "gemini"
+    DATABRICKS = "databricks"
     UNKNOWN = "unknown"
 
 
 def get_provider(base_url: str) -> Provider:
     if "anyscale" in str(base_url):
         return Provider.ANYSCALE
     elif "together" in str(base_url):
@@ -57,14 +59,18 @@
         return Provider.GROQ
     elif "openai" in str(base_url):
         return Provider.OPENAI
     elif "mistral" in str(base_url):
         return Provider.MISTRAL
     elif "cohere" in str(base_url):
         return Provider.COHERE
+    elif "gemini" in str(base_url):
+        return Provider.GEMINI
+    elif "databricks" in str(base_url):
+        return Provider.DATABRICKS
     return Provider.UNKNOWN
 
 
 def extract_json_from_codeblock(content: str) -> str:
     first_paren = content.find("{")
     last_paren = content.rfind("}")
     return content[first_paren : last_paren + 1]
@@ -168,21 +174,30 @@
         is_coroutine = is_coroutine or inspect.iscoroutinefunction(func)
     return is_coroutine
 
 
 def merge_consecutive_messages(messages: list[dict[str, Any]]) -> list[dict[str, Any]]:
     # merge all consecutive user messages into a single message
     new_messages: list[dict[str, Any]] = []
+    # Detect whether all messages have a flat content (i.e. all string)
+    # Some providers require content to be a string, so we need to check that and behave accordingly
+    flat_string = all(isinstance(m["content"], str) for m in messages)
     for message in messages:
         new_content = message["content"]
-        if isinstance(new_content, str):
+        if not flat_string and isinstance(new_content, str):
+            # If content is not flat, transform it into a list of text
             new_content = [{"type": "text", "text": new_content}]
 
         if len(new_messages) > 0 and message["role"] == new_messages[-1]["role"]:
-            new_messages[-1]["content"].extend(new_content)
+            if flat_string:
+                # New content is a string
+                new_messages[-1]["content"] += f"\n\n{new_content}"
+            else:
+                # New content is a list
+                new_messages[-1]["content"].extend(new_content)
         else:
             new_messages.append(
                 {
                     "role": message["role"],
                     "content": new_content,
                 }
             )
@@ -205,7 +220,25 @@
     """
 
     def __init__(self, method: Callable[[Any], R_co]) -> None:
         self.cproperty = method
 
     def __get__(self, instance: object, cls: type[Any]) -> R_co:
         return self.cproperty(cls)
+
+
+def transform_to_gemini_prompt(
+    messages_chatgpt: list[ChatCompletionMessageParam],
+) -> list[dict[str, Any]]:
+    messages_gemini: list[dict[str, Any]] = []
+    system_prompt = ""
+    for message in messages_chatgpt:
+        if message["role"] == "system":
+            system_prompt = message["content"]
+        elif message["role"] == "user":
+            messages_gemini.append({"role": "user", "parts": [message["content"]]})
+        elif message["role"] == "assistant":
+            messages_gemini.append({"role": "model", "parts": [message["content"]]})
+    if system_prompt:
+        messages_gemini[0]["parts"].insert(0, f"*{system_prompt}*")
+
+    return messages_gemini
```

### Comparing `instructor-1.2.6/pyproject.toml` & `instructor-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.6"
+version = "1.3.0"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
@@ -23,27 +23,29 @@
 fastapi = { version = "^0.109.2", optional = true }
 redis = { version = "^5.0.1", optional = true }
 diskcache = { version = "^5.6.3", optional = true }
 pandas = { version = "^2.2.0", optional = true }
 tabulate = { version = "^0.9.0", optional = true }
 pydantic_extra_types = { version = "^2.6.0", optional = true }
 litellm = { version = "^1.35.31", optional = true }
-anthropic = { version = "^0.23.1", optional = true }
+anthropic = { version = "^0.26.0", optional = true }
 xmltodict = { version = "^0.13.0", optional = true }
 groq = { version = "^0.4.2", optional = true }
 cohere = { version = "^5.1.8", optional = true }
 mistralai = { version = "^0.1.8", optional = true }
+google-generativeai = { version = "^0.5.4", optional = true }
 
 [tool.poetry.extras]
 anthropic = ["anthropic", "xmltodict"]
 groq = ["groq"]
 cohere = ["cohere"]
 test-docs = ["fastapi", "redis", "diskcache", "pandas", "tabulate", "pydantic_extra_types", "litellm", "anthropic", "groq", "cohere", "mistralai"]
 mistralai = ["mistralai"]
 litellm = ["litellm"]
+google-generativeai = ["google-generativeai"]
 
 [tool.poetry.scripts]
 instructor = "instructor.cli.cli:app"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
@@ -58,25 +60,25 @@
 pytest-examples = "^0.0.10"
 mkdocs-jupyter = "^0.24.6"
 mkdocs-rss-plugin = "^1.12.0"
 mkdocs-minify-plugin = "^0.8.0"
 mkdocs-redirects = "^1.2.1"
 
 [tool.poetry.group.anthropic.dependencies]
-anthropic = "^0.23.1"
+anthropic = "^0.26.0"
 
 [tool.poetry.group.test-docs.dependencies]
 fastapi = "^0.109.2"
 redis = "^5.0.1"
 diskcache = "^5.6.3"
 pandas = "^2.2.0"
 tabulate = "^0.9.0"
 pydantic_extra_types = "^2.6.0"
 litellm = "^1.35.31"
-anthropic = "^0.23.1"
+anthropic = "^0.26.0"
 xmltodict = "^0.13.0"
 groq = "^0.4.2"
 phonenumbers = "^8.13.33"
 cohere = "^5.1.8"
 mistralai = "^0.1.8"
 
 [tool.poetry.group.litellm.dependencies]
```

### Comparing `instructor-1.2.6/PKG-INFO` & `instructor-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.6
+Version: 1.3.0
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Provides-Extra: cohere
+Provides-Extra: google-generativeai
 Provides-Extra: groq
 Provides-Extra: litellm
 Provides-Extra: mistralai
 Provides-Extra: test-docs
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "test-docs"
+Requires-Dist: anthropic (>=0.26.0,<0.27.0) ; extra == "anthropic" or extra == "test-docs"
 Requires-Dist: cohere (>=5.1.8,<6.0.0) ; extra == "cohere" or extra == "test-docs"
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.16,<0.17)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
+Requires-Dist: google-generativeai (>=0.5.4,<0.6.0) ; extra == "google-generativeai"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
 Requires-Dist: litellm (>=1.35.31,<2.0.0) ; extra == "test-docs" or extra == "litellm"
 Requires-Dist: mistralai (>=0.1.8,<0.2.0) ; extra == "test-docs" or extra == "mistralai"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
@@ -43,25 +45,25 @@
 Description-Content-Type: text/markdown
 
 # Instructor: Structured LLM Outputs
 
 Instructor is a Python library that makes it a breeze to work with structured outputs from large language models (LLMs). Built on top of Pydantic, it provides a simple, transparent, and user-friendly API to manage validation, retries, and streaming responses. Get ready to supercharge your LLM workflows!
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/jxnlco?style=social)](https://twitter.com/jxnlco)
-[![Discord](https://img.shields.io/discord/1192334452110659664?label=discord)](https://discord.gg/CV8sPM5k5Y)
+[![Discord](https://img.shields.io/discord/1192334452110659664?label=discord)](https://discord.gg/bD9YE9JArw)
 [![Downloads](https://img.shields.io/pypi/dm/instructor.svg)](https://pypi.python.org/pypi/instructor)
 
-
 ## Key Features
 
 - **Response Models**: Specify Pydantic models to define the structure of your LLM outputs
 - **Retry Management**: Easily configure the number of retry attempts for your requests
 - **Validation**: Ensure LLM responses conform to your expectations with Pydantic validation
 - **Streaming Support**: Work with Lists and Partial responses effortlessly
 - **Flexible Backends**: Seamlessly integrate with various LLM providers beyond OpenAI
+- **Support in many Languages**: We support many languages including [Python](https://python.useinstructor.com), [TypeScript](https://js.useinstructor.com), [Ruby](https://ruby.useinstructor.com), [Go](https://go.useinstructor.com), and [Elixir](https://hex.pm/packages/instructor)
 
 ## Get Started in Minutes
 
 Install Instructor with a single command:
 
 ```bash
 pip install -U instructor
@@ -165,14 +167,54 @@
 )
 
 assert isinstance(resp, User)
 assert resp.name == "Jason"
 assert resp.age == 25
 ```
 
+### Using Gemini Models
+
+Make sure you [install](https://ai.google.dev/api/python/google/generativeai#setup) the Google AI Python SDK. You should set a `GOOGLE_API_KEY` environment variable with your API key.
+
+```
+pip install google-generativeai
+```
+
+```python
+import instructor
+import google.generativeai as genai
+from pydantic import BaseModel
+
+class User(BaseModel):
+    name: str
+    age: int
+
+# genai.configure(api_key=os.environ["API_KEY"]) # alternative API key configuration
+client = instructor.from_gemini(
+    client=genai.GenerativeModel(
+        model_name="models/gemini-1.5-flash-latest", # model defaults to "gemini-pro"
+    ),
+    mode=instructor.Mode.GEMINI_JSON,
+)
+
+# note that client.chat.completions.create will also work
+resp = client.chat.completions.create(
+    messages=[
+        {
+            "role": "user",
+            "content": "Extract Jason is 25 years old.",
+        }
+    ],
+    response_model=User,
+)
+
+assert isinstance(resp, User)
+assert resp.name == "Jason"
+assert resp.age == 25
+```
 
 ### Using Litellm
 
 ```python
 import instructor
 from litellm import completion
 from pydantic import BaseModel
@@ -291,15 +333,14 @@
     ],
     response_model=User,
 )
 ```
 
 ![with_completion](./docs/blog/posts/img/with_completion.png)
 
-
 ### Streaming Partial Objects: `create_partial`
 
 In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simply the type inference, we've added `create_iterable` and `create_partial` methods as well!
 
 ```python
 import openai
 import instructor
```

