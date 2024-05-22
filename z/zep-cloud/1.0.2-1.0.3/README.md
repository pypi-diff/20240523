# Comparing `tmp/zep_cloud-1.0.2.tar.gz` & `tmp/zep_cloud-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_cloud-1.0.2.tar", max compression
+gzip compressed data, was "zep_cloud-1.0.3.tar", max compression
```

## Comparing `zep_cloud-1.0.2.tar` & `zep_cloud-1.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5078 2024-05-14 05:00:57.004809 zep_cloud-1.0.2/README.md
--rw-r--r--   0        0        0      670 2024-05-14 05:00:57.012809 zep_cloud-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1610 2024-05-14 05:00:57.012809 zep_cloud-1.0.2/src/zep_cloud/__init__.py
--rw-r--r--   0        0        0     6052 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/base_client.py
--rw-r--r--   0        0        0     2188 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/client.py
--rw-r--r--   0        0        0      853 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/api_error.py
--rw-r--r--   0        0        0     1501 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/core/request_options.py
--rw-r--r--   0        0        0       65 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/document/__init__.py
--rw-r--r--   0        0        0    93354 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/document/client.py
--rw-r--r--   0        0        0      158 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/environment.py
--rw-r--r--   0        0        0      352 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/errors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/errors/bad_request_error.py
--rw-r--r--   0        0        0      360 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/errors/internal_server_error.py
--rw-r--r--   0        0        0      354 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/errors/not_found_error.py
--rw-r--r--   0        0        0      358 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/errors/unauthorized_error.py
--rw-r--r--   0        0        0      581 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/external_clients/document.py
--rw-r--r--   0        0        0      563 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/external_clients/memory.py
--rw-r--r--   0        0        0      545 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/external_clients/user.py
--rw-r--r--   0        0        0      186 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/langchain/__init__.py
--rw-r--r--   0        0        0      380 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/langchain/helpers.py
--rw-r--r--   0        0        0     6905 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/langchain/history.py
--rw-r--r--   0        0        0    19893 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/langchain/vectorstore.py
--rw-r--r--   0        0        0      153 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/memory/__init__.py
--rw-r--r--   0        0        0   108548 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/memory/client.py
--rw-r--r--   0        0        0      178 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/memory/types/__init__.py
--rw-r--r--   0        0        0      208 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/memory/types/memory_get_request_memory_type.py
--rw-r--r--   0        0        0        0 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/py.typed
--rw-r--r--   0        0        0     1730 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/__init__.py
--rw-r--r--   0        0        0      872 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/api_error.py
--rw-r--r--   0        0        0     1044 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/classify_session_response.py
--rw-r--r--   0        0        0     1055 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/create_document_request.py
--rw-r--r--   0        0        0     1772 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/document_collection_response.py
--rw-r--r--   0        0        0     1342 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/document_response.py
--rw-r--r--   0        0        0     1387 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/document_search_result.py
--rw-r--r--   0        0        0     1173 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/document_search_result_page.py
--rw-r--r--   0        0        0     1549 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/memory.py
--rw-r--r--   0        0        0     1155 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/memory_search_result.py
--rw-r--r--   0        0        0     2061 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/message.py
--rw-r--r--   0        0        0     1251 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/message_list_response.py
--rw-r--r--   0        0        0      962 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/models_zep_data_class.py
--rw-r--r--   0        0        0      873 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/question.py
--rw-r--r--   0        0        0      193 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/role_type.py
--rw-r--r--   0        0        0      158 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/search_scope.py
--rw-r--r--   0        0        0      155 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/search_type.py
--rw-r--r--   0        0        0     1606 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/session.py
--rw-r--r--   0        0        0     1023 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/session_list_response.py
--rw-r--r--   0        0        0      879 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/success_response.py
--rw-r--r--   0        0        0     1567 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/summary.py
--rw-r--r--   0        0        0     1019 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/summary_list_response.py
--rw-r--r--   0        0        0     1087 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/update_document_list_request.py
--rw-r--r--   0        0        0     1480 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/user.py
--rw-r--r--   0        0        0     1003 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/types/user_list_response.py
--rw-r--r--   0        0        0       65 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/user/__init__.py
--rw-r--r--   0        0        0    37852 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/user/client.py
--rw-r--r--   0        0        0       77 2024-05-14 05:00:57.016809 zep_cloud-1.0.2/src/zep_cloud/version.py
--rw-r--r--   0        0        0     5573 1970-01-01 00:00:00.000000 zep_cloud-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5078 2024-05-22 22:39:41.040478 zep_cloud-1.0.3/README.md
+-rw-r--r--   0        0        0      670 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1610 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/__init__.py
+-rw-r--r--   0        0        0     6052 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/base_client.py
+-rw-r--r--   0        0        0     2424 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/client.py
+-rw-r--r--   0        0        0      853 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/api_error.py
+-rw-r--r--   0        0        0     1501 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/document/__init__.py
+-rw-r--r--   0        0        0    93354 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/document/client.py
+-rw-r--r--   0        0        0      158 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/environment.py
+-rw-r--r--   0        0        0      352 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/errors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/errors/bad_request_error.py
+-rw-r--r--   0        0        0      360 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/errors/internal_server_error.py
+-rw-r--r--   0        0        0      354 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/errors/not_found_error.py
+-rw-r--r--   0        0        0      358 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      581 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/external_clients/document.py
+-rw-r--r--   0        0        0      563 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/external_clients/memory.py
+-rw-r--r--   0        0        0      545 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/external_clients/user.py
+-rw-r--r--   0        0        0      186 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/langchain/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/langchain/helpers.py
+-rw-r--r--   0        0        0     6905 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/langchain/history.py
+-rw-r--r--   0        0        0    19893 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/langchain/vectorstore.py
+-rw-r--r--   0        0        0      153 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/memory/__init__.py
+-rw-r--r--   0        0        0   108548 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/memory/client.py
+-rw-r--r--   0        0        0      178 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/memory/types/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/memory/types/memory_get_request_memory_type.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/py.typed
+-rw-r--r--   0        0        0     1730 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/api_error.py
+-rw-r--r--   0        0        0     1044 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/classify_session_response.py
+-rw-r--r--   0        0        0     1055 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/create_document_request.py
+-rw-r--r--   0        0        0     1772 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/document_collection_response.py
+-rw-r--r--   0        0        0     1342 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/document_response.py
+-rw-r--r--   0        0        0     1387 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/document_search_result.py
+-rw-r--r--   0        0        0     1173 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/document_search_result_page.py
+-rw-r--r--   0        0        0     1722 2024-05-22 22:39:41.048478 zep_cloud-1.0.3/src/zep_cloud/types/memory.py
+-rw-r--r--   0        0        0     1155 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/memory_search_result.py
+-rw-r--r--   0        0        0     2061 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/message.py
+-rw-r--r--   0        0        0     1251 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/message_list_response.py
+-rw-r--r--   0        0        0      962 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/models_zep_data_class.py
+-rw-r--r--   0        0        0      873 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/question.py
+-rw-r--r--   0        0        0      193 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/role_type.py
+-rw-r--r--   0        0        0      158 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/search_scope.py
+-rw-r--r--   0        0        0      155 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/search_type.py
+-rw-r--r--   0        0        0     1606 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/session.py
+-rw-r--r--   0        0        0     1023 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/session_list_response.py
+-rw-r--r--   0        0        0      879 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/success_response.py
+-rw-r--r--   0        0        0     1567 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/summary.py
+-rw-r--r--   0        0        0     1019 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/summary_list_response.py
+-rw-r--r--   0        0        0     1087 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/update_document_list_request.py
+-rw-r--r--   0        0        0     1480 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/user.py
+-rw-r--r--   0        0        0     1003 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/types/user_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/user/__init__.py
+-rw-r--r--   0        0        0    37852 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/user/client.py
+-rw-r--r--   0        0        0       77 2024-05-22 22:39:41.052478 zep_cloud-1.0.3/src/zep_cloud/version.py
+-rw-r--r--   0        0        0     5573 1970-01-01 00:00:00.000000 zep_cloud-1.0.3/PKG-INFO
```

### Comparing `zep_cloud-1.0.2/README.md` & `zep_cloud-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/pyproject.toml` & `zep_cloud-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-cloud"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "zep_cloud", from = "src"}
 ]
