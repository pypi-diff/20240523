# Comparing `tmp/taskara-0.1.87.tar.gz` & `tmp/taskara-0.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.87.tar", max compression
+gzip compressed data, was "taskara-0.1.89.tar", max compression
```

## Comparing `taskara-0.1.87.tar` & `taskara-0.1.89.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.87/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.87/README.md
--rw-r--r--   0        0        0     1149 2024-05-22 02:10:01.421342 taskara-0.1.87/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.87/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.87/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.87/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.87/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.87/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.87/taskara/auth/transport.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.87/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.87/taskara/config.py
--rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.87/taskara/db/conn.py
--rw-r--r--   0        0        0     1682 2024-05-22 02:05:59.304348 taskara-0.1.87/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.87/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.87/taskara/metrics.py
--rw-r--r--   0        0        0    11823 2024-05-22 02:05:59.304732 taskara-0.1.87/taskara/runtime/base.py
--rw-r--r--   0        0        0    14256 2024-05-22 02:05:59.305169 taskara-0.1.87/taskara/runtime/docker.py
--rw-r--r--   0        0        0    30487 2024-05-22 02:05:59.305538 taskara-0.1.87/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.87/taskara/runtime/load.py
--rw-r--r--   0        0        0    16251 2024-05-22 02:05:59.305817 taskara-0.1.87/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.87/taskara/server/app.py
--rw-r--r--   0        0        0     2798 2024-05-22 02:05:59.306098 taskara-0.1.87/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.87/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    36114 2024-05-22 02:09:57.737020 taskara-0.1.87/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.87/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.87/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.89/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.89/README.md
+-rw-r--r--   0        0        0     1149 2024-05-22 04:12:34.676236 taskara-0.1.89/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.89/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.89/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.89/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.89/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.89/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.89/taskara/auth/transport.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.89/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.89/taskara/config.py
+-rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.89/taskara/db/conn.py
+-rw-r--r--   0        0        0     1682 2024-05-22 02:05:59.304348 taskara-0.1.89/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.89/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.89/taskara/metrics.py
+-rw-r--r--   0        0        0    12133 2024-05-22 04:12:34.676830 taskara-0.1.89/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14256 2024-05-22 02:05:59.305169 taskara-0.1.89/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30487 2024-05-22 02:05:59.305538 taskara-0.1.89/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.89/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16251 2024-05-22 02:05:59.305817 taskara-0.1.89/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.89/taskara/server/app.py
+-rw-r--r--   0        0        0     2798 2024-05-22 02:05:59.306098 taskara-0.1.89/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.89/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36114 2024-05-22 02:09:57.737020 taskara-0.1.89/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.89/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.89/PKG-INFO
```

### Comparing `taskara-0.1.87/LICENSE` & `taskara-0.1.89/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/README.md` & `taskara-0.1.89/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/pyproject.toml` & `taskara-0.1.89/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.87"
+version = "0.1.89"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,16 +14,16 @@
 docker = {version = "^7.0.0", optional = true}
 kubernetes = {version = "^29.0.0", optional = true}
 google-auth = {version = "^2.29.0", optional = true}
 google-cloud-container = {version = "^2.45.0", optional = true}
 namesgenerator = "^0.3"
 typer = {version = "^0.12.3", optional = true}
 tabulate = {version = "^0.9.0", optional = true}
-skillpacks = "^0.1.27"
-devicebay = "^0.1.24"
+skillpacks = "^0.1.29"
+devicebay = "^0.1.25"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
 pytest-env = "^1.1.3"
