# Comparing `tmp/httpauth-0.3.tar.gz` & `tmp/httpauth-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpauth-0.3.tar", last modified: Sun Feb  7 18:26:01 2016, max compression
+gzip compressed data, was "httpauth-0.4.tar", last modified: Tue May 21 12:05:19 2024, max compression
```

## Comparing `httpauth-0.3.tar` & `httpauth-0.4.tar`

### file list

```diff
@@ -1,7 +1,12 @@
-drwxr-xr-x   0 j          (501) staff       (20)        0 2016-02-07 18:26:01.000000 httpauth-0.3/
--rw-r--r--   0 j          (501) staff       (20)     6711 2015-11-01 21:34:46.000000 httpauth-0.3/httpauth.py
--rw-r--r--   0 j          (501) staff       (20)       83 2014-11-11 20:31:45.000000 httpauth-0.3/Makefile
--rw-r--r--   0 j          (501) staff       (20)      601 2016-02-07 18:26:01.000000 httpauth-0.3/PKG-INFO
--rw-r--r--   0 j          (501) staff       (20)     1072 2014-11-11 20:31:45.000000 httpauth-0.3/README.rst
--rw-r--r--   0 j          (501) staff       (20)      669 2016-02-07 18:23:39.000000 httpauth-0.3/setup.py
--rw-r--r--   0 j          (501) staff       (20)     4241 2015-11-01 21:40:35.000000 httpauth-0.3/tests.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-21 12:05:19.227639 httpauth-0.4/
+-rw-r--r--   0 j          (501) wheel        (0)      748 2024-05-21 12:03:58.000000 httpauth-0.4/LICENSE
+-rw-r--r--   0 j          (501) wheel        (0)      434 2024-05-21 12:05:19.227500 httpauth-0.4/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     1197 2024-05-21 12:03:58.000000 httpauth-0.4/README.rst
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-21 12:05:19.227362 httpauth-0.4/httpauth.egg-info/
+-rw-r--r--   0 j          (501) wheel        (0)      434 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)      167 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/SOURCES.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/dependency_links.txt
+-rw-r--r--   0 j          (501) wheel        (0)        9 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/top_level.txt
+-rw-r--r--   0 j          (501) wheel        (0)     6788 2024-05-21 12:03:58.000000 httpauth-0.4/httpauth.py
+-rw-r--r--   0 j          (501) wheel        (0)       38 2024-05-21 12:05:19.227668 httpauth-0.4/setup.cfg
+-rw-r--r--   0 j          (501) wheel        (0)      522 2024-05-21 12:05:13.000000 httpauth-0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `httpauth-0.3/httpauth.py` & `httpauth-0.4/httpauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 """
 import os
 import re
 import time
 import hashlib
 try: # Python 3
     from urllib.request import parse_http_list, parse_keqv_list
+    PY2 = False
 except ImportError: # Python 2
     from urllib2 import parse_http_list, parse_keqv_list
+    PY2 = True
 
 
 def md5(x):
     return hashlib.md5(x).hexdigest()
 
 def md5_str(x):
     return md5(x.encode('utf8'))
@@ -128,15 +130,16 @@
         return response == make_auth_response(nonce, HA1, make_HA2(http_method, uri))
 
     def challenge(self, environ, start_response):
         start_response(
             '401 Authentication Required',
             [('WWW-Authenticate', make_www_authenticate_header(self.realm))],
         )
-        return ['<h1>401 - Authentication Required</h1>']
+        html = '<h1>401 - Authentication Required</h1>'
+        return [html if PY2 else html.encode()]
 
 
 class DigestFileHttpAuthMiddleware(BaseHttpAuthMiddleware):
     """
     Reads credentials from an Apache-style .htdigest file.
 
     `filelike`
```

### Comparing `httpauth-0.3/README.rst` & `httpauth-0.4/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 httpauth
 ========
 
 a WSGI middleware that secures some/all routes using HTTP Digest Authentication.
 
+.. image:: https://travis-ci.org/jonashaag/httpauth.svg?branch=master
+    :target: https://travis-ci.org/jonashaag/httpauth
+
 
 Installation
 ------------
 ::
 
    pip install httpauth
```

