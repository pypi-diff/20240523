# Comparing `tmp/FSV-1.0.8-py3-none-any.whl.zip` & `tmp/FSV-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 173454 bytes, number of entries: 29
+Zip file size: 173453 bytes, number of entries: 29
 -rw-rw-r--  2.0 unx     8399 b- defN 23-Oct-30 11:23 FSV/Calculator.py
 -rw-rw-r--  2.0 unx      804 b- defN 23-Oct-23 11:13 FSV/Molecule.py
--rw-rw-r--  2.0 unx    53900 b- defN 23-Oct-25 10:23 FSV/Results.py
+-rw-rw-r--  2.0 unx    53900 b- defN 23-Nov-06 08:17 FSV/Results.py
 -rw-rw-r--  2.0 unx     3334 b- defN 23-Oct-23 11:13 FSV/Strain_energy.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Oct-23 11:13 FSV/__init__.py
 -rw-rw-r--  2.0 unx    31571 b- defN 23-Oct-25 08:52 FSV/basis_functions.py
 -rw-rw-r--  2.0 unx    19569 b- defN 23-Oct-27 06:08 FSV/fragmentation.py
 -rw-rw-r--  2.0 unx    15452 b- defN 23-Oct-23 11:13 FSV/inputs.py
 -rw-rw-r--  2.0 unx    73960 b- defN 23-Oct-23 08:08 FSV/lib/ONIOM_Cscale.txt
 -rwxrwxr-x  2.0 unx    73960 b- defN 23-Oct-23 08:08 FSV/lib/ONIOM_Hscale.txt
@@ -19,13 +19,13 @@
 -rw-rw-r--  2.0 unx    27699 b- defN 23-Oct-23 08:08 OBSV/basis_functions.py
 -rw-rw-r--  2.0 unx    19574 b- defN 23-Oct-23 08:08 OBSV/fragmentation.py
 -rw-rw-r--  2.0 unx    14179 b- defN 23-Oct-23 08:08 OBSV/inputs.py
 -rw-rw-r--  2.0 unx    73960 b- defN 23-Oct-23 08:08 OBSV/lib/ONIOM_Cscale.txt
 -rwxrwxr-x  2.0 unx    73960 b- defN 23-Oct-23 08:08 OBSV/lib/ONIOM_Hscale.txt
 -rw-rw-r--  2.0 unx    73960 b- defN 23-Oct-23 08:08 OBSV/lib/ONIOM_Nscale.txt
 -rw-rw-r--  2.0 unx    73960 b- defN 23-Oct-23 08:08 OBSV/lib/ONIOM_Oscale.txt
--rw-rw-r--  2.0 unx     4934 b- defN 23-Oct-31 02:01 FSV-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Oct-31 02:01 FSV-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      434 b- defN 23-Oct-31 02:01 FSV-1.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-Oct-31 02:01 FSV-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2225 b- defN 23-Oct-31 02:01 FSV-1.0.8.dist-info/RECORD
-29 files, 853532 bytes uncompressed, 169980 bytes compressed:  80.1%
+-rw-rw-r--  2.0 unx     4934 b- defN 23-Nov-11 01:25 FSV-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Nov-11 01:25 FSV-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      434 b- defN 23-Nov-11 01:25 FSV-1.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-Nov-11 01:25 FSV-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2225 b- defN 23-Nov-11 01:25 FSV-1.0.9.dist-info/RECORD
+29 files, 853532 bytes uncompressed, 169979 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: OBSV/lib/ONIOM_Nscale.txt
 Comment: 
 
 Filename: OBSV/lib/ONIOM_Oscale.txt
 Comment: 
 
-Filename: FSV-1.0.8.dist-info/METADATA
+Filename: FSV-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: FSV-1.0.8.dist-info/WHEEL
+Filename: FSV-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: FSV-1.0.8.dist-info/entry_points.txt
+Filename: FSV-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: FSV-1.0.8.dist-info/top_level.txt
+Filename: FSV-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: FSV-1.0.8.dist-info/RECORD
+Filename: FSV-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `FSV-1.0.8.dist-info/METADATA` & `FSV-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSV
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fragmentation-based Strain Visualisation 
 Home-page: 
 Author-email: yanzy@sustech.edu.cn
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 
 ### Fragmentation-based Strain Visualisation (FSV)
```

## Comparing `FSV-1.0.8.dist-info/RECORD` & `FSV-1.0.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 OBSV/basis_functions.py,sha256=EzFXbDStFsLcL4DorS302-2af2bcidhPxqqk-H2Hbi4,27699
 OBSV/fragmentation.py,sha256=F-LwkOXXgduskOAc3E8tHunuKkPp_8lJmnfkDH6gwws,19574
 OBSV/inputs.py,sha256=KgYOs3ohB4UGJ6zpgP1ZJbZ1GPGO-IqH52eigONFt8Y,14179
 OBSV/lib/ONIOM_Cscale.txt,sha256=sMcnNce4RVdBVhLveMxQQ-4vle49asWsfCJsZY6FN4w,73960
 OBSV/lib/ONIOM_Hscale.txt,sha256=pvuYpGp78AsHIYV4M1ntQ0lbOjmKsMeG5gqhU3_nQFA,73960
 OBSV/lib/ONIOM_Nscale.txt,sha256=H01WCRvhhT9dLZD0VJS028DLzfHnPrB9rvR-Pmt_oVQ,73960
 OBSV/lib/ONIOM_Oscale.txt,sha256=gKF5QbVVBjG5YYTXnnDfnYBZSOd4UZwUlQQk3uyzDfA,73960
-FSV-1.0.8.dist-info/METADATA,sha256=For6SuMszGo9E4n6ZgDBLC7kzNWsMbB_XKEjL6UFxQ0,4934
-FSV-1.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-FSV-1.0.8.dist-info/entry_points.txt,sha256=gf7_YdFO38cVrcM_KfHenZYboNlTl_2UT8rBfr7l7b0,434
-FSV-1.0.8.dist-info/top_level.txt,sha256=2F6a9b1ngeMm5Wiiqh32TaTMSLTZvJBjKQ7tu2Inmss,4
-FSV-1.0.8.dist-info/RECORD,,
+FSV-1.0.9.dist-info/METADATA,sha256=EyVRFs7BhGv-E_mAaBm-eEMgDvRBLABvxmRpUbHXOxU,4934
+FSV-1.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+FSV-1.0.9.dist-info/entry_points.txt,sha256=gf7_YdFO38cVrcM_KfHenZYboNlTl_2UT8rBfr7l7b0,434
+FSV-1.0.9.dist-info/top_level.txt,sha256=2F6a9b1ngeMm5Wiiqh32TaTMSLTZvJBjKQ7tu2Inmss,4
+FSV-1.0.9.dist-info/RECORD,,
```

