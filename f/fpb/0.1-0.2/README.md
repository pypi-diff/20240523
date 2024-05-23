# Comparing `tmp/fpb-0.1.tar.gz` & `tmp/fpb-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpb-0.1.tar", last modified: Sat May  4 22:29:06 2024, max compression
+gzip compressed data, was "fpb-0.2.tar", last modified: Thu May 23 03:53:41 2024, max compression
```

## Comparing `fpb-0.1.tar` & `fpb-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 22:29:06.607254 fpb-0.1/
--rw-rw-rw-   0        0        0      169 2024-05-04 22:29:06.607254 fpb-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 22:29:06.595899 fpb-0.1/fingerprint_browser/
--rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.1/fingerprint_browser/__init__.py
--rw-rw-rw-   0        0        0    17408 2024-05-04 22:17:54.000000 fpb-0.1/fingerprint_browser/hubstudio.py
-drwxrwxrwx   0        0        0        0 2024-05-04 22:29:06.607254 fpb-0.1/fpb.egg-info/
--rw-rw-rw-   0        0        0      169 2024-05-04 22:29:06.000000 fpb-0.1/fpb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-04 22:29:06.000000 fpb-0.1/fpb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 22:29:06.000000 fpb-0.1/fpb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-04 22:29:06.000000 fpb-0.1/fpb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-04 22:29:06.000000 fpb-0.1/fpb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 22:29:06.607254 fpb-0.1/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-04 20:20:57.000000 fpb-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.596844 fpb-0.2/
+-rw-rw-rw-   0        0        0      169 2024-05-23 03:53:41.595845 fpb-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.583849 fpb-0.2/fingerprint_browser/
+-rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.2/fingerprint_browser/__init__.py
+-rw-rw-rw-   0        0        0    17547 2024-05-23 03:47:41.000000 fpb-0.2/fingerprint_browser/hubstudio.py
+-rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.2/fingerprint_browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.595845 fpb-0.2/fpb.egg-info/
+-rw-rw-rw-   0        0        0      169 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:53:41.596844 fpb-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-23 03:47:58.000000 fpb-0.2/setup.py
```

### Comparing `fpb-0.1/fingerprint_browser/hubstudio.py` & `fpb-0.2/fingerprint_browser/hubstudio.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import atexit
 import os.path
 import subprocess
 import re
 import typing
 import aiohttp
 import inflection
+import utils
 
 
 class HubStudioAsync:
     def __init__(self, host: str = "localhost", port: int = 16000):
         self.__http_port = port
         self.__host = host
 
@@ -57,15 +58,21 @@
         p = await asyncio.create_subprocess_exec(
             os.path.join(client_path, "hubstudio_connector.exe"),
             *cmds,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             creationflags=subprocess.CREATE_NO_WINDOW,
         )
-        atexit.register(p.kill)
+
+        def on_exit():
+            p.kill()
+            utils.terminate_process_by_name("hubstudio_connector.exe")
+
+        atexit.register(on_exit)
+
         while True:
             output_line = await p.stdout.readline()
             output_line = output_line.decode().strip()
             if echo:
                 print(output_line)
             if re.match(r'Program started: +{"\d+":"hubstudio_connector.exe"', output_line):
                 break
```

