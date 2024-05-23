# Comparing `tmp/tconnectsync-0.9.5.tar.gz` & `tmp/tconnectsync-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tconnectsync-0.9.5.tar", last modified: Sun Oct  1 00:51:31 2023, max compression
+gzip compressed data, was "tconnectsync-0.9.7.tar", last modified: Thu May 23 06:09:19 2024, max compression
```

## Comparing `tconnectsync-0.9.5.tar` & `tconnectsync-0.9.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.088110 tconnectsync-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    23851 2023-10-01 00:51:31.088110 tconnectsync-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23200 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-10-01 00:51:31.088110 tconnectsync-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/android.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/controliq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/webui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/api/ws2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/domain/bolus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/domain/device_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/domain/therapy_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/domain/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/nightscout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/parser/ciq_therapy_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/parser/nightscout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/parser/tconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/basal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/bolus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/cgm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/iob.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/sync/pump_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.084109 tconnectsync-0.9.5/tconnectsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tconnectsync/util/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.088110 tconnectsync-0.9.5/tconnectsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23851 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-01 00:51:31.000000 tconnectsync-0.9.5/tconnectsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 00:51:31.088110 tconnectsync-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15111 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tests/test_autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    41692 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-10-01 00:51:18.000000 tconnectsync-0.9.5/tests/test_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23314 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.412083 tconnectsync-0.9.7/tconnectsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.412083 tconnectsync-0.9.7/tconnectsync/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/controliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/webui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/api/ws2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.412083 tconnectsync-0.9.7/tconnectsync/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/domain/bolus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/domain/device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/domain/therapy_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/domain/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/nightscout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.412083 tconnectsync-0.9.7/tconnectsync/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/parser/ciq_therapy_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/parser/nightscout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/parser/tconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/tconnectsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/basal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/bolus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/cgm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/iob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/sync/pump_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/tconnectsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tconnectsync/util/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/tconnectsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 06:09:19.000000 tconnectsync-0.9.7/tconnectsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:09:19.416083 tconnectsync-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tests/test_autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41692 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-23 06:09:15.000000 tconnectsync-0.9.7/tests/test_secret.py
```

### Comparing `tconnectsync-0.9.5/LICENSE.md` & `tconnectsync-0.9.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/PKG-INFO` & `tconnectsync-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tconnectsync
-Version: 0.9.5
+Version: 0.9.7
 Summary: Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 Home-page: https://github.com/jwoglom/tconnectsync
 Author: James Woglom
 Author-email: j@wogloms.net
 Project-URL: Bug Tracker, https://github.com/jwoglom/tconnectsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,15 +71,15 @@
   * Site/Cartridge Change (occurs for both a site change and a cartridge change)
   * Empty Cartridge/Pump Shutdown (from my investigation, occurs either when the cartridge runs out of insulin OR you hard-shut off the pump)
   * User Suspended (occurs when you manually disable insulin delivery)
   * Exercise Mode (in Nightscout, appears with a start and end time)
   * Sleep Mode (in Nightscout, appears with a start and end time)
 * `IOB`: Insulin-on-board data. Only the most recent IOB entry is saved to Nightscout, as an "activity". The Nightscout UI does not currently display this information. In order to read this value, you need to query the Nightscout activity API endpoint. If you don't know what that means, then there is no reason to enable this option.
 
