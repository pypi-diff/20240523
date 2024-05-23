# Comparing `tmp/openlit-1.7.0.tar.gz` & `tmp/openlit-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.7.0.tar", max compression
+gzip compressed data, was "openlit-1.8.0.tar", max compression
```

## Comparing `openlit-1.7.0.tar` & `openlit-1.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11357 2024-05-17 11:26:01.639458 openlit-1.7.0/LICENSE
--rw-r--r--   0        0        0    10980 2024-05-17 11:26:01.639458 openlit-1.7.0/README.md
--rw-r--r--   0        0        0      966 2024-05-17 11:26:01.639458 openlit-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/__helpers.py
--rw-r--r--   0        0        0     9917 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    16026 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16068 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10407 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20381 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     1911 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0    19084 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/groq/async_groq.py
--rw-r--r--   0        0        0    19048 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/groq/groq.py
--rw-r--r--   0        0        0     1758 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/haystack/__init__.py
--rw-r--r--   0        0        0     3891 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/haystack/haystack.py
--rw-r--r--   0        0        0     2531 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7639 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     1973 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     4048 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/llamaindex/llamaindex.py
--rw-r--r--   0        0        0     2961 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/milvus/__init__.py
--rw-r--r--   0        0        0     9121 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/milvus/milvus.py
--rw-r--r--   0        0        0     3156 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21361 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21212 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0     3812 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/ollama/__init__.py
--rw-r--r--   0        0        0    28991 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/ollama/async_ollama.py
--rw-r--r--   0        0        0    28901 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/ollama/ollama.py
--rw-r--r--   0        0        0    16265 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8765 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     4799 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0    14436 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/qdrant/qdrant.py
--rw-r--r--   0        0        0     1478 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     6079 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/vertexai/__init__.py
--rw-r--r--   0        0        0    52372 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/vertexai/async_vertexai.py
--rw-r--r--   0        0        0    52125 2024-05-17 11:26:01.639458 openlit-1.7.0/src/openlit/instrumentation/vertexai/vertexai.py
--rw-r--r--   0        0        0     4291 2024-05-17 11:26:01.643458 openlit-1.7.0/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3712 2024-05-17 11:26:01.643458 openlit-1.7.0/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     6328 2024-05-17 11:26:01.643458 openlit-1.7.0/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    12280 1970-01-01 00:00:00.000000 openlit-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 11:34:43.013329 openlit-1.8.0/LICENSE
+-rw-r--r--   0        0        0    11181 2024-05-23 11:34:43.013329 openlit-1.8.0/README.md
+-rw-r--r--   0        0        0      966 2024-05-23 11:34:43.013329 openlit-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5545 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0    10141 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16068 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10407 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20381 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     1911 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0    19084 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/async_groq.py
+-rw-r--r--   0        0        0    19048 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/groq.py
+-rw-r--r--   0        0        0     1758 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/haystack/__init__.py
+-rw-r--r--   0        0        0     3891 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/haystack/haystack.py
+-rw-r--r--   0        0        0     2531 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7639 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     1973 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     4048 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/llamaindex/llamaindex.py
+-rw-r--r--   0        0        0     2961 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/milvus/__init__.py
+-rw-r--r--   0        0        0     9121 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/milvus/milvus.py
+-rw-r--r--   0        0        0     3156 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21212 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0     3812 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/__init__.py
+-rw-r--r--   0        0        0    28991 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/async_ollama.py
+-rw-r--r--   0        0        0    28901 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/ollama.py
+-rw-r--r--   0        0        0    16265 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8765 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     4799 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0    14436 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1478 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     6079 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0    52372 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/async_vertexai.py
+-rw-r--r--   0        0        0    52125 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/vertexai.py
+-rw-r--r--   0        0        0     4291 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3712 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     6328 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    12481 1970-01-01 00:00:00.000000 openlit-1.8.0/PKG-INFO
```

### Comparing `openlit-1.7.0/LICENSE` & `openlit-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/README.md` & `openlit-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 | `meter`                 | An OpenTelemetry Metrics instance for capturing metrics.                                      | `None`         |    No    |
 | `otlp_endpoint`         | Specifies the OTLP endpoint for transmitting telemetry data.                                  | `None`         |    No    |
 | `otlp_headers`          | Defines headers for the OTLP exporter, useful for backends requiring authentication.          | `None`         |    No    |
 | `disable_batch`         | A flag to disable batch span processing, favoring immediate dispatch.                         | `False`        |    No    |
 | `trace_content`         | Enables tracing of content for deeper insights.                                               | `True`         |    No    |
 | `disabled_instrumentors`| List of instrumentors to disable. Choices: `["openai", "anthropic", "langchain", "cohere", "mistral", "transformers", "chroma", "pinecone"]`. | `None` |    No    |
 | `disable_metrics`       | If set, disables the collection of metrics.                                                   | `False`        |    No    |
