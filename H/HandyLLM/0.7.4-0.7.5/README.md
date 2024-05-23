# Comparing `tmp/handyllm-0.7.4.tar.gz` & `tmp/handyllm-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handyllm-0.7.4.tar", last modified: Wed May 22 10:14:08 2024, max compression
+gzip compressed data, was "handyllm-0.7.5.tar", last modified: Thu May 23 10:29:38 2024, max compression
```

## Comparing `handyllm-0.7.4.tar` & `handyllm-0.7.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.993337 handyllm-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 10:14:04.000000 handyllm-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-22 10:14:08.993337 handyllm-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-22 10:14:04.000000 handyllm-0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 10:14:04.000000 handyllm-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:14:08.993337 handyllm-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.989337 handyllm-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.993337 handyllm-0.7.4/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 10:14:08.000000 handyllm-0.7.4/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.989337 handyllm-0.7.4/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.993337 handyllm-0.7.4/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-22 10:14:04.000000 handyllm-0.7.4/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:08.993337 handyllm-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-22 10:14:04.000000 handyllm-0.7.4/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-22 10:14:04.000000 handyllm-0.7.4/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-22 10:14:04.000000 handyllm-0.7.4/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 10:14:04.000000 handyllm-0.7.4/tests/test_hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 10:14:04.000000 handyllm-0.7.4/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 10:29:35.000000 handyllm-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-23 10:29:38.960876 handyllm-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-23 10:29:35.000000 handyllm-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 10:29:35.000000 handyllm-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:29:38.960876 handyllm-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.952875 handyllm-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.956875 handyllm-0.7.5/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32282 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16985 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_tts.py
```

### Comparing `handyllm-0.7.4/LICENSE` & `handyllm-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/PKG-INFO` & `handyllm-0.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.4
+Version: 0.7.5
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `handyllm-0.7.4/README.md` & `handyllm-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/pyproject.toml` & `handyllm-0.7.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `handyllm-0.7.4/src/HandyLLM.egg-info/PKG-INFO` & `handyllm-0.7.5/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.4
+Version: 0.7.5
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `handyllm-0.7.4/src/HandyLLM.egg-info/SOURCES.txt` & `handyllm-0.7.5/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 src/handyllm/utils.py
 src/handyllm/deprecated/api_request.py
 src/handyllm/deprecated/openai_api.py
 tests/test_azure.py
 tests/test_client_async_sync.py
 tests/test_endpoint.py
 tests/test_hprompt.py
-tests/test_prompt.py
+tests/test_prompt.py
+tests/test_tts.py
```

### Comparing `handyllm-0.7.4/src/handyllm/_str_enum.py` & `handyllm-0.7.5/src/handyllm/_str_enum.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/_utils.py` & `handyllm-0.7.5/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/cli.py` & `handyllm-0.7.5/src/handyllm/cli.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/deprecated/api_request.py` & `handyllm-0.7.5/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/deprecated/openai_api.py` & `handyllm-0.7.5/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/endpoint_manager.py` & `handyllm-0.7.5/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/hprompt.py` & `handyllm-0.7.5/src/handyllm/hprompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -316,55 +316,61 @@
     def _serialize_data(self, data) -> str:
         '''
         Serialize the data to a string. 
         This method can be overridden by subclasses.
         '''
         return str(data)
     
-    @staticmethod
-    def _dumps_frontmatter(request: dict, run_config: RunConfig, base_path: Optional[PathType] = None) -> str:
+    @classmethod
+    def _dumps_frontmatter(cls, request: dict, run_config: RunConfig, base_path: Optional[PathType] = None) -> str:
         # dump frontmatter
         if not run_config and not request:
             return ""
-        front_data = copy.deepcopy(request)
+        # need to filter the request
+        front_data = cls._filter_request(request, run_config)
         if run_config:
             front_data['meta'] = run_config.to_dict(retain_fd=False, base_path=base_path)
         post = frontmatter.Post("", None, **front_data)
         return frontmatter.dumps(post, handler).strip() + "\n\n"
     
