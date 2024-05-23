# Comparing `tmp/e2enetworks-1.2.4.tar.gz` & `tmp/e2enetworks-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.2.4.tar", last modified: Thu May  2 10:18:52 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.5.tar", last modified: Thu May 23 06:58:59 2024, max compression
```

## Comparing `e2enetworks-1.2.4.tar` & `e2enetworks-1.2.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.197772 e2enetworks-1.2.4/
--rw-r--r--   0 aman       (501) staff       (20)    10786 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/LICENSE.txt
--rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-02 10:18:52.197592 e2enetworks-1.2.4/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/README.rst
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.189750 e2enetworks-1.2.4/e2enetworks/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.191265 e2enetworks-1.2.4/e2enetworks/cloud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)      147 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/test.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.196534 e2enetworks-1.2.4/e2enetworks/cloud/tir/
--rw-r--r--   0 aman       (501) staff       (20)     2390 2024-05-01 12:23:40.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     9305 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 aman       (501) staff       (20)     2794 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 aman       (501) staff       (20)     9394 2024-05-01 11:52:21.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 aman       (501) staff       (20)     8779 2024-05-02 06:03:17.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 aman       (501) staff       (20)     5630 2024-05-01 11:21:31.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 aman       (501) staff       (20)    13823 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/endpoints.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.197276 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/
--rw-r--r--   0 aman       (501) staff       (20)        0 2024-04-30 09:51:50.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)      382 2024-05-01 09:25:21.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/constants.py
--rw-r--r--   0 aman       (501) staff       (20)     9809 2024-05-02 06:26:59.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/finetuner.py
--rw-r--r--   0 aman       (501) staff       (20)     3057 2024-04-30 05:41:18.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 aman       (501) staff       (20)     1368 2023-11-28 07:27:23.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 aman       (501) staff       (20)     2105 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 aman       (501) staff       (20)     6455 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 aman       (501) staff       (20)     6022 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 aman       (501) staff       (20)     9999 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 aman       (501) staff       (20)     2849 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 aman       (501) staff       (20)     4268 2024-05-01 10:15:57.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 aman       (501) staff       (20)     2391 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 aman       (501) staff       (20)     1059 2024-05-02 06:16:05.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 aman       (501) staff       (20)       23 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 aman       (501) staff       (20)     1561 2024-05-02 06:03:17.000000 e2enetworks-1.2.4/e2enetworks/constants.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.190865 e2enetworks-1.2.4/e2enetworks.egg-info/
--rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)     1051 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 aman       (501) staff       (20)        1 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 aman       (501) staff       (20)       40 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 aman       (501) staff       (20)       12 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 aman       (501) staff       (20)       38 2024-05-02 10:18:52.197838 e2enetworks-1.2.4/setup.cfg
--rw-r--r--   0 aman       (501) staff       (20)     1710 2024-05-02 07:30:01.000000 e2enetworks-1.2.4/setup.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.895915 e2enetworks-1.2.5/
+-rw-r--r--   0 aman       (501) staff       (20)    10786 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/LICENSE.txt
+-rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-23 06:58:59.895574 e2enetworks-1.2.5/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/README.rst
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.884729 e2enetworks-1.2.5/e2enetworks/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.886582 e2enetworks-1.2.5/e2enetworks/cloud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      147 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/test.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.893726 e2enetworks-1.2.5/e2enetworks/cloud/tir/
+-rw-r--r--   0 aman       (501) staff       (20)     2390 2024-05-01 12:23:40.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     9305 2024-04-23 09:50:02.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 aman       (501) staff       (20)     2794 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 aman       (501) staff       (20)     9394 2024-05-01 11:52:21.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 aman       (501) staff       (20)     8779 2024-05-02 06:03:17.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     5630 2024-05-01 11:21:31.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 aman       (501) staff       (20)    13823 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/endpoints.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.894758 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2024-04-30 09:51:50.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      382 2024-05-01 09:25:21.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     9809 2024-05-22 10:54:24.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/finetuner.py
+-rw-r--r--   0 aman       (501) staff       (20)     3057 2024-05-22 10:54:35.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     1368 2023-11-28 07:27:23.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 aman       (501) staff       (20)     2105 2024-04-23 09:50:02.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     6934 2024-05-23 06:01:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 aman       (501) staff       (20)     6022 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 aman       (501) staff       (20)     9999 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 aman       (501) staff       (20)     2849 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 aman       (501) staff       (20)     4268 2024-05-01 10:15:57.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 aman       (501) staff       (20)     2391 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 aman       (501) staff       (20)     1059 2024-05-02 06:16:05.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 aman       (501) staff       (20)       23 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 aman       (501) staff       (20)     1566 2024-05-22 11:49:33.000000 e2enetworks-1.2.5/e2enetworks/constants.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.886151 e2enetworks-1.2.5/e2enetworks.egg-info/
+-rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     1051 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 aman       (501) staff       (20)        1 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 aman       (501) staff       (20)       40 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 aman       (501) staff       (20)       12 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 aman       (501) staff       (20)       38 2024-05-23 06:58:59.895998 e2enetworks-1.2.5/setup.cfg
+-rw-r--r--   0 aman       (501) staff       (20)     1710 2024-05-23 06:02:59.000000 e2enetworks-1.2.5/setup.py
```

### Comparing `e2enetworks-1.2.4/LICENSE.txt` & `e2enetworks-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/PKG-INFO` & `e2enetworks-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.4
+Version: 1.2.5
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/api_client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/datasets.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/endpoints.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/endpoints.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/finetuner.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/finetuner.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/helpers.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/images.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/minio_service.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,28 @@
             minio_service = MinioService(access_key=access_key, secret_key=secret_key)
             minio_service.download_directory_recursive(bucket_name=model.bucket.bucket_name, local_path=local_path, prefix=prefix)
             print("Model downloaded successfully")
         except Exception as e:
             print(e)
             raise ValueError("invalid model id")
 
