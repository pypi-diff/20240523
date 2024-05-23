# Comparing `tmp/ai_server_sdk-0.0.17.tar.gz` & `tmp/ai-server-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_server_sdk-0.0.17.tar", last modified: Thu May 23 18:29:12 2024, max compression
+gzip compressed data, was "ai-server-sdk-0.0.9.tar", last modified: Tue Oct 17 00:09:46 2023, max compression
```

## Comparing `ai_server_sdk-0.0.17.tar` & `ai-server-sdk-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.123951 ai_server_sdk-0.0.17/
--rw-rw-rw-   0        0        0     1091 2024-03-19 20:02:29.000000 ai_server_sdk-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     8551 2024-05-23 18:29:12.119954 ai_server_sdk-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     6176 2024-05-23 18:27:08.000000 ai_server_sdk-0.0.17/README.md
--rw-rw-rw-   0        0        0     1187 2024-05-23 18:27:08.000000 ai_server_sdk-0.0.17/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 18:29:12.124952 ai_server_sdk-0.0.17/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.015950 ai_server_sdk-0.0.17/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.020951 ai_server_sdk-0.0.17/src/ai_server/
--rw-rw-rw-   0        0        0     1615 2024-05-23 18:26:54.000000 ai_server_sdk-0.0.17/src/ai_server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:11.999924 ai_server_sdk-0.0.17/src/ai_server/py_client/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.049951 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/
--rw-rw-rw-   0        0        0        0 2024-03-19 20:02:29.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/__init__.py
--rw-rw-rw-   0        0        0     5938 2024-05-23 13:00:38.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/database.py
--rw-rw-rw-   0        0        0     1368 2024-05-23 13:28:36.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/function.py
--rw-rw-rw-   0        0        0    11537 2024-05-23 13:00:45.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/model.py
--rw-rw-rw-   0        0        0     3809 2024-05-23 13:00:51.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/storage.py
--rw-rw-rw-   0        0        0     6751 2024-05-23 13:00:57.000000 ai_server_sdk-0.0.17/src/ai_server/py_client/gaas/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.058950 ai_server_sdk-0.0.17/src/ai_server/server_resources/
--rw-rw-rw-   0        0        0    16584 2024-05-23 18:27:08.000000 ai_server_sdk-0.0.17/src/ai_server/server_resources/server_client.py
--rw-rw-rw-   0        0        0     9505 2024-05-23 13:01:42.000000 ai_server_sdk-0.0.17/src/ai_server/server_resources/server_proxy.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.115953 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/
--rw-rw-rw-   0        0        0     8551 2024-05-23 18:29:11.000000 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      759 2024-05-23 18:29:11.000000 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:29:11.000000 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-23 18:29:11.000000 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 18:29:11.000000 ai_server_sdk-0.0.17/src/ai_server_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      689 2024-05-23 18:27:08.000000 ai_server_sdk-0.0.17/src/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:29:12.110953 ai_server_sdk-0.0.17/tests/
--rw-rw-rw-   0        0        0      682 2024-05-19 19:47:29.000000 ai_server_sdk-0.0.17/tests/test_base_connection.py
--rw-rw-rw-   0        0        0      695 2024-05-19 19:47:29.000000 ai_server_sdk-0.0.17/tests/test_database.py
--rw-rw-rw-   0        0        0     1971 2024-05-19 19:47:29.000000 ai_server_sdk-0.0.17/tests/test_model.py
--rw-rw-rw-   0        0        0     2497 2024-05-19 19:47:29.000000 ai_server_sdk-0.0.17/tests/test_openai_endpoints.py
--rw-rw-rw-   0        0        0      489 2024-03-26 21:21:13.000000 ai_server_sdk-0.0.17/tests/test_run_pixel.py
--rw-rw-rw-   0        0        0     2110 2024-05-19 19:47:29.000000 ai_server_sdk-0.0.17/tests/test_vector.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.753161 ai-server-sdk-0.0.9/
+-rw-rw-rw-   0        0        0     5138 2023-10-17 00:09:46.751174 ai-server-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-10-17 00:09:33.000000 ai-server-sdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.714097 ai-server-sdk-0.0.9/ai_server/
+-rw-rw-rw-   0        0        0      163 2023-10-05 16:26:33.000000 ai-server-sdk-0.0.9/ai_server/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/config.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.716087 ai-server-sdk-0.0.9/ai_server/py_client/
+-rw-rw-rw-   0        0        0      188 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.731095 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/
+-rw-rw-rw-   0        0        0      210 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/__init__.py
+-rw-rw-rw-   0        0        0     4488 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_database.py
+-rw-rw-rw-   0        0        0     1372 2023-09-22 21:59:46.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_driver.py
+-rw-rw-rw-   0        0        0     3965 2023-10-05 16:25:52.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_model.py
+-rw-rw-rw-   0        0        0     4966 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_storage.py
+-rw-rw-rw-   0        0        0     9820 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_rest_server.py
+-rw-rw-rw-   0        0        0     6951 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_server_proxy.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.735094 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/
+-rw-rw-rw-   0        0        0        0 2023-10-05 16:23:13.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/__init__.py
+-rw-rw-rw-   0        0        0      641 2023-10-06 15:51:53.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.740142 ai-server-sdk-0.0.9/ai_server/utils/
+-rw-rw-rw-   0        0        0       72 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/__init__.py
+-rw-rw-rw-   0        0        0       49 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/_constants_manager.py
+-rw-rw-rw-   0        0        0      731 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/_stdout.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.749148 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5138 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-17 00:09:46.753161 ai-server-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-10-17 00:08:56.000000 ai-server-sdk-0.0.9/setup.py
```

### Comparing `ai_server_sdk-0.0.17/README.md` & `ai-server-sdk-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: ai-server-sdk
+Version: 0.0.9
+Summary: Utility package to connect to AI Server instances.
+Author: Thomas Trankle
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+
 # **AI Server**
 
 *ai-server-sdk* is a python client SDK to connect to the AI Server
 
 ## Using this package you can:
 
  - Inference with Models you have acces to within the server
