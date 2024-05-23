# Comparing `tmp/pbx_cloud_utils-1.3.0-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.3.0a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7567 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 09:00 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    12094 b- defN 24-May-23 08:46 cloud_utils/aio_storage.py
--rw-r--r--  2.0 unx       57 b- defN 24-May-23 08:46 cloud_utils/const.py
--rw-r--r--  2.0 unx      284 b- defN 24-May-23 08:46 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx    10262 b- defN 24-May-23 08:46 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1365 b- defN 24-May-23 08:46 cloud_utils/types.py
--rw-r--r--  2.0 unx      346 b- defN 24-May-23 08:46 cloud_utils/utils.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-23 09:00 pbx_cloud_utils-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 09:00 pbx_cloud_utils-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-23 09:00 pbx_cloud_utils-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      879 b- defN 24-May-23 09:00 pbx_cloud_utils-1.3.0.dist-info/RECORD
-11 files, 25713 bytes uncompressed, 6077 bytes compressed:  76.4%
+Zip file size: 7589 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-May-15 07:01 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    12094 b- defN 24-May-15 06:42 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx       57 b- defN 24-May-14 09:38 cloud_utils/const.py
+-rw-r--r--  2.0 unx      284 b- defN 24-May-14 09:38 cloud_utils/exceptions.py
+-rw-r--r--  2.0 unx    10262 b- defN 24-May-15 06:57 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1365 b- defN 24-May-15 06:42 cloud_utils/types.py
+-rw-r--r--  2.0 unx      346 b- defN 24-May-14 09:38 cloud_utils/utils.py
+-rw-r--r--  2.0 unx      324 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/RECORD
+11 files, 25723 bytes uncompressed, 6083 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0.dist-info/METADATA
+Filename: pbx_cloud_utils-1.3.0a0.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.3.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.3.0a0.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0.dist-info/RECORD
+Filename: pbx_cloud_utils-1.3.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pbx_cloud_utils-1.3.0.dist-info/RECORD` & `pbx_cloud_utils-1.3.0a0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cloud_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cloud_utils/aio_storage.py,sha256=hTMYwaK2Bx64vQVUj1PFKXg_649-sOIy3PQnSRpuifE,12094
 cloud_utils/const.py,sha256=I0vJw5LuVCMJZK3ajhM1v2O85cpxnnirDG-scWyxeRE,57
 cloud_utils/exceptions.py,sha256=4TFl0EqL8X2vEgs4xpNgev93bDMcawfVc9DAty7SAqw,284
 cloud_utils/storage.py,sha256=BQy7Fk9_AeZSoTRp0g-9cClNAvxvXHldPBMNOV7s0r0,10262
 cloud_utils/types.py,sha256=o98xCZ9mwhjvvm2-CmGkgcEVbdj8wbZxwIgKICr2E08,1365
 cloud_utils/utils.py,sha256=gi__PPdP5YKxehoe9Az5lhAgN11sFxk3YLmHM0cxm1I,346
-pbx_cloud_utils-1.3.0.dist-info/METADATA,sha256=dWkyjJZOD2IPFmDfV4TgrR9KaThPHtaVEAAfbozkULU,322
-pbx_cloud_utils-1.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_cloud_utils-1.3.0.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
-pbx_cloud_utils-1.3.0.dist-info/RECORD,,
+pbx_cloud_utils-1.3.0a0.dist-info/METADATA,sha256=p_X04oWOMstSa5GBb5jW2JZUpobq_3zQgp6QEOZeifk,324
+pbx_cloud_utils-1.3.0a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_cloud_utils-1.3.0a0.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
+pbx_cloud_utils-1.3.0a0.dist-info/RECORD,,
```

