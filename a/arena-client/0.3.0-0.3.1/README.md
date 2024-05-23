# Comparing `tmp/arena_client-0.3.0.tar.gz` & `tmp/arena_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena_client-0.3.0.tar", max compression
+gzip compressed data, was "arena_client-0.3.1.tar", max compression
```

## Comparing `arena_client-0.3.0.tar` & `arena_client-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      123 2024-05-23 15:50:43.500275 arena_client-0.3.0/README.md
--rw-r--r--   0        0        0     1387 2024-05-23 15:50:43.500275 arena_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      154 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/__init__.py
--rw-r--r--   0        0        0    15342 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/client.py
--rw-r--r--   0        0        0     1018 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/__init__.py
--rw-r--r--   0        0        0     4009 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/anthropic.py
--rw-r--r--   0        0        0     4364 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/chat_completion.py
--rw-r--r--   0        0        0      281 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/evaluation.py
--rw-r--r--   0        0        0     2287 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/mistral.py
--rw-r--r--   0        0        0     1444 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/openai.py
--rw-r--r--   0        0        0      237 2024-05-23 15:50:43.500275 arena_client-0.3.0/src/arena/models/settings.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 arena_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-05-23 16:05:15.360416 arena_client-0.3.1/README.md
+-rw-r--r--   0        0        0     1387 2024-05-23 16:05:15.360416 arena_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/__init__.py
+-rw-r--r--   0        0        0    15342 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/client.py
+-rw-r--r--   0        0        0     1018 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/anthropic.py
+-rw-r--r--   0        0        0     4364 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/chat_completion.py
+-rw-r--r--   0        0        0      281 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/evaluation.py
+-rw-r--r--   0        0        0     2287 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/mistral.py
+-rw-r--r--   0        0        0     1444 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/openai.py
+-rw-r--r--   0        0        0      237 2024-05-23 16:05:15.360416 arena_client-0.3.1/src/arena/models/settings.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 arena_client-0.3.1/PKG-INFO
```

### Comparing `arena_client-0.3.0/pyproject.toml` & `arena_client-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "arena-client"
-version = "0.3.0"
+version = "0.3.1"
 description = "A client to use arena AI"
 authors = ["Nicolas Grislain <ng@sarus.tech>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [{from = "src", include = "arena"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 httpx = "^0.25"
 openai = "^1.23"
 anthropic = "^0.21"
 mistralai = "^0.1"
 anyio = {extras = ["trio"], version = "^4.3.0"}
 pyarrow = "^16.1.0"
 parquet = "^1.3.1"
@@ -26,15 +26,15 @@
 faker = "^25.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-target-version = "py311"
+target-version = "py310"
 
 [tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
```

### Comparing `arena_client-0.3.0/src/arena/client.py` & `arena_client-0.3.1/src/arena/client.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/src/arena/models/__init__.py` & `arena_client-0.3.1/src/arena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/src/arena/models/anthropic.py` & `arena_client-0.3.1/src/arena/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/src/arena/models/chat_completion.py` & `arena_client-0.3.1/src/arena/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/src/arena/models/mistral.py` & `arena_client-0.3.1/src/arena/models/mistral.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/src/arena/models/openai.py` & `arena_client-0.3.1/src/arena/models/openai.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.3.0/PKG-INFO` & `arena_client-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: arena-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: A client to use arena AI
 License: Apache-2
 Author: Nicolas Grislain
 Author-email: ng@sarus.tech
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.21,<0.22)
 Requires-Dist: anyio[trio] (>=4.3.0,<5.0.0)
 Requires-Dist: httpx (>=0.25,<0.26)
 Requires-Dist: mistralai (>=0.1,<0.2)
 Requires-Dist: openai (>=1.23,<2.0)
```

