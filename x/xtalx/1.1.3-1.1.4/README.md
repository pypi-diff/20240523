# Comparing `tmp/xtalx-1.1.3.tar.gz` & `tmp/xtalx-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtalx-1.1.3.tar", last modified: Tue Feb  6 23:31:08 2024, max compression
+gzip compressed data, was "xtalx-1.1.4.tar", last modified: Thu May 23 05:45:09 2024, max compression
```

## Comparing `xtalx-1.1.3.tar` & `xtalx-1.1.4.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.289960 xtalx-1.1.3/
--rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-07-27 00:41:10.000000 xtalx-1.1.3/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     5209 2024-02-06 23:31:08.290026 xtalx-1.1.3/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     4704 2023-09-12 00:58:41.000000 xtalx-1.1.3/README.rst
--rw-r--r--   0 greent7    (502) staff       (20)     1276 2024-02-06 23:31:08.290291 xtalx-1.1.3/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-27 00:41:10.000000 xtalx-1.1.3/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.284892 xtalx-1.1.3/xtalx/
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.286229 xtalx-1.1.3/xtalx/p_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)      718 2023-08-04 23:44:45.000000 xtalx-1.1.3/xtalx/p_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      109 2023-08-04 23:44:45.000000 xtalx-1.1.3/xtalx/p_sensor/exception.py
--rw-r--r--   0 greent7    (502) staff       (20)    21608 2024-01-30 23:27:53.000000 xtalx-1.1.3/xtalx/p_sensor/xti.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.284838 xtalx-1.1.3/xtalx/tools/
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.286455 xtalx-1.1.3/xtalx/tools/config/
--rw-r--r--   0 greent7    (502) staff       (20)      203 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/tools/config/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      835 2023-11-24 03:41:26.000000 xtalx-1.1.3/xtalx/tools/config/config.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.286654 xtalx-1.1.3/xtalx/tools/csv/
--rw-r--r--   0 greent7    (502) staff       (20)      143 2024-01-30 23:27:53.000000 xtalx-1.1.3/xtalx/tools/csv/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1554 2024-01-30 23:27:53.000000 xtalx-1.1.3/xtalx/tools/csv/decoder.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.286849 xtalx-1.1.3/xtalx/tools/influxdb/
--rw-r--r--   0 greent7    (502) staff       (20)       89 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/tools/influxdb/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     3405 2024-01-19 21:43:10.000000 xtalx-1.1.3/xtalx/tools/influxdb/push_queue.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.287155 xtalx-1.1.3/xtalx/tools/math/
--rw-r--r--   0 greent7    (502) staff       (20)      215 2023-11-16 00:10:23.000000 xtalx-1.1.3/xtalx/tools/math/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/tools/math/lorentz.py
--rw-r--r--   0 greent7    (502) staff       (20)     2667 2024-01-30 23:27:53.000000 xtalx-1.1.3/xtalx/tools/math/xy_series.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.287845 xtalx-1.1.3/xtalx/tools/p_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:44:45.000000 xtalx-1.1.3/xtalx/tools/p_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1597 2024-01-30 23:27:53.000000 xtalx-1.1.3/xtalx/tools/p_sensor/csv_resample.py
--rw-r--r--   0 greent7    (502) staff       (20)      520 2023-08-04 23:44:45.000000 xtalx-1.1.3/xtalx/tools/p_sensor/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     8038 2024-02-06 23:29:25.000000 xtalx-1.1.3/xtalx/tools/p_sensor/gl_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)      789 2024-01-11 03:11:15.000000 xtalx-1.1.3/xtalx/tools/p_sensor/xtalx_test_read.py
--rw-r--r--   0 greent7    (502) staff       (20)     2687 2023-08-04 23:44:45.000000 xtalx-1.1.3/xtalx/tools/p_sensor/xtalx_test_yield.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.287954 xtalx-1.1.3/xtalx/tools/usb/
--rw-r--r--   0 greent7    (502) staff       (20)      977 2023-08-04 23:59:51.000000 xtalx-1.1.3/xtalx/tools/usb/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.288840 xtalx-1.1.3/xtalx/tools/z_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/tools/z_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1086 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/tools/z_sensor/cli_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)      476 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/tools/z_sensor/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     3166 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/tools/z_sensor/get_info.py
--rw-r--r--   0 greent7    (502) staff       (20)     5345 2024-01-30 23:28:20.000000 xtalx-1.1.3/xtalx/tools/z_sensor/gl_scope_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)     7231 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/tools/z_sensor/gl_sweep_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)    16101 2024-01-30 23:28:20.000000 xtalx-1.1.3/xtalx/tools/z_sensor/gl_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)     7162 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/tools/z_sensor/z_common.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.289865 xtalx-1.1.3/xtalx/z_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)      976 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/z_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    10479 2024-01-30 23:28:20.000000 xtalx-1.1.3/xtalx/z_sensor/peak_tracker.py
--rw-r--r--   0 greent7    (502) staff       (20)     5448 2023-09-12 00:58:41.000000 xtalx-1.1.3/xtalx/z_sensor/predicate_queue.py
--rw-r--r--   0 greent7    (502) staff       (20)      861 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/z_sensor/scope_data.py
--rw-r--r--   0 greent7    (502) staff       (20)     3588 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/z_sensor/sweeper.py
--rw-r--r--   0 greent7    (502) staff       (20)    21964 2024-01-30 23:28:20.000000 xtalx-1.1.3/xtalx/z_sensor/tcsc.py
--rw-r--r--   0 greent7    (502) staff       (20)      205 2023-08-04 23:45:01.000000 xtalx-1.1.3/xtalx/z_sensor/tcsc_u5.py
--rw-r--r--   0 greent7    (502) staff       (20)     1819 2023-09-13 20:20:19.000000 xtalx-1.1.3/xtalx/z_sensor/tincan.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-02-06 23:31:08.285927 xtalx-1.1.3/xtalx.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     5209 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     1316 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      373 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       87 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        6 2024-02-06 23:31:08.000000 xtalx-1.1.3/xtalx.egg-info/top_level.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.330386 xtalx-1.1.4/
+-rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-07-27 00:41:10.000000 xtalx-1.1.4/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 05:45:09.330327 xtalx-1.1.4/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     4704 2023-09-12 00:58:41.000000 xtalx-1.1.4/README.rst
+-rw-r--r--   0 greent7    (502) staff       (20)     1338 2024-05-23 05:45:09.330617 xtalx-1.1.4/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-27 00:41:10.000000 xtalx-1.1.4/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.324666 xtalx-1.1.4/xtalx/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326306 xtalx-1.1.4/xtalx/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      718 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      109 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/p_sensor/exception.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21608 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/p_sensor/xti.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.324615 xtalx-1.1.4/xtalx/tools/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326567 xtalx-1.1.4/xtalx/tools/config/
+-rw-r--r--   0 greent7    (502) staff       (20)      203 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/config/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      835 2024-04-03 23:21:00.000000 xtalx-1.1.4/xtalx/tools/config/config.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326786 xtalx-1.1.4/xtalx/tools/csv/
+-rw-r--r--   0 greent7    (502) staff       (20)      143 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/csv/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1554 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/csv/decoder.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326997 xtalx-1.1.4/xtalx/tools/influxdb/
+-rw-r--r--   0 greent7    (502) staff       (20)       89 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/influxdb/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3405 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/influxdb/push_queue.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.327301 xtalx-1.1.4/xtalx/tools/math/
+-rw-r--r--   0 greent7    (502) staff       (20)      215 2023-11-16 00:10:23.000000 xtalx-1.1.4/xtalx/tools/math/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/math/lorentz.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2667 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/math/xy_series.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.328030 xtalx-1.1.4/xtalx/tools/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1597 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/csv_resample.py
+-rw-r--r--   0 greent7    (502) staff       (20)      520 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     8038 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/gl_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)      632 2024-04-03 23:28:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read.py
+-rw-r--r--   0 greent7    (502) staff       (20)      789 2024-04-03 23:28:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read_async.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2687 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_yield.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.328136 xtalx-1.1.4/xtalx/tools/usb/
+-rw-r--r--   0 greent7    (502) staff       (20)      977 2023-08-04 23:59:51.000000 xtalx-1.1.4/xtalx/tools/usb/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.329088 xtalx-1.1.4/xtalx/tools/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1086 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/cli_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)      476 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3166 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/get_info.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5345 2024-01-30 23:28:20.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_scope_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7231 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_sweep_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16101 2024-05-21 22:41:40.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10119 2024-05-23 05:44:38.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_wat_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7162 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/z_common.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.329958 xtalx-1.1.4/xtalx/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      976 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    11028 2024-05-23 05:43:44.000000 xtalx-1.1.4/xtalx/z_sensor/peak_tracker.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5448 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/z_sensor/predicate_queue.py
+-rw-r--r--   0 greent7    (502) staff       (20)      861 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/scope_data.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3588 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/sweeper.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21964 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/z_sensor/tcsc.py
+-rw-r--r--   0 greent7    (502) staff       (20)      205 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/tcsc_u5.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1819 2023-09-13 20:20:19.000000 xtalx-1.1.4/xtalx/z_sensor/tincan.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.330112 xtalx-1.1.4/xtalx.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     1398 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      434 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       87 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        6 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/top_level.txt
```

### Comparing `xtalx-1.1.3/LICENSE` & `xtalx-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/PKG-INFO` & `xtalx-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.1.3
+Version: 1.1.4
 Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: btype>=0.1.5
