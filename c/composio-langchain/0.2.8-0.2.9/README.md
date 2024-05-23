# Comparing `tmp/composio_langchain-0.2.8.tar.gz` & `tmp/composio_langchain-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.2.8.tar", last modified: Thu Apr 18 18:07:38 2024, max compression
+gzip compressed data, was "composio_langchain-0.2.9.tar", last modified: Thu Apr 18 18:49:46 2024, max compression
```

## Comparing `composio_langchain-0.2.8.tar` & `composio_langchain-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:38.036958 composio_langchain-0.2.8/
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_langchain-0.2.8/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-18 18:07:38.036703 composio_langchain-0.2.8/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-15 07:39:40.000000 composio_langchain-0.2.8/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:38.035408 composio_langchain-0.2.8/composio_langchain/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      101 2024-04-15 07:39:40.000000 composio_langchain-0.2.8/composio_langchain/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5332 2024-04-18 18:05:51.000000 composio_langchain-0.2.8/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-15 07:39:40.000000 composio_langchain-0.2.8/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:38.036363 composio_langchain-0.2.8/composio_langchain.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-18 18:07:38.000000 composio_langchain-0.2.8/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-18 18:07:38.000000 composio_langchain-0.2.8/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:07:38.000000 composio_langchain-0.2.8/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      148 2024-04-18 18:07:38.000000 composio_langchain-0.2.8/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-18 18:07:38.000000 composio_langchain-0.2.8/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      454 2024-04-18 18:07:01.000000 composio_langchain-0.2.8/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:07:38.037011 composio_langchain-0.2.8/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-18 18:07:01.000000 composio_langchain-0.2.8/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:46.814406 composio_langchain-0.2.9/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_langchain-0.2.9/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-18 18:49:46.814221 composio_langchain-0.2.9/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-15 07:39:40.000000 composio_langchain-0.2.9/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:46.812709 composio_langchain-0.2.9/composio_langchain/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      101 2024-04-15 07:39:40.000000 composio_langchain-0.2.9/composio_langchain/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5332 2024-04-18 18:05:51.000000 composio_langchain-0.2.9/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-15 07:39:40.000000 composio_langchain-0.2.9/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:46.814017 composio_langchain-0.2.9/composio_langchain.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-18 18:49:46.000000 composio_langchain-0.2.9/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-18 18:49:46.000000 composio_langchain-0.2.9/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:46.000000 composio_langchain-0.2.9/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      148 2024-04-18 18:49:46.000000 composio_langchain-0.2.9/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-18 18:49:46.000000 composio_langchain-0.2.9/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      454 2024-04-18 18:44:03.000000 composio_langchain-0.2.9/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:46.814447 composio_langchain-0.2.9/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-18 18:44:03.000000 composio_langchain-0.2.9/setup.py
```

### Comparing `composio_langchain-0.2.8/PKG-INFO` & `composio_langchain-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.8
+Requires-Dist: composio_core===0.2.9
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.2.8/README.md` & `composio_langchain-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.8/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.2.9/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.8/composio_langchain/pydantic_utils.py` & `composio_langchain-0.2.9/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.8/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.2.9/composio_langchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.8
+Requires-Dist: composio_core===0.2.9
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.2.8/setup.py` & `composio_langchain-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.2.8",
+    version="0.2.9",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