-    def get(self, model_id):
+    def _update_repo(self, model_id, score={}):
+        if type(model_id) != int:
+            raise ValueError(model_id)
+        payload = {
+            "score": score
+        }
 
+        url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/serving/model/{model_id}/"
+        req = requests.Request('PUT', url, json=payload)
+        response = client.Default.make_request(req)
+        response = prepare_object(response)
+        return response
+
+    def get(self, model_id):
         if type(model_id) != int:
             raise ValueError(model_id)
 
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/serving/model/" \
               f"{model_id}/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
```

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/notebook.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/notebook.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/pipelines.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/projects.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/skus.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.5/e2enetworks/cloud/tir/utils.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/e2enetworks/constants.py` & `e2enetworks-1.2.5/e2enetworks/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 BASE_URL_MODEL_API_CLIENT = os.environ.get("MODEL_API_CLIENT_HOST", "https://infer.e2enetworks.net/")
-MY_ACCOUNT_LB_URL = os.environ.get("E2E_TIR_API_HOST", "https://api.e2enetworks.com/myaccount/")
+MY_ACCOUNT_LB_URL = os.environ.get("E2E_TIR_API_HOST", "https://api-thor.e2enetworks.net/myaccount/")
 
 GPU_URL = "api/v1/gpu/"
 BASE_GPU_URL = f"{MY_ACCOUNT_LB_URL}{GPU_URL}"
 VALIDATED_SUCCESSFULLY = "Validated Successfully"
 INVALID_CREDENTIALS = "Validation Failed, Invalid APIkey or Token"
 headers = {
     'Connection': 'keep-alive',
```

### Comparing `e2enetworks-1.2.4/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-1.2.5/e2enetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.4
+Version: 1.2.5
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
```

### Comparing `e2enetworks-1.2.4/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.5/e2enetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.4/setup.py` & `e2enetworks-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.2.4"
+version = "1.2.5"
 install_requires = [
     "requests",
     "urllib3",
     "minio",
     "prettytable",
     "tqdm"
 ]
```

