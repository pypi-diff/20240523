# Comparing `tmp/taskara-0.1.89.tar.gz` & `tmp/taskara-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.89.tar", max compression
+gzip compressed data, was "taskara-0.1.90.tar", max compression
```

## Comparing `taskara-0.1.89.tar` & `taskara-0.1.90.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.89/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.89/README.md
--rw-r--r--   0        0        0     1149 2024-05-22 04:12:34.676236 taskara-0.1.89/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.89/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.89/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.89/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.89/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.89/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.89/taskara/auth/transport.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.89/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.89/taskara/config.py
--rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.89/taskara/db/conn.py
--rw-r--r--   0        0        0     1682 2024-05-22 02:05:59.304348 taskara-0.1.89/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.89/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.89/taskara/metrics.py
--rw-r--r--   0        0        0    12133 2024-05-22 04:12:34.676830 taskara-0.1.89/taskara/runtime/base.py
--rw-r--r--   0        0        0    14256 2024-05-22 02:05:59.305169 taskara-0.1.89/taskara/runtime/docker.py
--rw-r--r--   0        0        0    30487 2024-05-22 02:05:59.305538 taskara-0.1.89/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.89/taskara/runtime/load.py
--rw-r--r--   0        0        0    16251 2024-05-22 02:05:59.305817 taskara-0.1.89/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.89/taskara/server/app.py
--rw-r--r--   0        0        0     2798 2024-05-22 02:05:59.306098 taskara-0.1.89/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.89/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    36114 2024-05-22 02:09:57.737020 taskara-0.1.89/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.89/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.89/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.90/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.90/README.md
+-rw-r--r--   0        0        0     1149 2024-05-23 03:34:03.414008 taskara-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.90/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.90/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.90/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.90/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.90/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.90/taskara/auth/transport.py
+-rw-r--r--   0        0        0    12082 2024-05-23 03:34:03.414355 taskara-0.1.90/taskara/benchmark.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.90/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-23 03:23:29.445785 taskara-0.1.90/taskara/config.py
+-rw-r--r--   0        0        0     2128 2024-05-23 03:34:03.414774 taskara-0.1.90/taskara/db/conn.py
+-rw-r--r--   0        0        0     3504 2024-05-23 03:34:03.415046 taskara-0.1.90/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.90/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.90/taskara/metrics.py
+-rw-r--r--   0        0        0    12133 2024-05-22 04:12:34.676830 taskara-0.1.90/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14307 2024-05-23 03:34:03.415462 taskara-0.1.90/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30554 2024-05-23 03:34:03.415905 taskara-0.1.90/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.90/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16258 2024-05-23 03:34:03.416381 taskara-0.1.90/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.90/taskara/server/app.py
+-rw-r--r--   0        0        0     3511 2024-05-23 03:34:03.416593 taskara-0.1.90/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.90/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36105 2024-05-23 03:34:03.417001 taskara-0.1.90/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.90/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.90/PKG-INFO
```

### Comparing `taskara-0.1.89/LICENSE` & `taskara-0.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/README.md` & `taskara-0.1.90/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/pyproject.toml` & `taskara-0.1.90/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.89"
+version = "0.1.90"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `taskara-0.1.89/taskara/agent.py` & `taskara-0.1.90/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/auth/key.py` & `taskara-0.1.90/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/auth/provider.py` & `taskara-0.1.90/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/auth/transport.py` & `taskara-0.1.90/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/cli/main.py` & `taskara-0.1.90/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/config.py` & `taskara-0.1.90/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/metrics.py` & `taskara-0.1.90/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/runtime/base.py` & `taskara-0.1.90/taskara/runtime/base.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/runtime/docker.py` & `taskara-0.1.90/taskara/runtime/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import signal
 import sys
 import urllib.request
 import urllib.error
 import urllib.parse
 import json
 import os
+import logging
 
 import docker
 from docker.errors import NotFound
 from taskara.util import find_open_port
 from pydantic import BaseModel
 
 from taskara.server.models import (
@@ -18,14 +19,17 @@
     V1ResourceLimits,
     V1ResourceRequests,
 )
 
 from .base import Tracker, TrackerRuntime
 
 
+logger = logging.getLogger(__name__)
+
+
 class DockerConnectConfig(BaseModel):
     timeout: Optional[int] = None
     image: str = "us-central1-docker.pkg.dev/agentsea-dev/taskara/api:latest"
 
 
 class DockerTrackerRuntime(TrackerRuntime["DockerTrackerRuntime", DockerConnectConfig]):
 
@@ -359,15 +363,15 @@
         Reconciles the database against the Docker containers running.
 
         Parameters:
             owner_id (Optional[str]): The owner ID to filter the trackers. If None, refreshes for all owners.
         """
         # List all Docker containers with the specific label
         label_filter = {"label": "provisioner=taskara"}
-        running_containers = self.client.containers.list(filters=label_filter, all=True)
+        running_containers = self.client.containers.list(filters=label_filter)
         running_container_names = {container.name for container in running_containers}  # type: ignore
 
         # List all trackers in the database
         if owner_id:
             db_trackers = Tracker.find(owner_id=owner_id, runtime_name=self.name())
         else:
             db_trackers = Tracker.find(runtime_name=self.name())
@@ -406,10 +410,10 @@
             )
             if not trackers:
                 continue
 
             tracker = trackers[0]
             tracker.delete()
 
-        print(
+        logger.debug(
             f"Refresh completed: added {len(containers_to_add)} trackers, removed {len(containers_to_remove)} trackers."
         )
```

