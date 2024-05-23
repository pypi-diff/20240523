# Comparing `tmp/loaderch-0.1.0-py3-none-any.whl.zip` & `tmp/loaderch-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17250 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       33 b- defN 24-May-23 17:38 loaderch/__init__.py
--rw-rw-rw-  2.0 fat       98 b- defN 24-May-23 14:55 loaderch/__main__.py
+Zip file size: 17247 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       24 b- defN 24-May-23 17:43 loaderch/__init__.py
+-rw-rw-rw-  2.0 fat       98 b- defN 24-May-23 17:43 loaderch/__main__.py
 -rw-rw-rw-  2.0 fat    13642 b- defN 24-May-23 17:38 loaderch/uploader.py
--rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 17:39 loaderch-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 17:39 loaderch-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:39 loaderch-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 17:39 loaderch-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      618 b- defN 24-May-23 17:39 loaderch-0.1.0.dist-info/RECORD
-8 files, 50997 bytes uncompressed, 16172 bytes compressed:  68.3%
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 17:44 loaderch-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 17:44 loaderch-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:44 loaderch-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 17:44 loaderch-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      618 b- defN 24-May-23 17:44 loaderch-0.1.1.dist-info/RECORD
+8 files, 50988 bytes uncompressed, 16169 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: loaderch/__main__.py
 Comment: 
 
 Filename: loaderch/uploader.py
 Comment: 
 
-Filename: loaderch-0.1.0.dist-info/LICENSE
+Filename: loaderch-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: loaderch-0.1.0.dist-info/METADATA
+Filename: loaderch-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: loaderch-0.1.0.dist-info/WHEEL
+Filename: loaderch-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: loaderch-0.1.0.dist-info/top_level.txt
+Filename: loaderch-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: loaderch-0.1.0.dist-info/RECORD
+Filename: loaderch-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loaderch/__init__.py

```diff
@@ -1 +1 @@
-from loaderch.uploader import GUI
+from uploader import GUI
```

## Comparing `loaderch-0.1.0.dist-info/LICENSE` & `loaderch-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `loaderch-0.1.0.dist-info/METADATA` & `loaderch-0.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: loaderch
-Version: 0.1.0
-Summary: Uploader tool for flashing firmware onto the CH552 device. v0.1.0
+Version: 0.1.1
+Summary: Uploader tool for flashing firmware onto the CH552 device. v0.1.1
 Author: Master
 Author-email: name@email.com
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tk
 Requires-Dist: pyusb
```

## Comparing `loaderch-0.1.0.dist-info/RECORD` & `loaderch-0.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-loaderch/__init__.py,sha256=mhEQLqf5LuR9lNdwrOy9rN2A07nV7NcOwdXypT1QXaw,33
+loaderch/__init__.py,sha256=bn7T6wWAhYIUU-uW0bMi3EDYtpiDz73SWtRacVbmrgM,24
 loaderch/__main__.py,sha256=xlQQ_issPH_qLonPMKUZyfo4kHsq1T9SpPk3_ZEsFik,98
 loaderch/uploader.py,sha256=4W8XO-QGLcnZy2KRhXduysjvsCmwT3EyQDnrpk9RnNw,13642
-loaderch-0.1.0.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-loaderch-0.1.0.dist-info/METADATA,sha256=DuCOXRZXgPTijLqroFtm6tFvqCP1uE-IENlJBEWpQMc,684
-loaderch-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-loaderch-0.1.0.dist-info/top_level.txt,sha256=S2cLsgZknyvh2AE2PCxR5QAkhMNpuEoYZ7uT0k31rk0,9
-loaderch-0.1.0.dist-info/RECORD,,
+loaderch-0.1.1.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+loaderch-0.1.1.dist-info/METADATA,sha256=5DzO64Gxo3is8ZruO3267Zu7gH_8bd7BPd73mq_p8Yw,684
+loaderch-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+loaderch-0.1.1.dist-info/top_level.txt,sha256=S2cLsgZknyvh2AE2PCxR5QAkhMNpuEoYZ7uT0k31rk0,9
+loaderch-0.1.1.dist-info/RECORD,,
```

