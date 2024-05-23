# Comparing `tmp/answerrocket_client-0.2.6.tar.gz` & `tmp/answerrocket_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.6.tar", last modified: Tue May 21 20:57:26 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.7.tar", last modified: Thu May 23 19:17:19 2024, max compression
```

## Comparing `answerrocket_client-0.2.6.tar` & `answerrocket_client-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.560246 answerrocket_client-0.2.6/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.560246 answerrocket_client-0.2.6/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51799 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52290 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/test/test_client.py
```

### Comparing `answerrocket_client-0.2.6/PKG-INFO` & `answerrocket_client-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.6/answer_rocket/auth.py` & `answerrocket_client-0.2.7/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/chat.py` & `answerrocket_client-0.2.7/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/client.py` & `answerrocket_client-0.2.7/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/config.py` & `answerrocket_client-0.2.7/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/data.py` & `answerrocket_client-0.2.7/answer_rocket/data.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.7/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.7/answer_rocket/graphql/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,22 +296,30 @@
     length = sgqlc.types.Field(Int, graphql_name='length')
     precision = sgqlc.types.Field(Int, graphql_name='precision')
     scale = sgqlc.types.Field(Int, graphql_name='scale')
 
 
 class MaxCopilot(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('copilot_id', 'name', 'description', 'system_prompt', 'beta_yaml', 'global_python_code', 'copilot_questions')
+    __field_names__ = ('copilot_id', 'name', 'description', 'system_prompt', 'beta_yaml', 'global_python_code', 'copilot_questions', 'connection_datasets')
     copilot_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotId')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     system_prompt = sgqlc.types.Field(String, graphql_name='systemPrompt')
     beta_yaml = sgqlc.types.Field(String, graphql_name='betaYaml')
     global_python_code = sgqlc.types.Field(String, graphql_name='globalPythonCode')
     copilot_questions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxCopilotQuestion'))), graphql_name='copilotQuestions')
+    connection_datasets = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxCopilotConnectionDataset'))), graphql_name='connectionDatasets')
+
+
+class MaxCopilotConnectionDataset(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('dataset_id', 'name')
+    dataset_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='datasetId')
+    name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
 
 
 class MaxCopilotQuestion(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('copilot_question_id', 'nl', 'skill_id', 'parameters', 'is_starter', 'hint', 'created_user_id', 'created_utc', 'last_modified_user_id', 'last_modified_utc', 'version', 'is_deleted')
     copilot_question_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotQuestionId')
     nl = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='nl')
```

### Comparing `answerrocket_client-0.2.6/answer_rocket/graphql/sdk_operations.py` & `answerrocket_client-0.2.7/answer_rocket/graphql/sdk_operations.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/output.py` & `answerrocket_client-0.2.7/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answer_rocket/skill.py` & `answerrocket_client-0.2.7/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.7/answerrocket_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.6/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.7/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.6/readme.md` & `answerrocket_client-0.2.7/readme.md`

 * *Files identical despite different names*

