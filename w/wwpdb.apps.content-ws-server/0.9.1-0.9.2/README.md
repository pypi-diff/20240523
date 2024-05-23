# Comparing `tmp/wwpdb.apps.content_ws_server-0.9.1.tar.gz` & `tmp/wwpdb_apps_content_ws_server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.content_ws_server-0.9.1.tar", last modified: Mon Dec 26 12:41:44 2022, max compression
+gzip compressed data, was "wwpdb_apps_content_ws_server-0.9.2.tar", last modified: Thu May 23 20:07:28 2024, max compression
```

## Comparing `wwpdb.apps.content_ws_server-0.9.1.tar` & `wwpdb_apps_content_ws_server-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/
--rw-r--r--   0 vsts      (1001) docker     (123)    11357 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      765 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    10883 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2419 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.464480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.464480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.464480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/
--rw-r--r--   0 vsts      (1001) docker     (123)      151 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/
--rw-r--r--   0 vsts      (1001) docker     (123)     9005 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequest.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1721 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestPolicyFilter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3543 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestProxyReportPdbx.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7241 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3433 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5131 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportPdbx.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content_definitions/
--rw-r--r--   0 vsts      (1001) docker     (123)      273 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content_definitions/ContentDefintions.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15684 2022-12-26 12:41:34.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content_definitions/ws_content_type_definitions.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/message_queue/
--rw-r--r--   0 vsts      (1001) docker     (123)      518 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/message_queue/MessageQueue.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/message_queue/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/register/
--rw-r--r--   0 vsts      (1001) docker     (123)     2533 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/register/Register.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/register/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/service/
--rw-r--r--   0 vsts      (1001) docker     (123)     8091 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/service/ContentRequestServiceHandler.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/service/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.468480 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    25172 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/ContentServiceAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4363 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/WebServiceApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9185 2022-12-26 12:40:15.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2022-12-26 12:41:44.464480 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      765 2022-12-26 12:41:44.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1613 2022-12-26 12:41:44.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2022-12-26 12:41:44.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2022-12-26 12:41:29.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      210 2022-12-26 12:41:44.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2022-12-26 12:41:44.000000 wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1182 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    10883 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-23 20:07:28.537666 wwpdb_apps_content_ws_server-0.9.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2419 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.529665 wwpdb_apps_content_ws_server-0.9.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.529665 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9005 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1721 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestPolicyFilter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3543 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestProxyReportPdbx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7241 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportDb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3433 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5131 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportPdbx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content_definitions/ContentDefintions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15684 2024-05-23 20:07:20.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content_definitions/ws_content_type_definitions.json
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/message_queue/
+-rw-r--r--   0 vsts      (1001) docker     (127)      518 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/message_queue/MessageQueue.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/message_queue/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/register/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2533 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/register/Register.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/register/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/service/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8091 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/service/ContentRequestServiceHandler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/service/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    25195 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/ContentServiceAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4363 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/WebServiceApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9185 2024-05-23 20:06:33.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:07:28.533666 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1182 2024-05-23 20:07:28.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-05-23 20:07:28.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 20:07:28.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 20:07:16.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-05-23 20:07:28.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-23 20:07:28.000000 wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.content_ws_server-0.9.1/LICENSE` & `wwpdb_apps_content_ws_server-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/README.md` & `wwpdb_apps_content_ws_server-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/setup.py` & `wwpdb_apps_content_ws_server-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequest.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestPolicyFilter.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestPolicyFilter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestProxyReportPdbx.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestProxyReportPdbx.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportDb.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportIo.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content/ContentRequestReportPdbx.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content/ContentRequestReportPdbx.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/content_definitions/ws_content_type_definitions.json` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/content_definitions/ws_content_type_definitions.json`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/message_queue/MessageQueue.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/message_queue/MessageQueue.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/register/Register.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/register/Register.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/service/ContentRequestServiceHandler.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/service/ContentRequestServiceHandler.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/ContentServiceAppWorker.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/ContentServiceAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,15 @@
         if not ok:
             sst.setServiceCompletionFlag(ok)
             sst.setServiceError(msg="Session acquire failed")
         else:
             sD = self._getSessionStoreDict()
             ok = False
             pD = {}
+            fName = ""
             #
             #   Check for a test request
             #
             pD["worker_test_mode"] = self._reqObj.getValueOrDefault("worker_test_mode", default=False)
             pD["worker_test_duration"] = self._reqObj.getValueOrDefault("worker_test_duration", default=1)
             pD["exp_method"] = self._reqObj.getValueOrDefault("exp_method", default="unassigned")
             #
```

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/WebServiceApp.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/WebServiceApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb/apps/content_ws_server/webapp/wsgi.py` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb/apps/content_ws_server/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.content_ws_server-0.9.1/wwpdb.apps.content_ws_server.egg-info/SOURCES.txt` & `wwpdb_apps_content_ws_server-0.9.2/wwpdb.apps.content_ws_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

