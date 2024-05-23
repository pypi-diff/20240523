# Comparing `tmp/apify-1.7.1b3.tar.gz` & `tmp/apify-1.7.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.7.1b3.tar", last modified: Wed May 22 14:28:39 2024, max compression
+gzip compressed data, was "apify-1.7.1b4.tar", last modified: Thu May 23 07:52:56 2024, max compression
```

## Comparing `apify-1.7.1b3.tar` & `apify-1.7.1b4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.869960 apify-1.7.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-22 14:28:09.000000 apify-1.7.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-22 14:28:39.869960 apify-1.7.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-22 14:28:09.000000 apify-1.7.1b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-22 14:28:37.000000 apify-1.7.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:28:39.873960 apify-1.7.1b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.857960 apify-1.7.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.861960 apify-1.7.1b3/src/apify/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.865960 apify-1.7.1b3/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.865960 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59997 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.865960 apify-1.7.1b3/src/apify/scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.865960 apify-1.7.1b3/src/apify/scrapy/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/middlewares/apify_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.865960 apify-1.7.1b3/src/apify/scrapy/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/pipelines/actor_dataset_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/scrapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.869960 apify-1.7.1b3/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-22 14:28:09.000000 apify-1.7.1b3/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:28:39.869960 apify-1.7.1b3/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-22 14:28:39.000000 apify-1.7.1b3/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-22 14:28:39.000000 apify-1.7.1b3/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:28:39.000000 apify-1.7.1b3/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-22 14:28:39.000000 apify-1.7.1b3/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 14:28:39.000000 apify-1.7.1b3/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.037572 apify-1.7.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-23 07:52:21.000000 apify-1.7.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 07:52:56.037572 apify-1.7.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-23 07:52:21.000000 apify-1.7.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-23 07:52:53.000000 apify-1.7.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:52:56.037572 apify-1.7.1b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.025572 apify-1.7.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.029572 apify-1.7.1b4/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.029572 apify-1.7.1b4/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59997 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/middlewares/apify_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/pipelines/actor_dataset_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.7.1b3/LICENSE` & `apify-1.7.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/PKG-INFO` & `apify-1.7.1b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b3
+Version: 1.7.1b4
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
@@ -33,31 +33,31 @@
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: psutil>=5.9.5
 Requires-Dist: pyee>=11.0.1
 Requires-Dist: sortedcollections>=2.0.1
 Requires-Dist: typing-extensions>=4.1.0
 Requires-Dist: websockets>=10.1
 Provides-Extra: dev
