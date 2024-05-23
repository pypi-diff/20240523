# Comparing `tmp/tdrpa.tdworker-1.1.4.15-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.16-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 432144 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1232896 b- defN 24-May-22 04:57 tdrpa/tdworker.cp39-win_amd64.pyd
+Zip file size: 435446 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1236480 b- defN 24-May-23 04:39 tdrpa/tdworker.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      165 b- defN 24-May-19 14:22 tdrpa/tdworker/__init__.pyi
 -rw-rw-rw-  2.0 fat     4254 b- defN 24-May-19 14:22 tdrpa/tdworker/_w.pyi
 -rw-rw-rw-  2.0 fat    17376 b- defN 24-May-19 14:22 tdrpa/tdworker/_winE.pyi
 -rw-rw-rw-  2.0 fat     5403 b- defN 24-May-19 14:23 tdrpa/tdworker/_winK.pyi
 -rw-rw-rw-  2.0 fat     7920 b- defN 24-May-19 14:24 tdrpa/tdworker/_winM.pyi
--rw-rw-rw-  2.0 fat      677 b- defN 24-May-22 04:57 tdrpa.tdworker-1.1.4.15.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 04:57 tdrpa.tdworker-1.1.4.15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-22 04:57 tdrpa.tdworker-1.1.4.15.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      834 b- defN 24-May-22 04:57 tdrpa.tdworker-1.1.4.15.dist-info/RECORD
-10 files, 1269623 bytes uncompressed, 430720 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat      701 b- defN 24-May-23 04:39 tdrpa.tdworker-1.1.4.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 04:39 tdrpa.tdworker-1.1.4.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-23 04:39 tdrpa.tdworker-1.1.4.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      834 b- defN 24-May-23 04:39 tdrpa.tdworker-1.1.4.16.dist-info/RECORD
+10 files, 1273231 bytes uncompressed, 434022 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.15.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.16.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.15.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.16.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.15.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.16.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.15.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tdrpa.tdworker-1.1.4.15.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.16.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.15
+Version: 1.1.4.16
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: tdrpa.tdcore >=1.1.38
+Requires-Dist: tdrpa.tdcore >=1.1.39
+Requires-Dist: pywin32
 Requires-Dist: pyperclip
 Requires-Dist: WMI
 Requires-Dist: pycryptodome
 
 tdworker for tdrpa developers. supports python3.8+, windows x64
```

## Comparing `tdrpa.tdworker-1.1.4.15.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.16.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp39-win_amd64.pyd,sha256=PcEpeJpSVYRoOuPzckGD3BOdWdtbzwqwWz76ISyAWYM,1232896
+tdrpa/tdworker.cp39-win_amd64.pyd,sha256=HW_Mgg05UzQB5wWfwHbTLI2XPx3NUMjkNrQVJFQFjlw,1236480
 tdrpa/tdworker/__init__.pyi,sha256=6k2uZwCB6qT_NC84U7Cw8Ev9j0EW7VLtZZKE3szptSc,165
 tdrpa/tdworker/_w.pyi,sha256=ZXgV35kxk0kjX2mHu2vL_TnB3_5bGkacQJbnglNsRtE,4254
 tdrpa/tdworker/_winE.pyi,sha256=0URMn5AuJ8Q5EHNUr9zHQjHueh5kMEIPdAGXzcpZ4p8,17376
 tdrpa/tdworker/_winK.pyi,sha256=d-0w5wjbXbJiUx148UtfzaSUfZtKR_JbtYg7j2_sPp4,5403
 tdrpa/tdworker/_winM.pyi,sha256=xBzTZ5ncrwuotlmzxIYIkfqBm25Xz9go6tP8NESZAks,7920
-tdrpa.tdworker-1.1.4.15.dist-info/METADATA,sha256=dQRTVkw9IcIWNhToHHkjY7h4IOpxN9UlkpaY5q6imvI,677
-tdrpa.tdworker-1.1.4.15.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.15.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.15.dist-info/RECORD,,
+tdrpa.tdworker-1.1.4.16.dist-info/METADATA,sha256=lTOFF_tyS-WKKDzNiQSKniKsKfp1L7L3fXCMdQQxiTA,701
+tdrpa.tdworker-1.1.4.16.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.16.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.16.dist-info/RECORD,,
```