-    @classmethod
-    def _dumps(cls, request, run_config: RunConfig, content: str, base_path: Optional[PathType] = None) -> str:
-        return cls._dumps_frontmatter(request, run_config, base_path) + content
-    
     def dumps(self, base_path: Optional[PathType] = None) -> str:
         serialized_data = self._serialize_data(self.data)
         base_path = base_path or self.base_path
-        return self._dumps(self.request, self.run_config, serialized_data, base_path)
+        return self._dumps_frontmatter(self.request, self.run_config, base_path) + serialized_data
     
     def dump(self, fd: io.IOBase, base_path: Optional[PathType] = None) -> None:
         text = self.dumps(base_path=base_path)
         fd.write(text)
     
     def dump_to(self, path: PathType) -> None:
         with open(path, "w", encoding="utf-8") as fd:
             self.dump(fd, base_path=Path(path).parent.resolve())
     
     @abstractmethod
     def _eval_data(self: PromptType, run_config: RunConfig) -> Union[str, list]:
         ...
     
-    def eval(self: PromptType, run_config: RunConfig) -> PromptType:
-        new_data = self._eval_data(run_config)
-        if new_data != self.data:
-            return self.__class__(
-                new_data,
-                copy.deepcopy(self.request),
-                replace(self.run_config),
-            )
-        return self
+    def eval(
+        self: PromptType, 
+        run_config: RunConfig = DEFAULT_CONFIG,
+        **kwargs) -> PromptType:
+        '''
+        Evaluate the prompt with the given run_config. 
+        A new prompt object is returned.
+        '''
+        new_run_config = self.eval_run_config(run_config)
+        new_data = self._eval_data(new_run_config)
+        # update the request with the keyword arguments
+        evaled_request = copy.deepcopy(self.request)
+        evaled_request.update(kwargs)
+        return self.__class__(
+            new_data,
+            evaled_request,
+            new_run_config,
+        )
     
     def eval_run_config(
         self: PromptType, 
         run_config: RunConfig, 
         ) -> RunConfig:
         # merge runtime run_config with the original run_config
         run_config = self.run_config.merge(run_config)
@@ -386,59 +392,59 @@
                 p = Path(run_config.credential_path)
                 if p.suffix:
                     run_config.credential_type = p.suffix[1:]
                 else:
                     run_config.credential_type = CredentialType.ENV
         return run_config
     