-Requires-Dist: build~=1.0.3; extra == "dev"
-Requires-Dist: filelock~=3.12.4; extra == "dev"
-Requires-Dist: mypy~=1.7.1; extra == "dev"
-Requires-Dist: pre-commit~=3.4.0; extra == "dev"
-Requires-Dist: pydoc-markdown~=4.8.2; extra == "dev"
-Requires-Dist: pytest~=7.4.2; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.21.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
-Requires-Dist: pytest-only~=2.0.0; extra == "dev"
-Requires-Dist: pytest-timeout~=2.2.0; extra == "dev"
-Requires-Dist: pytest-xdist~=3.3.1; extra == "dev"
-Requires-Dist: respx~=0.20.1; extra == "dev"
-Requires-Dist: ruff~=0.1.13; extra == "dev"
-Requires-Dist: twine~=4.0.2; extra == "dev"
-Requires-Dist: types-aiofiles~=23.2.0.0; extra == "dev"
-Requires-Dist: types-colorama~=0.4.15.12; extra == "dev"
-Requires-Dist: types-psutil~=5.9.5.17; extra == "dev"
+Requires-Dist: build~=1.2.0; extra == "dev"
+Requires-Dist: filelock~=3.14.0; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.5.0; extra == "dev"
+Requires-Dist: pydoc-markdown~=4.8.0; extra == "dev"
+Requires-Dist: pytest~=8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
+Requires-Dist: pytest-only~=2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
+Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
+Requires-Dist: respx~=0.21.0; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: twine~=5.1.0; extra == "dev"
+Requires-Dist: types-aiofiles~=23.2.0.20240403; extra == "dev"
+Requires-Dist: types-colorama~=0.4.15.20240311; extra == "dev"
+Requires-Dist: types-psutil~=5.9.5.20240516; extra == "dev"
 Provides-Extra: scrapy
 Requires-Dist: scrapy>=2.11.0; extra == "scrapy"
 
 # Apify SDK for Python
 
 The Apify SDK for Python is the official library to create [Apify Actors](https://docs.apify.com/platform/actors)
 in Python. It provides useful features like Actor lifecycle management, local storage emulation, and Actor
```

### Comparing `apify-1.7.1b3/README.md` & `apify-1.7.1b4/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/pyproject.toml` & `apify-1.7.1b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify"
-version = "1.7.1b3"
+version = "1.7.1b4"
 description = "Apify SDK for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "sdk", "actor", "scraping", "automation"]
 
 classifiers = [
@@ -38,31 +38,31 @@
     "sortedcollections >= 2.0.1",
     "typing-extensions >= 4.1.0",
     "websockets >= 10.1",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "build ~= 1.0.3",
-    "filelock ~= 3.12.4",
-    "mypy ~= 1.7.1",
-    "pre-commit ~= 3.4.0",
-    "pydoc-markdown ~= 4.8.2",
-    "pytest ~= 7.4.2",
-    "pytest-asyncio ~= 0.21.0",
-    "pytest-cov ~= 4.1.0",
-    "pytest-only ~= 2.0.0",
-    "pytest-timeout ~= 2.2.0",
-    "pytest-xdist ~= 3.3.1",
-    "respx ~= 0.20.1",
-    "ruff ~= 0.1.13",
-    "twine ~= 4.0.2",
-    "types-aiofiles ~= 23.2.0.0",
-    "types-colorama ~= 0.4.15.12",
-    "types-psutil ~= 5.9.5.17",
+    "build ~= 1.2.0",
+    "filelock ~= 3.14.0",
+    "mypy ~= 1.10.0",
+    "pre-commit ~= 3.5.0",
+    "pydoc-markdown ~= 4.8.0",
+    "pytest ~= 8.2.0",
+    "pytest-asyncio ~= 0.23.0",
+    "pytest-cov ~= 5.0.0",
+    "pytest-only ~= 2.1.0",
+    "pytest-timeout ~= 2.3.0",
+    "pytest-xdist ~= 3.6.0",
+    "respx ~= 0.21.0",
+    "ruff ~= 0.4.0",
+    "twine ~= 5.1.0",
+    "types-aiofiles ~= 23.2.0.20240403",
+    "types-colorama ~= 0.4.15.20240311",
+    "types-psutil ~= 5.9.5.20240516",
 ]
 scrapy = [
     "scrapy >= 2.11.0",
 ]
 
 [project.urls]
 "Homepage" = "https://docs.apify.com/sdk/python/"
```

### Comparing `apify-1.7.1b3/src/apify/_crypto.py` & `apify-1.7.1b4/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.7.1b4/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.7.1b4/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/_utils.py` & `apify-1.7.1b4/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/actor.py` & `apify-1.7.1b4/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/config.py` & `apify-1.7.1b4/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/consts.py` & `apify-1.7.1b4/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/event_manager.py` & `apify-1.7.1b4/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/log.py` & `apify-1.7.1b4/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/proxy_configuration.py` & `apify-1.7.1b4/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/scrapy/middlewares/apify_proxy.py` & `apify-1.7.1b4/src/apify/scrapy/middlewares/apify_proxy.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/scrapy/pipelines/actor_dataset_push.py` & `apify-1.7.1b4/src/apify/scrapy/pipelines/actor_dataset_push.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/scrapy/requests.py` & `apify-1.7.1b4/src/apify/scrapy/requests.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/scrapy/scheduler.py` & `apify-1.7.1b4/src/apify/scrapy/scheduler.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/scrapy/utils.py` & `apify-1.7.1b4/src/apify/scrapy/utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/storages/base_storage.py` & `apify-1.7.1b4/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/storages/dataset.py` & `apify-1.7.1b4/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/storages/key_value_store.py` & `apify-1.7.1b4/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/storages/request_queue.py` & `apify-1.7.1b4/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify/storages/storage_client_manager.py` & `apify-1.7.1b4/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify.egg-info/PKG-INFO` & `apify-1.7.1b4/src/apify.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b3
+Version: 1.7.1b4
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
@@ -33,31 +33,31 @@
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: psutil>=5.9.5
 Requires-Dist: pyee>=11.0.1
 Requires-Dist: sortedcollections>=2.0.1
 Requires-Dist: typing-extensions>=4.1.0
 Requires-Dist: websockets>=10.1
 Provides-Extra: dev
-Requires-Dist: build~=1.0.3; extra == "dev"
-Requires-Dist: filelock~=3.12.4; extra == "dev"
-Requires-Dist: mypy~=1.7.1; extra == "dev"
-Requires-Dist: pre-commit~=3.4.0; extra == "dev"
-Requires-Dist: pydoc-markdown~=4.8.2; extra == "dev"
-Requires-Dist: pytest~=7.4.2; extra == "dev"
-Requires-Dist: pytest-asyncio~=0.21.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
-Requires-Dist: pytest-only~=2.0.0; extra == "dev"
-Requires-Dist: pytest-timeout~=2.2.0; extra == "dev"
-Requires-Dist: pytest-xdist~=3.3.1; extra == "dev"
-Requires-Dist: respx~=0.20.1; extra == "dev"
-Requires-Dist: ruff~=0.1.13; extra == "dev"
-Requires-Dist: twine~=4.0.2; extra == "dev"
-Requires-Dist: types-aiofiles~=23.2.0.0; extra == "dev"
-Requires-Dist: types-colorama~=0.4.15.12; extra == "dev"
-Requires-Dist: types-psutil~=5.9.5.17; extra == "dev"
+Requires-Dist: build~=1.2.0; extra == "dev"
+Requires-Dist: filelock~=3.14.0; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pre-commit~=3.5.0; extra == "dev"
+Requires-Dist: pydoc-markdown~=4.8.0; extra == "dev"
+Requires-Dist: pytest~=8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
+Requires-Dist: pytest-only~=2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
+Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
+Requires-Dist: respx~=0.21.0; extra == "dev"
+Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: twine~=5.1.0; extra == "dev"
+Requires-Dist: types-aiofiles~=23.2.0.20240403; extra == "dev"
+Requires-Dist: types-colorama~=0.4.15.20240311; extra == "dev"
+Requires-Dist: types-psutil~=5.9.5.20240516; extra == "dev"
 Provides-Extra: scrapy
 Requires-Dist: scrapy>=2.11.0; extra == "scrapy"
 
 # Apify SDK for Python
 
 The Apify SDK for Python is the official library to create [Apify Actors](https://docs.apify.com/platform/actors)
 in Python. It provides useful features like Actor lifecycle management, local storage emulation, and Actor
```

### Comparing `apify-1.7.1b3/src/apify.egg-info/SOURCES.txt` & `apify-1.7.1b4/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b3/src/apify.egg-info/requires.txt` & `apify-1.7.1b4/src/apify.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 psutil>=5.9.5
 pyee>=11.0.1
 sortedcollections>=2.0.1
 typing-extensions>=4.1.0
 websockets>=10.1
 
 [dev]
-build~=1.0.3
-filelock~=3.12.4
-mypy~=1.7.1
-pre-commit~=3.4.0
-pydoc-markdown~=4.8.2
-pytest~=7.4.2
-pytest-asyncio~=0.21.0
-pytest-cov~=4.1.0
-pytest-only~=2.0.0
-pytest-timeout~=2.2.0
-pytest-xdist~=3.3.1
-respx~=0.20.1
-ruff~=0.1.13
-twine~=4.0.2
-types-aiofiles~=23.2.0.0
-types-colorama~=0.4.15.12
-types-psutil~=5.9.5.17
+build~=1.2.0
+filelock~=3.14.0
+mypy~=1.10.0
+pre-commit~=3.5.0
+pydoc-markdown~=4.8.0
+pytest~=8.2.0
+pytest-asyncio~=0.23.0
+pytest-cov~=5.0.0
+pytest-only~=2.1.0
+pytest-timeout~=2.3.0
+pytest-xdist~=3.6.0
+respx~=0.21.0
+ruff~=0.4.0
+twine~=5.1.0
+types-aiofiles~=23.2.0.20240403
+types-colorama~=0.4.15.20240311
+types-psutil~=5.9.5.20240516
 
 [scrapy]
 scrapy>=2.11.0
```

