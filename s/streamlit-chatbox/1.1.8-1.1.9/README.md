# Comparing `tmp/streamlit_chatbox-1.1.8-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9608 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      410 b- defN 23-Sep-17 15:37 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     8149 b- defN 23-Sep-18 11:29 streamlit_chatbox/elements.py
+Zip file size: 9621 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      400 b- defN 23-Sep-19 02:11 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     8149 b- defN 23-Sep-19 01:47 streamlit_chatbox/elements.py
 -rw-rw-rw-  2.0 fat      323 b- defN 23-Aug-09 03:40 streamlit_chatbox/flows.py
--rw-rw-rw-  2.0 fat    15767 b- defN 23-Sep-18 11:51 streamlit_chatbox/messages.py
--rw-rw-rw-  2.0 fat     6362 b- defN 23-Sep-18 11:57 streamlit_chatbox-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-18 11:57 streamlit_chatbox-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Sep-18 11:57 streamlit_chatbox-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      678 b- defN 23-Sep-18 11:57 streamlit_chatbox-1.1.8.dist-info/RECORD
-8 files, 31799 bytes uncompressed, 8416 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 fat    15769 b- defN 23-Sep-19 02:14 streamlit_chatbox/messages.py
+-rw-rw-rw-  2.0 fat     6367 b- defN 23-Sep-19 02:16 streamlit_chatbox-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-19 02:16 streamlit_chatbox-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Sep-19 02:16 streamlit_chatbox-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      678 b- defN 23-Sep-19 02:16 streamlit_chatbox-1.1.9.dist-info/RECORD
+8 files, 31796 bytes uncompressed, 8429 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: streamlit_chatbox/flows.py
 Comment: 
 
 Filename: streamlit_chatbox/messages.py
 Comment: 
 
-Filename: streamlit_chatbox-1.1.8.dist-info/METADATA
+Filename: streamlit_chatbox-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-1.1.8.dist-info/WHEEL
+Filename: streamlit_chatbox-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-1.1.8.dist-info/top_level.txt
+Filename: streamlit_chatbox-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-1.1.8.dist-info/RECORD
+Filename: streamlit_chatbox-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -1,15 +1,16 @@
 from typing import *
-import streamlit as st
-import time
 # from streamlit_option_menu import option_menu
 import asyncio
 from .messages import *
 
 
+__version__ = "1.1.9"
+
+
 __all__ = [
     "ChatBox",
     "Markdown",
     "Image",
     "Audio",
     "Video",
     "OutputElement",
```

## streamlit_chatbox/messages.py

```diff
@@ -113,15 +113,15 @@
             return {
                 "role": msg["role"],
                 "content": "\n\n".join(content),
             }
 
         def default_stop(history):
             if isinstance(history_len, int):
-                user_count = len(x for x in history if x["role"] == "user")
+                user_count = len([x for x in history if x["role"] == "user"])
                 return user_count >= history_len
             else:
                 return False
 
         if filter is None:
             filter = default_filter
```

## Comparing `streamlit_chatbox-1.1.8.dist-info/METADATA` & `streamlit_chatbox-1.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 1.1.8
+Version: 1.1.9
 Summary: A chat box and some helpful tools used to build chatbot app with streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=1.26.0)
@@ -21,15 +21,18 @@
 This package(>=1.0.0) will focus on wrapper of official chat elements to make chat with LLMs more convenient.
 
 # Chatbox component for streamlit
 
 A Streamlit component to show chat messages.
 It's basiclly a wrapper of streamlit officeial elements including the chat elemnts.
 
+- demo
 ![](demo.gif)
+
+- demo agent
 ![](demo_agent.gif)
 
 ## Features
 
 - support streaming output.
 - support markdown/image/video/audio messages, and all streamlit elements could be supported by customized `OutputElement`.
 - output multiple messages at once, and make them collapsable.
@@ -123,15 +126,14 @@
         Audio('https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4'))
 
 if cols[1].button('run agent'):
     chat_box.user_say('run agent')
     agent = FakeAgent()
     text = ""
 
-    if streaming:
     # streaming:
     chat_box.ai_say() # generate a blank placeholder to render messages
     for d in agent.run_stream():
         if d["type"] == "complete":
             chat_box.update_msg(expanded=False, state="complete")
             chat_box.insert_msg(d["llm_output"])
             break
```

