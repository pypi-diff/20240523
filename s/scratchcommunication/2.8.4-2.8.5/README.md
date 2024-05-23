# Comparing `tmp/scratchcommunication-2.8.4.tar.gz` & `tmp/scratchcommunication-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.8.4.tar", last modified: Tue May 21 09:35:11 2024, max compression
+gzip compressed data, was "scratchcommunication-2.8.5.tar", last modified: Thu May 23 13:33:57 2024, max compression
```

## Comparing `scratchcommunication-2.8.4.tar` & `scratchcommunication-2.8.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-21 09:35:11.000000 scratchcommunication-2.8.4/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 09:35:11.000000 scratchcommunication-2.8.4/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:35:11.000000 scratchcommunication-2.8.4/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 09:35:11.000000 scratchcommunication-2.8.4/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:35:11.000000 scratchcommunication-2.8.4/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:35:11.151384 scratchcommunication-2.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 09:35:07.000000 scratchcommunication-2.8.4/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:57.404892 scratchcommunication-2.8.5/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-23 13:33:57.000000 scratchcommunication-2.8.5/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 13:33:57.000000 scratchcommunication-2.8.5/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:33:57.000000 scratchcommunication-2.8.5/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 13:33:57.000000 scratchcommunication-2.8.5/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 13:33:57.000000 scratchcommunication-2.8.5/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:57.408892 scratchcommunication-2.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 13:33:53.000000 scratchcommunication-2.8.5/tests/test1.py
```

### Comparing `scratchcommunication-2.8.4/LICENSE` & `scratchcommunication-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/PKG-INFO` & `scratchcommunication-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.4
+Version: 2.8.5
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.4/README.md` & `scratchcommunication-2.8.5/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/scratchcommunication/cloud.py` & `scratchcommunication-2.8.5/scratchcommunication/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         self.data_reception = StoppableThread(target=self.receive_data, daemon=daemon_thread)
         self.data_reception.start()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        pass
+        self.stop_thread()
 
     def stop_thread(self):
         """
         Use for stopping the underlying thread.
         """
         self.thread_running = False
         self.data_reception.stop(StopException)
```

### Comparing `scratchcommunication-2.8.4/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.8.5/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.8.5/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.8.5/scratchcommunication/cloudrequests/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
             self.uses_thread = True
             self.thread = StoppableThread(target=lambda : self.start(thread=False), daemon=daemon_thread)
             self.thread.start()
             return
         clients : list[tuple[CloudSocketConnection, str]] = []
         end_time = duration and (time.time() + duration)
         while (not end_time) or time.time() < end_time:
+            time.sleep(0.05)
             try:
                 try:
                     clients.append(self.cloud_socket.accept(timeout=0))
                 except TimeoutError:
                     pass
                 for client, username in clients:
                     try:
@@ -79,29 +80,29 @@
                                 name, args, kwargs = parse_python_request(raw_req, req_name)
                             elif not re.match(r"\w+(.*)$", raw_req):
                                 name, args, kwargs = parse_normal_request(raw_req, req_name)
                             else:
                                 raise PermissionError("Python syntax is not allowed for this.")
                     except Exception:
                         response = "The command syntax was wrong."
-                        warnings.warn("Received a request with an invalid syntax.", RuntimeWarning)
+                        warnings.warn("Received a request with an invalid syntax: \n"+traceback.format_exc(), RuntimeWarning)
                     else:
                         try:
                             self.execute_request(name, args=args, kwargs=kwargs, client=client)
                             response = None
                         except Exception:
                             response = "Something went wrong."
                             warnings.warn("Something went wrong with a request.", RuntimeWarning)
                     if response:
                         client.send(response)
             except Exception:
                 warnings.warn(f"There was an uncaught error in the request handler: {traceback.format_exc()}", RuntimeWarning)
                 
     
-    def execute_request(self, name, *, args : Sequence[Any], kwargs : Mapping[str, Any], client : CloudSocketConnection) -> Union[str, float, int]:
+    def execute_request(self, name, *, args : Sequence[Any], kwargs : Mapping[str, Any], client : CloudSocketConnection) -> None:
         """
         Execute a request.
         """
         request_handling_function = self.requests[name]
         args, kwargs, return_converter = type_casting(func=request_handling_function, signature=inspect.signature(request_handling_function), args=args, kwargs=kwargs)
         def respond():
             try:
```

### Comparing `scratchcommunication-2.8.4/scratchcommunication/security.py` & `scratchcommunication-2.8.5/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/scratchcommunication/session.py` & `scratchcommunication-2.8.5/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.8.5/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.4
+Version: 2.8.5
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.4/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.8.5/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.4/setup.py` & `scratchcommunication-2.8.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.8.4'
+VERSION = '2.8.5'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.8.4/tests/test1.py` & `scratchcommunication-2.8.5/tests/test1.py`

 * *Files identical despite different names*

