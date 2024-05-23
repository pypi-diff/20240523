# Comparing `tmp/agoraiot-1.1.55-py2.py3-none-any.whl.zip` & `tmp/agoraiot-1.1.56-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2094 bytes, number of entries: 6
+Zip file size: 2155 bytes, number of entries: 6
 -rw-r--r--  2.0 fat      387 b- defN 24-May-14 10:46 agoraiot/__init__.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:56 agoraiot/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.55.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.55.dist-info/WHEEL
--rw-r--r--  2.0 fat     1061 b- defN 16-Jan-01 00:00 agoraiot-1.1.55.dist-info/METADATA
--rw-r--r--  2.0 fat      451 b- defN 16-Jan-01 00:00 agoraiot-1.1.55.dist-info/RECORD
-6 files, 2157 bytes uncompressed, 1278 bytes compressed:  40.8%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-23 11:47 agoraiot/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.56.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.56.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1192 b- defN 16-Jan-01 00:00 agoraiot-1.1.56.dist-info/METADATA
+-rw-r--r--  2.0 fat      451 b- defN 16-Jan-01 00:00 agoraiot-1.1.56.dist-info/RECORD
+6 files, 2288 bytes uncompressed, 1339 bytes compressed:  41.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: agoraiot/__init__.py
 Comment: 
 
 Filename: agoraiot/version.py
 Comment: 
 
-Filename: agoraiot-1.1.55.dist-info/LICENSE
+Filename: agoraiot-1.1.56.dist-info/LICENSE
 Comment: 
 
-Filename: agoraiot-1.1.55.dist-info/WHEEL
+Filename: agoraiot-1.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: agoraiot-1.1.55.dist-info/METADATA
+Filename: agoraiot-1.1.56.dist-info/METADATA
 Comment: 
 
-Filename: agoraiot-1.1.55.dist-info/RECORD
+Filename: agoraiot-1.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agoraiot/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.55'
+__version__ = '1.1.56'
```

## Comparing `agoraiot-1.1.55.dist-info/METADATA` & `agoraiot-1.1.56.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: agoraiot
-Version: 1.1.55
+Version: 1.1.56
 Summary: AgoraIoT Python Libraries
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.55
-Requires-Dist: agora_busclient == 1.1.55
-Requires-Dist: agora_config == 1.1.55
-Requires-Dist: agora_redis_client == 1.1.55
-Requires-Dist: agora_twin_property == 1.1.55
-Requires-Dist: agora_utils == 1.1.55
+Requires-Dist: agora_logging == 1.1.56
+Requires-Dist: agora_busclient == 1.1.56
+Requires-Dist: agora_config == 1.1.56
+Requires-Dist: agora_redis_client == 1.1.56
+Requires-Dist: agora_twin_property == 1.1.56
+Requires-Dist: agora_utils == 1.1.56
 Project-URL: Documentation, https://agoraiot.github.io
 Project-URL: Home, https://www.agoraiot.com
 
 # agoraiot
 
 This primary package for the entire Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.56
+- Fix bug to set the default redis server to be the redis container name on the gateway if not found in the AEA.json 
+
 ### v1.1.53
 - Added Twin Property Module
 
 ### v1.0.18
 
 - Make versions of all modules the same
```

