# Comparing `tmp/agora_logging-1.1.55-py2.py3-none-any.whl.zip` & `tmp/agora_logging-1.1.56-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6584 bytes, number of entries: 12
+Zip file size: 6647 bytes, number of entries: 12
 -rw-r--r--  2.0 fat       67 b- defN 23-May-29 15:17 agora_logging/__init__.py
 -rw-r--r--  2.0 fat     5690 b- defN 24-Apr-23 15:18 agora_logging/agora_logger.py
 -rw-r--r--  2.0 fat     1612 b- defN 23-May-12 13:38 agora_logging/colored_text.py
 -rw-r--r--  2.0 fat      972 b- defN 23-Sep-06 12:54 agora_logging/log_level.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:55 agora_logging/version.py
+-rw-r--r--  2.0 fat       25 b- defN 24-May-23 11:47 agora_logging/version.py
 -rw-r--r--  2.0 fat        0 b- defN 23-May-12 13:38 agora_logging/handlers/__init__.py
 -rw-r--r--  2.0 fat     2963 b- defN 24-Apr-23 15:18 agora_logging/handlers/base_handler.py
 -rw-r--r--  2.0 fat      847 b- defN 24-Jan-19 19:27 agora_logging/handlers/stream_handler.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_logging-1.1.55.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.1.55.dist-info/WHEEL
--rw-r--r--  2.0 fat      951 b- defN 16-Jan-01 00:00 agora_logging-1.1.55.dist-info/METADATA
--rw-r--r--  2.0 fat     1012 b- defN 16-Jan-01 00:00 agora_logging-1.1.55.dist-info/RECORD
-12 files, 14372 bytes uncompressed, 4860 bytes compressed:  66.2%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_logging-1.1.56.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.1.56.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1083 b- defN 16-Jan-01 00:00 agora_logging-1.1.56.dist-info/METADATA
+-rw-r--r--  2.0 fat     1013 b- defN 16-Jan-01 00:00 agora_logging-1.1.56.dist-info/RECORD
+12 files, 14505 bytes uncompressed, 4923 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: agora_logging/handlers/base_handler.py
 Comment: 
 
 Filename: agora_logging/handlers/stream_handler.py
 Comment: 
 
-Filename: agora_logging-1.1.55.dist-info/LICENSE
+Filename: agora_logging-1.1.56.dist-info/LICENSE
 Comment: 
 
-Filename: agora_logging-1.1.55.dist-info/WHEEL
+Filename: agora_logging-1.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: agora_logging-1.1.55.dist-info/METADATA
+Filename: agora_logging-1.1.56.dist-info/METADATA
 Comment: 
 
-Filename: agora_logging-1.1.55.dist-info/RECORD
+Filename: agora_logging-1.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_logging/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.55'
+__version__ = '1.1.56'
```

## Comparing `agora_logging-1.1.55.dist-info/METADATA` & `agora_logging-1.1.56.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agora_logging
-Version: 1.1.55
+Version: 1.1.56
 Summary: Logging libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
 
 
@@ -12,14 +12,17 @@
 
 This package is the Logging library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.56
+- Fix bug to set the default redis server to be the redis container name on the gateway if not found in the AEA.json s
+
 ### v1.1.53
 - Make versions of all modules the same
 
 ### v1.0.20
 
 - Fix message about Verbosity instead of LogLevel
 - Force flush of sys.stdout when writing exception logs
```

## Comparing `agora_logging-1.1.55.dist-info/RECORD` & `agora_logging-1.1.56.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 agora_logging/__init__.py,sha256=PPi6BVmhWVjdeOMQYg-FEj51McSHrNif9p05X9otteo,67
 agora_logging/agora_logger.py,sha256=ts2EvkAO79Y9LREQjqycuIO0fxmDV-eLvRUqvgV3pzs,5690
 agora_logging/colored_text.py,sha256=EpksqRhjUz1clYH4YZWqnYUAvbSaETtJya6PxFZAat0,1612
 agora_logging/log_level.py,sha256=BR5UwX1pFgy2zt_RzpWA5G0ZnUX7SWq8-Is_MesCU9s,972
-agora_logging/version.py,sha256=UIT0aCiTGWEy2qWr4VqukZwUGe31Qh5aJKvW2JtVB1w,25
+agora_logging/version.py,sha256=g_qoTW7pb6iFGwl3C82jYosDdc0alpL93p9gCljatF0,25
 agora_logging/handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 agora_logging/handlers/base_handler.py,sha256=U-sSiYApP4w7wLDCqRE007yiYxN50DD3vlsByIaWqyI,2963
 agora_logging/handlers/stream_handler.py,sha256=i9K3FHCbzJY2kJstfggb2K1S2pGtJa1wkNlnr0L_SyQ,847
-agora_logging-1.1.55.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_logging-1.1.55.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_logging-1.1.55.dist-info/METADATA,sha256=L9WN6ec2RFMtAMRNCyVVzEWbYdUB9BFyCgjcCypMpA0,951
-agora_logging-1.1.55.dist-info/RECORD,,
+agora_logging-1.1.56.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_logging-1.1.56.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_logging-1.1.56.dist-info/METADATA,sha256=BCfGHDOdLsSKOPrC1_bdxpOVEKuli29BFmH5ekDoBUE,1083
+agora_logging-1.1.56.dist-info/RECORD,,
```