```

### Comparing `zep_cloud-1.0.2/src/zep_cloud/__init__.py` & `zep_cloud-1.0.3/src/zep_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/base_client.py` & `zep_cloud-1.0.3/src/zep_cloud/base_client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/client.py` & `zep_cloud-1.0.3/src/zep_cloud/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,17 @@
             base_url: typing.Optional[str] = None,
             environment: ZepEnvironment = ZepEnvironment.DEFAULT,
             api_key: typing.Optional[str] = os.getenv("ZEP_API_KEY"),
             timeout: typing.Optional[float] = None,
             follow_redirects: typing.Optional[bool] = None,
             httpx_client: typing.Optional[httpx.Client] = None
     ):
+        env_api_url = os.getenv("ZEP_API_URL")
+        if env_api_url:
+            base_url = f"{env_api_url}/api/v2"
         super().__init__(
             base_url=base_url,
             environment=environment,
             api_key=api_key,
             timeout=timeout,
             follow_redirects=follow_redirects,
             httpx_client=httpx_client
@@ -40,14 +43,17 @@
             base_url: typing.Optional[str] = None,
             environment: ZepEnvironment = ZepEnvironment.DEFAULT,
             api_key: typing.Optional[str] = os.getenv("ZEP_API_KEY"),
             timeout: typing.Optional[float] = None,
             follow_redirects: typing.Optional[bool] = None,
             httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
+        env_api_url = os.getenv("ZEP_API_URL")
+        if env_api_url:
+            base_url = f"{env_api_url}/api/v2"
         super().__init__(
             base_url=base_url,
             environment=environment,
             api_key=api_key,
             timeout=timeout,
             follow_redirects=follow_redirects,
             httpx_client=httpx_client
```

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/__init__.py` & `zep_cloud-1.0.3/src/zep_cloud/core/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/client_wrapper.py` & `zep_cloud-1.0.3/src/zep_cloud/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "zep-cloud",
-            "X-Fern-SDK-Version": "1.0.2",
+            "X-Fern-SDK-Version": "1.0.3",
         }
         headers["Authorization"] = f"Api-Key {self.api_key}"
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/datetime_utils.py` & `zep_cloud-1.0.3/src/zep_cloud/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/file.py` & `zep_cloud-1.0.3/src/zep_cloud/core/file.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/http_client.py` & `zep_cloud-1.0.3/src/zep_cloud/core/http_client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/jsonable_encoder.py` & `zep_cloud-1.0.3/src/zep_cloud/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/core/request_options.py` & `zep_cloud-1.0.3/src/zep_cloud/core/request_options.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/document/client.py` & `zep_cloud-1.0.3/src/zep_cloud/document/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/external_clients/document.py` & `zep_cloud-1.0.3/src/zep_cloud/external_clients/document.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/external_clients/memory.py` & `zep_cloud-1.0.3/src/zep_cloud/external_clients/memory.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/external_clients/user.py` & `zep_cloud-1.0.3/src/zep_cloud/external_clients/user.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/langchain/history.py` & `zep_cloud-1.0.3/src/zep_cloud/langchain/history.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/langchain/vectorstore.py` & `zep_cloud-1.0.3/src/zep_cloud/langchain/vectorstore.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/memory/client.py` & `zep_cloud-1.0.3/src/zep_cloud/memory/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/__init__.py` & `zep_cloud-1.0.3/src/zep_cloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/api_error.py` & `zep_cloud-1.0.3/src/zep_cloud/types/api_error.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/classify_session_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/classify_session_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/create_document_request.py` & `zep_cloud-1.0.3/src/zep_cloud/types/create_document_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/document_collection_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/document_collection_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/document_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/document_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/document_search_result.py` & `zep_cloud-1.0.3/src/zep_cloud/types/document_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/document_search_result_page.py` & `zep_cloud-1.0.3/src/zep_cloud/types/document_search_result_page.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/memory.py` & `zep_cloud-1.0.3/src/zep_cloud/types/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     """
 
     metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
     A dictionary containing metadata associated with the memory.
     """
 
+    relevant_summaries: typing.Optional[typing.List[Summary]] = pydantic_v1.Field(default=None)
+    """
+    Summary list result from Summary Retriever Memory Type.
+    """
+
     summary: typing.Optional[Summary] = pydantic_v1.Field(default=None)
     """
     A Summary object.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/memory_search_result.py` & `zep_cloud-1.0.3/src/zep_cloud/types/memory_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/message.py` & `zep_cloud-1.0.3/src/zep_cloud/types/message.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/message_list_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/message_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/models_zep_data_class.py` & `zep_cloud-1.0.3/src/zep_cloud/types/models_zep_data_class.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/question.py` & `zep_cloud-1.0.3/src/zep_cloud/types/question.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/session.py` & `zep_cloud-1.0.3/src/zep_cloud/types/session.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/session_list_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/session_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/success_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/success_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/summary.py` & `zep_cloud-1.0.3/src/zep_cloud/types/summary.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/summary_list_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/summary_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/update_document_list_request.py` & `zep_cloud-1.0.3/src/zep_cloud/types/update_document_list_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/user.py` & `zep_cloud-1.0.3/src/zep_cloud/types/user.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/types/user_list_response.py` & `zep_cloud-1.0.3/src/zep_cloud/types/user_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/src/zep_cloud/user/client.py` & `zep_cloud-1.0.3/src/zep_cloud/user/client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-1.0.2/PKG-INFO` & `zep_cloud-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-cloud
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zep-cloud Version: 1.0.2 Summary: Requires-Python:
+Metadata-Version: 2.1 Name: zep-cloud Version: 1.0.3 Summary: Requires-Python:
 >=3.8.1,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2) Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown [![Release to PyPI](https://github.com/
 getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/
```