```

### Comparing `taskara-0.1.87/taskara/agent.py` & `taskara-0.1.89/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/auth/key.py` & `taskara-0.1.89/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/auth/provider.py` & `taskara-0.1.89/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/auth/transport.py` & `taskara-0.1.89/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/cli/main.py` & `taskara-0.1.89/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/config.py` & `taskara-0.1.89/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/db/conn.py` & `taskara-0.1.89/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/db/models.py` & `taskara-0.1.89/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/metrics.py` & `taskara-0.1.89/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/runtime/base.py` & `taskara-0.1.89/taskara/runtime/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,24 @@
                 .filter_by(**kwargs)
                 .order_by(TrackerRecord.created.desc())
                 .all()
             )
             return [cls.from_record(record) for record in records]
         raise ValueError("No session")
 
+    @classmethod
+    def active_runtimes(cls) -> List["TrackerRuntime"]:
+        """Get all runtimes currently being used by a tracker
+
+        Returns:
+            List[TrackerRuntime]: a list of tracker runtimes
+        """
+        trackers = cls.find()
+        return [tracker.runtime for tracker in trackers]
+
     def to_v1(self) -> V1Tracker:
         """Convert to V1 API model"""
         return V1Tracker(
             name=self._name,
             runtime=V1TrackerRuntimeConnect(
                 name=self._runtime.name(), connect_config=self.runtime.connect_config()
             ),
@@ -395,16 +405,15 @@
             headers (Optional[dict], optional): Headers. Defaults to None.
 
         Returns:
             Tuple[int, str]: Status code and response text
         """
         pass
 
-    
     @abstractmethod
     def refresh(self, owner_id: Optional[str] = None) -> None:
         """Refresh the runtime
 
         Args:
             owner_id (Optional[str], optional): Owner id to scope it to. Defaults to None.
         """
-        pass
+        pass
```

### Comparing `taskara-0.1.87/taskara/runtime/docker.py` & `taskara-0.1.89/taskara/runtime/docker.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/runtime/kube.py` & `taskara-0.1.89/taskara/runtime/kube.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/runtime/load.py` & `taskara-0.1.89/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/runtime/process.py` & `taskara-0.1.89/taskara/runtime/process.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/server/app.py` & `taskara-0.1.89/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/server/models.py` & `taskara-0.1.89/taskara/server/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/server/router/tasks.py` & `taskara-0.1.89/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/task.py` & `taskara-0.1.89/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/taskara/util.py` & `taskara-0.1.89/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.87/PKG-INFO` & `taskara-0.1.89/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.87
+Version: 0.1.89
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: runtime
-Requires-Dist: devicebay (>=0.1.24,<0.2.0)
+Requires-Dist: devicebay (>=0.1.25,<0.2.0)
 Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: skillpacks (>=0.1.27,<0.2.0)
+Requires-Dist: skillpacks (>=0.1.29,<0.2.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "cli" or extra == "all"
 Requires-Dist: threadmem (>=0.2.26,<0.3.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all"
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.87 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.89 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
-Extra: runtime Requires-Dist: devicebay (>=0.1.24,<0.2.0) Requires-Dist: docker
+Extra: runtime Requires-Dist: devicebay (>=0.1.25,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
 auth (>=2.29.0,<3.0.0) ; extra == "runtime" or extra == "all" Requires-Dist:
 google-cloud-container (>=2.45.0,<3.0.0) ; extra == "runtime" or extra == "all"
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0) ; extra == "runtime" or extra ==
 "all" Requires-Dist: namesgenerator (>=0.3,<0.4) Requires-Dist: pydantic
-(>=2.6.4,<3.0.0) Requires-Dist: skillpacks (>=0.1.27,<0.2.0) Requires-Dist:
+(>=2.6.4,<3.0.0) Requires-Dist: skillpacks (>=0.1.29,<0.2.0) Requires-Dist:
 sqlalchemy (>=2.0.29,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra
 == "cli" or extra == "all" Requires-Dist: threadmem (>=0.2.26,<0.3.0) Requires-
 Dist: typer (>=0.12.3,<0.13.0) ; extra == "cli" or extra == "all" Description-
 Content-Type: text/markdown
                              ************ TTaasskkaarraa ************
                         Task management for AI agents
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
```