### Comparing `taskara-0.1.89/taskara/runtime/kube.py` & `taskara-0.1.90/taskara/runtime/kube.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from tenacity import retry, stop_after_attempt, wait_fixed
 import socket
 import base64
 import subprocess
 import atexit
 import signal
 import sys
+import logging
 
 from kubernetes import client, config
 from google.oauth2 import service_account
 from google.cloud import container_v1
 from google.auth.transport.requests import Request
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import portforward
@@ -25,14 +26,16 @@
 from pydantic import BaseModel
 
 from taskara.server.models import V1Task
 from taskara.util import find_open_port
 from .base import TrackerRuntime, Tracker
 from taskara.server.models import V1Tracker, V1ResourceLimits, V1ResourceRequests
 
+logger = logging.getLogger(__name__)
+
 
 class GKEOpts(BaseModel):
     cluster_name: str
     region: str
     service_account_json: str
 
 
@@ -768,15 +771,15 @@
         # List all Kubernetes pods with the specific label
         label_selector = "provisioner=surfkit"
         try:
             running_pods = self.core_api.list_namespaced_pod(
                 namespace=self.namespace, label_selector=label_selector
             )
         except ApiException as e:
-            print(f"Failed to list pods: {e}")
+            logger.error(f"Failed to list pods: {e}")
             raise
 
         running_pod_names = {pod.metadata.name for pod in running_pods.items}
 
         # List all trackers in the database
         if owner_id:
             db_trackers = Tracker.find(owner_id=owner_id, runtime_name=self.name())
@@ -809,10 +812,10 @@
                 name=tracker_name, owner_id=owner_id, runtime_name=self.name()
             )
             if not trackers:
                 continue
             tracker = trackers[0]
             tracker.delete()
 
-        print(
+        logger.debug(
             f"Refresh completed: added {len(pods_to_add)} trackers, removed {len(pods_to_remove)} trackers."
         )
```

### Comparing `taskara-0.1.89/taskara/runtime/load.py` & `taskara-0.1.90/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/runtime/process.py` & `taskara-0.1.90/taskara/runtime/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,10 +451,10 @@
                 name=tracker_name, owner_id=owner_id, runtime_name=self.name()
             )
             if not trackers:
                 continue
             tracker = trackers[0]
             tracker.delete()
 
-        print(
+        logger.debug(
             f"Refresh completed: added {len(processes_to_add)} trackers, removed {len(processes_to_remove)} trackers."
         )
```

### Comparing `taskara-0.1.89/taskara/server/app.py` & `taskara-0.1.90/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/server/models.py` & `taskara-0.1.90/taskara/server/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,32 @@
     episode_id: Optional[str] = None
 
 
 class V1Tasks(BaseModel):
     tasks: List[V1Task]
 
 
+class V1TaskTemplate(BaseModel):
+    id: str = Field(default_factory=lambda: str(uuid.uuid4()))
+    description: str
+    max_steps: int = 30
+    device: Optional[V1Device] = None
+    device_type: Optional[V1DeviceType] = None
+    expect_schema: Optional[Dict[str, Any]] = None
+    parameters: Optional[Dict[str, Any]] = {}
+    owner_id: Optional[str] = None
+    tags: List[str] = []
+    labels: Dict[str, str] = {}
+    created: float
+
+
+class V1TaskTemplates(BaseModel):
+    templates: List[V1TaskTemplate]
+
+
 class V1UserProfile(BaseModel):
     email: Optional[str] = None
     display_name: Optional[str] = None
     handle: Optional[str] = None
     picture: Optional[str] = None
     created: Optional[int] = None
     updated: Optional[int] = None
@@ -110,7 +128,18 @@
     cpu: str = "1"
     memory: str = "500m"
     gpu: Optional[str] = None
 
 
 class V1Prompts(BaseModel):
     prompts: List[V1Prompt]
+
+
+class V1Benchmark(BaseModel):
+    id: str
+    name: str
+    description: str
+    tasks: List[V1TaskTemplate]
+    owner_id: Optional[str]
+    tags: List[str]
+    labels: Dict[str, str]
+    created: float
```

### Comparing `taskara-0.1.89/taskara/server/router/tasks.py` & `taskara-0.1.90/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/taskara/task.py` & `taskara-0.1.90/taskara/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         completed: float = 0.0,
         threads: List[RoleThread] = [],
         prompts: List[Prompt] = [],
         assigned_to: Optional[str] = None,
         assigned_type: Optional[str] = None,
         error: Optional[str] = None,
         output: Optional[str] = None,
-        parameters: Optional[Dict[str, Any]] = {},
+        parameters: Dict[str, Any] = {},
         remote: Optional[str] = None,
         version: Optional[str] = None,
         labels: Dict[str, str] = {},
         tags: List[str] = [],
         episode: Optional[Episode] = None,
     ):
         self._id = id if id is not None else str(uuid.uuid4())
@@ -348,15 +348,15 @@
         obj._error = record.error
         obj._output = record.output
         obj._threads = threads
         obj._prompts = prompts
         obj._version = record.version
         obj._parameters = parameters
         obj._remote = None
-        obj.tags = json.loads(str(record.tags))
+        obj._tags = json.loads(str(record.tags))
         obj._labels = json.loads(str(record.labels))
         obj._episode = episode
         return obj
 
     def post_message(
         self,
         role: str,
```

### Comparing `taskara-0.1.89/taskara/util.py` & `taskara-0.1.90/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.89/PKG-INFO` & `taskara-0.1.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.89
+Version: 0.1.90
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.89 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.90 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.25,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
```