+| `pricing_json`          | URL or file path of the pricing JSON file.                                             | `https://github.com/openlit/openlit/blob/main/assets/pricing.json`        |    No    |
 
 ## 🌱 Contributing
 
 Whether it's big or small, we love contributions 💚. Check out our [Contribution guide](../../CONTRIBUTING.md) to get started
 
 Unsure where to start? Here are a few ways to get involved:
 
@@ -154,8 +155,8 @@
 ## 💚 Community & Support
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
-- 𝕏 Follow us on [X](https://twitter.com/openlit) for the latest updates and news.
+- 𝕏 Follow us on [X](https://x.com/openlit_io) for the latest updates and news.
```

### Comparing `openlit-1.7.0/pyproject.toml` & `openlit-1.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.7.0"
+version = "1.8.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.7.0/src/openlit/__helpers.py` & `openlit-1.8.0/src/openlit/__helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=bare-except, broad-exception-caught
 """
 This module has functions to calculate model costs based on tokens and to fetch pricing information.
 """
-
+import json
 import logging
+from urllib.parse import urlparse
 import requests
 import tiktoken
 from opentelemetry.trace import Status, StatusCode
 
 # Set up logging
 logger = logging.getLogger(__name__)
 
@@ -118,19 +119,43 @@
     """
     try:
         cost = (len(prompt) / 1000) * pricing_info["audio"][model]
     except:
         cost = 0
     return cost
 
-def fetch_pricing_info():
-    """Fetches pricing information from a specified URL."""
-    pricing_url = "https://raw.githubusercontent.com/openlit/openlit/main/assets/pricing.json"
+def fetch_pricing_info(pricing_json=None):
+    """
+    Fetches pricing information from a specified URL or File Path.
+
+    Args:
+        pricing_json(str): path or url to the pricing json file
+
+    Returns:
+        dict: The pricing json
+    """
+    if pricing_json:
+        is_url = urlparse(pricing_json).scheme != ""
+        if is_url:
+            pricing_url = pricing_json
+        else:
+            try:
+                with open(pricing_json, mode='r', encoding='utf-8') as f:
+                    return json.load(f)
+            except FileNotFoundError:
+                logger.error("Pricing information file not found: %s", pricing_json)
+            except json.JSONDecodeError:
+                logger.error("Error decoding JSON from file: %s", pricing_json)
+            except Exception as file_err:
+                logger.error("Unexpected error occurred while reading file: %s", file_err)
+            return {}
+    else:
+        pricing_url = "https://raw.githubusercontent.com/openlit/openlit/main/assets/pricing.json"
     try:
-         # Set a timeout of 10 seconds for both the connection and the read
+        # Set a timeout of 10 seconds for both the connection and the read
         response = requests.get(pricing_url, timeout=20)
         response.raise_for_status()
         return response.json()
     except requests.HTTPError as http_err:
         logger.error("HTTP error occured while fetching pricing info: %s", http_err)
     except Exception as err:
         logger.error("Unexpected error occurred while fetching pricing info: %s", err)
```

### Comparing `openlit-1.7.0/src/openlit/__init__.py` & `openlit-1.8.0/src/openlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,31 +71,33 @@
         cls.otlp_headers = None
         cls.disable_batch = False
         cls.trace_content = True
         cls.disable_metrics = False
 
     @classmethod
     def update_config(cls, environment, application_name, tracer, otlp_endpoint,
-                      otlp_headers, disable_batch, trace_content, metrics_dict, disable_metrics):
+                      otlp_headers, disable_batch, trace_content, metrics_dict,
+                      disable_metrics, pricing_json):
         """
         Updates the configuration based on provided parameters.
 
         Args:
             environment (str): Deployment environment.
             application_name (str): Application name.
             tracer: Tracer instance.
             meter: Metric Instance
             otlp_endpoint (str): OTLP endpoint.
             otlp_headers (Dict[str, str]): OTLP headers.
             disable_batch (bool): Disable batch span processing flag.
             trace_content (bool): Enable or disable content tracing.
+            pricing_json(str): path or url to the pricing json file
         """
         cls.environment = environment
         cls.application_name = application_name
-        cls.pricing_info = fetch_pricing_info()
+        cls.pricing_info = fetch_pricing_info(pricing_json)
         cls.tracer = tracer
         cls.metrics_dict = metrics_dict
         cls.otlp_endpoint = otlp_endpoint
         cls.otlp_headers = otlp_headers
         cls.disable_batch = disable_batch
         cls.trace_content = trace_content
         cls.disable_metrics = disable_metrics
@@ -122,15 +124,15 @@
 
         # pylint: disable=broad-exception-caught
         except Exception as e:
             logger.error("Failed to instrument %s: %s", instrumentor_name, e)
 
 def init(environment="default", application_name="default", tracer=None, otlp_endpoint=None,
          otlp_headers=None, disable_batch=False, trace_content=True, disabled_instrumentors=None,
-         meter=None, disable_metrics=False):
+         meter=None, disable_metrics=False, pricing_json=None):
     """
     Initializes the openLIT configuration and setups tracing.
     
     This function sets up the openLIT environment with provided configurations 
     and initializes instrumentors for tracing.
     
     Args:
@@ -140,14 +142,15 @@
         meter: OpenTelemetry Metrics Instance (Optional).
         otlp_endpoint (str): OTLP endpoint for exporter (Optional).
         otlp_headers (Dict[str, str]): OTLP headers for exporter (Optional).
         disable_batch (bool): Flag to disable batch span processing (Optional).
         trace_content (bool): Flag to trace content (Optional).
         disabled_instrumentors (List[str]): Optional. List of instrumentor names to disable.
         disable_metrics (bool): Flag to disable metrics (Optional)
+        pricing_json(str): File path or url to the pricing json (Optional)
     """
     disabled_instrumentors = disabled_instrumentors if disabled_instrumentors else []
     # Check for invalid instrumentor names
 
     module_name_map = {
         "openai": "openai",
         "anthropic": "anthropic",  
@@ -195,15 +198,15 @@
         if not metrics_dict:
             logger.error("openLIT metrics setup failed. Metrics will not be available.")
             return
 
         # Update global configuration with the provided settings.
         config.update_config(environment, application_name, tracer, otlp_endpoint,
                              otlp_headers, disable_batch, trace_content,
-                             metrics_dict, disable_metrics)
+                             metrics_dict, disable_metrics, pricing_json)
 
         # Map instrumentor names to their instances
         instrumentor_instances = {
             "openai": OpenAIInstrumentor(),
             "anthropic": AnthropicInstrumentor(),
             "cohere": CohereInstrumentor(),
             "mistral": MistralInstrumentor(),
```

### Comparing `openlit-1.7.0/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.8.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.8.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.8.0/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.8.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.8.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/groq/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/groq/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/groq/async_groq.py` & `openlit-1.8.0/src/openlit/instrumentation/groq/async_groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/groq/groq.py` & `openlit-1.8.0/src/openlit/instrumentation/groq/groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/haystack/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/haystack/haystack.py` & `openlit-1.8.0/src/openlit/instrumentation/haystack/haystack.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.8.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/llamaindex/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/llamaindex/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/llamaindex/llamaindex.py` & `openlit-1.8.0/src/openlit/instrumentation/llamaindex/llamaindex.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/milvus/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/milvus/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/milvus/milvus.py` & `openlit-1.8.0/src/openlit/instrumentation/milvus/milvus.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.8.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.8.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/ollama/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/ollama/async_ollama.py` & `openlit-1.8.0/src/openlit/instrumentation/ollama/async_ollama.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/ollama/ollama.py` & `openlit-1.8.0/src/openlit/instrumentation/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.8.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.8.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.8.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/openai/openai.py` & `openlit-1.8.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.8.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/qdrant/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/qdrant/qdrant.py` & `openlit-1.8.0/src/openlit/instrumentation/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.8.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/vertexai/__init__.py` & `openlit-1.8.0/src/openlit/instrumentation/vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/vertexai/async_vertexai.py` & `openlit-1.8.0/src/openlit/instrumentation/vertexai/async_vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/instrumentation/vertexai/vertexai.py` & `openlit-1.8.0/src/openlit/instrumentation/vertexai/vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/otel/metrics.py` & `openlit-1.8.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/otel/tracing.py` & `openlit-1.8.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/src/openlit/semcov/__init__.py` & `openlit-1.8.0/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.7.0/PKG-INFO` & `openlit-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.7.0
+Version: 1.8.0
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -161,14 +161,15 @@
 | `meter`                 | An OpenTelemetry Metrics instance for capturing metrics.                                      | `None`         |    No    |
 | `otlp_endpoint`         | Specifies the OTLP endpoint for transmitting telemetry data.                                  | `None`         |    No    |
 | `otlp_headers`          | Defines headers for the OTLP exporter, useful for backends requiring authentication.          | `None`         |    No    |
 | `disable_batch`         | A flag to disable batch span processing, favoring immediate dispatch.                         | `False`        |    No    |
 | `trace_content`         | Enables tracing of content for deeper insights.                                               | `True`         |    No    |
 | `disabled_instrumentors`| List of instrumentors to disable. Choices: `["openai", "anthropic", "langchain", "cohere", "mistral", "transformers", "chroma", "pinecone"]`. | `None` |    No    |
 | `disable_metrics`       | If set, disables the collection of metrics.                                                   | `False`        |    No    |
+| `pricing_json`          | URL or file path of the pricing JSON file.                                             | `https://github.com/openlit/openlit/blob/main/assets/pricing.json`        |    No    |
 
 ## 🌱 Contributing
 
 Whether it's big or small, we love contributions 💚. Check out our [Contribution guide](../../CONTRIBUTING.md) to get started
 
 Unsure where to start? Here are a few ways to get involved:
 
@@ -179,9 +180,9 @@
 ## 💚 Community & Support
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
-- 𝕏 Follow us on [X](https://twitter.com/openlit) for the latest updates and news.
+- 𝕏 Follow us on [X](https://x.com/openlit_io) for the latest updates and news.
```

