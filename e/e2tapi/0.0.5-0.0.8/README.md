# Comparing `tmp/e2tapi-0.0.5.tar.gz` & `tmp/e2tapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2tapi-0.0.5.tar", last modified: Wed May 22 20:13:26 2024, max compression
+gzip compressed data, was "e2tapi-0.0.8.tar", last modified: Thu May 23 19:53:01 2024, max compression
```

## Comparing `e2tapi-0.0.5.tar` & `e2tapi-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:13:26.356041 e2tapi-0.0.5/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 20:13:26.356041 e2tapi-0.0.5/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.5/README.md
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:13:26.352041 e2tapi-0.0.5/e2t/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.5/e2t/__init__.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:13:26.352041 e2tapi-0.0.5/e2t/mktdata/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42596 2024-05-22 19:35:52.000000 e2tapi-0.0.5/e2t/mktdata/IBKR_MDG_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.5/e2t/mktdata/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6011 2024-05-22 19:54:27.000000 e2tapi-0.0.5/e2t/mktdata/ibkr.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:13:26.352041 e2tapi-0.0.5/e2t/oms/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    26353 2024-05-20 17:41:14.000000 e2tapi-0.0.5/e2t/oms/IBKR_OMS_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.5/e2t/oms/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4494 2024-05-22 20:08:02.000000 e2tapi-0.0.5/e2t/oms/ibkr.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:13:26.356041 e2tapi-0.0.5/e2tapi.egg-info/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 20:13:26.000000 e2tapi-0.0.5/e2tapi.egg-info/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      333 2024-05-22 20:13:26.000000 e2tapi-0.0.5/e2tapi.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-22 20:13:26.000000 e2tapi-0.0.5/e2tapi.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-22 20:13:26.000000 e2tapi-0.0.5/e2tapi.egg-info/requires.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-22 20:13:26.000000 e2tapi-0.0.5/e2tapi.egg-info/top_level.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-22 20:13:26.356041 e2tapi-0.0.5/setup.cfg
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-22 20:13:22.000000 e2tapi-0.0.5/setup.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.890423 e2tapi-0.0.8/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:53:01.886423 e2tapi-0.0.8/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.8/README.md
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.878423 e2tapi-0.0.8/e2t/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.8/e2t/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.882423 e2tapi-0.0.8/e2t/mktdata/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    97648 2024-05-23 19:46:58.000000 e2tapi-0.0.8/e2t/mktdata/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42353 2024-05-23 19:50:12.000000 e2tapi-0.0.8/e2t/mktdata/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.8/e2t/mktdata/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    12652 2024-05-23 19:51:38.000000 e2tapi-0.0.8/e2t/mktdata/byma.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6015 2024-05-23 19:51:38.000000 e2tapi-0.0.8/e2t/mktdata/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.886423 e2tapi-0.0.8/e2t/oms/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    36422 2024-05-23 19:38:27.000000 e2tapi-0.0.8/e2t/oms/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    23586 2024-05-23 19:45:17.000000 e2tapi-0.0.8/e2t/oms/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       39 2024-05-23 19:01:40.000000 e2tapi-0.0.8/e2t/oms/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     5650 2024-05-23 19:40:58.000000 e2tapi-0.0.8/e2t/oms/byma.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4491 2024-05-23 19:24:30.000000 e2tapi-0.0.8/e2t/oms/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.886423 e2tapi-0.0.8/e2tapi.egg-info/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      423 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/requires.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/top_level.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-23 19:53:01.890423 e2tapi-0.0.8/setup.cfg
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-23 19:52:57.000000 e2tapi-0.0.8/setup.py
```

### Comparing `e2tapi-0.0.5/PKG-INFO` & `e2tapi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.5
+Version: 0.0.8
 Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `e2tapi-0.0.5/README.md` & `e2tapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.5/e2t/mktdata/IBKR_MDG_Messages_pb2.py` & `e2tapi-0.0.8/e2t/mktdata/IBKR_Messages_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: IBKR_MDG_Messages.proto
+# source: IBKR_Messages.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='IBKR_MDG_Messages.proto',
+  name='IBKR_Messages.proto',
   package='',
   syntax='proto3',
-  serialized_options=b'\n\'com.event2trading.mktdata.ibkr.protobufB\021IBKR_MDG_MessagesH\001',
+  serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x17IBKR_MDG_Messages.proto\"\x8e\x01\n\nMktDataReq\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x08\x12\r\n\x05offer\x18\x03 \x01(\x08\x12\x0c\n\x04last\x18\x04 \x01(\x08\x12\x0c\n\x04open\x18\x05 \x01(\x08\x12\r\n\x05\x63lose\x18\x06 \x01(\x08\x12\x0c\n\x04high\x18\x07 \x01(\x08\x12\x0b\n\x03low\x18\x08 \x01(\x08\x12\x0e\n\x06volume\x18\t \x01(\x08\"\xbf\x01\n\x08Snapshot\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x01\x12\x0e\n\x06\x62idQty\x18\x03 \x01(\x03\x12\r\n\x05offer\x18\x04 \x01(\x01\x12\x10\n\x08offerQty\x18\x05 \x01(\x03\x12\x0c\n\x04last\x18\x06 \x01(\x01\x12\x0f\n\x07lastQty\x18\x07 \x01(\x03\x12\x0c\n\x04open\x18\x08 \x01(\x01\x12\r\n\x05\x63lose\x18\t \x01(\x01\x12\x0c\n\x04high\x18\n \x01(\x01\x12\x0b\n\x03low\x18\x0b \x01(\x01\x12\x0e\n\x06volume\x18\x0c \x01(\x03\"\"\n\x03\x42id\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x01\"(\n\x06\x42idQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06\x62idQty\x18\x02 \x01(\x03\"&\n\x05Offer\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05offer\x18\x02 \x01(\x01\",\n\x08OfferQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x10\n\x08offerQty\x18\x02 \x01(\x03\"$\n\x04Last\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04last\x18\x02 \x01(\x01\"*\n\x07LastQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07lastQty\x18\x02 \x01(\x03\"$\n\x04Open\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04open\x18\x02 \x01(\x01\"&\n\x05\x43lose\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05\x63lose\x18\x02 \x01(\x01\"$\n\x04High\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04high\x18\x02 \x01(\x01\"\"\n\x03Low\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03low\x18\x02 \x01(\x01\"(\n\x06Volume\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06volume\x18\x02 \x01(\x01\"(\n\x06Reject\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x03\n\x07Message\x12!\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x0c.MessageType\x12\x1f\n\nmktDataReq\x18\x02 \x01(\x0b\x32\x0b.MktDataReq\x12\x1b\n\x08snapshot\x18\x03 \x01(\x0b\x32\t.Snapshot\x12\x11\n\x03\x62id\x18\x04 \x01(\x0b\x32\x04.Bid\x12\x17\n\x06\x62idQty\x18\x05 \x01(\x0b\x32\x07.BidQty\x12\x15\n\x05offer\x18\x06 \x01(\x0b\x32\x06.Offer\x12\x1b\n\x08offerQty\x18\x07 \x01(\x0b\x32\t.OfferQty\x12\x13\n\x04last\x18\x08 \x01(\x0b\x32\x05.Last\x12\x19\n\x07lastQty\x18\t \x01(\x0b\x32\x08.LastQty\x12\x13\n\x04open\x18\n \x01(\x0b\x32\x05.Open\x12\x15\n\x05\x63lose\x18\x0b \x01(\x0b\x32\x06.Close\x12\x13\n\x04high\x18\x0c \x01(\x0b\x32\x05.High\x12\x11\n\x03low\x18\r \x01(\x0b\x32\x04.Low\x12\x17\n\x06volume\x18\x0e \x01(\x0b\x32\x07.Volume\x12\x17\n\x06Reject\x18\x63 \x01(\x0b\x32\x07.Reject*\xbc\x01\n\x0bMessageType\x12\x08\n\x04NONE\x10\x00\x12\x10\n\x0cMTK_DATA_REQ\x10\x01\x12\x0c\n\x08SNAPSHOT\x10\x02\x12\x07\n\x03\x42ID\x10\x03\x12\n\n\x06\x42IDQTY\x10\x04\x12\t\n\x05OFFER\x10\x05\x12\x0c\n\x08OFFERQTY\x10\x06\x12\x08\n\x04LAST\x10\x07\x12\x0b\n\x07LASTQTY\x10\x08\x12\x08\n\x04OPEN\x10\t\x12\t\n\x05\x43LOSE\x10\n\x12\x08\n\x04HIGH\x10\x0b\x12\x07\n\x03LOW\x10\x0c\x12\n\n\x06VOLUME\x10\r\x12\n\n\x06REJECT\x10\x63\x42>\n\'com.event2trading.mktdata.ibkr.protobufB\x11IBKR_MDG_MessagesH\x01\x62\x06proto3'
+  serialized_pb=b'\n\x13IBKR_Messages.proto\"\x8e\x01\n\nMktDataReq\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x08\x12\r\n\x05offer\x18\x03 \x01(\x08\x12\x0c\n\x04last\x18\x04 \x01(\x08\x12\x0c\n\x04open\x18\x05 \x01(\x08\x12\r\n\x05\x63lose\x18\x06 \x01(\x08\x12\x0c\n\x04high\x18\x07 \x01(\x08\x12\x0b\n\x03low\x18\x08 \x01(\x08\x12\x0e\n\x06volume\x18\t \x01(\x08\"\xbf\x01\n\x08Snapshot\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x01\x12\x0e\n\x06\x62idQty\x18\x03 \x01(\x03\x12\r\n\x05offer\x18\x04 \x01(\x01\x12\x10\n\x08offerQty\x18\x05 \x01(\x03\x12\x0c\n\x04last\x18\x06 \x01(\x01\x12\x0f\n\x07lastQty\x18\x07 \x01(\x03\x12\x0c\n\x04open\x18\x08 \x01(\x01\x12\r\n\x05\x63lose\x18\t \x01(\x01\x12\x0c\n\x04high\x18\n \x01(\x01\x12\x0b\n\x03low\x18\x0b \x01(\x01\x12\x0e\n\x06volume\x18\x0c \x01(\x03\"\"\n\x03\x42id\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03\x62id\x18\x02 \x01(\x01\"(\n\x06\x42idQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06\x62idQty\x18\x02 \x01(\x03\"&\n\x05Offer\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05offer\x18\x02 \x01(\x01\",\n\x08OfferQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x10\n\x08offerQty\x18\x02 \x01(\x03\"$\n\x04Last\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04last\x18\x02 \x01(\x01\"*\n\x07LastQty\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07lastQty\x18\x02 \x01(\x03\"$\n\x04Open\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04open\x18\x02 \x01(\x01\"&\n\x05\x43lose\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05\x63lose\x18\x02 \x01(\x01\"$\n\x04High\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04high\x18\x02 \x01(\x01\"\"\n\x03Low\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0b\n\x03low\x18\x02 \x01(\x01\"(\n\x06Volume\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06volume\x18\x02 \x01(\x01\"(\n\x06Reject\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x03\n\x07Message\x12!\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x0c.MessageType\x12\x1f\n\nmktDataReq\x18\x02 \x01(\x0b\x32\x0b.MktDataReq\x12\x1b\n\x08snapshot\x18\x03 \x01(\x0b\x32\t.Snapshot\x12\x11\n\x03\x62id\x18\x04 \x01(\x0b\x32\x04.Bid\x12\x17\n\x06\x62idQty\x18\x05 \x01(\x0b\x32\x07.BidQty\x12\x15\n\x05offer\x18\x06 \x01(\x0b\x32\x06.Offer\x12\x1b\n\x08offerQty\x18\x07 \x01(\x0b\x32\t.OfferQty\x12\x13\n\x04last\x18\x08 \x01(\x0b\x32\x05.Last\x12\x19\n\x07lastQty\x18\t \x01(\x0b\x32\x08.LastQty\x12\x13\n\x04open\x18\n \x01(\x0b\x32\x05.Open\x12\x15\n\x05\x63lose\x18\x0b \x01(\x0b\x32\x06.Close\x12\x13\n\x04high\x18\x0c \x01(\x0b\x32\x05.High\x12\x11\n\x03low\x18\r \x01(\x0b\x32\x04.Low\x12\x17\n\x06volume\x18\x0e \x01(\x0b\x32\x07.Volume\x12\x17\n\x06Reject\x18\x63 \x01(\x0b\x32\x07.Reject*\xbc\x01\n\x0bMessageType\x12\x08\n\x04NONE\x10\x00\x12\x10\n\x0cMTK_DATA_REQ\x10\x01\x12\x0c\n\x08SNAPSHOT\x10\x02\x12\x07\n\x03\x42ID\x10\x03\x12\n\n\x06\x42IDQTY\x10\x04\x12\t\n\x05OFFER\x10\x05\x12\x0c\n\x08OFFERQTY\x10\x06\x12\x08\n\x04LAST\x10\x07\x12\x0b\n\x07LASTQTY\x10\x08\x12\x08\n\x04OPEN\x10\t\x12\t\n\x05\x43LOSE\x10\n\x12\x08\n\x04HIGH\x10\x0b\x12\x07\n\x03LOW\x10\x0c\x12\n\n\x06VOLUME\x10\r\x12\n\n\x06REJECT\x10\x63\x62\x06proto3'
 )
 
 _MESSAGETYPE = _descriptor.EnumDescriptor(
   name='MessageType',
   full_name='MessageType',
   filename=None,
   file=DESCRIPTOR,
@@ -104,16 +104,16 @@
       name='REJECT', index=14, number=99,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1236,
-  serialized_end=1424,
+  serialized_start=1232,
+  serialized_end=1420,
 )
 _sym_db.RegisterEnumDescriptor(_MESSAGETYPE)
 
 MessageType = enum_type_wrapper.EnumTypeWrapper(_MESSAGETYPE)
 NONE = 0
 MTK_DATA_REQ = 1
 SNAPSHOT = 2
@@ -211,16 +211,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=28,
-  serialized_end=170,
+  serialized_start=24,
+  serialized_end=166,
 )
 
 
 _SNAPSHOT = _descriptor.Descriptor(
   name='Snapshot',
   full_name='Snapshot',
   filename=None,
@@ -320,16 +320,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=173,
-  serialized_end=364,
+  serialized_start=169,
+  serialized_end=360,
 )
 
 
 _BID = _descriptor.Descriptor(
   name='Bid',
   full_name='Bid',
   filename=None,
@@ -359,16 +359,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=366,
-  serialized_end=400,
+  serialized_start=362,
+  serialized_end=396,
 )
 
 
 _BIDQTY = _descriptor.Descriptor(
   name='BidQty',
   full_name='BidQty',
   filename=None,
@@ -398,16 +398,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=402,
-  serialized_end=442,
+  serialized_start=398,
+  serialized_end=438,
 )
 
 
 _OFFER = _descriptor.Descriptor(
   name='Offer',
   full_name='Offer',
   filename=None,
@@ -437,16 +437,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=444,
-  serialized_end=482,
+  serialized_start=440,
+  serialized_end=478,
 )
 
 
 _OFFERQTY = _descriptor.Descriptor(
   name='OfferQty',
   full_name='OfferQty',
   filename=None,
@@ -476,16 +476,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=484,
-  serialized_end=528,
+  serialized_start=480,
+  serialized_end=524,
 )
 
 
 _LAST = _descriptor.Descriptor(
   name='Last',
   full_name='Last',
   filename=None,
@@ -515,16 +515,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=530,
-  serialized_end=566,
+  serialized_start=526,
+  serialized_end=562,
 )
 
 
 _LASTQTY = _descriptor.Descriptor(
   name='LastQty',
   full_name='LastQty',
   filename=None,
@@ -554,16 +554,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=568,
-  serialized_end=610,
+  serialized_start=564,
+  serialized_end=606,
 )
 
 
 _OPEN = _descriptor.Descriptor(
   name='Open',
   full_name='Open',
   filename=None,
@@ -593,16 +593,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=612,
-  serialized_end=648,
+  serialized_start=608,
+  serialized_end=644,
 )
 
 
 _CLOSE = _descriptor.Descriptor(
   name='Close',
   full_name='Close',
   filename=None,
@@ -632,16 +632,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=650,
-  serialized_end=688,
+  serialized_start=646,
+  serialized_end=684,
 )
 
 
 _HIGH = _descriptor.Descriptor(
   name='High',
   full_name='High',
   filename=None,
@@ -671,16 +671,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=690,
-  serialized_end=726,
+  serialized_start=686,
+  serialized_end=722,
 )
 
 
 _LOW = _descriptor.Descriptor(
   name='Low',
   full_name='Low',
   filename=None,
@@ -710,16 +710,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=728,
-  serialized_end=762,
+  serialized_start=724,
+  serialized_end=758,
 )
 
 
 _VOLUME = _descriptor.Descriptor(
   name='Volume',
   full_name='Volume',
   filename=None,
@@ -749,16 +749,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=764,
-  serialized_end=804,
+  serialized_start=760,
+  serialized_end=800,
 )
 
 
 _REJECT = _descriptor.Descriptor(
   name='Reject',
   full_name='Reject',
   filename=None,
@@ -788,16 +788,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=806,
-  serialized_end=846,
+  serialized_start=802,
+  serialized_end=842,
 )
 
 
 _MESSAGE = _descriptor.Descriptor(
   name='Message',
   full_name='Message',
   filename=None,
@@ -918,16 +918,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=849,
-  serialized_end=1233,
+  serialized_start=845,
+  serialized_end=1229,
 )
 
 _MESSAGE.fields_by_name['messageType'].enum_type = _MESSAGETYPE
 _MESSAGE.fields_by_name['mktDataReq'].message_type = _MKTDATAREQ
 _MESSAGE.fields_by_name['snapshot'].message_type = _SNAPSHOT
 _MESSAGE.fields_by_name['bid'].message_type = _BID
 _MESSAGE.fields_by_name['bidQty'].message_type = _BIDQTY
@@ -957,113 +957,112 @@
 DESCRIPTOR.message_types_by_name['Reject'] = _REJECT
 DESCRIPTOR.message_types_by_name['Message'] = _MESSAGE
 DESCRIPTOR.enum_types_by_name['MessageType'] = _MESSAGETYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 MktDataReq = _reflection.GeneratedProtocolMessageType('MktDataReq', (_message.Message,), {
   'DESCRIPTOR' : _MKTDATAREQ,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:MktDataReq)
   })
 _sym_db.RegisterMessage(MktDataReq)
 
 Snapshot = _reflection.GeneratedProtocolMessageType('Snapshot', (_message.Message,), {
   'DESCRIPTOR' : _SNAPSHOT,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Snapshot)
   })
 _sym_db.RegisterMessage(Snapshot)
 
 Bid = _reflection.GeneratedProtocolMessageType('Bid', (_message.Message,), {
   'DESCRIPTOR' : _BID,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Bid)
   })
 _sym_db.RegisterMessage(Bid)
 
 BidQty = _reflection.GeneratedProtocolMessageType('BidQty', (_message.Message,), {
   'DESCRIPTOR' : _BIDQTY,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:BidQty)
   })
 _sym_db.RegisterMessage(BidQty)
 
 Offer = _reflection.GeneratedProtocolMessageType('Offer', (_message.Message,), {
   'DESCRIPTOR' : _OFFER,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Offer)
   })
 _sym_db.RegisterMessage(Offer)
 
 OfferQty = _reflection.GeneratedProtocolMessageType('OfferQty', (_message.Message,), {
   'DESCRIPTOR' : _OFFERQTY,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:OfferQty)
   })
 _sym_db.RegisterMessage(OfferQty)
 
 Last = _reflection.GeneratedProtocolMessageType('Last', (_message.Message,), {
   'DESCRIPTOR' : _LAST,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Last)
   })
 _sym_db.RegisterMessage(Last)
 
 LastQty = _reflection.GeneratedProtocolMessageType('LastQty', (_message.Message,), {
   'DESCRIPTOR' : _LASTQTY,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:LastQty)
   })
 _sym_db.RegisterMessage(LastQty)
 
 Open = _reflection.GeneratedProtocolMessageType('Open', (_message.Message,), {
   'DESCRIPTOR' : _OPEN,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Open)
   })
 _sym_db.RegisterMessage(Open)
 
 Close = _reflection.GeneratedProtocolMessageType('Close', (_message.Message,), {
   'DESCRIPTOR' : _CLOSE,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Close)
   })
 _sym_db.RegisterMessage(Close)
 
 High = _reflection.GeneratedProtocolMessageType('High', (_message.Message,), {
   'DESCRIPTOR' : _HIGH,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:High)
   })
 _sym_db.RegisterMessage(High)
 
 Low = _reflection.GeneratedProtocolMessageType('Low', (_message.Message,), {
   'DESCRIPTOR' : _LOW,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Low)
   })
 _sym_db.RegisterMessage(Low)
 
 Volume = _reflection.GeneratedProtocolMessageType('Volume', (_message.Message,), {
   'DESCRIPTOR' : _VOLUME,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Volume)
   })
 _sym_db.RegisterMessage(Volume)
 
 Reject = _reflection.GeneratedProtocolMessageType('Reject', (_message.Message,), {
   'DESCRIPTOR' : _REJECT,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Reject)
   })
 _sym_db.RegisterMessage(Reject)
 
 Message = _reflection.GeneratedProtocolMessageType('Message', (_message.Message,), {
   'DESCRIPTOR' : _MESSAGE,
-  '__module__' : 'IBKR_MDG_Messages_pb2'
+  '__module__' : 'IBKR_Messages_pb2'
   # @@protoc_insertion_point(class_scope:Message)
   })
 _sym_db.RegisterMessage(Message)
 
 
-DESCRIPTOR._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `e2tapi-0.0.5/e2t/mktdata/ibkr.py` & `e2tapi-0.0.8/e2t/mktdata/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import threading
 import random
 import string
 from google.protobuf.message import DecodeError
 from google.protobuf.internal.encoder import _VarintBytes
 from google.protobuf.internal.decoder import _DecodeVarint32
 
