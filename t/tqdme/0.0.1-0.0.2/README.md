# Comparing `tmp/tqdme-0.0.1.tar.gz` & `tmp/tqdme-0.0.2.tar.gz`

## Comparing `tqdme-0.0.1.tar` & `tqdme-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tqdme-0.0.1/.env
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tqdme-0.0.1/.gitattributes
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 tqdme-0.0.1/demo_progress.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 tqdme-0.0.1/demo_server.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tqdme-0.0.1/license.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tqdme-0.0.1/src/tqdme/__init__.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 tqdme-0.0.1/src/tqdme/server.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 tqdme-0.0.1/src/tqdme/tqdme.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tqdme-0.0.1/src/tqdme/utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tqdme-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tqdme-0.0.1/README.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 tqdme-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 tqdme-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tqdme-0.0.2/.env
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tqdme-0.0.2/.gitattributes
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 tqdme-0.0.2/demo_neuroconv_conversion.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 tqdme-0.0.2/demo_progress.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 tqdme-0.0.2/demo_server.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tqdme-0.0.2/license.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tqdme-0.0.2/src/tqdme/__init__.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 tqdme-0.0.2/src/tqdme/server.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 tqdme-0.0.2/src/tqdme/tqdme.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tqdme-0.0.2/src/tqdme/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tqdme-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tqdme-0.0.2/README.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 tqdme-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 tqdme-0.0.2/PKG-INFO
```

### Comparing `tqdme-0.0.1/demo_progress.py` & `tqdme-0.0.2/demo_progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-"""Demo of parallel tqdm visualization using tqdm.me polyfill"""
-
-# Replace tqdm with tqdme (works in other packages)
-from src.tqdme import tqdme
-import tqdm
-tqdm.tqdm = tqdme
+"""Demo of parallel tqdme visualization"""
 
 # Load environment variables
 from dotenv import load_dotenv
 load_dotenv() 
 
 # Import the necessary libraries for the demo
 import time
 from datetime import datetime
 from typing import List
 from concurrent.futures import ProcessPoolExecutor, as_completed
-from threading import Thread
 
-from tqdm import tqdm
+from tqdme import tqdme
 
 N_JOBS = 3
 
 # Each outer entry is a list of 'tasks' to perform on a particular worker
 # For demonstration purposes, each in the list of tasks is the length of time in seconds
 # that each iteration of the task takes to run and update the progress bar (emulated by sleeping)
 BASE_SECONDS_PER_TASK = 0.5  # The base time for each task; actual time increases proportional to the index of the task
