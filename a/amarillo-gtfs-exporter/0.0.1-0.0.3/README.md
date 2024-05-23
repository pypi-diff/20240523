# Comparing `tmp/amarillo-gtfs-exporter-0.0.1.tar.gz` & `tmp/amarillo_gtfs_exporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarillo-gtfs-exporter-0.0.1.tar", last modified: Wed Mar 27 10:52:51 2024, max compression
+gzip compressed data, was "amarillo_gtfs_exporter-0.0.3.tar", last modified: Thu May 23 08:54:47 2024, max compression
```

## Comparing `amarillo-gtfs-exporter-0.0.1.tar` & `amarillo_gtfs_exporter-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    34523 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      176 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       68 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       64 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       64 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       33 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4421 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      393 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs_constants.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9968 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs_export.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2478 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs_generator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12321 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/gtfs_realtime_pb2.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2543 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/realtime_extension_pb2.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/models/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/models/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1716 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/models/gtfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2494 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/router.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/tests/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/tests/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5355 2024-03-21 14:51:00.000000 amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/tests/test_gtfs.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      176 2024-03-27 10:52:51.000000 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      920 2024-03-27 10:52:51.000000 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-03-27 10:52:51.000000 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       43 2024-03-27 10:52:51.000000 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       14 2024-03-27 10:52:51.000000 amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      180 2024-03-27 10:52:37.000000 amarillo-gtfs-exporter-0.0.1/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2024-03-27 10:52:51.389988 amarillo-gtfs-exporter-0.0.1/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/
+-rw-r--r--   0 user      (1000) user      (1000)    34523 2024-01-29 14:38:33.000000 amarillo_gtfs_exporter-0.0.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      112 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)       68 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.645766 amarillo_gtfs_exporter-0.0.3/amarillo/
+-rw-r--r--   0 user      (1000) user      (1000)       64 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.645766 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/
+-rw-r--r--   0 user      (1000) user      (1000)       64 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.645766 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      263 2024-05-09 12:00:04.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/config.py
+-rw-r--r--   0 user      (1000) user      (1000)     4421 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs.py
+-rw-r--r--   0 user      (1000) user      (1000)      393 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs_constants.py
+-rw-r--r--   0 user      (1000) user      (1000)     9968 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs_export.py
+-rw-r--r--   0 user      (1000) user      (1000)      137 2024-05-17 12:20:42.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs_generator.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    12321 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/gtfs_realtime_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2543 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/realtime_extension_pb2.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/models/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/models/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1716 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/models/gtfs.py
+-rw-r--r--   0 user      (1000) user      (1000)     3796 2024-05-17 13:07:22.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/router.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5355 2024-04-10 10:02:46.000000 amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/tests/test_gtfs.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      112 2024-05-23 08:54:47.000000 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      959 2024-05-23 08:54:47.000000 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-23 08:54:47.000000 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2024-05-23 08:54:47.000000 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       47 2024-05-23 08:54:47.000000 amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      131 2024-05-23 08:53:03.000000 amarillo_gtfs_exporter-0.0.3/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-23 08:54:47.649766 amarillo_gtfs_exporter-0.0.3/setup.cfg
```

### Comparing `amarillo-gtfs-exporter-0.0.1/LICENSE` & `amarillo_gtfs_exporter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfs_export.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfs_export.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/gtfs_realtime_pb2.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/gtfs_realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/gtfsrt/realtime_extension_pb2.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/gtfsrt/realtime_extension_pb2.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/models/gtfs.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/models/gtfs.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo/plugins/gtfs_export/tests/test_gtfs.py` & `amarillo_gtfs_exporter-0.0.3/amarillo/plugins/gtfs_export/tests/test_gtfs.py`

 * *Files identical despite different names*

### Comparing `amarillo-gtfs-exporter-0.0.1/amarillo_gtfs_exporter.egg-info/SOURCES.txt` & `amarillo_gtfs_exporter-0.0.3/amarillo_gtfs_exporter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 amarillo/__init__.py
 amarillo/plugins/__init__.py
 amarillo/plugins/gtfs_export/__init__.py
+amarillo/plugins/gtfs_export/config.py
 amarillo/plugins/gtfs_export/gtfs.py
 amarillo/plugins/gtfs_export/gtfs_constants.py
 amarillo/plugins/gtfs_export/gtfs_export.py
 amarillo/plugins/gtfs_export/gtfs_generator.py
 amarillo/plugins/gtfs_export/router.py
 amarillo/plugins/gtfs_export/gtfsrt/__init__.py
 amarillo/plugins/gtfs_export/gtfsrt/gtfs_realtime_pb2.py
```