+Requires-Dist: glotlib>=0.9.6
+Requires-Dist: influxdb
+Requires-Dist: libusb_package>=1.0.26.2
+Requires-Dist: numpy
+Requires-Dist: pyusb>=1.2.1
+Requires-Dist: scipy
 
 xtalx
 =====
 This package provides a library for interfacing with the XtalX pressure and
 density/viscosity sensors.  Python version 3 is required.  The easiest way to
 install the xtalx module is using pip::
```

### Comparing `xtalx-1.1.3/README.rst` & `xtalx-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/setup.cfg` & `xtalx-1.1.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xtalx
-version = 1.1.3
+version = 1.1.4
 author = Phase Advanced Sensor Systems Corp.
 author_email = tgreeniaus@phasesensors.com
 description = Drivers and tools for the XtalX sensor family.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = xtalx
 url = https://github.com/phasesensors/xtalx_python
@@ -40,12 +40,13 @@
 console_scripts = 
 	xtalx_p_discover = xtalx.tools.p_sensor.discover:_main
 	xtalx_p_test = xtalx.tools.p_sensor.xtalx_test_yield:_main
 	xtalx_z_cli_track_mode = xtalx.tools.z_sensor.cli_track_mode:_main
 	xtalx_z_discover = xtalx.tools.z_sensor.discover:main
 	xtalx_z_get_info = xtalx.tools.z_sensor.get_info:_main
 	xtalx_z_gl_track_mode = xtalx.tools.z_sensor.gl_track_mode:_main
