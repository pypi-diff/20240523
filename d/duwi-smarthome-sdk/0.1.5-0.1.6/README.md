# Comparing `tmp/duwi_smarthome_sdk-0.1.5.tar.gz` & `tmp/duwi_smarthome_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk-0.1.5.tar", last modified: Thu May 23 02:45:10 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk-0.1.6.tar", last modified: Thu May 23 02:58:04 2024, max compression
```

## Comparing `duwi_smarthome_sdk-0.1.5.tar` & `duwi_smarthome_sdk-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.122175 duwi_smarthome_sdk-0.1.5/
--rw-rw-rw-   0        0        0      705 2024-05-23 02:45:10.121158 duwi_smarthome_sdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-05-15 08:27:04.000000 duwi_smarthome_sdk-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.079104 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.097294 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2530 2024-05-20 09:11:05.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/account.py
--rw-rw-rw-   0        0        0     1759 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/control.py
--rw-rw-rw-   0        0        0     4536 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2647 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/floor.py
--rw-rw-rw-   0        0        0     5136 2024-05-23 02:36:45.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/group.py
--rw-rw-rw-   0        0        0     2675 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/house.py
--rw-rw-rw-   0        0        0     2145 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2755 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/room.py
--rw-rw-rw-   0        0        0     3137 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/terminal.py
--rw-rw-rw-   0        0        0     4790 2024-05-23 02:19:06.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.101379 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       91 2024-05-15 08:04:07.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/const.py
--rw-rw-rw-   0        0        0      603 2024-05-20 07:42:46.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/status.py
--rw-rw-rw-   0        0        0     1470 2024-05-23 02:44:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.103308 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.105289 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-05-22 09:33:52.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.114556 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.118184 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.120140 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/
--rw-rw-rw-   0        0        0      705 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-23 02:45:10.000000 duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 02:45:10.122175 duwi_smarthome_sdk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      937 2024-05-23 02:44:59.000000 duwi_smarthome_sdk-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:45:10.119146 duwi_smarthome_sdk-0.1.5/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.651173 duwi_smarthome_sdk-0.1.6/
+-rw-rw-rw-   0        0        0      705 2024-05-23 02:58:04.650055 duwi_smarthome_sdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-15 08:27:04.000000 duwi_smarthome_sdk-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.606617 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.624918 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2530 2024-05-20 09:11:05.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/account.py
+-rw-rw-rw-   0        0        0     2037 2024-05-23 02:50:43.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4536 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2647 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     5136 2024-05-23 02:36:45.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/group.py
+-rw-rw-rw-   0        0        0     2675 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2145 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2755 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/room.py
+-rw-rw-rw-   0        0        0     3137 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/terminal.py
+-rw-rw-rw-   0        0        0     4790 2024-05-23 02:19:06.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.629800 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       91 2024-05-15 08:04:07.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/const.py
+-rw-rw-rw-   0        0        0      603 2024-05-20 07:42:46.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-23 02:44:10.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.630777 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.632730 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-22 09:33:52.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.641519 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.646145 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.649094 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-23 02:58:04.000000 duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:58:04.651173 duwi_smarthome_sdk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-23 02:50:56.000000 duwi_smarthome_sdk-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:58:04.648103 duwi_smarthome_sdk-0.1.6/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.6/test/__init__.py
```

### Comparing `duwi_smarthome_sdk-0.1.5/PKG-INFO` & `duwi_smarthome_sdk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: duwitech@163.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/account.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/discover.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/floor.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/group.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/house.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/refresh_token.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/room.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/terminal.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/api/ws.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/status.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/const/type_map.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/req/device_control.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/auth.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/device.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/floor.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/group.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/house.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/room.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/model/resp/terminal.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/http.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk/util/sign.py` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/PKG-INFO` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: duwitech@163.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk-0.1.5/duwi_smarthome_sdk.egg-info/SOURCES.txt` & `duwi_smarthome_sdk-0.1.6/duwi_smarthome_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.5/setup.py` & `duwi_smarthome_sdk-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk",
     version=VERSION,
     author="duwi",
     author_email="duwitech@163.com",
```

