# Comparing `tmp/dooth-1.1.3-py3-none-any.whl.zip` & `tmp/dooth-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6050 bytes, number of entries: 12
+Zip file size: 6051 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 24-May-10 18:16 doot/__init__.py
 -rw-r--r--  2.0 unx     8617 b- defN 24-May-16 07:00 doot/bot.py
 -rw-r--r--  2.0 unx      329 b- defN 24-May-16 05:53 doot/callback.py
 -rw-r--r--  2.0 unx      728 b- defN 24-May-16 06:02 doot/command_handler.py
 -rw-r--r--  2.0 unx      232 b- defN 24-May-12 12:24 doot/exception.py
--rw-r--r--  2.0 unx     4255 b- defN 24-May-11 09:22 doot/message.py
+-rw-r--r--  2.0 unx     4183 b- defN 24-May-23 11:04 doot/message.py
 -rw-r--r--  2.0 unx      702 b- defN 24-May-16 06:02 doot/message_handler.py
 -rw-r--r--  2.0 unx     2527 b- defN 24-May-12 15:15 doot/response.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-16 07:03 dooth-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 07:03 dooth-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-16 07:03 dooth-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      873 b- defN 24-May-16 07:03 dooth-1.1.3.dist-info/RECORD
-12 files, 18434 bytes uncompressed, 4602 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx       74 b- defN 24-May-23 11:05 dooth-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 11:05 dooth-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-23 11:05 dooth-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 24-May-23 11:05 dooth-1.1.4.dist-info/RECORD
+12 files, 18362 bytes uncompressed, 4603 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: doot/message_handler.py
 Comment: 
 
 Filename: doot/response.py
 Comment: 
 
-Filename: dooth-1.1.3.dist-info/METADATA
+Filename: dooth-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: dooth-1.1.3.dist-info/WHEEL
+Filename: dooth-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: dooth-1.1.3.dist-info/top_level.txt
+Filename: dooth-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: dooth-1.1.3.dist-info/RECORD
+Filename: dooth-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doot/message.py

```diff
@@ -3,27 +3,27 @@
 from datetime import datetime
 
 
 @dataclass
 class User:
     id: int
     is_bot: bool
-    username: str
     language_code: str
-    first_name: str
-    last_name: str = None
+    first_name: str = 'NA'
+    last_name: str = 'NA'
+    username: str = 'NA'
 
 
 @dataclass
 class Chat:
     id: int
-    username: str
     type: str
-    first_name: str
-    last_name: str = ''
+    first_name: str = 'NA'
+    last_name: str = 'NA'
+    username: str = 'NA'
 
 
 @dataclass
 class Message:
     message_id: int
     from_user: User
     chat: Chat
@@ -75,21 +75,19 @@
                     "update_id": 300080505,
                     "message": {
                         "message_id": 527,
                         "from": {
                             "id": 6247567702,
                             "is_bot": false,
                             "first_name": "Amit Kumar Sharma",
-                            "username": "amit_9b",
                             "language_code": "en"
                         },
                         "chat": {
                             "id": 6247567702,
                             "first_name": "Amit Kumar Sharma",
-                            "username": "amit_9b",
                             "type": "private"
                         },
                         "date": 1715326007,
                         "text": "hello"
                     }
                 },
                 {
```

## Comparing `dooth-1.1.3.dist-info/RECORD` & `dooth-1.1.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 doot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 doot/bot.py,sha256=YRk0tfbfEJ4xe4dJHkcJGUQI_jBNle5EyFvslP23WVM,8617
 doot/callback.py,sha256=Yyxw7P994bus6CCdc43G8enYdArwZc8qgnXICkp_JaY,329
 doot/command_handler.py,sha256=39fV4bk2XP21z6D4MBTNqqk-5hxGSauf0K9v1Q0nGrM,728
 doot/exception.py,sha256=Ys10w9WqxYIyzn6QPbkxoX_ykgMf_fTUDIH7UsRAWyQ,232
-doot/message.py,sha256=hiXeJ7TOTMvF2TGXj0fqbo3LTAxPi_lW6H1bMeG6UEI,4255
+doot/message.py,sha256=ULzEXD2ZGWppUTbl0J8u5m3LKC7eQXbK6U5uU2OPu_Q,4183
 doot/message_handler.py,sha256=vA_HPP31iHUF-L4OmW4_oSPeXWegYhfJmN1zURYnpi0,702
 doot/response.py,sha256=iAFsgMb3nEJ_gRizDFG7xv-euzIbqRZYVpL6KfsnLX0,2527
-dooth-1.1.3.dist-info/METADATA,sha256=HUnbInA0V6ZyqFprCzZ4tmHoVOImX1DkO3jMgs5Csk8,74
-dooth-1.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dooth-1.1.3.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
-dooth-1.1.3.dist-info/RECORD,,
+dooth-1.1.4.dist-info/METADATA,sha256=hBGMQYtEQSUnQEUpejx5hxdUBqtdYwVxWXXwr0NSodE,74
+dooth-1.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dooth-1.1.4.dist-info/top_level.txt,sha256=259wJJXfvmJdcDJ_Bs4a1f9A0kyxtMNUn1hzSoaHU94,5
+dooth-1.1.4.dist-info/RECORD,,
```

