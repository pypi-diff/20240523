# Comparing `tmp/agent-bdi-2.4.4.tar.gz` & `tmp/agent-bdi-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.4.4.tar", last modified: Sat May 18 16:05:47 2024, max compression
+gzip compressed data, was "agent-bdi-2.4.5.tar", last modified: Thu May 23 20:29:30 2024, max compression
```

## Comparing `agent-bdi-2.4.4.tar` & `agent-bdi-2.4.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.234370 agent-bdi-2.4.4/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-05-18 16:05:47.233369 agent-bdi-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 16:05:47.234370 agent-bdi-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-18 16:04:56.000000 agent-bdi-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.050170 agent-bdi-2.4.4/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.067186 agent-bdi-2.4.4/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-18 16:05:46.000000 agent-bdi-2.4.4/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.089997 agent-bdi-2.4.4/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.4/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.4/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.107428 agent-bdi-2.4.4/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.4/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.127034 agent-bdi-2.4.4/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.4/src/holon/Heart.py
--rw-rw-rw-   0        0        0     9856 2024-05-04 16:12:54.000000 agent-bdi-2.4.4/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.4/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.4/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.179896 agent-bdi-2.4.4/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.4/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.4/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.4/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5283 2024-05-11 08:16:35.000000 agent-bdi-2.4.4/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6780 2024-05-07 17:25:25.000000 agent-bdi-2.4.4/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     3335 2024-05-18 14:28:14.000000 agent-bdi-2.4.4/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     5112 2024-05-18 14:31:46.000000 agent-bdi-2.4.4/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.4/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:05:47.231361 agent-bdi-2.4.4/tests/
--rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.4/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.4/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.4/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.4/tests/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.649205 agent-bdi-2.4.5/
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/LICENSE.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3202 2024-05-23 20:29:30.648091 agent-bdi-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:29:30.649205 agent-bdi-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-23 20:29:05.000000 agent-bdi-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.584122 agent-bdi-2.4.5/src/
+-rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/abdi_config.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.605547 agent-bdi-2.4.5/src/agent_bdi.egg-info/
+-rw-rw-rw-   0        0        0     3202 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-23 20:29:30.000000 agent-bdi-2.4.5/src/agent_bdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.618125 agent-bdi-2.4.5/src/broker/
+-rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/broker_maker.py
+-rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/empty_broker.py
+-rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/message_broker.py
+-rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.5/src/broker/mqtt_broker.py
+-rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/broker/notifier.py
+-rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/redis_broker.py
+-rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/ros_broker.py
+-rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.5/src/broker/ros_noetic_broker.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.624774 agent-bdi-2.4.5/src/core/
+-rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.5/src/core/Agent.py
+-rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Belief.py
+-rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Desire.py
+-rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/Intention.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.632223 agent-bdi-2.4.5/src/holon/
+-rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/Blackboard.py
+-rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.5/src/holon/Heart.py
+-rw-rw-rw-   0        0        0    10481 2024-05-23 19:22:38.000000 agent-bdi-2.4.5/src/holon/HolonicAgent.py
+-rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/HolonicDesire.py
+-rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.5/src/holon/HolonicIntention.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.5/src/holon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.641089 agent-bdi-2.4.5/src/holon/logistics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.5/src/holon/logistics/__init__.py
+-rw-rw-rw-   0        0        0      722 2024-04-27 17:02:10.000000 agent-bdi-2.4.5/src/holon/logistics/base_logistic.py
+-rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.5/src/holon/logistics/broker_logistic.py
+-rw-rw-rw-   0        0        0     5283 2024-05-11 08:16:35.000000 agent-bdi-2.4.5/src/holon/logistics/loading_coordinator.py
+-rw-rw-rw-   0        0        0     6780 2024-05-07 17:25:25.000000 agent-bdi-2.4.5/src/holon/logistics/payload_wrapper.py
+-rw-rw-rw-   0        0        0     3335 2024-05-18 14:28:14.000000 agent-bdi-2.4.5/src/holon/logistics/request_logistic.py
+-rw-rw-rw-   0        0        0     5112 2024-05-18 14:31:46.000000 agent-bdi-2.4.5/src/holon/logistics/response_logistic.py
+-rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.5/src/holon/payload.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:29:30.645865 agent-bdi-2.4.5/tests/
+-rw-rw-rw-   0        0        0      404 2024-04-27 15:27:38.000000 agent-bdi-2.4.5/tests/test01.py
+-rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.5/tests/test_loadingbal.py
+-rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.5/tests/test_request.py
+-rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.5/tests/test_send.py
```

### Comparing `agent-bdi-2.4.4/PKG-INFO` & `agent-bdi-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.4
+Version: 2.4.5
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.4/README.md` & `agent-bdi-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/setup.py` & `agent-bdi-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "2.4.4",
+    version = "2.4.5",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-2.4.4/src/abdi_config.py` & `agent-bdi-2.4.5/src/abdi_config.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.4.5/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.4.4
+Version: 2.4.5
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.4.4/src/agent_bdi.egg-info/SOURCES.txt` & `agent-bdi-2.4.5/src/agent_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/broker_maker.py` & `agent-bdi-2.4.5/src/broker/broker_maker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/empty_broker.py` & `agent-bdi-2.4.5/src/broker/empty_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/message_broker.py` & `agent-bdi-2.4.5/src/broker/message_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/mqtt_broker.py` & `agent-bdi-2.4.5/src/broker/mqtt_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/redis_broker.py` & `agent-bdi-2.4.5/src/broker/redis_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/ros_broker.py` & `agent-bdi-2.4.5/src/broker/ros_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/broker/ros_noetic_broker.py` & `agent-bdi-2.4.5/src/broker/ros_noetic_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/holon/HolonicAgent.py` & `agent-bdi-2.4.5/src/holon/HolonicAgent.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from holon.HolonicIntention import HolonicIntention
 from holon.logistics.base_logistic import BaseLogistic
 
 
 logger = logging.getLogger(LOGGER_NAME)
 
 
