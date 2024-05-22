# Comparing `tmp/llama_index_readers_pebblo-0.1.0.tar.gz` & `tmp/llama_index_readers_pebblo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_pebblo-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_readers_pebblo-0.1.1.tar", max compression
```

## Comparing `llama_index_readers_pebblo-0.1.0.tar` & `llama_index_readers_pebblo-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2003 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/BUILD
--rw-r--r--   0        0        0      102 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/__init__.py
--rw-r--r--   0        0        0     9164 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/base.py
--rw-r--r--   0        0        0     6237 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/utility.py
--rw-r--r--   0        0        0     1620 2024-05-09 04:20:44.421718 llama_index_readers_pebblo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 llama_index_readers_pebblo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2003 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/BUILD
+-rw-r--r--   0        0        0      102 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/__init__.py
+-rw-r--r--   0        0        0     9164 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/base.py
+-rw-r--r--   0        0        0     6237 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/utility.py
+-rw-r--r--   0        0        0     1653 2024-05-22 23:07:54.422797 llama_index_readers_pebblo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 llama_index_readers_pebblo-0.1.1/PKG-INFO
```

### Comparing `llama_index_readers_pebblo-0.1.0/README.md` & `llama_index_readers_pebblo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/base.py` & `llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_pebblo-0.1.0/llama_index/readers/pebblo/utility.py` & `llama_index_readers_pebblo-0.1.1/llama_index/readers/pebblo/utility.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_pebblo-0.1.0/pyproject.toml` & `llama_index_readers_pebblo-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 [tool.poetry]
 authors = ["Yograj Shisode <yograj.shisode@opcito.com>"]
 description = "llama-index readers pebblo integration"
 license = "MIT"
 name = "llama-index-readers-pebblo"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
-llama-index = "^0.10.20"
+langchain-community = ">=0.0.303"
+langchain = ">=0.0.303"
 requests = "^2"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_readers_pebblo-0.1.0/PKG-INFO` & `llama_index_readers_pebblo-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-pebblo
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index readers pebblo integration
 License: MIT
 Author: Yograj Shisode
 Author-email: yograj.shisode@opcito.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index (>=0.10.20,<0.11.0)
+Requires-Dist: langchain (>=0.0.303)
+Requires-Dist: langchain-community (>=0.0.303)
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
 Requires-Dist: requests (>=2,<3)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: Pebblo
 
 ## Pebblo Safe DocumentReader
```