-import IBKR_MDG_Messages_pb2 as pb
+from e2t.mktdata import IBKR_Messages_pb2 as pb
 
 
-class E2T_MKTDATA():
+class IBKR:
 
     @abstractmethod
     def snapshot(self, message):
         pass
 
     @abstractmethod
     def bid(self, symbol, type, value):
```

### Comparing `e2tapi-0.0.5/e2t/oms/IBKR_OMS_Messages_pb2.py` & `e2tapi-0.0.8/e2t/oms/IBKR_Messages_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: IBKR_OMS_Messages.proto
+# source: IBKR_Messages.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='IBKR_OMS_Messages.proto',
-  package='com.event2trading.gateways.e2tibgw.protobuf',
+  name='IBKR_Messages.proto',
+  package='',
   syntax='proto3',
-  serialized_options=b'\n+com.event2trading.gateways.e2tibgw.protobufB\017IB_DAG_MessagesH\001',
+  serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x17IBKR_OMS_Messages.proto\x12+com.event2trading.gateways.e2tibgw.protobuf\"^\n\nLimitOrder\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0c\n\x04side\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08quantity\x18\x04 \x01(\x01\x12\r\n\x05price\x18\x05 \x01(\x01\"S\n\x0cLimitReplace\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\x12\x10\n\x08quantity\x18\x03 \x01(\x01\x12\r\n\x05price\x18\x04 \x01(\x01\"1\n\x0bLimitCancel\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\"\x81\x01\n\x0bOrderStatus\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\x12\x0c\n\x04live\x18\x03 \x01(\x08\x12\x0e\n\x06\x63umQty\x18\x04 \x01(\x01\x12\x11\n\tleavesQty\x18\x05 \x01(\x01\x12\r\n\x05\x61vgPx\x18\x06 \x01(\x01\x12\x0e\n\x06lastPx\x18\x07 \x01(\x01\"{\n\nTradeOrder\x12\x0f\n\x07orderId\x18\x01 \x01(\x05\x12\x0e\n\x06\x65xecId\x18\x02 \x01(\t\x12\x0c\n\x04time\x18\x03 \x01(\t\x12\x0f\n\x07lastQty\x18\x04 \x01(\x01\x12\x0e\n\x06lastPx\x18\x05 \x01(\x01\x12\r\n\x05\x61vgPx\x18\x06 \x01(\x01\x12\x0e\n\x06\x63umQty\x18\x07 \x01(\x01\"\'\n\x06Reject\x12\r\n\x05idRef\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\xa6\x04\n\x07Message\x12M\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x38.com.event2trading.gateways.e2tibgw.protobuf.MessageType\x12K\n\nlimitOrder\x18\x02 \x01(\x0b\x32\x37.com.event2trading.gateways.e2tibgw.protobuf.LimitOrder\x12O\n\x0climitReplace\x18\x03 \x01(\x0b\x32\x39.com.event2trading.gateways.e2tibgw.protobuf.LimitReplace\x12M\n\x0blimitCancel\x18\x04 \x01(\x0b\x32\x38.com.event2trading.gateways.e2tibgw.protobuf.LimitCancel\x12M\n\x0borderStatus\x18\x05 \x01(\x0b\x32\x38.com.event2trading.gateways.e2tibgw.protobuf.OrderStatus\x12K\n\ntradeOrder\x18\x06 \x01(\x0b\x32\x37.com.event2trading.gateways.e2tibgw.protobuf.TradeOrder\x12\x43\n\x06reject\x18\x63 \x01(\x0b\x32\x33.com.event2trading.gateways.e2tibgw.protobuf.Reject*r\n\x0bMessageType\x12\x0f\n\x0bLIMIT_ORDER\x10\x00\x12\x11\n\rLIMIT_REPLACE\x10\x01\x12\x10\n\x0cLIMIT_CANCEL\x10\x02\x12\x10\n\x0cORDER_STATUS\x10\x03\x12\x0f\n\x0bTRADE_ORDER\x10\x04\x12\n\n\x06REJECT\x10\x63\x42@\n+com.event2trading.gateways.e2tibgw.protobufB\x0fIB_DAG_MessagesH\x01\x62\x06proto3'
+  serialized_pb=b'\n\x13IBKR_Messages.proto\"^\n\nLimitOrder\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0c\n\x04side\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08quantity\x18\x04 \x01(\x01\x12\r\n\x05price\x18\x05 \x01(\x01\"S\n\x0cLimitReplace\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\x12\x10\n\x08quantity\x18\x03 \x01(\x01\x12\r\n\x05price\x18\x04 \x01(\x01\"1\n\x0bLimitCancel\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\"\x81\x01\n\x0bOrderStatus\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x05\x12\x0c\n\x04live\x18\x03 \x01(\x08\x12\x0e\n\x06\x63umQty\x18\x04 \x01(\x01\x12\x11\n\tleavesQty\x18\x05 \x01(\x01\x12\r\n\x05\x61vgPx\x18\x06 \x01(\x01\x12\x0e\n\x06lastPx\x18\x07 \x01(\x01\"{\n\nTradeOrder\x12\x0f\n\x07orderId\x18\x01 \x01(\x05\x12\x0e\n\x06\x65xecId\x18\x02 \x01(\t\x12\x0c\n\x04time\x18\x03 \x01(\t\x12\x0f\n\x07lastQty\x18\x04 \x01(\x01\x12\x0e\n\x06lastPx\x18\x05 \x01(\x01\x12\r\n\x05\x61vgPx\x18\x06 \x01(\x01\x12\x0e\n\x06\x63umQty\x18\x07 \x01(\x01\"\'\n\x06Reject\x12\r\n\x05idRef\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\xf2\x01\n\x07Message\x12!\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x0c.MessageType\x12\x1f\n\nlimitOrder\x18\x02 \x01(\x0b\x32\x0b.LimitOrder\x12#\n\x0climitReplace\x18\x03 \x01(\x0b\x32\r.LimitReplace\x12!\n\x0blimitCancel\x18\x04 \x01(\x0b\x32\x0c.LimitCancel\x12!\n\x0borderStatus\x18\x05 \x01(\x0b\x32\x0c.OrderStatus\x12\x1f\n\ntradeOrder\x18\x06 \x01(\x0b\x32\x0b.TradeOrder\x12\x17\n\x06reject\x18\x63 \x01(\x0b\x32\x07.Reject*r\n\x0bMessageType\x12\x0f\n\x0bLIMIT_ORDER\x10\x00\x12\x11\n\rLIMIT_REPLACE\x10\x01\x12\x10\n\x0cLIMIT_CANCEL\x10\x02\x12\x10\n\x0cORDER_STATUS\x10\x03\x12\x0f\n\x0bTRADE_ORDER\x10\x04\x12\n\n\x06REJECT\x10\x63\x62\x06proto3'
 )
 
 _MESSAGETYPE = _descriptor.EnumDescriptor(
   name='MessageType',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.MessageType',
+  full_name='MessageType',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
       name='LIMIT_ORDER', index=0, number=0,
       serialized_options=None,
@@ -59,16 +59,16 @@
       name='REJECT', index=5, number=99,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1155,
-  serialized_end=1269,
+  serialized_start=798,
+  serialized_end=912,
 )
 _sym_db.RegisterEnumDescriptor(_MESSAGETYPE)
 
 MessageType = enum_type_wrapper.EnumTypeWrapper(_MESSAGETYPE)
 LIMIT_ORDER = 0
 LIMIT_REPLACE = 1
 LIMIT_CANCEL = 2
