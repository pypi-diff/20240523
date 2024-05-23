# Comparing `tmp/eppo_server_sdk-3.0.2.tar.gz` & `tmp/eppo_server_sdk-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo_server_sdk-3.0.2.tar", last modified: Thu May  2 23:36:50 2024, max compression
+gzip compressed data, was "eppo_server_sdk-3.0.3.tar", last modified: Tue May 14 16:43:09 2024, max compression
```

## Comparing `eppo_server_sdk-3.0.2.tar` & `eppo_server_sdk-3.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/eppo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/assignment_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/configuration_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/configuration_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/read_write_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/sharders.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/eppo_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:36:50.567749 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 23:36:50.000000 eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 23:36:46.000000 eppo_server_sdk-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 23:36:50.571749 eppo_server_sdk-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/eppo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/assignment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/configuration_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/configuration_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/sharders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/eppo_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:09.919875 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 16:43:09.000000 eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 16:43:06.000000 eppo_server_sdk-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 16:43:09.923875 eppo_server_sdk-3.0.3/setup.cfg
```

### Comparing `eppo_server_sdk-3.0.2/LICENSE` & `eppo_server_sdk-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/__init__.py` & `eppo_server_sdk-3.0.3/eppo_client/__init__.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/client.py` & `eppo_server_sdk-3.0.3/eppo_client/client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/configuration_requestor.py` & `eppo_server_sdk-3.0.3/eppo_client/configuration_requestor.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/configuration_store.py` & `eppo_server_sdk-3.0.3/eppo_client/configuration_store.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/eval.py` & `eppo_server_sdk-3.0.3/eppo_client/eval.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/http_client.py` & `eppo_server_sdk-3.0.3/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/models.py` & `eppo_server_sdk-3.0.3/eppo_client/models.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/poller.py` & `eppo_server_sdk-3.0.3/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/read_write_lock.py` & `eppo_server_sdk-3.0.3/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_client/rules.py` & `eppo_server_sdk-3.0.3/eppo_client/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         if condition.value:
             return subject_value is None
         return subject_value is not None
 
     if subject_value is not None:
         if condition.operator == OperatorType.MATCHES:
             return isinstance(condition.value, str) and bool(
-                re.match(condition.value, str(subject_value))
+                re.search(condition.value, str(subject_value))
             )
         if condition.operator == OperatorType.NOT_MATCHES:
             return isinstance(condition.value, str) and not bool(
-                re.match(condition.value, str(subject_value))
+                re.search(condition.value, str(subject_value))
             )
         elif condition.operator == OperatorType.ONE_OF:
             return isinstance(condition.value, list) and str(subject_value).lower() in [
                 str(value).lower() for value in condition.value
             ]
         elif condition.operator == OperatorType.NOT_ONE_OF:
             return isinstance(condition.value, list) and str(
```

### Comparing `eppo_server_sdk-3.0.2/eppo_client/sharders.py` & `eppo_server_sdk-3.0.3/eppo_client/sharders.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo_server_sdk-3.0.3/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.0.2/setup.cfg` & `eppo_server_sdk-3.0.3/setup.cfg`

 * *Files identical despite different names*

