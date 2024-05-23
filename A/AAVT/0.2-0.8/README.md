# Comparing `tmp/AAVT-0.2.tar.gz` & `tmp/AAVT-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAVT-0.2.tar", last modified: Thu May 23 15:46:23 2024, max compression
+gzip compressed data, was "AAVT-0.8.tar", last modified: Wed May 22 15:04:47 2024, max compression
```

## Comparing `AAVT-0.2.tar` & `AAVT-0.8.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 15:46:23.841112 AAVT-0.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 15:46:23.823171 AAVT-0.2/AAVT/
--rw-rw-rw-   0        0        0      172 2024-05-22 11:23:11.000000 AAVT-0.2/AAVT/__init__.py
--rw-rw-rw-   0        0        0     7170 2024-05-22 14:43:12.000000 AAVT-0.2/AAVT/blog.py
--rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.2/AAVT/merge.py
--rw-rw-rw-   0        0        0     4422 2024-05-23 15:40:34.000000 AAVT-0.2/AAVT/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:46:23.835530 AAVT-0.2/AAVT/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.2/AAVT/utils/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.2/AAVT/utils/srt.py
--rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.2/AAVT/whisper_faster.py
--rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.2/AAVT/whisper_openai.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:46:23.832159 AAVT-0.2/AAVT.egg-info/
--rw-rw-rw-   0        0        0     2234 2024-05-23 15:46:23.000000 AAVT-0.2/AAVT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-23 15:46:23.000000 AAVT-0.2/AAVT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:46:23.000000 AAVT-0.2/AAVT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-23 15:46:23.000000 AAVT-0.2/AAVT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 15:46:23.000000 AAVT-0.2/AAVT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2234 2024-05-23 15:46:23.839911 AAVT-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1413 2024-05-22 15:03:49.000000 AAVT-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 15:46:23.841112 AAVT-0.2/setup.cfg
--rw-rw-rw-   0        0        0      752 2024-05-23 15:44:10.000000 AAVT-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:46:23.837874 AAVT-0.2/test/
--rw-rw-rw-   0        0        0     7334 2024-05-23 15:44:10.000000 AAVT-0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:04:47.778011 AAVT-0.8/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:04:47.765697 AAVT-0.8/AAVT/
+-rw-rw-rw-   0        0        0      172 2024-05-22 11:23:11.000000 AAVT-0.8/AAVT/__init__.py
+-rw-rw-rw-   0        0        0     7170 2024-05-22 14:43:12.000000 AAVT-0.8/AAVT/blog.py
+-rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.8/AAVT/merge.py
+-rw-rw-rw-   0        0        0     4424 2024-05-21 11:37:39.000000 AAVT-0.8/AAVT/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:04:47.775526 AAVT-0.8/AAVT/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.8/AAVT/utils/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.8/AAVT/utils/srt.py
+-rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.8/AAVT/whisper_faster.py
+-rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.8/AAVT/whisper_openai.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:04:47.772718 AAVT-0.8/AAVT.egg-info/
+-rw-rw-rw-   0        0        0     2234 2024-05-22 15:04:47.000000 AAVT-0.8/AAVT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-22 15:04:47.000000 AAVT-0.8/AAVT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:04:47.000000 AAVT-0.8/AAVT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-22 15:04:47.000000 AAVT-0.8/AAVT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 15:04:47.000000 AAVT-0.8/AAVT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2234 2024-05-22 15:04:47.777799 AAVT-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2024-05-22 15:03:49.000000 AAVT-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:04:47.778549 AAVT-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      752 2024-05-22 15:04:40.000000 AAVT-0.8/setup.py
```

### Comparing `AAVT-0.2/AAVT/blog.py` & `AAVT-0.8/AAVT/blog.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/AAVT/merge.py` & `AAVT-0.8/AAVT/merge.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/AAVT/translate.py` & `AAVT-0.8/AAVT/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 from openai import OpenAI
 from .utils.srt import generate_srt_from_result
 
 
 def translate(result: dict, api_key: str, base_url: str = None, model: str = None, local: bool = False,
-              language: str = None, wait_time: float = None, srt: bool = True, output_path: str = None) -> dict:
+              language: str = None, wait_time: float = None, srt: float = False, output_path: str = None) -> dict:
     """
     使用翻译功能进行文本翻译
 
     -- 参数
 
     - **result**: 包含待翻译文本的字典。
     - **api_key**: OpenAI API KEY。
```

### Comparing `AAVT-0.2/AAVT/utils/srt.py` & `AAVT-0.8/AAVT/utils/srt.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/AAVT/whisper_faster.py` & `AAVT-0.8/AAVT/whisper_faster.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/AAVT/whisper_openai.py` & `AAVT-0.8/AAVT/whisper_openai.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/AAVT.egg-info/PKG-INFO` & `AAVT-0.8/AAVT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.2
+Version: 0.8
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
 License: UNKNOWN
 Description: # Chenyme-AAVT 
         > AI Auto Video(Audio) Translation
```

### Comparing `AAVT-0.2/PKG-INFO` & `AAVT-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.2
+Version: 0.8
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
 License: UNKNOWN
 Description: # Chenyme-AAVT 
         > AI Auto Video(Audio) Translation
```

### Comparing `AAVT-0.2/README.md` & `AAVT-0.8/README.md`

 * *Files identical despite different names*

### Comparing `AAVT-0.2/setup.py` & `AAVT-0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AAVT',
-    version='0.2',
+    version='0.8',
     packages=find_packages(),
     install_requires=[
         'faster-whisper',
         'openai',
         'opencv-python',
     ],
     description='A Python package for Video Translate and Some Tools for Video',
```

