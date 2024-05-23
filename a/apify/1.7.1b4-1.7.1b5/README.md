# Comparing `tmp/apify-1.7.1b4.tar.gz` & `tmp/apify-1.7.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.7.1b4.tar", last modified: Thu May 23 07:52:56 2024, max compression
+gzip compressed data, was "apify-1.7.1b5.tar", last modified: Thu May 23 14:00:41 2024, max compression
```

## Comparing `apify-1.7.1b4.tar` & `apify-1.7.1b5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.037572 apify-1.7.1b4/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-23 07:52:21.000000 apify-1.7.1b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 07:52:56.037572 apify-1.7.1b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-23 07:52:21.000000 apify-1.7.1b4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-23 07:52:53.000000 apify-1.7.1b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:52:56.037572 apify-1.7.1b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.025572 apify-1.7.1b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.029572 apify-1.7.1b4/src/apify/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.029572 apify-1.7.1b4/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59997 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/middlewares/apify_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/scrapy/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/pipelines/actor_dataset_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/scrapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 07:52:21.000000 apify-1.7.1b4/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:52:56.033572 apify-1.7.1b4/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 07:52:56.000000 apify-1.7.1b4/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.322569 apify-1.7.1b5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-23 14:00:11.000000 apify-1.7.1b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 14:00:41.322569 apify-1.7.1b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-23 14:00:11.000000 apify-1.7.1b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-23 14:00:39.000000 apify-1.7.1b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:00:41.322569 apify-1.7.1b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.310569 apify-1.7.1b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.314569 apify-1.7.1b5/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.314569 apify-1.7.1b5/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.314569 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60423 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.318569 apify-1.7.1b5/src/apify/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.318569 apify-1.7.1b5/src/apify/scrapy/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/middlewares/apify_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.318569 apify-1.7.1b5/src/apify/scrapy/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/pipelines/actor_dataset_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/scrapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.318569 apify-1.7.1b5/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 14:00:11.000000 apify-1.7.1b5/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:00:41.318569 apify-1.7.1b5/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 14:00:41.000000 apify-1.7.1b5/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 14:00:41.000000 apify-1.7.1b5/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:00:41.000000 apify-1.7.1b5/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 14:00:41.000000 apify-1.7.1b5/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 14:00:41.000000 apify-1.7.1b5/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.7.1b4/LICENSE` & `apify-1.7.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/PKG-INFO` & `apify-1.7.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b4
+Version: 1.7.1b5
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.7.1b4/README.md` & `apify-1.7.1b5/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/pyproject.toml` & `apify-1.7.1b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify"
-version = "1.7.1b4"
+version = "1.7.1b5"
 description = "Apify SDK for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "sdk", "actor", "scraping", "automation"]
 
 classifiers = [
```

### Comparing `apify-1.7.1b4/src/apify/_crypto.py` & `apify-1.7.1b5/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.7.1b5/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.7.1b5/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.7.1b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/_utils.py` & `apify-1.7.1b5/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/actor.py` & `apify-1.7.1b5/src/apify/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import inspect
 import os
 import sys
-from datetime import datetime, timezone
+from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, TypeVar, cast
 
 from apify_client import ApifyClientAsync
 from apify_shared.consts import ActorEnvVars, ActorEventTypes, ActorExitCodes, ApifyEnvVars, WebhookEventType
 from apify_shared.utils import ignore_docs, maybe_extract_enum_member_value
 
 from apify._crypto import decrypt_input_secrets, load_private_key
@@ -297,64 +297,70 @@
     @classmethod
     async def exit(
         cls: type[Actor],
         *,
         exit_code: int = 0,
         event_listeners_timeout_secs: float | None = EVENT_LISTENERS_TIMEOUT_SECS,
         status_message: str | None = None,
+        cleanup_timeout: timedelta = timedelta(seconds=30),
     ) -> None:
         """Exit the actor instance.
 
         This stops the Actor instance.
         It cancels all the intervals for regularly sending `PERSIST_STATE` events,
         sends a final `PERSIST_STATE` event,
         waits for all the event listeners to finish,
         and stops the event manager.
 
         Args:
             exit_code (int, optional): The exit code with which the actor should fail (defaults to `0`).
             event_listeners_timeout_secs (float, optional): How long should the actor wait for actor event listeners to finish before exiting.
             status_message (str, optional): The final status message that the actor should display.
+            cleanup_timeout (timedelta, optional): How long we should wait for event listeners.
         """
         return await cls._get_default_instance().exit(
             exit_code=exit_code,
             event_listeners_timeout_secs=event_listeners_timeout_secs,
             status_message=status_message,
+            cleanup_timeout=cleanup_timeout,
         )
 
     async def _exit_internal(
         self: Actor,
         *,
         exit_code: int = 0,
         event_listeners_timeout_secs: float | None = EVENT_LISTENERS_TIMEOUT_SECS,
         status_message: str | None = None,
+        cleanup_timeout: timedelta = timedelta(seconds=30),
     ) -> None:
         self._raise_if_not_initialized()
 
         self._is_exiting = True
 
         exit_code = maybe_extract_enum_member_value(exit_code)
 
         self.log.info('Exiting actor', extra={'exit_code': exit_code})
 
-        await self._cancel_event_emitting_intervals()
+        async def finalize() -> None:
+            await self._cancel_event_emitting_intervals()
 
-        # Send final persist state event
-        if not self._was_final_persist_state_emitted:
-            self._event_manager.emit(ActorEventTypes.PERSIST_STATE, {'isMigrating': False})
-            self._was_final_persist_state_emitted = True
+            # Send final persist state event
+            if not self._was_final_persist_state_emitted:
+                self._event_manager.emit(ActorEventTypes.PERSIST_STATE, {'isMigrating': False})
+                self._was_final_persist_state_emitted = True
 
-        if status_message is not None:
-            await self.set_status_message(status_message, is_terminal=True)
+            if status_message is not None:
+                await self.set_status_message(status_message, is_terminal=True)
 
-        # Sleep for a bit so that the listeners have a chance to trigger
-        await asyncio.sleep(0.1)
+            # Sleep for a bit so that the listeners have a chance to trigger
+            await asyncio.sleep(0.1)
 
-        await self._event_manager.close(event_listeners_timeout_secs=event_listeners_timeout_secs)
+            await self._event_manager.close(event_listeners_timeout_secs=event_listeners_timeout_secs)
 
+        await asyncio.wait_for(finalize(), cleanup_timeout.total_seconds())
         self._is_initialized = False
 
         if is_running_in_ipython():
             self.log.debug(f'Not calling sys.exit({exit_code}) because actor is running in IPython')
         elif os.getenv('PYTEST_CURRENT_TEST', default=False):  # noqa: PLW1508
             self.log.debug(f'Not calling sys.exit({exit_code}) because actor is running in an unit test')
         elif hasattr(asyncio, '_nest_patched'):
```

### Comparing `apify-1.7.1b4/src/apify/config.py` & `apify-1.7.1b5/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/consts.py` & `apify-1.7.1b5/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/event_manager.py` & `apify-1.7.1b5/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/log.py` & `apify-1.7.1b5/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/proxy_configuration.py` & `apify-1.7.1b5/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/scrapy/middlewares/apify_proxy.py` & `apify-1.7.1b5/src/apify/scrapy/middlewares/apify_proxy.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/scrapy/pipelines/actor_dataset_push.py` & `apify-1.7.1b5/src/apify/scrapy/pipelines/actor_dataset_push.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/scrapy/requests.py` & `apify-1.7.1b5/src/apify/scrapy/requests.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/scrapy/scheduler.py` & `apify-1.7.1b5/src/apify/scrapy/scheduler.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/scrapy/utils.py` & `apify-1.7.1b5/src/apify/scrapy/utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/storages/base_storage.py` & `apify-1.7.1b5/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/storages/dataset.py` & `apify-1.7.1b5/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/storages/key_value_store.py` & `apify-1.7.1b5/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/storages/request_queue.py` & `apify-1.7.1b5/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify/storages/storage_client_manager.py` & `apify-1.7.1b5/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify.egg-info/PKG-INFO` & `apify-1.7.1b5/src/apify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b4
+Version: 1.7.1b5
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.7.1b4/src/apify.egg-info/SOURCES.txt` & `apify-1.7.1b5/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b4/src/apify.egg-info/requires.txt` & `apify-1.7.1b5/src/apify.egg-info/requires.txt`

 * *Files identical despite different names*