-class HolonicAgent(Agent, BrokerNotifier) :
+class HolonicAgent(Agent, BrokerNotifier):
     def __init__(self, config:AbdiConfig=None, b:Blackboard=None, d:HolonicDesire=None, i: HolonicIntention=None):
         b = b or Blackboard()
         d = d or HolonicDesire()
         i = i or HolonicIntention()
         super().__init__(b, d, i)
         
         # self.agent_id = None
@@ -47,14 +47,36 @@
         self._agent_thread = None        
         self._broker = None
         self._topic_handlers = {}
         # self._logistics = None
 
 
     @final
+    def get_data(self, key:str):
+        return self.__repository.get(key)
+
+
+    @final
+    def pop_data(self, key:str):
+        data = None
+        self.__repository_lock.acquire()
+        if key in self.__repository:
+            data = self.__repository.pop(key)
+        self.__repository_lock.release()
+        return data
+
+
+    @final
+    def put_data(self, key:str, data):
+        self.__repository_lock.acquire()
+        self.__repository[key] = data
+        self.__repository_lock.release()        
+
+
+    @final
     def start(self, head=False):
         self._agent_proc = Process(target=self._run, args=(self.config,))
         self._agent_proc.start()
         
         for a in self.head_agents:
             a.start()
         for a in self.body_agents:
@@ -104,14 +126,17 @@
         self._running()
         self._run_end()
     
 
     def _run_begin(self):
         self.on_begining()
 
+        self.__repository = {}
+        self.__repository_lock = threading.Lock()
+
         def signal_handler(signal, frame):
             logger.warning(f"{self.short_id}> {self.name} Ctrl-C: {self.__class__.__name__}")
             self.terminate()
         if self._agent_proc:
             signal.signal(signal.SIGINT, signal_handler)
 
         # self.agent_id = str(uuid.uuid1()).replace("-", "")
```

### Comparing `agent-bdi-2.4.4/src/holon/logistics/base_logistic.py` & `agent-bdi-2.4.5/src/holon/logistics/base_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.4.5/src/holon/logistics/loading_coordinator.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.4.5/src/holon/logistics/payload_wrapper.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/holon/logistics/request_logistic.py` & `agent-bdi-2.4.5/src/holon/logistics/request_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/src/holon/logistics/response_logistic.py` & `agent-bdi-2.4.5/src/holon/logistics/response_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/tests/test_loadingbal.py` & `agent-bdi-2.4.5/tests/test_loadingbal.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/tests/test_request.py` & `agent-bdi-2.4.5/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.4.4/tests/test_send.py` & `agent-bdi-2.4.5/tests/test_send.py`

 * *Files identical despite different names*

