# Comparing `tmp/foundationallm-0.7.3.tar.gz` & `tmp/foundationallm-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundationallm-0.7.3.tar", last modified: Thu May 23 12:15:10 2024, max compression
+gzip compressed data, was "foundationallm-0.7.4.tar", last modified: Thu May 23 12:17:07 2024, max compression
```

## Comparing `foundationallm-0.7.3.tar` & `foundationallm-0.7.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.714139 foundationallm-0.7.3/
--rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.3/LICENSE
--rw-rw-rw-   0        0        0      633 2024-05-23 12:15:10.713138 foundationallm-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-05-23 11:31:53.000000 foundationallm-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.594606 foundationallm-0.7.3/foundationallm/
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.650165 foundationallm-0.7.3/foundationallm/config/
--rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.3/foundationallm/config/__init__.py
--rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.3/foundationallm/config/configuration.py
--rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.3/foundationallm/config/context.py
--rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.3/foundationallm/config/environment_variables.py
--rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.3/foundationallm/config/user_identity.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.594606 foundationallm-0.7.3/foundationallm/models/
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.708137 foundationallm-0.7.3/foundationallm/models/orchestration/
--rw-rw-rw-   0        0        0      402 2024-05-23 12:09:21.000000 foundationallm-0.7.3/foundationallm/models/orchestration/__init__.py
--rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.3/foundationallm/models/orchestration/citation.py
--rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.3/foundationallm/models/orchestration/completion_request_base.py
--rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.3/foundationallm/models/orchestration/completion_response.py
--rw-rw-rw-   0        0        0      479 2024-05-07 13:15:07.000000 foundationallm-0.7.3/foundationallm/models/orchestration/endpoint_settings.py
--rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.3/foundationallm/models/orchestration/message_history_item.py
--rw-rw-rw-   0        0        0      154 2024-05-07 13:15:07.000000 foundationallm-0.7.3/foundationallm/models/orchestration/operation_types.py
--rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.3/foundationallm/models/orchestration/orchestration_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:15:10.711138 foundationallm-0.7.3/foundationallm.egg-info/
--rw-rw-rw-   0        0        0      633 2024-05-23 12:15:10.000000 foundationallm-0.7.3/foundationallm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      828 2024-05-23 12:15:10.000000 foundationallm-0.7.3/foundationallm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:15:10.000000 foundationallm-0.7.3/foundationallm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 12:15:10.000000 foundationallm-0.7.3/foundationallm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      614 2024-05-23 12:14:41.000000 foundationallm-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 12:15:10.714139 foundationallm-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.540451 foundationallm-0.7.4/
+-rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0      633 2024-05-23 12:17:07.539451 foundationallm-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-05-23 11:31:53.000000 foundationallm-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.491938 foundationallm-0.7.4/foundationallm/
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.516939 foundationallm-0.7.4/foundationallm/config/
+-rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.4/foundationallm/config/__init__.py
+-rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.4/foundationallm/config/configuration.py
+-rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.4/foundationallm/config/context.py
+-rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.4/foundationallm/config/environment_variables.py
+-rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.4/foundationallm/config/user_identity.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.491938 foundationallm-0.7.4/foundationallm/models/
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.536451 foundationallm-0.7.4/foundationallm/models/orchestration/
+-rw-rw-rw-   0        0        0      402 2024-05-23 12:09:21.000000 foundationallm-0.7.4/foundationallm/models/orchestration/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.4/foundationallm/models/orchestration/citation.py
+-rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.4/foundationallm/models/orchestration/completion_request_base.py
+-rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.4/foundationallm/models/orchestration/completion_response.py
+-rw-rw-rw-   0        0        0      469 2024-05-23 12:16:43.000000 foundationallm-0.7.4/foundationallm/models/orchestration/endpoint_settings.py
+-rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.4/foundationallm/models/orchestration/message_history_item.py
+-rw-rw-rw-   0        0        0      154 2024-05-07 13:15:07.000000 foundationallm-0.7.4/foundationallm/models/orchestration/operation_types.py
+-rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.4/foundationallm/models/orchestration/orchestration_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:17:07.538451 foundationallm-0.7.4/foundationallm.egg-info/
+-rw-rw-rw-   0        0        0      633 2024-05-23 12:17:07.000000 foundationallm-0.7.4/foundationallm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2024-05-23 12:17:07.000000 foundationallm-0.7.4/foundationallm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:17:07.000000 foundationallm-0.7.4/foundationallm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 12:17:07.000000 foundationallm-0.7.4/foundationallm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      614 2024-05-23 12:16:56.000000 foundationallm-0.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:17:07.541453 foundationallm-0.7.4/setup.cfg
```

### Comparing `foundationallm-0.7.3/PKG-INFO` & `foundationallm-0.7.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.3/foundationallm/config/configuration.py` & `foundationallm-0.7.4/foundationallm/config/configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/foundationallm/config/context.py` & `foundationallm-0.7.4/foundationallm/config/context.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/foundationallm/config/user_identity.py` & `foundationallm-0.7.4/foundationallm/config/user_identity.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/foundationallm/models/orchestration/completion_response.py` & `foundationallm-0.7.4/foundationallm/models/orchestration/completion_response.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/foundationallm/models/orchestration/orchestration_settings.py` & `foundationallm-0.7.4/foundationallm/models/orchestration/orchestration_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/foundationallm.egg-info/PKG-INFO` & `foundationallm-0.7.4/foundationallm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.3
+Version: 0.7.4
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.3/foundationallm.egg-info/SOURCES.txt` & `foundationallm-0.7.4/foundationallm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.3/pyproject.toml` & `foundationallm-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foundationallm"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="FoundationaLLM", email="dev@foundationallm.ai" },
 ]
 description = "Enables integration with the FoundationaLLM platform."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