@@ -10,133 +19,92 @@
  - Run pixel and get the direct output or full json response.
  - Pull data products from an existing insight using REST API.
 
 ## **Install**
 
     pip install ai-server-sdk
 
-or
-
-    pip install ai-server-sdk[full]
-
-  *Note*: The `full` option installs optional dependencies for langchain support.
 
 ## **Usage**
 
 To interract with an ai-server instance, import the `ai_server` package and connect via RESTServer.
 
 *Note*: secret and access keys are required
 
 
 ### Setup
 ```python
->>> from ai_server import ServerClient
+>>> import ai_server
 
 # define access keys
 >>> loginKeys = {"secretKey":"<your_secret_key>","accessKey":"<your_access_key>"}
 
 # create connection object by passing in the secret key, access key and base url for the api
->>> server_connection = ServerClient(
-...     access_key=loginKeys['accessKey'],
-...     secret_key=loginKeys['secretKey'],
-...     base='<Your deployed server Monolith URL>'
-... )
+>>> server_connection = ai_server.RESTServer(access_key=loginKeys['accessKey'], secret_key=loginKeys['secretKey'], base='<Your deployed server Monolith URL>')
 ```
 
 ### Inference with different Model Engines
 ```python
-# import the model engine class for the ai_server package
->>> from ai_server import ModelEngine
-
->>> model = ModelEngine(
-...     engine_id="2c6de0ff-62e0-4dd0-8380-782ac4d40245", 
-...     insight_id=server_connection.cur_insight
-... )
-
 # define a question and grab the engine id from the server
->>> model.ask(question = 'What is the capital of France?')
+>>> question = 'What is the capital of France?'
+>>> engine_id = "2c6de0ff-62e0-4dd0-8380-782ac4d40245"
+
+### Option 1 - User ModelEngine directly
+>>> model = ai_server.ModelEngine(engine_id = engine_id, insight_id = server_connection.cur_insight)
+>>> model.ask(question = question)
 [{'response': 'The capital of France is Paris.',
   'messageId': '0a80c2ce-76f9-4466-b2a2-8455e4cab34a',
   'roomId': '28261853-0e41-49b0-8a50-df34e8c62a19'}]
-```
 
