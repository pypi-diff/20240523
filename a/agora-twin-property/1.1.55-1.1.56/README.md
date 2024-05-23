# Comparing `tmp/agora_twin_property-1.1.55-py2.py3-none-any.whl.zip` & `tmp/agora_twin_property-1.1.56-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4838 bytes, number of entries: 8
+Zip file size: 4895 bytes, number of entries: 8
 -rw-r--r--  2.0 fat       31 b- defN 24-May-13 16:50 agora_twin_property/__init__.py
 -rw-r--r--  2.0 fat     7931 b- defN 24-May-13 16:50 agora_twin_property/twin_property.py
 -rw-r--r--  2.0 fat     2092 b- defN 24-May-13 16:50 agora_twin_property/twin_property_observer.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:56 agora_twin_property/version.py
--rw-r--r--  2.0 fat      131 b- defN 24-May-13 16:50 agora_twin_property-1.1.55.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.55.dist-info/WHEEL
--rw-r--r--  2.0 fat      893 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.55.dist-info/METADATA
--rw-r--r--  2.0 fat      710 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.55.dist-info/RECORD
-8 files, 11912 bytes uncompressed, 3576 bytes compressed:  70.0%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-23 11:47 agora_twin_property/version.py
+-rw-r--r--  2.0 fat      131 b- defN 24-May-13 16:50 agora_twin_property-1.1.56.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.56.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1024 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.56.dist-info/METADATA
+-rw-r--r--  2.0 fat      711 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.56.dist-info/RECORD
+8 files, 12044 bytes uncompressed, 3633 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: agora_twin_property/twin_property_observer.py
 Comment: 
 
 Filename: agora_twin_property/version.py
 Comment: 
 
-Filename: agora_twin_property-1.1.55.dist-info/LICENSE
+Filename: agora_twin_property-1.1.56.dist-info/LICENSE
 Comment: 
 
-Filename: agora_twin_property-1.1.55.dist-info/WHEEL
+Filename: agora_twin_property-1.1.56.dist-info/WHEEL
 Comment: 
 
-Filename: agora_twin_property-1.1.55.dist-info/METADATA
+Filename: agora_twin_property-1.1.56.dist-info/METADATA
 Comment: 
 
-Filename: agora_twin_property-1.1.55.dist-info/RECORD
+Filename: agora_twin_property-1.1.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_twin_property/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.55'
+__version__ = '1.1.56'
```

## Comparing `agora_twin_property-1.1.55.dist-info/METADATA` & `agora_twin_property-1.1.56.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: agora_twin_property
-Version: 1.1.55
+Version: 1.1.56
 Summary: Agora twin property for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.55
-Requires-Dist: agora_config == 1.1.55
+Requires-Dist: agora_logging == 1.1.56
+Requires-Dist: agora_config == 1.1.56
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_twin_property
 
 This package is the twin property library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.56
+- Fix bug to set the default redis server to be the redis container name on the gateway if not found in the AEA.json 
+
 ### v1.1.53
 - Make versions of all modules the same
 
 ### v1.0.46 - Beta
 
 - Initial test release.
```

## Comparing `agora_twin_property-1.1.55.dist-info/RECORD` & `agora_twin_property-1.1.56.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 agora_twin_property/__init__.py,sha256=cfx1i4EcSLR_i010IftPW73I12U1Ylp47mMvf6V3Hls,31
 agora_twin_property/twin_property.py,sha256=csRc76zHV5qiRj39xWh9LjM5cJJ_IahCHB5iK38SfKs,7931
 agora_twin_property/twin_property_observer.py,sha256=JFROy3CKAi0N5BG46q4kSlOiSH02B_THTL6VGbnhp-w,2092
-agora_twin_property/version.py,sha256=UIT0aCiTGWEy2qWr4VqukZwUGe31Qh5aJKvW2JtVB1w,25
-agora_twin_property-1.1.55.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
-agora_twin_property-1.1.55.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_twin_property-1.1.55.dist-info/METADATA,sha256=oUQFmpHrW2aomZO42cOV3TiAY1swrscUPfsRLy-MHZo,893
-agora_twin_property-1.1.55.dist-info/RECORD,,
+agora_twin_property/version.py,sha256=g_qoTW7pb6iFGwl3C82jYosDdc0alpL93p9gCljatF0,25
+agora_twin_property-1.1.56.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
+agora_twin_property-1.1.56.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_twin_property-1.1.56.dist-info/METADATA,sha256=_oQNH2pzRKp-00FporyYJjQHGJd0S1fmPCoLpIXYcBE,1024
+agora_twin_property-1.1.56.dist-info/RECORD,,
```

