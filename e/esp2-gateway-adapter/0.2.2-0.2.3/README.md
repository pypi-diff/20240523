# Comparing `tmp/esp2_gateway_adapter-0.2.2.tar.gz` & `tmp/esp2_gateway_adapter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp2_gateway_adapter-0.2.2.tar", last modified: Thu May 23 09:41:54 2024, max compression
+gzip compressed data, was "esp2_gateway_adapter-0.2.3.tar", last modified: Thu May 23 11:24:00 2024, max compression
```

## Comparing `esp2_gateway_adapter-0.2.2.tar` & `esp2_gateway_adapter-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/src/esp3_serial_com.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/src/esp3_tcp_com.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:24:00.985642 esp2_gateway_adapter-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 11:23:56.000000 esp2_gateway_adapter-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 11:24:00.985642 esp2_gateway_adapter-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 11:23:56.000000 esp2_gateway_adapter-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:24:00.985642 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 11:24:00.000000 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 11:24:00.000000 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:24:00.000000 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 11:24:00.000000 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 11:24:00.000000 esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:24:00.985642 esp2_gateway_adapter-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 11:23:56.000000 esp2_gateway_adapter-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:24:00.985642 esp2_gateway_adapter-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-23 11:23:56.000000 esp2_gateway_adapter-0.2.3/src/esp3_serial_com.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-23 11:23:56.000000 esp2_gateway_adapter-0.2.3/src/esp3_tcp_com.py
```

### Comparing `esp2_gateway_adapter-0.2.2/LICENSE` & `esp2_gateway_adapter-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esp2_gateway_adapter-0.2.2/PKG-INFO` & `esp2_gateway_adapter-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
```

### Comparing `esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/PKG-INFO` & `esp2_gateway_adapter-0.2.3/esp2_gateway_adapter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
```

### Comparing `esp2_gateway_adapter-0.2.2/setup.py` & `esp2_gateway_adapter-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 required = ['eltako14bus>=0.0.46', 'enocean>=0.60.1', 'pyserial', 'pyserial-asyncio', 'aiocoap', 'zeroconf==0.132.2']
 
 
 
 setup(
     name='esp2_gateway_adapter',
-    version='0.2.2',
+    version='0.2.3',
     package_dir={"esp2_gateway_adapter":'src'},
     package=[""],
     include_package_data=True,
     install_requires=required,
     author="Philipp Grimm",
     description="Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration",
     long_description=long_description,
```

### Comparing `esp2_gateway_adapter-0.2.2/src/esp3_serial_com.py` & `esp2_gateway_adapter-0.2.3/src/esp3_serial_com.py`

 * *Files identical despite different names*

### Comparing `esp2_gateway_adapter-0.2.2/src/esp3_tcp_com.py` & `esp2_gateway_adapter-0.2.3/src/esp3_tcp_com.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,19 +42,24 @@
                  port,
                  log=None, 
                  callback=None, 
                  reconnection_timeout:float=10,
                  esp2_translation_enabled:bool=False,  
                  auto_reconnect=True):
         
+        self.__recon_time = reconnection_timeout
+        self.esp2_translation_enabled = esp2_translation_enabled
+        self._outside_callback = callback
+        self._auto_reconnect = auto_reconnect
+        
         super(TCP2SerialCommunicator, self).__init__(None, log, callback, None, reconnection_timeout, esp2_translation_enabled, auto_reconnect)
 
         self._host = host
         self._port = port
-
+        
         self.log = log or logging.getLogger('eltakobus.tcp2serial')
 
         self.__ser = None
 
 
     def run(self):
         self.logger.info('TCP2SerialCommunicator started')
```

