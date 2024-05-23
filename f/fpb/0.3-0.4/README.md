# Comparing `tmp/fpb-0.3.tar.gz` & `tmp/fpb-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpb-0.3.tar", last modified: Thu May 23 04:03:23 2024, max compression
+gzip compressed data, was "fpb-0.4.tar", last modified: Thu May 23 04:05:15 2024, max compression
```

## Comparing `fpb-0.3.tar` & `fpb-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.751048 fpb-0.3/
--rw-rw-rw-   0        0        0      169 2024-05-23 04:03:23.751048 fpb-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.747048 fpb-0.3/fingerprint_browser/
--rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.3/fingerprint_browser/__init__.py
--rw-rw-rw-   0        0        0    17618 2024-05-23 03:58:14.000000 fpb-0.3/fingerprint_browser/hubstudio.py
--rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.3/fingerprint_browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.750048 fpb-0.3/fpb.egg-info/
--rw-rw-rw-   0        0        0      169 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 04:03:23.751048 fpb-0.3/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-23 03:57:26.000000 fpb-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.972958 fpb-0.4/
+-rw-rw-rw-   0        0        0      169 2024-05-23 04:05:15.972958 fpb-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.965954 fpb-0.4/fingerprint_browser/
+-rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.4/fingerprint_browser/__init__.py
+-rw-rw-rw-   0        0        0    17625 2024-05-23 04:05:02.000000 fpb-0.4/fingerprint_browser/hubstudio.py
+-rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.4/fingerprint_browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.971958 fpb-0.4/fpb.egg-info/
+-rw-rw-rw-   0        0        0      169 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:05:15.972958 fpb-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-23 04:05:13.000000 fpb-0.4/setup.py
```

### Comparing `fpb-0.3/fingerprint_browser/hubstudio.py` & `fpb-0.4/fingerprint_browser/hubstudio.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import atexit
 import os.path
 import subprocess
 import re
 import typing
 import aiohttp
 import inflection
-import utils
+from . import utils
 
 
 class HubStudioAsync:
     def __init__(self, host: str = "localhost", port: int = 16000):
         self.__http_port = port
         self.__host = host
```