@@ -45,15 +39,15 @@
     sleep_time : float
         The amount of time this task emulates having taken to complete.
     iteration_index : int
         The index of this task in the list of all tasks from the buffer map.
         Each index would map to a different tqdm position.
     """
 
-    sub_progress_bar = tqdm(
+    sub_progress_bar = tqdme(
         iterable=task_times,
         position=iteration_index + 1,
         desc=f"Progress on iteration {iteration_index}",
         leave=False,
         tqdme_options=dict(
             parent=group
         )
@@ -80,15 +74,15 @@
                     task_times=task_times_per_job,
                     iteration_index=iteration_index,
                     group=group
                 )
             )
 
         total_tasks_iterable = as_completed(futures)
-        total_tasks_progress_bar = tqdm(
+        total_tasks_progress_bar = tqdme(
             iterable=total_tasks_iterable, 
             total=len(all_task_times), 
             desc=f"Total tasks completed",
             tqdme_options=dict(
                 group=group
             )
         )
```

### Comparing `tqdme-0.0.1/license.txt` & `tqdme-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `tqdme-0.0.1/src/tqdme/server.py` & `tqdme-0.0.2/src/tqdme/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,25 +54,31 @@
 
     if metadata.get("done"):
         changes["id"] = False
 
     return state, changes
 
 
+def get_client_ip():
+    if request.headers.get('X-Forwarded-For'):
+        return request.headers.get('X-Forwarded-For').split(',')[0]
+    return request.remote_addr
+
 def create(base_path, host, port):
 
     STATES = {}
 
     app = Flask(__name__)
     app.config['CORS_HEADERS'] = 'Content-Type'
     socketio = SocketIO(app, cors_allowed_origins="*")
 
     def update_local_state(metadata):
 
-        metadata["user_id"] = request.remote_addr # Add request IP address as the unique User ID
+        if (not metadata.get("user_id")):
+            metadata["user_id"] = get_client_ip() # Add request IP address as the unique User ID
 
         state, changes = update_states(STATES, metadata)
 
         user_changes = changes.get("user_id")
         if user_changes:
             url = get_url(host, port, metadata)
             message = 'onremoved' if not user_changes else 'onadded'
@@ -110,15 +116,15 @@
     @cross_origin()
     def update():
         data = json.loads(request.data) if request.data else {}
 
         state = update_local_state(data)
         
         # Send to frontend
-        socketio.emit('progress', state, room=request.remote_addr)
+        socketio.emit('progress', state, room=state["user_id"])
 
         # Create pages for each User ID
         return get_response(host, port, data)
 
     
     @socketio.on('subscribe')
     def subscribe(page_id):
```

### Comparing `tqdme-0.0.1/src/tqdme/tqdme.py` & `tqdme-0.0.2/src/tqdme/tqdme.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from tqdm import tqdm as base_tqdm
 from .utils import getBoolEnv
 
 ACTIVE_BARS = dict()
 
 DEFAULT_CONFIG = dict(
+    user_id = lambda: os.getenv('TQDME_USER_ID', None),
     verbose = lambda: getBoolEnv('TQDME_VERBOSE'),
     display = lambda: getBoolEnv('TQDME_DISPLAY'),
     url = lambda: os.getenv('TQDME_URL', 'http://tqdm.me'),
     id = lambda: str(uuid4()),
     group = lambda: os.getpid(),
     parent = lambda: os.getppid()
 )
@@ -74,16 +75,15 @@
         if not self.__tqdme["display"] and 'file' not in kwargs:
             kwargs['file'] = BlockTqdmDisplay()
 
         # Initialize the base tqdm class
         super().__init__(*args, **kwargs)
 
         # Send initialization
-        update = dict(format=self.format_dict.copy())
-        self.__sendrequest('update', update)
+        self.__sendupdate()
 
     # Override the update method to run a callback function
     def update(self, n: int = 1) -> Union[bool, None]:
         displayed = super().update(n)
 
         self.__sendupdate()
         return displayed
@@ -97,14 +97,15 @@
             self.__sendrequest('ping', dict(done=True))
             ACTIVE_BARS.pop(self.__tqdme['id'], None)
             self.__done = True
 
     # Always send a consistent update
     def __sendupdate(self):
         update = dict(format=self.format_dict.copy())
+
         if update['format']['n'] == update['format']['total']:
             update['done'] = True
 
         return self.__sendrequest('update', update)
 
     # Check if the server has been rejected
     def __isconnected(self):
@@ -120,14 +121,19 @@
         if not self.__isconnected():
             return
 
         url = f"{self.__tqdme['url']}/{pathname}" 
 
         http = urllib3.PoolManager()
 
+        # Provide arbitrary user_id on all requests (if exists)
+        if self.__tqdme["user_id"] is not None:
+            data['user_id'] = self.__tqdme["user_id"]
+
+
         try:
             to_send = { key: self.__tqdme[key] for key in METADATA_TO_SEND }
             to_send.update(data)
 
             response = http.request('POST', url, body=json.dumps(to_send), headers={'Content-Type': 'application/json'})
             if response.status == 200:
                 return json.loads(response.data)
```

### Comparing `tqdme-0.0.1/README.md` & `tqdme-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tqdme-0.0.1/pyproject.toml` & `tqdme-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
 
 [project]
 name = "tqdme"
-version="0.0.1"
+version="0.0.2"
 authors = [
   { name="Garrett Flynn", email="garrettmflynn@gmail.com" }
 ]
 description = "Forward progress from tqdm to a public website"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "license.txt"}
```

### Comparing `tqdme-0.0.1/PKG-INFO` & `tqdme-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tqdme
-Version: 0.0.1
+Version: 0.0.2
 Summary: Forward progress from tqdm to a public website
 Project-URL: Homepage, https://github.com/tqdme/tqdme
 Project-URL: Bug Tracker, https://github.com/tqdme/tqdme/issues
 Author-email: Garrett Flynn <garrettmflynn@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Garrett Flynn
```

