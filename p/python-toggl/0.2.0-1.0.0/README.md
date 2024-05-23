# Comparing `tmp/python-toggl-0.2.0.tar.gz` & `tmp/python-toggl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-toggl-0.2.0.tar", last modified: Thu May 23 19:16:42 2024, max compression
+gzip compressed data, was "python-toggl-1.0.0.tar", last modified: Wed Oct 27 18:44:16 2021, max compression
```

## Comparing `python-toggl-0.2.0.tar` & `python-toggl-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-23 19:16:42.402383 python-toggl-0.2.0/
--rw-r--r--   0 andres     (501) staff       (20)    18025 2024-05-23 18:33:29.000000 python-toggl-0.2.0/LICENSE
--rw-r--r--   0 andres     (501) staff       (20)     2833 2024-05-23 19:16:42.402271 python-toggl-0.2.0/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     2573 2024-05-23 18:33:29.000000 python-toggl-0.2.0/README.rst
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-23 19:16:42.401888 python-toggl-0.2.0/python_toggl.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)     2833 2024-05-23 19:16:42.000000 python-toggl-0.2.0/python_toggl.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)      279 2024-05-23 19:16:42.000000 python-toggl-0.2.0/python_toggl.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-05-23 19:16:42.000000 python-toggl-0.2.0/python_toggl.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-05-23 18:34:43.000000 python-toggl-0.2.0/python_toggl.egg-info/not-zip-safe
--rw-r--r--   0 andres     (501) staff       (20)        9 2024-05-23 19:16:42.000000 python-toggl-0.2.0/python_toggl.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)        6 2024-05-23 19:16:42.000000 python-toggl-0.2.0/python_toggl.egg-info/top_level.txt
--rw-r--r--   0 andres     (501) staff       (20)       38 2024-05-23 19:16:42.402426 python-toggl-0.2.0/setup.cfg
--rw-r--r--   0 andres     (501) staff       (20)      533 2024-05-23 19:16:14.000000 python-toggl-0.2.0/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-23 19:16:42.402106 python-toggl-0.2.0/toggl/
--rw-r--r--   0 andres     (501) staff       (20)       29 2024-05-23 18:33:29.000000 python-toggl-0.2.0/toggl/__init__.py
--rw-r--r--   0 andres     (501) staff       (20)     6767 2024-05-23 19:16:14.000000 python-toggl-0.2.0/toggl/api_client.py
+drwxr-xr-x   0 andres     (501) admin       (80)        0 2021-10-27 18:44:16.349776 python-toggl-1.0.0/
+-rw-r--r--   0 andres     (501) admin       (80)    18025 2021-10-27 18:25:14.000000 python-toggl-1.0.0/LICENSE
+-rw-r--r--   0 andres     (501) admin       (80)     3606 2021-10-27 18:44:16.349480 python-toggl-1.0.0/PKG-INFO
+-rw-r--r--   0 andres     (501) admin       (80)     2573 2021-10-27 18:25:14.000000 python-toggl-1.0.0/README.rst
+drwxr-xr-x   0 andres     (501) admin       (80)        0 2021-10-27 18:44:16.347591 python-toggl-1.0.0/python_toggl.egg-info/
+-rw-r--r--   0 andres     (501) admin       (80)     3606 2021-10-27 18:44:16.000000 python-toggl-1.0.0/python_toggl.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) admin       (80)      279 2021-10-27 18:44:16.000000 python-toggl-1.0.0/python_toggl.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) admin       (80)        1 2021-10-27 18:44:16.000000 python-toggl-1.0.0/python_toggl.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) admin       (80)        1 2021-10-27 18:26:14.000000 python-toggl-1.0.0/python_toggl.egg-info/not-zip-safe
+-rw-r--r--   0 andres     (501) admin       (80)        9 2021-10-27 18:44:16.000000 python-toggl-1.0.0/python_toggl.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) admin       (80)        6 2021-10-27 18:44:16.000000 python-toggl-1.0.0/python_toggl.egg-info/top_level.txt
+-rw-r--r--   0 andres     (501) admin       (80)       38 2021-10-27 18:44:16.349875 python-toggl-1.0.0/setup.cfg
+-rw-r--r--   0 andres     (501) admin       (80)      533 2021-10-27 18:41:13.000000 python-toggl-1.0.0/setup.py
+drwxr-xr-x   0 andres     (501) admin       (80)        0 2021-10-27 18:44:16.348575 python-toggl-1.0.0/toggl/
+-rw-r--r--   0 andres     (501) admin       (80)       29 2021-10-27 18:25:14.000000 python-toggl-1.0.0/toggl/__init__.py
+-rw-r--r--   0 andres     (501) admin       (80)     6679 2021-10-27 18:38:50.000000 python-toggl-1.0.0/toggl/api_client.py
```

### Comparing `python-toggl-0.2.0/LICENSE` & `python-toggl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-toggl-0.2.0/PKG-INFO` & `python-toggl-1.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: python-toggl
-Version: 0.2.0
-Summary: Python Wrapper for Toggl API
-Home-page: https://github.com/swappsco/toggl-python-api-client
-Author: mechastorm
-Author-email: dev@swapps.co
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE
-
 toggl-python-api-client
 =======================
 
 `Toggl <http://toggl.com>`__ is an "insanely simple time tracking"
 service.
 
 This specific library is a Python-based REST client to interface with