@@ -76,50 +76,50 @@
 TRADE_ORDER = 4
 REJECT = 99
 
 
 
 _LIMITORDER = _descriptor.Descriptor(
   name='LimitOrder',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder',
+  full_name='LimitOrder',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='requestId', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder.requestId', index=0,
+      name='requestId', full_name='LimitOrder.requestId', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='side', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder.side', index=1,
+      name='side', full_name='LimitOrder.side', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='symbol', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder.symbol', index=2,
+      name='symbol', full_name='LimitOrder.symbol', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='quantity', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder.quantity', index=3,
+      name='quantity', full_name='LimitOrder.quantity', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='price', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitOrder.price', index=4,
+      name='price', full_name='LimitOrder.price', index=4,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -129,50 +129,50 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=72,
-  serialized_end=166,
+  serialized_start=23,
+  serialized_end=117,
 )
 
 
 _LIMITREPLACE = _descriptor.Descriptor(
   name='LimitReplace',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitReplace',
+  full_name='LimitReplace',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='requestId', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitReplace.requestId', index=0,
+      name='requestId', full_name='LimitReplace.requestId', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='orderId', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitReplace.orderId', index=1,
+      name='orderId', full_name='LimitReplace.orderId', index=1,
       number=2, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='quantity', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitReplace.quantity', index=2,
+      name='quantity', full_name='LimitReplace.quantity', index=2,
       number=3, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='price', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitReplace.price', index=3,
+      name='price', full_name='LimitReplace.price', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -182,36 +182,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=168,
-  serialized_end=251,
+  serialized_start=119,
+  serialized_end=202,
 )
 
 
 _LIMITCANCEL = _descriptor.Descriptor(
   name='LimitCancel',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitCancel',
+  full_name='LimitCancel',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='requestId', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitCancel.requestId', index=0,
+      name='requestId', full_name='LimitCancel.requestId', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='orderId', full_name='com.event2trading.gateways.e2tibgw.protobuf.LimitCancel.orderId', index=1,
+      name='orderId', full_name='LimitCancel.orderId', index=1,
       number=2, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -221,71 +221,71 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=253,
-  serialized_end=302,
+  serialized_start=204,
+  serialized_end=253,
 )
 
 
 _ORDERSTATUS = _descriptor.Descriptor(
   name='OrderStatus',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus',
+  full_name='OrderStatus',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='requestId', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.requestId', index=0,
+      name='requestId', full_name='OrderStatus.requestId', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='orderId', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.orderId', index=1,
+      name='orderId', full_name='OrderStatus.orderId', index=1,
       number=2, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='live', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.live', index=2,
+      name='live', full_name='OrderStatus.live', index=2,
       number=3, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cumQty', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.cumQty', index=3,
+      name='cumQty', full_name='OrderStatus.cumQty', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='leavesQty', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.leavesQty', index=4,
+      name='leavesQty', full_name='OrderStatus.leavesQty', index=4,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='avgPx', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.avgPx', index=5,
+      name='avgPx', full_name='OrderStatus.avgPx', index=5,
       number=6, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lastPx', full_name='com.event2trading.gateways.e2tibgw.protobuf.OrderStatus.lastPx', index=6,
+      name='lastPx', full_name='OrderStatus.lastPx', index=6,
       number=7, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -295,71 +295,71 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=305,
-  serialized_end=434,
+  serialized_start=256,
+  serialized_end=385,
 )
 
 
 _TRADEORDER = _descriptor.Descriptor(
   name='TradeOrder',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder',
+  full_name='TradeOrder',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='orderId', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.orderId', index=0,
+      name='orderId', full_name='TradeOrder.orderId', index=0,
       number=1, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='execId', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.execId', index=1,
+      name='execId', full_name='TradeOrder.execId', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='time', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.time', index=2,
+      name='time', full_name='TradeOrder.time', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lastQty', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.lastQty', index=3,
+      name='lastQty', full_name='TradeOrder.lastQty', index=3,
       number=4, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lastPx', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.lastPx', index=4,
+      name='lastPx', full_name='TradeOrder.lastPx', index=4,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='avgPx', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.avgPx', index=5,
+      name='avgPx', full_name='TradeOrder.avgPx', index=5,
       number=6, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cumQty', full_name='com.event2trading.gateways.e2tibgw.protobuf.TradeOrder.cumQty', index=6,
+      name='cumQty', full_name='TradeOrder.cumQty', index=6,
       number=7, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -369,36 +369,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=436,
-  serialized_end=559,
+  serialized_start=387,
+  serialized_end=510,
 )
 
 
 _REJECT = _descriptor.Descriptor(
   name='Reject',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.Reject',
+  full_name='Reject',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='idRef', full_name='com.event2trading.gateways.e2tibgw.protobuf.Reject.idRef', index=0,
+      name='idRef', full_name='Reject.idRef', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='reason', full_name='com.event2trading.gateways.e2tibgw.protobuf.Reject.reason', index=1,
+      name='reason', full_name='Reject.reason', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -408,71 +408,71 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=561,
-  serialized_end=600,
+  serialized_start=512,
+  serialized_end=551,
 )
 
 
 _MESSAGE = _descriptor.Descriptor(
   name='Message',
-  full_name='com.event2trading.gateways.e2tibgw.protobuf.Message',
+  full_name='Message',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='messageType', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.messageType', index=0,
+      name='messageType', full_name='Message.messageType', index=0,
       number=1, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='limitOrder', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.limitOrder', index=1,
+      name='limitOrder', full_name='Message.limitOrder', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='limitReplace', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.limitReplace', index=2,
+      name='limitReplace', full_name='Message.limitReplace', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='limitCancel', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.limitCancel', index=3,
+      name='limitCancel', full_name='Message.limitCancel', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='orderStatus', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.orderStatus', index=4,
+      name='orderStatus', full_name='Message.orderStatus', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='tradeOrder', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.tradeOrder', index=5,
+      name='tradeOrder', full_name='Message.tradeOrder', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='reject', full_name='com.event2trading.gateways.e2tibgw.protobuf.Message.reject', index=6,
+      name='reject', full_name='Message.reject', index=6,
       number=99, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -482,16 +482,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=603,
-  serialized_end=1153,
+  serialized_start=554,
+  serialized_end=796,
 )
 
 _MESSAGE.fields_by_name['messageType'].enum_type = _MESSAGETYPE
 _MESSAGE.fields_by_name['limitOrder'].message_type = _LIMITORDER
 _MESSAGE.fields_by_name['limitReplace'].message_type = _LIMITREPLACE
 _MESSAGE.fields_by_name['limitCancel'].message_type = _LIMITCANCEL
 _MESSAGE.fields_by_name['orderStatus'].message_type = _ORDERSTATUS
