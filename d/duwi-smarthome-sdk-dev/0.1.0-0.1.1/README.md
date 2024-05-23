# Comparing `tmp/duwi_smarthome_sdk_dev-0.1.0.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.1.0.tar", last modified: Wed May 22 08:27:34 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.1.1.tar", last modified: Wed May 22 08:49:17 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.1.0.tar` & `duwi_smarthome_sdk_dev-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.875171 duwi_smarthome_sdk_dev-0.1.0/
--rw-rw-rw-   0        0        0      722 2024-05-22 08:27:34.874194 duwi_smarthome_sdk_dev-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.783475 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.810771 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     2037 2024-05-22 08:25:29.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     5084 2024-05-22 07:35:29.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/group.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.816641 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.818587 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.821518 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-05-22 08:22:28.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.835223 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.843924 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.872249 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1861 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-22 08:27:34.000000 duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 08:27:34.875171 duwi_smarthome_sdk_dev-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-22 08:27:25.000000 duwi_smarthome_sdk_dev-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.845874 duwi_smarthome_sdk_dev-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:27:34.867358 duwi_smarthome_sdk_dev-0.1.0/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/__init__.py
--rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_account.py
--rw-rw-rw-   0        0        0      988 2024-05-22 08:26:30.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_control.py
--rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_discover.py
--rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_floor.py
--rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_group.py
--rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_house.py
--rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_login.py
--rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_room.py
--rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.0/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.443544 duwi_smarthome_sdk_dev-0.1.1/
+-rw-rw-rw-   0        0        0      722 2024-05-22 08:49:17.442561 duwi_smarthome_sdk_dev-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.382319 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.403817 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     2037 2024-05-22 08:25:29.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     5150 2024-05-22 08:49:15.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.407723 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.408700 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.410656 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-22 08:22:28.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.421041 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.425958 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.441585 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-22 08:49:17.000000 duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:49:17.443544 duwi_smarthome_sdk_dev-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-22 08:49:15.000000 duwi_smarthome_sdk_dev-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.426934 duwi_smarthome_sdk_dev-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.1.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:17.439630 duwi_smarthome_sdk_dev-0.1.1/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_account.py
+-rw-rw-rw-   0        0        0      988 2024-05-22 08:26:30.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_control.py
+-rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.1.1/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.1.0/PKG-INFO` & `duwi_smarthome_sdk_dev-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.1.0
+Version: 0.1.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/group.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,41 +80,41 @@
         Converts a dictionary representing a device group into a Group object.
 
         :param group_dict: A dictionary containing device group details.
         :return: A Group object.
         """
         return Group(
             device_group_no=group_dict.get("deviceGroupNo"),
-            device_group_name=group_dict.get("deviceGroupName"),
-            house_no=group_dict.get("houseNo"),
-            room_no=group_dict.get("roomNo"),
-            icon=group_dict.get("icon"),
+            device_group_name=group_dict.get("deviceGroupName", ""),
+            house_no=group_dict.get("houseNo", ""),
+            room_no=group_dict.get("roomNo", ""),
+            icon=group_dict.get("icon", ""),
             is_favorite=group_dict.get("isFavorite"),
-            favorite_time=group_dict.get("favoriteTime"),
-            create_time=group_dict.get("createTime"),
-            update_time=group_dict.get("updateTime"),
+            favorite_time=group_dict.get("favoriteTime", ""),
+            create_time=group_dict.get("createTime", ""),
+            update_time=group_dict.get("updateTime", ""),
             execute_way=group_dict.get("executeWay"),
-            device_group_type=group_dict.get("deviceGroupType"),
+            device_group_type=group_dict.get("deviceGroupType", ""),
             seq=group_dict.get("seq"),
             value=group_dict.get("value"),
-            sync_host_sequences=group_dict.get("syncHostSequences"),
-            device_no=group_dict.get("deviceGroupNo"),
-            device_name=group_dict.get("deviceGroupName"),
-            terminal_sequence=group_dict.get("terminalSequence"),
+            sync_host_sequences=group_dict.get("syncHostSequences", []),
+            device_no=group_dict.get("deviceNo", ""),
+            device_name=group_dict.get("deviceName", ""),
+            terminal_sequence=group_dict.get("terminalSequence", ""),
             route_num=group_dict.get("routeNum"),
-            device_type_no=group_dict.get("deviceTypeNo"),
-            device_sub_type_no=group_dict.get("deviceSubTypeNo"),
-            room_name=group_dict.get("roomName"),
-            floor_no=group_dict.get("floorNo"),
-            floor_name=group_dict.get("floorName"),
+            device_type_no=group_dict.get("deviceTypeNo", ""),
+            device_sub_type_no=group_dict.get("deviceSubTypeNo", ""),
+            room_name=group_dict.get("roomName", ""),
+            floor_no=group_dict.get("floorNo", ""),
+            floor_name=group_dict.get("floorName", ""),
             is_use=group_dict.get("isUse"),
             is_online=group_dict.get("isOnline"),
-            create_time_device=group_dict.get("createTimeDevice"),
+            create_time_device=group_dict.get("createTimeDevice", ""),
             seq_device=group_dict.get("seqDevice"),
             is_favorite_device=group_dict.get("isFavoriteDevice"),
-            favorite_time_device=group_dict.get("favoriteTimeDevice"),
+            favorite_time_device=group_dict.get("favoriteTimeDevice", ""),
             key_binding_quantity=group_dict.get("keyBindingQuantity"),
             key_mapping_quantity=group_dict.get("keyMappingQuantity"),
             value_device=group_dict.get("valueDevice")
         )
```

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/const/type_map.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/group.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/PKG-INFO` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.1.0
+Version: 0.1.1
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.1.0/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt` & `duwi_smarthome_sdk_dev-0.1.1/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/setup.py` & `duwi_smarthome_sdk_dev-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_account.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_control.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_discover.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_floor.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_group.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_house.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_login.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_room.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_terminal.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.1.0/test/api/test_ws.py` & `duwi_smarthome_sdk_dev-0.1.1/test/api/test_ws.py`

 * *Files identical despite different names*