+	xtalx_z_gl_wat_mode = xtalx.tools.z_sensor.gl_wat_mode:_main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xtalx-1.1.3/xtalx/p_sensor/__init__.py` & `xtalx-1.1.4/xtalx/p_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/p_sensor/xti.py` & `xtalx-1.1.4/xtalx/p_sensor/xti.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/config/config.py` & `xtalx-1.1.4/xtalx/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/csv/decoder.py` & `xtalx-1.1.4/xtalx/tools/csv/decoder.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/influxdb/push_queue.py` & `xtalx-1.1.4/xtalx/tools/influxdb/push_queue.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/math/lorentz.py` & `xtalx-1.1.4/xtalx/tools/math/lorentz.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/math/xy_series.py` & `xtalx-1.1.4/xtalx/tools/math/xy_series.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/p_sensor/csv_resample.py` & `xtalx-1.1.4/xtalx/tools/p_sensor/csv_resample.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/p_sensor/discover.py` & `xtalx-1.1.4/xtalx/tools/p_sensor/discover.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/p_sensor/gl_track_mode.py` & `xtalx-1.1.4/xtalx/tools/p_sensor/gl_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/p_sensor/xtalx_test_read.py` & `xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read_async.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/p_sensor/xtalx_test_yield.py` & `xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_yield.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/usb/__init__.py` & `xtalx-1.1.4/xtalx/tools/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/cli_track_mode.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/cli_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/get_info.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/get_info.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/gl_scope_mode.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/gl_scope_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/gl_sweep_mode.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/gl_sweep_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/gl_track_mode.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/gl_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/tools/z_sensor/z_common.py` & `xtalx-1.1.4/xtalx/tools/z_sensor/z_common.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/__init__.py` & `xtalx-1.1.4/xtalx/z_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/peak_tracker.py` & `xtalx-1.1.4/xtalx/z_sensor/peak_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,38 +49,42 @@
     def sweep_callback(self, tc, pt, t0_ns, duration_ms, points, fw_fit, hires,
                        temp_freq):
         pass
 
 
 class PeakTracker:
     def __init__(self, tc, amplitude, f0, f1, search_df, nfreqs, search_time,
-                 sweep_time, settle_ms=2, delegate=Delegate()):
+                 sweep_time, settle_ms=2, delegate=Delegate(),
+                 enable_chirp=True):
         self.tc             = tc
         self.amplitude      = amplitude
         self.f0             = f0
         self.f1             = f1
         self.search_df      = search_df
         self.nfreqs         = nfreqs
         self.search_min_f   = min(f0, f1)
         self.search_max_f   = max(f0, f1)
         self.search_time    = search_time
         self.sweep_time     = sweep_time
         self.settle_ms      = settle_ms
         self.delegate       = delegate