-The following synchronization features are under development, [**but are not yet ready for use**](https://github.com/jwoglom/tconnectsync/issues/16):
+The following synchronization features are considered to be in alpha, and haven't been widely tested. If you want to use them, [set `ENABLE_TESTING_MODES=true` for them to show up](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/features.py#L29):
 * `BOLUS_BG`: Adds BG readings which are associated with boluses on the pump into the Nightscout treatment object. It will determine whether the BG reading was automatically filled via the Dexcom connection on the pump or was manually entered by seeing if the BG reading matches the current CGM reading as known to the pump at that time. Support for this is nearly complete.
 * `CGM`: Adds Dexcom CGM readings from the pump to Nightscout as SGV (sensor glucose value) entries. This should only be used in a situation where xDrip/Dexcom Share/etc. is not used and the pump connection to the CGM will be the only source of CGM data to Nightscout. This requires additional testing before it should be considered ready.
 
 To specify custom synchronization features, pass the names of the desired features to the `--features` flag, e.g.:
 
 ```bash
 $ tconnectsync --features BASAL BOLUS PUMP_EVENTS PROFILES
```

### Comparing `tconnectsync-0.9.5/README.md` & `tconnectsync-0.9.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   * Site/Cartridge Change (occurs for both a site change and a cartridge change)
   * Empty Cartridge/Pump Shutdown (from my investigation, occurs either when the cartridge runs out of insulin OR you hard-shut off the pump)
   * User Suspended (occurs when you manually disable insulin delivery)
   * Exercise Mode (in Nightscout, appears with a start and end time)
   * Sleep Mode (in Nightscout, appears with a start and end time)
 * `IOB`: Insulin-on-board data. Only the most recent IOB entry is saved to Nightscout, as an "activity". The Nightscout UI does not currently display this information. In order to read this value, you need to query the Nightscout activity API endpoint. If you don't know what that means, then there is no reason to enable this option.
 
-The following synchronization features are under development, [**but are not yet ready for use**](https://github.com/jwoglom/tconnectsync/issues/16):
+The following synchronization features are considered to be in alpha, and haven't been widely tested. If you want to use them, [set `ENABLE_TESTING_MODES=true` for them to show up](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/features.py#L29):
 * `BOLUS_BG`: Adds BG readings which are associated with boluses on the pump into the Nightscout treatment object. It will determine whether the BG reading was automatically filled via the Dexcom connection on the pump or was manually entered by seeing if the BG reading matches the current CGM reading as known to the pump at that time. Support for this is nearly complete.
 * `CGM`: Adds Dexcom CGM readings from the pump to Nightscout as SGV (sensor glucose value) entries. This should only be used in a situation where xDrip/Dexcom Share/etc. is not used and the pump connection to the CGM will be the only source of CGM data to Nightscout. This requires additional testing before it should be considered ready.
 
 To specify custom synchronization features, pass the names of the desired features to the `--features` flag, e.g.:
 
 ```bash
 $ tconnectsync --features BASAL BOLUS PUMP_EVENTS PROFILES
```

### Comparing `tconnectsync-0.9.5/setup.cfg` & `tconnectsync-0.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tconnectsync
-version = 0.9.5
+version = 0.9.7
 author = James Woglom
 author_email = j@wogloms.net
 description = Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jwoglom/tconnectsync
 project_urls =
```

### Comparing `tconnectsync-0.9.5/tconnectsync/__init__.py` & `tconnectsync-0.9.7/tconnectsync/__init__.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/__init__.py` & `tconnectsync-0.9.7/tconnectsync/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/android.py` & `tconnectsync-0.9.7/tconnectsync/api/android.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/common.py` & `tconnectsync-0.9.7/tconnectsync/api/common.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/controliq.py` & `tconnectsync-0.9.7/tconnectsync/api/controliq.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/webui.py` & `tconnectsync-0.9.7/tconnectsync/api/webui.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/api/ws2.py` & `tconnectsync-0.9.7/tconnectsync/api/ws2.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/autoupdate.py` & `tconnectsync-0.9.7/tconnectsync/autoupdate.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/check.py` & `tconnectsync-0.9.7/tconnectsync/check.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/domain/bolus.py` & `tconnectsync-0.9.7/tconnectsync/domain/bolus.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/domain/device_settings.py` & `tconnectsync-0.9.7/tconnectsync/domain/device_settings.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/domain/therapy_event.py` & `tconnectsync-0.9.7/tconnectsync/domain/therapy_event.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/domain/utility.py` & `tconnectsync-0.9.7/tconnectsync/domain/utility.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/features.py` & `tconnectsync-0.9.7/tconnectsync/features.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/nightscout.py` & `tconnectsync-0.9.7/tconnectsync/nightscout.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/parser/ciq_therapy_events.py` & `tconnectsync-0.9.7/tconnectsync/parser/ciq_therapy_events.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/parser/nightscout.py` & `tconnectsync-0.9.7/tconnectsync/parser/nightscout.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/parser/tconnect.py` & `tconnectsync-0.9.7/tconnectsync/parser/tconnect.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/process.py` & `tconnectsync-0.9.7/tconnectsync/process.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/secret.py` & `tconnectsync-0.9.7/tconnectsync/secret.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/basal.py` & `tconnectsync-0.9.7/tconnectsync/sync/basal.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/bolus.py` & `tconnectsync-0.9.7/tconnectsync/sync/bolus.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/cgm.py` & `tconnectsync-0.9.7/tconnectsync/sync/cgm.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/iob.py` & `tconnectsync-0.9.7/tconnectsync/sync/iob.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/profile.py` & `tconnectsync-0.9.7/tconnectsync/sync/profile.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/sync/pump_events.py` & `tconnectsync-0.9.7/tconnectsync/sync/pump_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,19 +188,19 @@
     if SKIP_NS_LAST_UPLOADED_CHECK:
         logger.warning("Overriding last upload check")
         last_upload = None
         last_upload_time = None
 
     add_count = 0
     for event in events:
-        created_at = event["time"]
-        if last_upload_time and arrow.get(created_at) <= last_upload_time:
+        created_at = arrow.get(event["time"])
+        if last_upload_time and created_at <= last_upload_time:
             skip = True
             if "duration_mins" in event.keys() and "duration" in last_upload.keys():
-                if created_at == last_upload["created_at"] and float(event["duration_mins"]) > float(last_upload["duration"]):
+                if created_at == arrow.get(last_upload["created_at"]) and float(event["duration_mins"]) > float(last_upload["duration"]):
                     logger.info("Latest %s event needs updating: duration has increased from %s to %s: %s" % (eventType, last_upload["duration"], event["duration_mins"], event))
                     logger.info("Deleting previous %s: %s" % (eventType, last_upload))
                     nightscout.delete_entry('treatments/%s' % last_upload["_id"])
                     skip = False
             
             if skip:
                 if pretend:
```

### Comparing `tconnectsync-0.9.5/tconnectsync/util/__init__.py` & `tconnectsync-0.9.7/tconnectsync/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync/util/cli.py` & `tconnectsync-0.9.7/tconnectsync/util/cli.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tconnectsync.egg-info/PKG-INFO` & `tconnectsync-0.9.7/tconnectsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tconnectsync
-Version: 0.9.5
+Version: 0.9.7
 Summary: Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 Home-page: https://github.com/jwoglom/tconnectsync
 Author: James Woglom
 Author-email: j@wogloms.net
 Project-URL: Bug Tracker, https://github.com/jwoglom/tconnectsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,15 +71,15 @@
   * Site/Cartridge Change (occurs for both a site change and a cartridge change)
   * Empty Cartridge/Pump Shutdown (from my investigation, occurs either when the cartridge runs out of insulin OR you hard-shut off the pump)
   * User Suspended (occurs when you manually disable insulin delivery)
   * Exercise Mode (in Nightscout, appears with a start and end time)
   * Sleep Mode (in Nightscout, appears with a start and end time)
 * `IOB`: Insulin-on-board data. Only the most recent IOB entry is saved to Nightscout, as an "activity". The Nightscout UI does not currently display this information. In order to read this value, you need to query the Nightscout activity API endpoint. If you don't know what that means, then there is no reason to enable this option.
 
-The following synchronization features are under development, [**but are not yet ready for use**](https://github.com/jwoglom/tconnectsync/issues/16):
+The following synchronization features are considered to be in alpha, and haven't been widely tested. If you want to use them, [set `ENABLE_TESTING_MODES=true` for them to show up](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/features.py#L29):
 * `BOLUS_BG`: Adds BG readings which are associated with boluses on the pump into the Nightscout treatment object. It will determine whether the BG reading was automatically filled via the Dexcom connection on the pump or was manually entered by seeing if the BG reading matches the current CGM reading as known to the pump at that time. Support for this is nearly complete.
 * `CGM`: Adds Dexcom CGM readings from the pump to Nightscout as SGV (sensor glucose value) entries. This should only be used in a situation where xDrip/Dexcom Share/etc. is not used and the pump connection to the CGM will be the only source of CGM data to Nightscout. This requires additional testing before it should be considered ready.
 
 To specify custom synchronization features, pass the names of the desired features to the `--features` flag, e.g.:
 
 ```bash
 $ tconnectsync --features BASAL BOLUS PUMP_EVENTS PROFILES
```

### Comparing `tconnectsync-0.9.5/tconnectsync.egg-info/SOURCES.txt` & `tconnectsync-0.9.7/tconnectsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tests/test_autoupdate.py` & `tconnectsync-0.9.7/tests/test_autoupdate.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tests/test_process.py` & `tconnectsync-0.9.7/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.5/tests/test_secret.py` & `tconnectsync-0.9.7/tests/test_secret.py`

 * *Files identical despite different names*

