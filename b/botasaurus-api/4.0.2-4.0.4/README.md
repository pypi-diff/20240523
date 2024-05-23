# Comparing `tmp/botasaurus_api-4.0.2.tar.gz` & `tmp/botasaurus_api-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_api-4.0.2.tar", last modified: Tue May 14 15:48:51 2024, max compression
+gzip compressed data, was "botasaurus_api-4.0.4.tar", last modified: Thu May 23 04:31:17 2024, max compression
```

## Comparing `botasaurus_api-4.0.2.tar` & `botasaurus_api-4.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.739036 botasaurus_api-4.0.2/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_api-4.0.2/LICENSE
--rw-rw-rw-   0        0        0     6962 2024-05-14 15:48:51.738411 botasaurus_api-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5863 2024-04-11 11:33:13.000000 botasaurus_api-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.694727 botasaurus_api-4.0.2/botasaurus_api/
--rw-rw-rw-   0        0        0    14011 2024-04-11 13:30:57.000000 botasaurus_api-4.0.2/botasaurus_api/__init__.py
--rw-rw-rw-   0        0        0     1881 2024-04-12 12:13:48.000000 botasaurus_api-4.0.2/botasaurus_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.736521 botasaurus_api-4.0.2/botasaurus_api.egg-info/
--rw-rw-rw-   0        0        0     6962 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-14 15:48:51.742700 botasaurus_api-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1644 2024-05-14 15:48:50.000000 botasaurus_api-4.0.2/setup.py
+drwxr-xr-x   0 om         (501) staff       (20)        0 2024-05-23 04:31:17.877226 botasaurus_api-4.0.4/
+-rwx------   0 om         (501) staff       (20)     1094 2024-03-03 08:47:04.000000 botasaurus_api-4.0.4/LICENSE
+-rw-r--r--   0 om         (501) staff       (20)     6718 2024-05-23 04:31:17.877106 botasaurus_api-4.0.4/PKG-INFO
+-rwx------   0 om         (501) staff       (20)     5863 2024-04-11 11:33:14.000000 botasaurus_api-4.0.4/README.md
+drwxr-xr-x   0 om         (501) staff       (20)        0 2024-05-23 04:31:17.876006 botasaurus_api-4.0.4/botasaurus_api/
+-rwx------   0 om         (501) staff       (20)    14043 2024-05-23 04:30:50.000000 botasaurus_api-4.0.4/botasaurus_api/__init__.py
+-rwx------   0 om         (501) staff       (20)     1881 2024-04-12 12:13:50.000000 botasaurus_api-4.0.4/botasaurus_api/utils.py
+drwxr-xr-x   0 om         (501) staff       (20)        0 2024-05-23 04:31:17.876871 botasaurus_api-4.0.4/botasaurus_api.egg-info/
+-rw-r--r--   0 om         (501) staff       (20)     6718 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/botasaurus_api.egg-info/PKG-INFO
+-rw-r--r--   0 om         (501) staff       (20)      276 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/botasaurus_api.egg-info/SOURCES.txt
+-rw-r--r--   0 om         (501) staff       (20)        1 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/botasaurus_api.egg-info/dependency_links.txt
+-rw-r--r--   0 om         (501) staff       (20)        9 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/botasaurus_api.egg-info/requires.txt
+-rw-r--r--   0 om         (501) staff       (20)       15 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/botasaurus_api.egg-info/top_level.txt
+-rwx------   0 om         (501) staff       (20)       79 2024-05-23 04:31:17.877479 botasaurus_api-4.0.4/setup.cfg
+-rwx------   0 om         (501) staff       (20)     1595 2024-05-23 04:31:17.000000 botasaurus_api-4.0.4/setup.py
```

### Comparing `botasaurus_api-4.0.2/LICENSE` & `botasaurus_api-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_api-4.0.2/PKG-INFO` & `botasaurus_api-4.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-Metadata-Version: 2.1
-Name: botasaurus_api
-Version: 4.0.2
-Summary: The Botasaurus API Client provides programmatic access to Botasaurus scrapers with a developer-friendly API.
-Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
-Author: Chetan Jain
-Author-email: chetan@omkar.cloud
-License: MIT
-Keywords: seleniumwire proxy authentication,proxy authentication
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Installation/Setup
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
-# Botasaurus API
-
-The Botasaurus API client is a Python library for interacting with Botasaurus Scrapers via an API. 
-
-It provides a simple and convenient way to create, fetch, download, abort, and delete tasks, as well as manage their results.
-
-## Installation
-
-To install the API client, use pip:
-
-```bash
-python -m pip install botasaurus_api
-```
-
-## Usage
-
-First, import the `Api` class from the library:
-
-```python
-from botasaurus_api import Api
-```
-
-Then, create an instance of the `Api` class:
-
-```python
-api = Api()
-```
-
-You can also provide an optional `api_url` parameter to specify the base URL for the API server. If the `api_url` parameter is not provided, it defaults to `http://127.0.0.1:8000`.
-
-```python
-api = Api('https://example.com/')
-```
-
-Additionally, the API client will create response JSON files in the `output/responses/` directory to help with debugging and development. If you want to disable this feature in production, you can set `create_response_files=False`.
-
-```python
-api = Api(create_response_files=False)
-```
-
-### Creating Tasks
-
-There are two types of tasks:
-
-- Asynchronous Task
-- Synchronous Task
-
-Asynchronous tasks run asynchronously, without waiting for the task to be completed. The server will return a response immediately, containing information about the task, but not the actual results. The client can then retrieve the results later.
-
-Synchronous tasks, on the other hand, wait for the completion of the task. The server response will contain the results of the task.
-
-You should use asynchronous tasks when you want to run a task in the background and retrieve the results later. Synchronous tasks are better suited for scenarios where you have a small number of tasks and want to wait and get the results immediately.
-
-To create an asynchronous task, use the `create_async_task` method:
-
-```python
-data = {'link': 'https://www.omkar.cloud/'}
-task = api.create_async_task(data)
-```
-
-You can also provide an optional `scraper_name` parameter to specify the scraper to be used for the task, if not provided, it will use the default scraper:
-
-```python
-task = api.create_async_task(data, scraper_name='scrape_heading_task')
-```
-
-To create a synchronous task, use the `create_sync_task` method:
-
-```python
-data = {'link': 'https://www.omkar.cloud/blog/'}
-task = api.create_sync_task(data)
-```
-
-You can create multiple asynchronous or synchronous tasks at once using the `create_async_tasks` and `create_sync_tasks` methods, respectively:
-
-```python
-data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
-tasks = api.create_async_tasks(data_items)
-tasks = api.create_sync_tasks(data_items)
-```
-
-### Fetching Tasks
-
-To fetch tasks from the server, use the `get_tasks` method:
-
-```python
-tasks = api.get_tasks()
-```
-
-By default, all tasks are returned. You can also apply pagination, views, sorts and filters:
-
-```python
-tasks = api.get_tasks(
-    page=1,
-    per_page=10,
-    # view='overview',
-    # sort='my-sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-To fetch a specific task by its ID, use the `get_task` method:
-
-```python
-task = api.get_task(task_id=1)
-```
-
-### Fetching Task Results
-
-To fetch the results of a specific task, use the `get_task_results` method:
-
-```pytho
-results = api.get_task_results(task_id=1)
-```
-
-You can also apply views, sorts and filters:
-
-```python
-results = api.get_task_results(
-    task_id=1,
-    page=1,
-    per_page=20,
-    # view='overview',
-    # sort='my_sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-### Downloading Task Results
-
-To download the results of a specific task in a particular format, use the `download_task_results` method:
-
-```python
-results_bytes, filename = api.download_task_results(task_id=1, format='csv')
-with open(filename, 'wb') as file:
-    file.write(results_bytes)
-```
-
-You can also apply views, sorts and filters:
-
-```python
-results_bytes, filename = api.download_task_results(
-    task_id=1,
-    format='excel',  # format can be one of: json, csv or excel
-    # view='overview',
-    # sort='my_sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-### Aborting and Deleting Tasks
-
-To abort a specific task, use the `abort_task` method:
-
-```python
-api.abort_task(task_id=1)
-```
-
-To delete a specific task, use the `delete_task` method:
-
-```python
-api.delete_task(task_id=1)
-```
-
-You can also bulk abort or delete multiple tasks at once using the `abort_tasks` and `delete_tasks` methods, respectively:
-
-```python
-api.abort_tasks(1, 2, 3)
-api.delete_tasks(4, 5, 6)
-```
-
-## Examples
-
-Here are some example usages of the API client:
-
-```python
-from botasaurus_api import Api
-
-# Create an instance of the API client
-api = Api()
-
-# Create an asynchronous task
-data = {'link': 'https://www.omkar.cloud/'}
-task = api.create_sync_task(data, scraper_name='scrape_heading_task')
-
-# Fetch the task
-task = api.get_task(task['id'])
-
-# Fetch the task results
-results = api.get_task_results(task['id'])
-
-# Download the task results as a CSV
-results_bytes, filename = api.download_task_results(task['id'], format='csv')
-
-# Abort the task
-api.abort_task(task['id'])
-
-# Delete the task
-api.delete_task(task['id'])
-
-# --- Bulk Operations ---
-
-# Create multiple synchronous tasks
-data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
-tasks = api.create_sync_tasks(data_items, scraper_name='scrape_heading_task')
-
-# Fetch all tasks
-all_tasks = api.get_tasks()
-
-# Bulk abort tasks
-api.abort_tasks(*[task['id'] for task in tasks])
-
-# Bulk delete tasks
-api.delete_tasks(*[task['id'] for task in tasks])
-```
-
-## That's It!
-
-Now, go and build something awesome.
+Metadata-Version: 2.1
+Name: botasaurus_api
+Version: 4.0.4
+Summary: The Botasaurus API Client provides programmatic access to Botasaurus scrapers with a developer-friendly API.
+Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
+Author: Chetan Jain
+Author-email: chetan@omkar.cloud
+License: MIT
+Keywords: seleniumwire proxy authentication,proxy authentication
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Installation/Setup
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# Botasaurus API
+
+The Botasaurus API client is a Python library for interacting with Botasaurus Scrapers via an API. 
+
+It provides a simple and convenient way to create, fetch, download, abort, and delete tasks, as well as manage their results.
+
+## Installation
+
+To install the API client, use pip:
+
+```bash
+python -m pip install botasaurus_api
+```
+
+## Usage
+
+First, import the `Api` class from the library:
+
+```python
+from botasaurus_api import Api
+```
+
+Then, create an instance of the `Api` class:
+
+```python
+api = Api()
+```
+
+You can also provide an optional `api_url` parameter to specify the base URL for the API server. If the `api_url` parameter is not provided, it defaults to `http://127.0.0.1:8000`.
+
+```python
+api = Api('https://example.com/')
+```
+
+Additionally, the API client will create response JSON files in the `output/responses/` directory to help with debugging and development. If you want to disable this feature in production, you can set `create_response_files=False`.
+
+```python
+api = Api(create_response_files=False)
+```
+
+### Creating Tasks
+
+There are two types of tasks:
+
+- Asynchronous Task
+- Synchronous Task
+
+Asynchronous tasks run asynchronously, without waiting for the task to be completed. The server will return a response immediately, containing information about the task, but not the actual results. The client can then retrieve the results later.
+
+Synchronous tasks, on the other hand, wait for the completion of the task. The server response will contain the results of the task.
+
+You should use asynchronous tasks when you want to run a task in the background and retrieve the results later. Synchronous tasks are better suited for scenarios where you have a small number of tasks and want to wait and get the results immediately.
+
+To create an asynchronous task, use the `create_async_task` method:
+
+```python
+data = {'link': 'https://www.omkar.cloud/'}
+task = api.create_async_task(data)
+```
+
+You can also provide an optional `scraper_name` parameter to specify the scraper to be used for the task, if not provided, it will use the default scraper:
+
+```python
+task = api.create_async_task(data, scraper_name='scrape_heading_task')
+```
+
+To create a synchronous task, use the `create_sync_task` method:
+
+```python
+data = {'link': 'https://www.omkar.cloud/blog/'}
+task = api.create_sync_task(data)
+```
+
+You can create multiple asynchronous or synchronous tasks at once using the `create_async_tasks` and `create_sync_tasks` methods, respectively:
+
+```python
+data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
+tasks = api.create_async_tasks(data_items)
+tasks = api.create_sync_tasks(data_items)
+```
+
+### Fetching Tasks
+
+To fetch tasks from the server, use the `get_tasks` method:
+
+```python
+tasks = api.get_tasks()
+```
+
+By default, all tasks are returned. You can also apply pagination, views, sorts and filters:
+
+```python
+tasks = api.get_tasks(
+    page=1,
+    per_page=10,
+    # view='overview',
+    # sort='my-sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+To fetch a specific task by its ID, use the `get_task` method:
+
+```python
+task = api.get_task(task_id=1)
+```
+
+### Fetching Task Results
+
+To fetch the results of a specific task, use the `get_task_results` method:
+
+```pytho
+results = api.get_task_results(task_id=1)
+```
+
+You can also apply views, sorts and filters:
+
+```python
+results = api.get_task_results(
+    task_id=1,
+    page=1,
+    per_page=20,
+    # view='overview',
+    # sort='my_sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+### Downloading Task Results
+
+To download the results of a specific task in a particular format, use the `download_task_results` method:
+
+```python
+results_bytes, filename = api.download_task_results(task_id=1, format='csv')
+with open(filename, 'wb') as file:
+    file.write(results_bytes)
+```
+
+You can also apply views, sorts and filters:
+
+```python
+results_bytes, filename = api.download_task_results(
+    task_id=1,
+    format='excel',  # format can be one of: json, csv or excel
+    # view='overview',
+    # sort='my_sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+### Aborting and Deleting Tasks
+
+To abort a specific task, use the `abort_task` method:
+
+```python
+api.abort_task(task_id=1)
+```
+
+To delete a specific task, use the `delete_task` method:
+
+```python
+api.delete_task(task_id=1)
+```
+
+You can also bulk abort or delete multiple tasks at once using the `abort_tasks` and `delete_tasks` methods, respectively:
+
+```python
+api.abort_tasks(1, 2, 3)
+api.delete_tasks(4, 5, 6)
+```
+
+## Examples
+
+Here are some example usages of the API client:
+
+```python
+from botasaurus_api import Api
+
+# Create an instance of the API client
+api = Api()
+
+# Create an asynchronous task
+data = {'link': 'https://www.omkar.cloud/'}
+task = api.create_sync_task(data, scraper_name='scrape_heading_task')
+
+# Fetch the task
+task = api.get_task(task['id'])
+
+# Fetch the task results
+results = api.get_task_results(task['id'])
+
+# Download the task results as a CSV
+results_bytes, filename = api.download_task_results(task['id'], format='csv')
+
+# Abort the task
+api.abort_task(task['id'])
+
+# Delete the task
+api.delete_task(task['id'])
+
+# --- Bulk Operations ---
+
+# Create multiple synchronous tasks
+data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
+tasks = api.create_sync_tasks(data_items, scraper_name='scrape_heading_task')
+
+# Fetch all tasks
+all_tasks = api.get_tasks()
+
+# Bulk abort tasks
+api.abort_tasks(*[task['id'] for task in tasks])
+
+# Bulk delete tasks
+api.delete_tasks(*[task['id'] for task in tasks])
+```
+
+## That's It!
+
+Now, go and build something awesome.
```

### Comparing `botasaurus_api-4.0.2/README.md` & `botasaurus_api-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus_api-4.0.2/botasaurus_api/__init__.py` & `botasaurus_api-4.0.4/botasaurus_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from requests.exceptions import ConnectionError
 from .utils import get_filename_from_response_headers, write_json_response, write_file_response, remove_after_first_slash
+from typing import Optional
 
 class ApiException(Exception):
      pass
 
 def _create_filename(path):
     return "output/responses/" + path + ".json"
 
@@ -16,15 +17,15 @@
                 raise ApiException(message)
             else:
                 response.raise_for_status()    
         elif 500 <= response.status_code < 600:
             response.raise_for_status()
 
 class Api:
-    def __init__(self, api_url: str | None = None, create_response_files: bool = True) -> None:
+    def __init__(self, api_url: Optional[str] = None, create_response_files: bool = True) -> None:
         """
         Initializes the API client with a specified server URL and an option to create response files.
         
         :param api_url: The base URL for the API server. If not specified, defaults to "http://127.0.0.1:8000".
         :param create_response_files: Indicates if the client should create response files for each API call. This is useful for debugging or development purposes. Defaults to True.
         """
         DEFAULT_API_URL = "http://127.0.0.1:8000"
```

### Comparing `botasaurus_api-4.0.2/botasaurus_api/utils.py` & `botasaurus_api-4.0.4/botasaurus_api/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_api-4.0.2/botasaurus_api.egg-info/PKG-INFO` & `botasaurus_api-4.0.4/botasaurus_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-Metadata-Version: 2.1
-Name: botasaurus_api
-Version: 4.0.2
-Summary: The Botasaurus API Client provides programmatic access to Botasaurus scrapers with a developer-friendly API.
-Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
-Author: Chetan Jain
-Author-email: chetan@omkar.cloud
-License: MIT
-Keywords: seleniumwire proxy authentication,proxy authentication
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Installation/Setup
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
-# Botasaurus API
-
-The Botasaurus API client is a Python library for interacting with Botasaurus Scrapers via an API. 
-
-It provides a simple and convenient way to create, fetch, download, abort, and delete tasks, as well as manage their results.
-
-## Installation
-
-To install the API client, use pip:
-
-```bash
-python -m pip install botasaurus_api
-```
-
-## Usage
-
-First, import the `Api` class from the library:
-
-```python
-from botasaurus_api import Api
-```
-
-Then, create an instance of the `Api` class:
-
-```python
-api = Api()
-```
-
-You can also provide an optional `api_url` parameter to specify the base URL for the API server. If the `api_url` parameter is not provided, it defaults to `http://127.0.0.1:8000`.
-
-```python
-api = Api('https://example.com/')
-```
-
-Additionally, the API client will create response JSON files in the `output/responses/` directory to help with debugging and development. If you want to disable this feature in production, you can set `create_response_files=False`.
-
-```python
-api = Api(create_response_files=False)
-```
-
-### Creating Tasks
-
-There are two types of tasks:
-
-- Asynchronous Task
-- Synchronous Task
-
-Asynchronous tasks run asynchronously, without waiting for the task to be completed. The server will return a response immediately, containing information about the task, but not the actual results. The client can then retrieve the results later.
-
-Synchronous tasks, on the other hand, wait for the completion of the task. The server response will contain the results of the task.
-
-You should use asynchronous tasks when you want to run a task in the background and retrieve the results later. Synchronous tasks are better suited for scenarios where you have a small number of tasks and want to wait and get the results immediately.
-
-To create an asynchronous task, use the `create_async_task` method:
-
-```python
-data = {'link': 'https://www.omkar.cloud/'}
-task = api.create_async_task(data)
-```
-
-You can also provide an optional `scraper_name` parameter to specify the scraper to be used for the task, if not provided, it will use the default scraper:
-
-```python
-task = api.create_async_task(data, scraper_name='scrape_heading_task')
-```
-
-To create a synchronous task, use the `create_sync_task` method:
-
-```python
-data = {'link': 'https://www.omkar.cloud/blog/'}
-task = api.create_sync_task(data)
-```
-
-You can create multiple asynchronous or synchronous tasks at once using the `create_async_tasks` and `create_sync_tasks` methods, respectively:
-
-```python
-data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
-tasks = api.create_async_tasks(data_items)
-tasks = api.create_sync_tasks(data_items)
-```
-
-### Fetching Tasks
-
-To fetch tasks from the server, use the `get_tasks` method:
-
-```python
-tasks = api.get_tasks()
-```
-
-By default, all tasks are returned. You can also apply pagination, views, sorts and filters:
-
-```python
-tasks = api.get_tasks(
-    page=1,
-    per_page=10,
-    # view='overview',
-    # sort='my-sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-To fetch a specific task by its ID, use the `get_task` method:
-
-```python
-task = api.get_task(task_id=1)
-```
-
-### Fetching Task Results
-
-To fetch the results of a specific task, use the `get_task_results` method:
-
-```pytho
-results = api.get_task_results(task_id=1)
-```
-
-You can also apply views, sorts and filters:
-
-```python
-results = api.get_task_results(
-    task_id=1,
-    page=1,
-    per_page=20,
-    # view='overview',
-    # sort='my_sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-### Downloading Task Results
-
-To download the results of a specific task in a particular format, use the `download_task_results` method:
-
-```python
-results_bytes, filename = api.download_task_results(task_id=1, format='csv')
-with open(filename, 'wb') as file:
-    file.write(results_bytes)
-```
-
-You can also apply views, sorts and filters:
-
-```python
-results_bytes, filename = api.download_task_results(
-    task_id=1,
-    format='excel',  # format can be one of: json, csv or excel
-    # view='overview',
-    # sort='my_sort',
-    # filters={'your_filter': 'value'},
-)
-```
-
-### Aborting and Deleting Tasks
-
-To abort a specific task, use the `abort_task` method:
-
-```python
-api.abort_task(task_id=1)
-```
-
-To delete a specific task, use the `delete_task` method:
-
-```python
-api.delete_task(task_id=1)
-```
-
-You can also bulk abort or delete multiple tasks at once using the `abort_tasks` and `delete_tasks` methods, respectively:
-
-```python
-api.abort_tasks(1, 2, 3)
-api.delete_tasks(4, 5, 6)
-```
-
-## Examples
-
-Here are some example usages of the API client:
-
-```python
-from botasaurus_api import Api
-
-# Create an instance of the API client
-api = Api()
-
-# Create an asynchronous task
-data = {'link': 'https://www.omkar.cloud/'}
-task = api.create_sync_task(data, scraper_name='scrape_heading_task')
-
-# Fetch the task
-task = api.get_task(task['id'])
-
-# Fetch the task results
-results = api.get_task_results(task['id'])
-
-# Download the task results as a CSV
-results_bytes, filename = api.download_task_results(task['id'], format='csv')
-
-# Abort the task
-api.abort_task(task['id'])
-
-# Delete the task
-api.delete_task(task['id'])
-
-# --- Bulk Operations ---
-
-# Create multiple synchronous tasks
-data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
-tasks = api.create_sync_tasks(data_items, scraper_name='scrape_heading_task')
-
-# Fetch all tasks
-all_tasks = api.get_tasks()
-
-# Bulk abort tasks
-api.abort_tasks(*[task['id'] for task in tasks])
-
-# Bulk delete tasks
-api.delete_tasks(*[task['id'] for task in tasks])
-```
-
-## That's It!
-
-Now, go and build something awesome.
+Metadata-Version: 2.1
+Name: botasaurus_api
+Version: 4.0.4
+Summary: The Botasaurus API Client provides programmatic access to Botasaurus scrapers with a developer-friendly API.
+Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
+Author: Chetan Jain
+Author-email: chetan@omkar.cloud
+License: MIT
+Keywords: seleniumwire proxy authentication,proxy authentication
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Installation/Setup
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+# Botasaurus API
+
+The Botasaurus API client is a Python library for interacting with Botasaurus Scrapers via an API. 
+
+It provides a simple and convenient way to create, fetch, download, abort, and delete tasks, as well as manage their results.
+
+## Installation
+
+To install the API client, use pip:
+
+```bash
+python -m pip install botasaurus_api
+```
+
+## Usage
+
+First, import the `Api` class from the library:
+
+```python
+from botasaurus_api import Api
+```
+
+Then, create an instance of the `Api` class:
+
+```python
+api = Api()
+```
+
+You can also provide an optional `api_url` parameter to specify the base URL for the API server. If the `api_url` parameter is not provided, it defaults to `http://127.0.0.1:8000`.
+
+```python
+api = Api('https://example.com/')
+```
+
+Additionally, the API client will create response JSON files in the `output/responses/` directory to help with debugging and development. If you want to disable this feature in production, you can set `create_response_files=False`.
+
+```python
+api = Api(create_response_files=False)
+```
+
+### Creating Tasks
+
+There are two types of tasks:
+
+- Asynchronous Task
+- Synchronous Task
+
+Asynchronous tasks run asynchronously, without waiting for the task to be completed. The server will return a response immediately, containing information about the task, but not the actual results. The client can then retrieve the results later.
+
+Synchronous tasks, on the other hand, wait for the completion of the task. The server response will contain the results of the task.
+
+You should use asynchronous tasks when you want to run a task in the background and retrieve the results later. Synchronous tasks are better suited for scenarios where you have a small number of tasks and want to wait and get the results immediately.
+
+To create an asynchronous task, use the `create_async_task` method:
+
+```python
+data = {'link': 'https://www.omkar.cloud/'}
+task = api.create_async_task(data)
+```
+
+You can also provide an optional `scraper_name` parameter to specify the scraper to be used for the task, if not provided, it will use the default scraper:
+
+```python
+task = api.create_async_task(data, scraper_name='scrape_heading_task')
+```
+
+To create a synchronous task, use the `create_sync_task` method:
+
+```python
+data = {'link': 'https://www.omkar.cloud/blog/'}
+task = api.create_sync_task(data)
+```
+
+You can create multiple asynchronous or synchronous tasks at once using the `create_async_tasks` and `create_sync_tasks` methods, respectively:
+
+```python
+data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
+tasks = api.create_async_tasks(data_items)
+tasks = api.create_sync_tasks(data_items)
+```
+
+### Fetching Tasks
+
+To fetch tasks from the server, use the `get_tasks` method:
+
+```python
+tasks = api.get_tasks()
+```
+
+By default, all tasks are returned. You can also apply pagination, views, sorts and filters:
+
+```python
+tasks = api.get_tasks(
+    page=1,
+    per_page=10,
+    # view='overview',
+    # sort='my-sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+To fetch a specific task by its ID, use the `get_task` method:
+
+```python
+task = api.get_task(task_id=1)
+```
+
+### Fetching Task Results
+
+To fetch the results of a specific task, use the `get_task_results` method:
+
+```pytho
+results = api.get_task_results(task_id=1)
+```
+
+You can also apply views, sorts and filters:
+
+```python
+results = api.get_task_results(
+    task_id=1,
+    page=1,
+    per_page=20,
+    # view='overview',
+    # sort='my_sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+### Downloading Task Results
+
+To download the results of a specific task in a particular format, use the `download_task_results` method:
+
+```python
+results_bytes, filename = api.download_task_results(task_id=1, format='csv')
+with open(filename, 'wb') as file:
+    file.write(results_bytes)
+```
+
+You can also apply views, sorts and filters:
+
+```python
+results_bytes, filename = api.download_task_results(
+    task_id=1,
+    format='excel',  # format can be one of: json, csv or excel
+    # view='overview',
+    # sort='my_sort',
+    # filters={'your_filter': 'value'},
+)
+```
+
+### Aborting and Deleting Tasks
+
+To abort a specific task, use the `abort_task` method:
+
+```python
+api.abort_task(task_id=1)
+```
+
+To delete a specific task, use the `delete_task` method:
+
+```python
+api.delete_task(task_id=1)
+```
+
+You can also bulk abort or delete multiple tasks at once using the `abort_tasks` and `delete_tasks` methods, respectively:
+
+```python
+api.abort_tasks(1, 2, 3)
+api.delete_tasks(4, 5, 6)
+```
+
+## Examples
+
+Here are some example usages of the API client:
+
+```python
+from botasaurus_api import Api
+
+# Create an instance of the API client
+api = Api()
+
+# Create an asynchronous task
+data = {'link': 'https://www.omkar.cloud/'}
+task = api.create_sync_task(data, scraper_name='scrape_heading_task')
+
+# Fetch the task
+task = api.get_task(task['id'])
+
+# Fetch the task results
+results = api.get_task_results(task['id'])
+
+# Download the task results as a CSV
+results_bytes, filename = api.download_task_results(task['id'], format='csv')
+
+# Abort the task
+api.abort_task(task['id'])
+
+# Delete the task
+api.delete_task(task['id'])
+
+# --- Bulk Operations ---
+
+# Create multiple synchronous tasks
+data_items = [{'link': 'https://www.omkar.cloud/'}, {'link': 'https://www.omkar.cloud/blog/'}]
+tasks = api.create_sync_tasks(data_items, scraper_name='scrape_heading_task')
+
+# Fetch all tasks
+all_tasks = api.get_tasks()
+
+# Bulk abort tasks
+api.abort_tasks(*[task['id'] for task in tasks])
+
+# Bulk delete tasks
+api.delete_tasks(*[task['id'] for task in tasks])
+```
+
+## That's It!
+
+Now, go and build something awesome.
```