+    @classmethod
     @abstractmethod
     def _run_with_client(
-        self: PromptType, 
+        cls, 
         client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> PromptType:
         ...
     
     def run(
         self: PromptType, 
         client: OpenAIClient = None, 
         run_config: RunConfig = DEFAULT_CONFIG,
         **kwargs) -> PromptType:
-        run_config, new_request, stream = self._prepare_run(run_config, kwargs)
+        evaled_prompt, stream = self._prepare_run(run_config, kwargs)
         if client:
-            new_prompt = self._run_with_client(client, run_config, new_request, stream)
+            new_prompt = self._run_with_client(client, evaled_prompt, stream)
         else:
             with OpenAIClient(ClientMode.SYNC) as client:
-                new_prompt = self._run_with_client(client, run_config, new_request, stream)
+                new_prompt = self._run_with_client(client, evaled_prompt, stream)
         self._post_check_output(stream, run_config, new_prompt)
         return new_prompt
     
+    @classmethod
     @abstractmethod
     async def _arun_with_client(
-        self: PromptType, 
+        cls, 
         client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> PromptType:
         ...
     
     async def arun(
         self: PromptType, 
         client: OpenAIClient = None, 
         run_config: RunConfig = DEFAULT_CONFIG,
         **kwargs) -> PromptType:
-        run_config, new_request, stream = self._prepare_run(run_config, kwargs)
+        evaled_prompt, stream = self._prepare_run(run_config, kwargs)
         if client:
-            new_prompt = await self._arun_with_client(client, run_config, new_request, stream)
+            new_prompt = await self._arun_with_client(client, evaled_prompt, stream)
         else:
             async with OpenAIClient(ClientMode.ASYNC) as client:
-                new_prompt = await self._arun_with_client(client, run_config, new_request, stream)
+                new_prompt = await self._arun_with_client(client, evaled_prompt, stream)
         self._post_check_output(stream, run_config, new_prompt)
         return new_prompt
     
     def _prepare_output_path(
         self, output_path: PathType, start_time: datetime, template_filename: str
         ) -> str:
         output_path = str(output_path).strip()
@@ -449,97 +455,92 @@
         # format output_path with the current time
         output_path = start_time.strftime(str(output_path))
         # create the parent directory if it does not exist
         Path(output_path).parent.mkdir(parents=True, exist_ok=True)
         return output_path
     
     def _prepare_run(self: PromptType, run_config: RunConfig, kwargs: dict):
-        # update the request with the keyword arguments
-        new_request = copy.deepcopy(self.request)
-        new_request.update(kwargs)
-        # get the stream flag
-        stream = new_request.get("stream", False)
+        # evaluate the prompt with the given run_config
+        evaled_prompt = self.eval(run_config=run_config, **kwargs)
+        evaled_run_config = evaled_prompt.run_config
+        evaled_request = evaled_prompt.request
         
-        # evaluate the run_config
-        run_config = self.eval_run_config(run_config)
+        # get the stream flag
+        stream = evaled_request.get("stream", False)
         
         # verbose output
-        if run_config.verbose:
+        if evaled_run_config.verbose:
             print("---", file=sys.stderr)
             print("NEW RUN")
             print(f"Start time: {datetime.now()}", file=sys.stderr)
-            run_config.pretty_print()
+            evaled_run_config.pretty_print()
             print("---", file=sys.stderr)
         
+        # output the evaluated prompt to a file or a file descriptor
+        # NOTE: should be done before loading the credential file
+        if evaled_run_config.output_evaled_prompt_fd:
+            evaled_prompt.dump(evaled_run_config.output_evaled_prompt_fd)
+        elif evaled_run_config.output_evaled_prompt_path:
+            evaled_prompt.dump_to(evaled_run_config.output_evaled_prompt_path)
+        
         # load the credential file
-        if run_config.credential_path:
-            if run_config.credential_type == CredentialType.ENV:
-                load_dotenv(run_config.credential_path, override=True)
-            elif run_config.credential_type in (CredentialType.JSON, CredentialType.YAML):
-                with open(run_config.credential_path, 'r', encoding='utf-8') as fin:
-                    if run_config.credential_type == CredentialType.JSON:
+        if evaled_run_config.credential_path:
+            if evaled_run_config.credential_type == CredentialType.ENV:
+                load_dotenv(evaled_run_config.credential_path, override=True)
+            elif evaled_run_config.credential_type in (CredentialType.JSON, CredentialType.YAML):
+                with open(evaled_run_config.credential_path, 'r', encoding='utf-8') as fin:
+                    if evaled_run_config.credential_type == CredentialType.JSON:
                         credential_dict = json.load(fin)
                     else:
                         credential_dict = yaml.safe_load(fin)
-                new_request.update(credential_dict)
+                # do not overwrite the existing request arguments
+                for key, value in credential_dict.items():
+                    if key not in evaled_request:
+                        evaled_request[key] = value
             else:
-                raise ValueError(f"unsupported credential type: {run_config.credential_type}")
+                raise ValueError(f"unsupported credential type: {evaled_run_config.credential_type}")
         
-        # output the evaluated prompt to a file or a file descriptor
-        if run_config.output_evaled_prompt_path \
-            or run_config.output_evaled_prompt_fd:
-            evaled_data = self._eval_data(run_config)
-            serialized_data = self._serialize_data(evaled_data)
-            text = self._dumps(
-                self.request, run_config, serialized_data, 
-                Path(run_config.output_evaled_prompt_path).parent.resolve() \
-                    if run_config.output_evaled_prompt_path else None
-            )
-            if run_config.output_evaled_prompt_path:
-                with open(run_config.output_evaled_prompt_path, 'w', encoding='utf-8') as fout:
-                    fout.write(text)
-            elif run_config.output_evaled_prompt_fd:
-                run_config.output_evaled_prompt_fd.write(text)
-        return run_config, new_request, stream
+        return evaled_prompt, stream
     
     def _post_check_output(self: PromptType, stream: bool, run_config: RunConfig, new_prompt: PromptType):
         if not stream:
             # if stream is True, the response is already streamed to 
             # a file or a file descriptor
-            if run_config.output_path:
-                new_prompt.dump_to(run_config.output_path)
-            elif run_config.output_fd:
+            if run_config.output_fd:
                 new_prompt.dump(run_config.output_fd)
+            elif run_config.output_path:
+                new_prompt.dump_to(run_config.output_path)
         return new_prompt
 
     def _merge_non_data(self: PromptType, other: PromptType, inplace=False) -> Union[None, tuple[dict, RunConfig]]:
         if inplace:
             merge(self.request, other.request, strategy=Strategy.ADDITIVE)
             self.run_config.merge(other.run_config, inplace=True)
         else:
             merged_request = merge({}, self.request, other.request, strategy=Strategy.ADDITIVE)
             merged_run_config = self.run_config.merge(other.run_config)
             return merged_request, merged_run_config
     
+    @staticmethod
     def _filter_request(
-        self, request: dict, 
+        request: dict, 
         run_config: RunConfig,
         ) -> dict:
         if run_config.record_request == RecordRequestMode.WHITELIST:
             if run_config.record_whitelist:
                 request = {key: value for key, value in request.items() if key in run_config.record_whitelist}
             else:
                 request = {}
         elif run_config.record_request == RecordRequestMode.NONE:
             request = {}
         elif run_config.record_request == RecordRequestMode.ALL:
             pass
         else:
             # default: blacklist
-            # will modify the original request
+            request = copy.deepcopy(request)
             real_blacklist = run_config.record_blacklist or DEFAULT_BLACKLIST
             for key in real_blacklist:
                 request.pop(key, None)
         return request
     
     def _parse_var_map(self, run_config: RunConfig):
         var_map = {}
@@ -582,77 +583,78 @@
         return self.messages[-1]['content']
     
     def _serialize_data(self, data) -> str:
         return converter.msgs2raw(data)
     
     def _eval_data(self, run_config: RunConfig) -> list:
         var_map = self._parse_var_map(run_config)
-        if var_map:
-            return converter.msgs_replace_variables(
-                self.messages, var_map, inplace=False)
-        else:
-            return self.messages
+        return converter.msgs_replace_variables(
+            self.messages, var_map, inplace=False)
     
+    @classmethod
     def _run_with_client(
-        self, client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        cls, 
+        client: OpenAIClient, 
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> ChatPrompt:
+        run_config = evaled_prompt.run_config
+        new_request = evaled_prompt.request
         response = client.chat(
-            messages=self._eval_data(run_config),
+            messages=evaled_prompt.data,
             **new_request
             ).call()
-        new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # dump frontmatter, no base_path
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
                 # stream response to a file descriptor
                 role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     # dump frontmatter
-                    fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
+                    fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
                     role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), fout)
             else:
                 role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
             [{"role": role, "content": content, "tool_calls": tool_calls}],
             new_request, run_config, base_path,
             response=response
         )
     