@@ -505,57 +505,56 @@
 DESCRIPTOR.message_types_by_name['Reject'] = _REJECT
 DESCRIPTOR.message_types_by_name['Message'] = _MESSAGE
 DESCRIPTOR.enum_types_by_name['MessageType'] = _MESSAGETYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 LimitOrder = _reflection.GeneratedProtocolMessageType('LimitOrder', (_message.Message,), {
   'DESCRIPTOR' : _LIMITORDER,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.LimitOrder)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:LimitOrder)
   })
 _sym_db.RegisterMessage(LimitOrder)
 
 LimitReplace = _reflection.GeneratedProtocolMessageType('LimitReplace', (_message.Message,), {
   'DESCRIPTOR' : _LIMITREPLACE,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.LimitReplace)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:LimitReplace)
   })
 _sym_db.RegisterMessage(LimitReplace)
 
 LimitCancel = _reflection.GeneratedProtocolMessageType('LimitCancel', (_message.Message,), {
   'DESCRIPTOR' : _LIMITCANCEL,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.LimitCancel)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:LimitCancel)
   })
 _sym_db.RegisterMessage(LimitCancel)
 
 OrderStatus = _reflection.GeneratedProtocolMessageType('OrderStatus', (_message.Message,), {
   'DESCRIPTOR' : _ORDERSTATUS,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.OrderStatus)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:OrderStatus)
   })
 _sym_db.RegisterMessage(OrderStatus)
 
 TradeOrder = _reflection.GeneratedProtocolMessageType('TradeOrder', (_message.Message,), {
   'DESCRIPTOR' : _TRADEORDER,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.TradeOrder)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:TradeOrder)
   })
 _sym_db.RegisterMessage(TradeOrder)
 
 Reject = _reflection.GeneratedProtocolMessageType('Reject', (_message.Message,), {
   'DESCRIPTOR' : _REJECT,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.Reject)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:Reject)
   })
 _sym_db.RegisterMessage(Reject)
 
 Message = _reflection.GeneratedProtocolMessageType('Message', (_message.Message,), {
   'DESCRIPTOR' : _MESSAGE,
-  '__module__' : 'IBKR_OMS_Messages_pb2'
-  # @@protoc_insertion_point(class_scope:com.event2trading.gateways.e2tibgw.protobuf.Message)
+  '__module__' : 'IBKR_Messages_pb2'
+  # @@protoc_insertion_point(class_scope:Message)
   })
 _sym_db.RegisterMessage(Message)
 
 
-DESCRIPTOR._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `e2tapi-0.0.5/e2t/oms/ibkr.py` & `e2tapi-0.0.8/e2t/oms/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from google.protobuf.internal.encoder import _VarintBytes
 from google.protobuf.internal.decoder import _DecodeVarint32
 from abc import abstractmethod
 
 from e2t.oms import IBKR_OMS_Messages_pb2 as pb
 
 
-class E2T_OMS:
+class IBKR:
 
     @abstractmethod
     def status(self, requestId, orderId, live, cumQty, leavesQty, avgPx, lastPx):
         pass
 
     @abstractmethod
     def reject(self, idRef, reason):
```

### Comparing `e2tapi-0.0.5/e2tapi.egg-info/PKG-INFO` & `e2tapi-0.0.8/e2tapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.5
+Version: 0.0.8
 Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `e2tapi-0.0.5/setup.py` & `e2tapi-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='e2tapi',
-    version='0.0.5',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[
         'protobuf>=3.0.0',
     ],
     include_package_data=True,
     description='SDK for e2t OMS',
     long_description=open('README.md').read(),
```