+        self.enable_chirp   = enable_chirp
         self.thread         = None
         self.thread_cond    = threading.Condition()
         self.thread_exc     = None
 
+        self.start_time_ns  = None
         self.t_timeout      = None
         self.hires_f_center = None
         self.hires_width    = None
         self.min_rr         = None
         self.min_w          = None
         self.sensor_ms      = None
         self.sweep          = 0
+        self.sweep_iter     = None
         self.sweep_t0_ns    = None
         self.state          = State.IDLE
         self.chirp_space    = np.linspace(CHIRP_F0, CHIRP_F1,
                                           int(CHIRP_F1 - CHIRP_F0))
 
     def _transition(self, new_state):
         if self.state == new_state:
@@ -113,15 +117,18 @@
             self.tc.warn('FwFit failed: %s s status %d niter %d' %
                          (fit.dt / 1e9, fit.status, fit.niter))
             fit = None
 
         return fit
 
     def _start_full_search(self):
-        self._start_chirp()
+        if self.enable_chirp:
+            self._start_chirp()
+        else:
+            self._start_peak_search_defaults()
 
     def _start_chirp(self):
         '''
         Start chirping and refine the data as it comes in.
         '''
         self.tc.info('Chirping from %f to %f...' % (CHIRP_F0, CHIRP_F1))
         self.tc.send_auto_chirp_cmd(CHIRP_F0, CHIRP_F1,
@@ -194,14 +201,20 @@
         temp_freq = self._get_temp_freq()
         fw_fit    = self._get_sweep_fit(temp_freq)
         hires     = (self.state == State.HIRES_SWEEP_WAIT_DATA)
 
         t1_ns = time.time_ns()
         dt_ms = round((t1_ns - t0_ns) / 1000000)
 
+        if (hires and fw_fit is not None and fw_fit.RR >= self.min_rr and
+                15000 <= fw_fit.peak_hz <= 35000):
+            self.sweep_iter += 1
+        else:
+            self.sweep_iter = 0
+
         self.delegate.sweep_callback(self.tc, self, self.sweep_t0_ns,
                                      self.sensor_ms + dt_ms, points, fw_fit,
                                      hires, temp_freq)
         self.sweep += 1
 
         if self.state == State.IDLE:
             return
@@ -261,14 +274,15 @@
             self.tc.info('Chirp failed with RR = %.5f' % lf.RR)
         else:
             self.tc.info('Chirp failed with no fit.')
         self._start_peak_search_defaults()
 
     def start_async(self):
         assert self.state == State.IDLE
+        self.start_time_ns = time.time_ns()
         self._start_full_search()
 
     def stop_async(self):
         assert self.state != State.IDLE
         self.t_timeout = None
         self._transition(State.IDLE)
 
@@ -299,13 +313,14 @@
             self.thread_cond.notify()
         t.join()
 
     def _poll_threaded(self):
         try:
             with self.thread_cond:
                 if self.thread:
+                    self.start_time_ns = time.time_ns()
                     self._start_full_search()
                     while self.thread:
                         dt = self.poll()
                         self.thread_cond.wait(timeout=dt)
         except Exception as e:
             self.thread_exc = e
```

### Comparing `xtalx-1.1.3/xtalx/z_sensor/predicate_queue.py` & `xtalx-1.1.4/xtalx/z_sensor/predicate_queue.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/scope_data.py` & `xtalx-1.1.4/xtalx/z_sensor/scope_data.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/sweeper.py` & `xtalx-1.1.4/xtalx/z_sensor/sweeper.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/tcsc.py` & `xtalx-1.1.4/xtalx/z_sensor/tcsc.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx/z_sensor/tincan.py` & `xtalx-1.1.4/xtalx/z_sensor/tincan.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.3/xtalx.egg-info/PKG-INFO` & `xtalx-1.1.4/xtalx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.1.3
+Version: 1.1.4
 Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: btype>=0.1.5
+Requires-Dist: glotlib>=0.9.6
+Requires-Dist: influxdb
+Requires-Dist: libusb_package>=1.0.26.2
+Requires-Dist: numpy
+Requires-Dist: pyusb>=1.2.1
+Requires-Dist: scipy
 
 xtalx
 =====
 This package provides a library for interfacing with the XtalX pressure and
 density/viscosity sensors.  Python version 3 is required.  The easiest way to
 install the xtalx module is using pip::
```

### Comparing `xtalx-1.1.3/xtalx.egg-info/SOURCES.txt` & `xtalx-1.1.4/xtalx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 xtalx/tools/math/lorentz.py
 xtalx/tools/math/xy_series.py
 xtalx/tools/p_sensor/__init__.py
 xtalx/tools/p_sensor/csv_resample.py
 xtalx/tools/p_sensor/discover.py
 xtalx/tools/p_sensor/gl_track_mode.py
 xtalx/tools/p_sensor/xtalx_test_read.py
+xtalx/tools/p_sensor/xtalx_test_read_async.py
 xtalx/tools/p_sensor/xtalx_test_yield.py
 xtalx/tools/usb/__init__.py
 xtalx/tools/z_sensor/__init__.py
 xtalx/tools/z_sensor/cli_track_mode.py
 xtalx/tools/z_sensor/discover.py
 xtalx/tools/z_sensor/get_info.py
 xtalx/tools/z_sensor/gl_scope_mode.py
 xtalx/tools/z_sensor/gl_sweep_mode.py
 xtalx/tools/z_sensor/gl_track_mode.py
+xtalx/tools/z_sensor/gl_wat_mode.py
 xtalx/tools/z_sensor/z_common.py
 xtalx/z_sensor/__init__.py
 xtalx/z_sensor/peak_tracker.py
 xtalx/z_sensor/predicate_queue.py
 xtalx/z_sensor/scope_data.py
 xtalx/z_sensor/sweeper.py
 xtalx/z_sensor/tcsc.py
```