@@ -103,9 +92,8 @@
 These tests are to check the connections to Toggl's API and to ensure
 that the client is handling the live responses from Toggl as expected.
 
 To avoid adding sensitive data to version control, no api credentials
 have been included. To enable live tests, - make a copy of
 ``tests/tests_live_config.json.sample`` as
 ``tests/tests_live_config.json`` - update the settings on
-``tests/tests_live_config.json`` as needed
-
+``tests/tests_live_config.json`` as needed
```

### Comparing `python-toggl-0.2.0/setup.py` & `python-toggl-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.rst") as f:
         return f.read()
 
 
 setup(
     name="python-toggl",
-    version="0.2.0",
+    version="1.0.0",
     description="Python Wrapper for Toggl API",
     long_description=readme(),
     url="https://github.com/swappsco/toggl-python-api-client",
     author="mechastorm",
     author_email="dev@swapps.co",
     license="MIT",
     packages=["toggl"],
```

### Comparing `python-toggl-0.2.0/toggl/api_client.py` & `python-toggl-1.0.0/toggl/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class TogglClientApi(object):
 
     defaultCredentials = {
         "username": "",
         "workspace_name": "",
         "base_url": "https://api.track.toggl.com/api",
-        "ver_api": 9,
+        "ver_api": 8,
         "base_url_report": "https://api.track.toggl.com/reports/api",
         "ver_report": 2,
     }
     credentials = {}
     api_token = ""
     api_username = ""
     api_base_url = None
@@ -52,19 +52,19 @@
                 workspace_found = workspace
 
         return workspace_found
 
     def get_workspaces(self):
         return self.query("/workspaces")
 
-    def get_projects(self, active=True):
-        return self.query("/workspaces/%i/projects" % self.workspace_id, params={"active": active})
+    def get_projects(self):
+        return self.query("/workspaces/%i/projects" % self.workspace_id)
 
     def get_workspace_members(self, workspace_id):
-        response = self.query("/workspaces/" + str(workspace_id) + "/users")
+        response = self.query("/workspaces/" + str(workspace_id) + "/workspace_users")
         return response
 
     """
     @param start_date YYYY-MM-DD
     @param end_date YYYY-MM-DD
     """ ""
 
@@ -116,15 +116,15 @@
             time_entries_response.raise_for_status()
 
         json_response = time_entries_response.json()
 
         return json_response
 
     def get_dashboard_data(self, params={}):
-        dashboard_response = self.query("/workspaces/%i/dashboard/all_activity" % self.workspace_id, params)
+        dashboard_response = self.query("/dashboard/%i" % self.workspace_id, params)
 
         if dashboard_response.status_code != requests.codes.ok:
             dashboard_response.raise_for_status()
 
         json_response = dashboard_response.json()
 
         return json_response
@@ -140,15 +140,15 @@
                 "duration":<duration-in-seconds>,
                 "start":"<iso8601-format-datetime>",
                 "pid":<project-id>,
                 "created_with":"<name-of-your-client-app>"
             }
         }
         """
-        response = self.query("/workspaces/%i/time_entries" % self.workspace_id, method="POST", json_data=json_data)
+        response = self.query("/time_entries", method="POST", json_data=json_data)
 
         if response.status_code != requests.codes.ok:
             response.raise_for_status()
 
         response = response.json()
 
         return response
```