-### Interact with a Vector Database by adding document(s), querying, and removing document(s)
-```python
-# import the vector engine class for the ai_server package
->>> from ai_server import VectorEngine
-
-# initialize the connection to the vector database
->>> vectorEngine = VectorEngine(
-...     engine_id="221a50a4-060c-4aa8-8b7c-e2bc97ee3396", 
-...     insight_id=server_connection.cur_insight
-... )
-
-# Add document(s) that have been uploaded to the insight
->>> vectorEngine.addDocument(file_paths = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
-
-# Perform a nearest neighbor search on the embedded documents
->>> vectorEngine.nearestNeighbor(search_statement = 'Sample Search Statement', limit = 5)
-
-# List all the documents the vector database currently comprises of
->>> vectorEngine.listDocuments()
-
-# Remove document(s) from the vector database
->>> vectorEngine.removeDocument(file_names = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
+### Option 2 - Use the Driver class
+>>> driver = ai_server.Driver(insight_id = server_connection.cur_insight)
+>>> driver.run_model(question = question, engine_id = engine_id)
+['The capital of France is Paris.']
 ```
 
 ### Connect to Databases and execute create, read, and delete operations
 
 #### Run the passed string query against the engine.  The query passed must be in the structure that the specific engine implementation.
 ```python
-# import the database engine class for the ai_server package
->>> from ai_server import DatabaseEngine
-
 # Create an relation to database based on the engine identifier
->>> database = DatabaseEngine(
-...     engine_id="4a1f9466-4e6d-49cd-894d-7d22182344cd", 
-...     insight_id=server_connection.cur_insight
-... )
+>>> engine_id = "4a1f9466-4e6d-49cd-894d-7d22182344cd"
+>>> database = ai_server.DatabaseEngine(engine_id = engine_id, insight_id=a.cur_insight)
 >>> database.execQuery(query='SELECT PATIENT, HEIGHT, WEIGHT FROM diab LIMIT 4')
 ```
 |    |   PATIENT |   HEIGHT |   WEIGHT |
 |---:|----------:|---------:|---------:|
 |  0 |     20337 |       64 |      114 |
 |  1 |      3750 |       64 |      161 |
 |  2 |     40785 |       67 |      187 |
 |  3 |     12778 |       72 |      145 |
 
-#### Run the passed string query against the engine as an insert query. Query must be in the structure that the specific engine implementation
+
+execQuery commands can also be run through the Driver class
 ```python
->>> database.insertData(query = 'INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1, value2, value3, ...)')
+### Use the Driver class
+>>> driver = ai_server.Driver(insight_id = server_connection.cur_insight)
+>>> driver.run_database(query = 'SELECT PATIENT, HEIGHT, WEIGHT FROM diab LIMIT 4', engine_id = engine_id)
 ```
+|    |   PATIENT |   HEIGHT |   WEIGHT |
+|---:|----------:|---------:|---------:|
+|  0 |     20337 |       64 |      114 |
+|  1 |      3750 |       64 |      161 |
+|  2 |     40785 |       67 |      187 |
+|  3 |     12778 |       72 |      145 |
 
-#### Run an update query on the database
+#### Run the passed string query against the engine as an insert query. Query must be in the structure that the specific engine implementation
 ```python
->>> database.updateData(query = 'UPDATE table_name set column1=value1 where age=19')
+>>> database.insertData(query = 'INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1, value2, value3, ...)')
 ```
 
 #### Run a delete query on the database
 ```python
 >>> database.removeData(query='DELETE FROM diab WHERE age=19;')
 ```
 
-### Run Function Engines
-```python
-# import the function engine class for the ai_server package
->>> from ai_server import FunctionEngine
-
-# initialize the connection ot the function engine
->>> function = FunctionEngine(
-...     engine_id="f3a4c8b2-7f3e-4d04-8c1f-2b0e3dabf5e9", 
-...     insight_id=server_connection.cur_insight
-... )
->>> function.execute({"lat":"37.540","lon":"77.4360"})
-'{"cloud_pct": 2, "temp": 28, "feels_like": 27, "humidity": 20, "min_temp": 28, "max_temp": 28, "wind_speed": 5, "wind_degrees": 352, "sunrise": 1716420915, "sunset": 1716472746}'
-```
-
 ### Using REST API to pull data product from an Insight
 ```python
 # define the Project ID
 >>> projectId = '30991037-1e73-49f5-99d3-f28210e6b95c'
 
 # define the Insight ID
 >>> inishgtId = '26b373b3-cd52-452c-a987-0adb8817bf73'
@@ -170,8 +138,8 @@
  'pixelReturn': [{'pixelId': '3',
    'pixelExpression': '1 + 1 ;',
    'isMeta': False,
    'output': 2,
    'operationType': ['OPERATION']}]}
 ```
 
----
+---
```

