# Comparing `tmp/ahk_server-0.0.1.tar.gz` & `tmp/ahk_server-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk_server-0.0.1.tar", last modified: Wed May 22 03:48:03 2024, max compression
+gzip compressed data, was "ahk_server-0.1.0.tar", last modified: Thu May 23 06:06:01 2024, max compression
```

## Comparing `ahk_server-0.0.1.tar` & `ahk_server-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:03.314109 ahk_server-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-22 03:47:59.000000 ahk_server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-22 03:48:03.314109 ahk_server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-22 03:47:59.000000 ahk_server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:03.314109 ahk_server-0.0.1/ahk_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:47:59.000000 ahk_server-0.0.1/ahk_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-22 03:47:59.000000 ahk_server-0.0.1/ahk_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:03.314109 ahk_server-0.0.1/ahk_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-22 03:48:03.000000 ahk_server-0.0.1/ahk_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 03:48:03.000000 ahk_server-0.0.1/ahk_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:48:03.000000 ahk_server-0.0.1/ahk_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 03:48:03.000000 ahk_server-0.0.1/ahk_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 03:48:03.000000 ahk_server-0.0.1/ahk_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 03:47:59.000000 ahk_server-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-22 03:48:03.314109 ahk_server-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:47:59.000000 ahk_server-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:06:01.729187 ahk_server-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 06:05:56.000000 ahk_server-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 06:06:01.729187 ahk_server-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-23 06:05:56.000000 ahk_server-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:06:01.725187 ahk_server-0.1.0/ahk_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 06:05:56.000000 ahk_server-0.1.0/ahk_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 06:05:56.000000 ahk_server-0.1.0/ahk_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-23 06:05:56.000000 ahk_server-0.1.0/ahk_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:06:01.729187 ahk_server-0.1.0/ahk_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 06:06:01.000000 ahk_server-0.1.0/ahk_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 06:06:01.000000 ahk_server-0.1.0/ahk_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:06:01.000000 ahk_server-0.1.0/ahk_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 06:06:01.000000 ahk_server-0.1.0/ahk_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 06:06:01.000000 ahk_server-0.1.0/ahk_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 06:05:56.000000 ahk_server-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-23 06:06:01.729187 ahk_server-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:05:56.000000 ahk_server-0.1.0/setup.py
```

### Comparing `ahk_server-0.0.1/LICENSE` & `ahk_server-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk_server-0.0.1/PKG-INFO` & `ahk_server-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk-server
-Version: 0.0.1
+Version: 0.1.0
 Summary: An AutoHotkey server allowing remote clients to execute ahk functionality
 Home-page: https://github.com/spyoungtech/ahk-server
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/ahk-server
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk-server
@@ -46,18 +46,29 @@
 Requires you have AutoHotkey installed. See [ahk readme](https://github.com/spyoungtech/ahk) for non-python dependencies.
 
 ## Usage
 
 To start the server:
 
 ```bash
+python -m ahk_server
+```
+This accepts two optional command line parameters: `--host` and `--port`. Alternatively, you can also configure the host 
+and port by setting the environment variables `AHK_SERVER_HOST` and `AHK_SERVER_PORT`.
+
+Alternatively still, you can also invoke the server using `uvicorn`
+```bash
 uvicorn ahk_server.app:app
 ```
 
-For the client project, see: [ahk-client](https://github.com/spyoungtech/ahk-client).
+## Standalone release
+
+`ahk-server` is also available in a standalone exe release which can be found in the [releases page](https://github.com/spyoungtech/ahk-server/releases)
+
+For connecting to the server, see the client project: [ahk-client](https://github.com/spyoungtech/ahk-client).
 
 
 ## Status
 
 This project (and its client counterpart) is usable, but in **very** early stages of development. 
 Notably, it does not currently include any authentication mechanisms for securing server connections, so use with caution.
```

### Comparing `ahk_server-0.0.1/ahk_server/app.py` & `ahk_server-0.1.0/ahk_server/app.py`

 * *Files identical despite different names*

### Comparing `ahk_server-0.0.1/ahk_server.egg-info/PKG-INFO` & `ahk_server-0.1.0/ahk_server.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk-server
-Version: 0.0.1
+Version: 0.1.0
 Summary: An AutoHotkey server allowing remote clients to execute ahk functionality
 Home-page: https://github.com/spyoungtech/ahk-server
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/ahk-server
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk-server
@@ -46,18 +46,29 @@
 Requires you have AutoHotkey installed. See [ahk readme](https://github.com/spyoungtech/ahk) for non-python dependencies.
 
 ## Usage
 
 To start the server:
 
 ```bash
+python -m ahk_server
+```
+This accepts two optional command line parameters: `--host` and `--port`. Alternatively, you can also configure the host 
+and port by setting the environment variables `AHK_SERVER_HOST` and `AHK_SERVER_PORT`.
+
+Alternatively still, you can also invoke the server using `uvicorn`
+```bash
 uvicorn ahk_server.app:app
 ```
 
-For the client project, see: [ahk-client](https://github.com/spyoungtech/ahk-client).
+## Standalone release
+
+`ahk-server` is also available in a standalone exe release which can be found in the [releases page](https://github.com/spyoungtech/ahk-server/releases)
+
+For connecting to the server, see the client project: [ahk-client](https://github.com/spyoungtech/ahk-client).
 
 
 ## Status
 
 This project (and its client counterpart) is usable, but in **very** early stages of development. 
 Notably, it does not currently include any authentication mechanisms for securing server connections, so use with caution.
```

### Comparing `ahk_server-0.0.1/setup.cfg` & `ahk_server-0.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk-server
-version = 0.0.1
+version = 0.1.0
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = An AutoHotkey server allowing remote clients to execute ahk functionality
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk-server
 project_urls =
```