+    @classmethod
     async def _arun_with_client(
-        self, client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        cls, 
+        client: OpenAIClient, 
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> ChatPrompt:
+        run_config = evaled_prompt.run_config
+        new_request = evaled_prompt.request
         response = await client.chat(
-            messages=self._eval_data(run_config),
+            messages=evaled_prompt.data,
             **new_request
             ).acall()
-        new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
                 role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
-                    fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
+                    fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
                     role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), fout)
             else:
                 role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
@@ -718,94 +720,97 @@
     
     @prompt.setter
     def prompt(self, value: str):
         self.data = value
     
     def _eval_data(self, run_config: RunConfig) -> str:
         var_map = self._parse_var_map(run_config)
-        if var_map:
-            new_prompt = self.prompt
-            for key, value in var_map.items():
-                new_prompt = new_prompt.replace(key, value)
-            return new_prompt
-        else:
-            return self.prompt
+        new_prompt = self.prompt
+        for key, value in var_map.items():
+            new_prompt = new_prompt.replace(key, value)
+        return new_prompt
     
-    def _stream_completions_proc(self, response, fd: Optional[io.IOBase] = None) -> str:
+    @staticmethod
+    def _stream_completions_proc(response, fd: Optional[io.IOBase] = None) -> str:
         # stream response to fd
         content = ""
         for text in stream_completions(response):
             if fd:
                 fd.write(text)
             content += text
         return content
 
