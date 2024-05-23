# Comparing `tmp/esp2_gateway_adapter-0.2.1.tar.gz` & `tmp/esp2_gateway_adapter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp2_gateway_adapter-0.2.1.tar", last modified: Wed May 22 21:05:06 2024, max compression
+gzip compressed data, was "esp2_gateway_adapter-0.2.2.tar", last modified: Thu May 23 09:41:54 2024, max compression
```

## Comparing `esp2_gateway_adapter-0.2.1.tar` & `esp2_gateway_adapter-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:05:06.146676 esp2_gateway_adapter-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 21:05:01.000000 esp2_gateway_adapter-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 21:05:06.142676 esp2_gateway_adapter-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 21:05:01.000000 esp2_gateway_adapter-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:05:06.142676 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 21:05:06.000000 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-22 21:05:06.000000 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:05:06.000000 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 21:05:06.000000 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 21:05:06.000000 esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:05:06.146676 esp2_gateway_adapter-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 21:05:01.000000 esp2_gateway_adapter-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:05:06.142676 esp2_gateway_adapter-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-22 21:05:01.000000 esp2_gateway_adapter-0.2.1/src/esp3_serial_com.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-22 21:05:01.000000 esp2_gateway_adapter-0.2.1/src/esp3_tcp_com.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 09:41:54.000000 esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:41:54.073369 esp2_gateway_adapter-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/src/esp3_serial_com.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-23 09:41:47.000000 esp2_gateway_adapter-0.2.2/src/esp3_tcp_com.py
```

### Comparing `esp2_gateway_adapter-0.2.1/LICENSE` & `esp2_gateway_adapter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esp2_gateway_adapter-0.2.1/PKG-INFO` & `esp2_gateway_adapter-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
```

### Comparing `esp2_gateway_adapter-0.2.1/esp2_gateway_adapter.egg-info/PKG-INFO` & `esp2_gateway_adapter-0.2.2/esp2_gateway_adapter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
```

### Comparing `esp2_gateway_adapter-0.2.1/setup.py` & `esp2_gateway_adapter-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 required = ['eltako14bus>=0.0.46', 'enocean>=0.60.1', 'pyserial', 'pyserial-asyncio', 'aiocoap', 'zeroconf==0.132.2']
 
 
 
 setup(
     name='esp2_gateway_adapter',
-    version='0.2.1',
+    version='0.2.2',
     package_dir={"esp2_gateway_adapter":'src'},
     package=[""],
     include_package_data=True,
     install_requires=required,
     author="Philipp Grimm",
     description="Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration",
     long_description=long_description,
```

### Comparing `esp2_gateway_adapter-0.2.1/src/esp3_serial_com.py` & `esp2_gateway_adapter-0.2.2/src/esp3_serial_com.py`

 * *Files identical despite different names*

### Comparing `esp2_gateway_adapter-0.2.1/src/esp3_tcp_com.py` & `esp2_gateway_adapter-0.2.2/src/esp3_tcp_com.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,32 @@
         self._host = host
         self._port = port
 
         self.log = log or logging.getLogger('eltakobus.tcp2serial')
 
         self.__ser = None
 
+
     def run(self):
         self.logger.info('TCP2SerialCommunicator started')
         self._fire_status_change_handler(connected=False)
         while not self._stop_flag.is_set():
             try:
                 # Initialize serial port
                 if self.__ser is None:
                     self.__ser = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                     self.__ser.connect((self._host, self._port))
-                    self.__ser.settimeout(0.5)
+                    self.__ser.settimeout(1)
+
+                    # Test connection
+                    self.__ser.send(b'\xff\x00\xff' * 5)
+                    try:
+                        self.__ser.recv(1024)
+                    except socket.timeout as e:
+                        pass
 
                     self.log.info("Established TCP connection to %s:%s", self._host, self._port)
                     
                     self.is_serial_connected.set()
                     self._fire_status_change_handler(connected=True)
                     
                 # If there's messages in transmit queue
@@ -85,16 +93,14 @@
                     data = self.__ser.recv(1024)
                     # print(hex(int.from_bytes(data, "big")))
                     if data != b'IM2M':
                         self._buffer = data
                         self.parse()
                 except socket.timeout as e:
                     pass
-                except Exception as e:
-                    self.log.exception(e)
                 time.sleep(0)
 
             except Exception as e:
                 self._fire_status_change_handler(connected=False)
                 self.is_serial_connected.clear()
                 self.log.error(e)
                 self.__ser = None
```
