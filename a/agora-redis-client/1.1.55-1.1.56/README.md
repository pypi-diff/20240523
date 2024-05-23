# Comparing `tmp/agora_redis_client-1.1.55-py2.py3-none-any.whl.zip` & `tmp/agora_redis_client-1.1.56-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2851 bytes, number of entries: 7
+Zip file size: 2908 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       31 b- defN 23-Jun-14 11:28 agora_redis_client/__init__.py
--rw-r--r--  2.0 fat     1762 b- defN 23-Sep-06 12:54 agora_redis_client/redis_client.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:56 agora_redis_client/version.py
--rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.55.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.55.dist-info/WHEEL
--rw-r--r--  2.0 fat      877 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.55.dist-info/METADATA
--rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.55.dist-info/RECORD
-7 files, 3525 bytes uncompressed, 1771 bytes compressed:  49.8%
+-rw-r--r--  2.0 fat     1765 b- defN 24-May-23 11:39 agora_redis_client/redis_client.py
+-rw-r--r--  2.0 fat       25 b- defN 24-May-23 11:47 agora_redis_client/version.py
+-rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.56.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.56.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1008 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.56.dist-info/METADATA
+-rw-r--r--  2.0 fat      601 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.56.dist-info/RECORD
+7 files, 3660 bytes uncompressed, 1828 bytes compressed:  50.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: agora_redis_client/redis_client.py
 Comment: 
 
 Filename: agora_redis_client/version.py
 Comment: 
 
-Filename: agora_redis_client-1.1.55.dist-info/LICENSE
+Filename: agora_redis_client-1.1.56.dist-info/LICENSE
 Comment: 
 
-Filename: agora_redis_client-1.1.55.dist-info/WHEEL
+Filename: agora_redis_client-1.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: agora_redis_client-1.1.55.dist-info/METADATA
+Filename: agora_redis_client-1.1.56.dist-info/METADATA
 Comment: 
 
-Filename: agora_redis_client-1.1.55.dist-info/RECORD
+Filename: agora_redis_client-1.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_redis_client/redis_client.py

```diff
@@ -26,15 +26,15 @@
         Use 'AEA2:RedisClient:Server' to set the server address (default = 'redis').
         Use 'AEA2:RedisClient:Port' to set the port (default = 6379).
         
         When running on gateway, the default values are appropriate.
         '''
         server = config["AEA2:RedisClient:Server"]
         if server == "":
-            server = "localhost"
+            server = "alpine-redis"
 
         port = config["AEA2:RedisClient:Port"]
         if port == "":
             port = "6379"  
 
         logger.info(f"redis_client connecting to '{server}:{port}'")
         self.connect_attempted = True
```

## agora_redis_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.55'
+__version__ = '1.1.56'
```

## Comparing `agora_redis_client-1.1.55.dist-info/METADATA` & `agora_redis_client-1.1.56.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: agora_redis_client
-Version: 1.1.55
+Version: 1.1.56
 Summary: Redis Client for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.55
-Requires-Dist: agora_config == 1.1.55
+Requires-Dist: agora_logging == 1.1.56
+Requires-Dist: agora_config == 1.1.56
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_redisclient
 
 This package is the Redis Client for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.56
+- Fix bug to set the default redis server to be the redis container name on the gateway if not found in the AEA.json 
+
 ### v1.1.53
 - Make versions of all modules the same
 
 ### v1.0.26
 
 - Initial Version of Redis Client
```

## Comparing `agora_redis_client-1.1.55.dist-info/RECORD` & `agora_redis_client-1.1.56.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 agora_redis_client/__init__.py,sha256=nIxsBty2jHDz3mqsvyOPRhUZoo6FtNNvfkNph7C4F4U,31
-agora_redis_client/redis_client.py,sha256=S7Zp_dZwL5M3914b0dLflTMTbidb5bYMyfJnkD0UHQ4,1762
-agora_redis_client/version.py,sha256=UIT0aCiTGWEy2qWr4VqukZwUGe31Qh5aJKvW2JtVB1w,25
-agora_redis_client-1.1.55.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
-agora_redis_client-1.1.55.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_redis_client-1.1.55.dist-info/METADATA,sha256=Bx-BCOiAS4VGVlxbZ1kB5hnj_wWHXlV5-lYX5h26G6Q,877
-agora_redis_client-1.1.55.dist-info/RECORD,,
+agora_redis_client/redis_client.py,sha256=pmkKJYaHcTwe-aB1Lzf74vNsOftXzuHwqXLGZz_u-zE,1765
+agora_redis_client/version.py,sha256=g_qoTW7pb6iFGwl3C82jYosDdc0alpL93p9gCljatF0,25
+agora_redis_client-1.1.56.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
+agora_redis_client-1.1.56.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_redis_client-1.1.56.dist-info/METADATA,sha256=qnahdzem5oCaZA9ff3Hf6n9JOtn1SISSZ4yj5i6OoE4,1008
+agora_redis_client-1.1.56.dist-info/RECORD,,
```

