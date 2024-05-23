# Comparing `tmp/balsamic-0.1.99.tar.gz` & `tmp/balsamic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.1.99.tar", last modified: Sat May 18 03:42:25 2024, max compression
+gzip compressed data, was "balsamic-0.2.0.tar", last modified: Thu May 23 21:45:06 2024, max compression
```

## Comparing `balsamic-0.1.99.tar` & `balsamic-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:42:25.885663 balsamic-0.1.99/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:42:25.885663 balsamic-0.1.99/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1702 2024-05-18 03:04:59.000000 balsamic-0.1.99/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:42:25.881663 balsamic-0.1.99/balsamic/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.1.99/balsamic/__innit__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2226 2024-05-18 02:50:42.000000 balsamic-0.1.99/balsamic/__main__.py
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1830 2024-05-18 03:40:32.000000 balsamic-0.1.99/balsamic/balsamic.py
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-18 03:42:25.885663 balsamic-0.1.99/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2237 2024-05-18 03:42:25.000000 balsamic-0.1.99/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-18 03:42:25.000000 balsamic-0.1.99/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-18 03:42:25.000000 balsamic-0.1.99/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:42:25.000000 balsamic-0.1.99/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-18 03:42:25.000000 balsamic-0.1.99/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-18 03:42:25.885663 balsamic-0.1.99/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1144 2024-05-18 03:42:08.000000 balsamic-0.1.99/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:45:06.529498 balsamic-0.2.0/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1670 2024-05-23 21:44:14.000000 balsamic-0.2.0/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/balsamic/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:32:39.000000 balsamic-0.2.0/balsamic/__innit__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2559 2024-05-23 21:43:15.000000 balsamic-0.2.0/balsamic/__main__.py
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2499 2024-05-23 21:39:01.000000 balsamic-0.2.0/balsamic/balsamic.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-23 21:45:06.529498 balsamic-0.2.0/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2204 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      241 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        9 2024-05-23 21:45:06.000000 balsamic-0.2.0/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-23 21:45:06.529498 balsamic-0.2.0/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1143 2024-05-23 21:40:18.000000 balsamic-0.2.0/setup.py
```

### Comparing `balsamic-0.1.99/PKG-INFO` & `balsamic-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.1.99
+Version: 0.2.0
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -16,26 +16,27 @@
 # Balsamic  
 balsamic is a library for sending malicious pickles to a vunlerable application, via web requests, or a malicious server or client(currently ipv4 only).  
 we will add more payloads but for now we just execute shell commands. via the oscmd payload.  
 
 ## useage (standalone)  
 web request mode  
 ```
-usage: balsamic.py webreq [-h] -s {http,https} [-m METHOD] -rh RHOST -rp RPORT [-p PARAMETER] [-co COOKIE] -P PAYLOAD [-c COMMAND]
+usage: balsamic.py webreq [-h] [-m METHOD] -u URL [-p PARAMETER] [-co COOKIE] -P PAYLOAD
+                          [-c COMMAND] [-H HEADERS]
 
 options:
   -h, --help            show this help message and exit
-  -s {http,https}, --schema {http,https}
   -m METHOD, --method METHOD
-  -rh RHOST, --rhost RHOST
-  -rp RPORT, --rport RPORT
+  -u URL, --url URL
   -p PARAMETER, --parameter PARAMETER
   -co COOKIE, --cookie COOKIE
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
+  -H HEADERS, --headers HEADERS
+
 ```
 socksend mode  
 ```
 usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS]
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `balsamic-0.1.99/README.md` & `balsamic-0.2.0/balsamic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+Metadata-Version: 2.1
+Name: balsamic
+Version: 0.2.0
+Summary: Send malicious pickles via requests or sockets
+Author: Witchdoctor (malectrica)
+Keywords: python,hack,pickle,serialization,security,sockets,web
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+
 # Balsamic  
 balsamic is a library for sending malicious pickles to a vunlerable application, via web requests, or a malicious server or client(currently ipv4 only).  
 we will add more payloads but for now we just execute shell commands. via the oscmd payload.  
 
 ## useage (standalone)  
 web request mode  
 ```
-usage: balsamic.py webreq [-h] -s {http,https} [-m METHOD] -rh RHOST -rp RPORT [-p PARAMETER] [-co COOKIE] -P PAYLOAD [-c COMMAND]
+usage: balsamic.py webreq [-h] [-m METHOD] -u URL [-p PARAMETER] [-co COOKIE] -P PAYLOAD
+                          [-c COMMAND] [-H HEADERS]
 
 options:
   -h, --help            show this help message and exit
-  -s {http,https}, --schema {http,https}
   -m METHOD, --method METHOD
-  -rh RHOST, --rhost RHOST
-  -rp RPORT, --rport RPORT
+  -u URL, --url URL
   -p PARAMETER, --parameter PARAMETER
   -co COOKIE, --cookie COOKIE
   -P PAYLOAD, --payload PAYLOAD
   -c COMMAND, --command COMMAND
+  -H HEADERS, --headers HEADERS
+
 ```
 socksend mode  
 ```
 usage: balsamic.py socksend [-h] -rh RHOST -rp RPORT -P PAYLOAD [-c COMMAND] [-s STEPS]
 
 options:
   -h, --help            show this help message and exit
```

### Comparing `balsamic-0.1.99/setup.py` & `balsamic-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.99'
+VERSION = '0.2.0'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
```

