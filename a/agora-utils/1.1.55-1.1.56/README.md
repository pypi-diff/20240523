# Comparing `tmp/agora_utils-1.1.55-py2.py3-none-any.whl.zip` & `tmp/agora_utils-1.1.56-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2573 bytes, number of entries: 8
+Zip file size: 2633 bytes, number of entries: 8
 -rw-r--r--  2.0 fat       75 b- defN 23-May-12 13:38 agora_utils/__init__.py
 -rw-r--r--  2.0 fat       23 b- defN 23-May-12 13:38 agora_utils/_version.py
 -rw-r--r--  2.0 fat      521 b- defN 23-Jul-27 17:24 agora_utils/agora_time.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:55 agora_utils/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.55.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.55.dist-info/WHEEL
--rw-r--r--  2.0 fat      933 b- defN 16-Jan-01 00:00 agora_utils-1.1.55.dist-info/METADATA
--rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.55.dist-info/RECORD
-8 files, 2436 bytes uncompressed, 1473 bytes compressed:  39.5%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-23 11:47 agora_utils/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.56.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.56.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1064 b- defN 16-Jan-01 00:00 agora_utils-1.1.56.dist-info/METADATA
+-rw-r--r--  2.0 fat      627 b- defN 16-Jan-01 00:00 agora_utils-1.1.56.dist-info/RECORD
+8 files, 2568 bytes uncompressed, 1533 bytes compressed:  40.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: agora_utils/agora_time.py
 Comment: 
 
 Filename: agora_utils/version.py
 Comment: 
 
-Filename: agora_utils-1.1.55.dist-info/LICENSE
+Filename: agora_utils-1.1.56.dist-info/LICENSE
 Comment: 
 
-Filename: agora_utils-1.1.55.dist-info/WHEEL
+Filename: agora_utils-1.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: agora_utils-1.1.55.dist-info/METADATA
+Filename: agora_utils-1.1.56.dist-info/METADATA
 Comment: 
 
-Filename: agora_utils-1.1.55.dist-info/RECORD
+Filename: agora_utils-1.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_utils/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.55'
+__version__ = '1.1.56'
```

## Comparing `agora_utils-1.1.55.dist-info/METADATA` & `agora_utils-1.1.56.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agora_utils
-Version: 1.1.55
+Version: 1.1.56
 Summary: Utilities libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
 
 
@@ -12,14 +12,17 @@
 
 This package is the Utilities library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.56
+- Fix bug to set the default redis server to be the redis container name on the gateway if not found in the AEA.json 
+
 ### v1.1.53
 - Make versions of all modules the same
 
 ### v1.0.18
 
 - Make versions of all modules all the same
 - Add ability to Mock (AEA2:BusClient:Mock (True/False)) the BusClient
```

## Comparing `agora_utils-1.1.55.dist-info/RECORD` & `agora_utils-1.1.56.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 agora_utils/__init__.py,sha256=bMi6zdciwSmg3ZDZCOfzQCUHMYaxcHk1GvAL_i2zh0s,75
 agora_utils/_version.py,sha256=kwEyWwKLIIqYSnkf5eXgPtRgw9Bz51riSupwtvDpJMA,23
 agora_utils/agora_time.py,sha256=3vMrPf5MGRQdXqqXxLEwcAv-jH1jcctgeEU-Nbo0d4Q,521
-agora_utils/version.py,sha256=UIT0aCiTGWEy2qWr4VqukZwUGe31Qh5aJKvW2JtVB1w,25
-agora_utils-1.1.55.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_utils-1.1.55.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_utils-1.1.55.dist-info/METADATA,sha256=oaofXdT5bMixvApD_i2Kp8eBvEsv4yPLoRBt4cym72c,933
-agora_utils-1.1.55.dist-info/RECORD,,
+agora_utils/version.py,sha256=g_qoTW7pb6iFGwl3C82jYosDdc0alpL93p9gCljatF0,25
+agora_utils-1.1.56.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_utils-1.1.56.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_utils-1.1.56.dist-info/METADATA,sha256=A4vJx-1r7ZoOI3_fJf5eZxVKGxVv8thrN6uLADd3iVU,1064
+agora_utils-1.1.56.dist-info/RECORD,,
```