+    @classmethod
     def _run_with_client(
-        self, client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        cls, 
+        client: OpenAIClient, 
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> CompletionsPrompt:
+        run_config = evaled_prompt.run_config
+        new_request = evaled_prompt.request
         response = client.completions(
-            prompt=self._eval_data(run_config),
+            prompt=evaled_prompt.data,
             **new_request
             ).call()
-        new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                content = self._stream_completions_proc(response, run_config.output_fd)
+                run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
+                content = cls._stream_completions_proc(response, run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
-                    fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    content = self._stream_completions_proc(response, fout)
+                    fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
+                    content = cls._stream_completions_proc(response, fout)
             else:
-                content = self._stream_completions_proc(response)
+                content = cls._stream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
 
-    async def _astream_completions_proc(self, response, fd: Optional[io.IOBase] = None) -> str:
+    @staticmethod
+    async def _astream_completions_proc(response, fd: Optional[io.IOBase] = None) -> str:
         # stream response to fd
         content = ""
         async for text in astream_completions(response):
             if fd:
                 fd.write(text)
             content += text
         return content
     
+    @classmethod
     async def _arun_with_client(
-        self, client: OpenAIClient, 
-        run_config: RunConfig,
-        new_request: dict,
+        cls, 
+        client: OpenAIClient, 
+        evaled_prompt: PromptType,
         stream: bool,
         ) -> CompletionsPrompt:
+        run_config = evaled_prompt.run_config
+        new_request = evaled_prompt.request
         response = await client.completions(
-            prompt=self._eval_data(run_config),
+            prompt=evaled_prompt.data,
             **new_request
             ).acall()
-        new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                content = await self._astream_completions_proc(response, run_config.output_fd)
+                run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
+                content = await cls._astream_completions_proc(response, run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
-                    fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    content = await self._astream_completions_proc(response, fout)
+                    fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
+                    content = await cls._astream_completions_proc(response, fout)
             else:
-                content = await self._astream_completions_proc(response)
+                content = await cls._astream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
     
     def __add__(self, other: Union[str, CompletionsPrompt]):
```

### Comparing `handyllm-0.7.4/src/handyllm/openai_api.py` & `handyllm-0.7.5/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/openai_client.py` & `handyllm-0.7.5/src/handyllm/openai_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,20 +188,26 @@
         api_version = self._infer_api_version(kwargs.pop('api_version', api_version))
         model_engine_map = self._infer_model_engine_map(kwargs.pop('model_engine_map', model_engine_map))
 
         deployment_id = kwargs.pop('deployment_id', None)
         engine = kwargs.pop('engine', deployment_id)
         # if using Azure and engine not provided, try to get it from model parameter
         if api_type and api_type.lower() in _API_TYPES_AZURE:
-            model = kwargs.pop('model', None)
-            if not engine and model:
-                if model_engine_map:
-                    engine = model_engine_map.get(model, model)
+            if not engine:
+                # keep or consume model parameter
+                keep_model = kwargs.pop('keep_model', False)
+                if keep_model:
+                    model = kwargs.get('model', None)
                 else:
-                    engine = model
+                    model = kwargs.pop('model', None)
+                if model:
+                    if model_engine_map:
+                        engine = model_engine_map.get(model, model)
+                    else:
+                        engine = model
         dest_url = kwargs.pop('dest_url', dest_url)
         return api_key, organization, api_base, api_type, api_version, engine, dest_url
 
     def _make_requestor(self, request_url, **kwargs) -> Requestor:
         api_key, organization, api_base, api_type, api_version, engine, dest_url = self._consume_kwargs(kwargs)
         url = join_url(api_base, request_url)
         requestor = Requestor(api_type, url, api_key, organization=organization, dest_url=dest_url, **kwargs)
@@ -340,17 +346,48 @@
 
     @api
     def images_variations(self, image, **kwargs) -> Requestor:
         files = { 'image': image }
         return self._make_requestor('/images/variations', method='post', files=files, **kwargs)
 
     @api
+    def audio_speech(self, stream=False, chunk_size=1024, **kwargs) -> Requestor:
+        api_key, organization, api_base, api_type, api_version, engine, dest_url = self._consume_kwargs(kwargs)
+        # NOTE: this api needs both model and engine parameters
+        return self._make_requestor(
+            get_request_url('/audio/speech', api_type, api_version, engine),
+            method='post', 
+            api_key=api_key,
+            organization=organization,
+            api_base=api_base,
+            api_type=api_type,
+            dest_url=dest_url,
+            stream=stream, 
+            chunk_size=chunk_size, 
+            raw=True,
+            # avoid poping model parameter
+            keep_model=True,
+            **kwargs
+            )
+
+    @api
     def audio_transcriptions(self, file, **kwargs) -> Requestor:
         files = { 'file': file }
-        return self._make_requestor('/audio/transcriptions', method='post', files=files, **kwargs)
+        api_key, organization, api_base, api_type, api_version, engine, dest_url = self._consume_kwargs(kwargs)
+        return self._make_requestor(
+            get_request_url('/audio/transcriptions', api_type, api_version, engine),
+            method='post', 
+            api_key=api_key,
+            organization=organization,
+            api_base=api_base,
+            api_type=api_type,
+            dest_url=dest_url,
+            files=files, 
+            **kwargs
+            )
 
     @api
     def audio_translations(self, file, **kwargs) -> Requestor:
         files = { 'file': file }
         return self._make_requestor('/audio/translations', method='post', files=files, **kwargs)
 
     @api
```

### Comparing `handyllm-0.7.4/src/handyllm/prompt_converter.py` & `handyllm-0.7.5/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/src/handyllm/requestor.py` & `handyllm-0.7.5/src/handyllm/requestor.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         api_key, 
         *,
         organization=None, 
         method='post', 
         timeout=None, 
         files=None, 
         azure_poll=False, 
+        raw=False, 
+        chunk_size=1024, 
         dest_url=None, 
         **kwargs) -> None:
         
         self._sync_client = None
         self._async_client = None
         self._prepare_callback = None
         self._response_callback = None
@@ -49,14 +51,16 @@
         else:
             self.api_key = api_key
         self.organization = organization
         self.method = method
         self.timeout = timeout
         self.files = files
         self.azure_poll = azure_poll
+        self.raw = raw
+        self.chunk_size = chunk_size
         self.dest_url = dest_url
 
         self.stream = kwargs.get('stream', False)
         if self.stream and azure_poll:
             raise Exception("Cannot use 'azure_poll' in stream mode.")
 
         self.headers = {}
@@ -133,20 +137,25 @@
             prepare_ret = None
         timeout_ddl = time.perf_counter()+self.timeout if self.timeout else None
         self._log_request()
         try:
             raw_response = self._call_raw()
 
             if self.stream:
-                response = self._gen_stream_response(raw_response, prepare_ret)
+                if self.raw:
+                    response = self._gen_stream_bin_response(raw_response, prepare_ret)
+                else:
+                    response = self._gen_stream_response(raw_response, prepare_ret)
             else:
                 if self.azure_poll:
                     poll_url = raw_response.headers['operation-location']
                     response = self.poll(poll_url, timeout_ddl=timeout_ddl).json()
                     response = response.get('result', response)
+                elif self.raw:
+                    response = raw_response.content
                 else:
                     response = raw_response.json()
             
             if self._response_callback:
                 response = self._response_callback(response, prepare_ret)
             return response
         except Exception as e:
@@ -184,14 +193,24 @@
                         if byte_line.startswith(b"data: "):
                             line = byte_line[len(b"data: "):].decode("utf-8")
                             yield json.loads(line)
             except Exception as e:
                 if self._exception_callback:
                     self._exception_callback(e, prepare_ret)
                 raise e
+    
+    def _gen_stream_bin_response(self, raw_response: requests.Response, prepare_ret):
+        with raw_response:
+            try:
+                for chunk in raw_response.iter_content(chunk_size=self.chunk_size):
+                    yield chunk
+            except Exception as e:
+                if self._exception_callback:
+                    self._exception_callback(e, prepare_ret)
+                raise e
 
     def poll(self, url, timeout_ddl=None, params=None) -> requests.Response:
         self._check_timeout(timeout_ddl)
         headers= { "api-key": self.api_key, "Content-Type": "application/json" }
         response = self._sync_client.request('get', url, headers=headers, params=params)
         self._check_image_error(response)
         while not self._check_image_end(response):
@@ -211,20 +230,25 @@
             prepare_ret = None
         timeout_ddl = time.perf_counter()+self.timeout if self.timeout else None
         self._log_request()
         try:
             raw_response = await self._acall_raw()
 
             if self.stream:
-                response = self._agen_stream_response(raw_response, prepare_ret)
+                if self.raw:
+                    response = self._agen_stream_bin_response(raw_response, prepare_ret)
+                else:
+                    response = self._agen_stream_response(raw_response, prepare_ret)
             else:
                 if self.azure_poll:
                     poll_url = raw_response.headers['operation-location']
                     response = await self.apoll(poll_url, timeout_ddl=timeout_ddl).json()
                     response = response.get('result', response)
+                elif self.raw:
+                    response = raw_response.content
                 else:
                     response = raw_response.json()
             
             if self._response_callback:
                 response = self._response_callback(response, prepare_ret)
             return response
         except Exception as e:
@@ -267,14 +291,25 @@
         except Exception as e:
             if self._exception_callback:
                 self._exception_callback(e, prepare_ret)
             raise e
         finally:
             await raw_response.aclose()
 
+    async def _agen_stream_bin_response(self, raw_response: httpx.Response, prepare_ret):
+        try:
+            async for chunk in raw_response.aiter_bytes():
+                yield chunk
+        except Exception as e:
+            if self._exception_callback:
+                self._exception_callback(e, prepare_ret)
+            raise e
+        finally:
+            await raw_response.aclose()
+
     async def apoll(self, url, timeout_ddl=None, params=None) -> httpx.Response:
         self._check_timeout(timeout_ddl)
         headers= { "api-key": self.api_key, "Content-Type": "application/json" }
         response = await self._async_client.request('get', url, headers=headers, params=params)
         self._check_image_error(response)
         while not self._check_image_end(response):
             self._check_timeout(timeout_ddl)
```

### Comparing `handyllm-0.7.4/src/handyllm/utils.py` & `handyllm-0.7.5/src/handyllm/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 from urllib.parse import urlparse
 import os
 import time
 
 
 def get_filename_from_url(download_url):
     # Parse the URL.
@@ -103,7 +104,22 @@
 async def astream_completions(response):
     async for data in response:
         try:
             yield data['choices'][0]['text']
         except (KeyError, IndexError):
             pass
 
+def stream_to_fd(response, fd: io.IOBase):
+    for data in response:
+        fd.write(data)
+
+def stream_to_file(response, file_path):
+    with open(file_path, 'wb') as f:
+        stream_to_fd(response, f)
+
+async def astream_to_fd(response, fd: io.IOBase):
+    async for data in response:
+        fd.write(data)
+
+async def astream_to_file(response, file_path):
+    with open(file_path, 'wb') as f:
+        await astream_to_fd(response, f)
```

### Comparing `handyllm-0.7.4/tests/test_azure.py` & `handyllm-0.7.5/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/tests/test_client_async_sync.py` & `handyllm-0.7.5/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/tests/test_endpoint.py` & `handyllm-0.7.5/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/tests/test_hprompt.py` & `handyllm-0.7.5/tests/test_hprompt.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.4/tests/test_prompt.py` & `handyllm-0.7.5/tests/test_prompt.py`

 * *Files identical despite different names*

