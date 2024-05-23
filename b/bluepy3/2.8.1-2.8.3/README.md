# Comparing `tmp/bluepy3-2.8.1.tar.gz` & `tmp/bluepy3-2.8.3.tar.gz`

## Comparing `bluepy3-2.8.1.tar` & `bluepy3-2.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/Makefile
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/__init__.py
--rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/blescan.py
--rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0        0        0    40922 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/btle.py
--rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/get_services.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/helpermaker.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/py.typed
--rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/uuids.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/version.h
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.47.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.50.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.60.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.66.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.68.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.70.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.71.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.72.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.73.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.75.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.76.h
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.8.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.8.1/LICENSE
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.8.1/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.8.1/pyproject.toml
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/Makefile
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/__init__.py
+-rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/blescan.py
+-rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0        0        0    41041 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/btle.py
+-rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/get_services.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/helpermaker.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/py.typed
+-rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/uuids.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/version.h
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.47.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.50.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.60.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.66.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.68.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.70.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.71.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.72.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.73.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.75.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.3/bluepy3/config/config.5.76.h
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.8.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.8.3/LICENSE
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.8.3/README.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.8.3/PKG-INFO
```

### Comparing `bluepy3-2.8.1/bluepy3/Makefile` & `bluepy3-2.8.3/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/blescan.py` & `bluepy3-2.8.3/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/bluepy3-helper.c` & `bluepy3-2.8.3/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/btle.py` & `bluepy3-2.8.3/bluepy3/btle.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,19 +437,19 @@
     def __eq__(self, other: Any) -> bool:
         return self.binVal == UUID(other).binVal
 
     def __hash__(self) -> int:
         return hash(self.binVal)
 
     def __str__(self) -> str:
-        s = binascii.b2a_hex(self.binVal).decode("utf-8")
+        s: str = binascii.b2a_hex(self.binVal).decode("utf-8")
         return "-".join([s[0:8], s[8:12], s[12:16], s[16:20], s[20:32]])
 
     def getCommonName(self) -> str:
-        s = AssignedNumbers.getCommonName(self)
+        s: str = AssignedNumbers.getCommonName(self)
         if s:
             return s
         s = str(self)
         if s.endswith("-0000-1000-8000-00805f9b34fb"):
             s = s[0:8]
             if s.startswith("0000"):
                 s = s[4:]
@@ -580,15 +580,15 @@
                 # Scan response when we weren't interested. Ignore it
                 continue
             raise BTLEInternalError(f"Unexpected response ({respType})", resp)
 
     def _writeCmd(self, cmd) -> None:
         if self._helper is None:
             raise BTLEInternalError("Helper not started (did you call connect()?)")
-        DBG(f"    -btle- Sent:   {cmd}")
+        DBG(f"    -btle- Sent:   {cmd.strip()}")
         self._helper.stdin.write(cmd)  # type:ignore[union-attr]
         self._helper.stdin.flush()  # type:ignore[union-attr]
 
     @staticmethod
     def parseResp(line: str) -> dict[str, list[Any]]:
         val: Any
         resp: dict[str, list] = {}
@@ -618,20 +618,20 @@
     def withDelegate(self, delegate_: DefaultDelegate) -> Self:
         self.delegate = delegate_
         return self
 
 
 class Peripheral(Bluepy3Helper):
     # fmt: off
-    def __init__(self, addr: str = "", addrType: str = ADDR_TYPE_PUBLIC, iface: str = "", timeout: float = BTLE_TIMEOUT) -> None:
+    def __init__(self, addr: str = "", addrType: str = ADDR_TYPE_PUBLIC, iface=None, timeout: float = BTLE_TIMEOUT) -> None:
         Bluepy3Helper.__init__(self)
         self._serviceMap: dict = {}  # Indexed by UUID
         self.addr: str = addr
         self.addrType: str = addrType
-        self.iface: str = iface
+        self.iface = iface
 
         if isinstance(addr, ScanEntry):
             self._connect(addr.addr, addr.addrType, addr.iface, timeout)
         elif addr:
             self._connect(addr, addrType, iface, timeout)
     # fmt: on
 
@@ -673,28 +673,28 @@
     def _readCharacteristicByUUID(self, uuid, startHnd: int, endHnd: int) -> dict[str, list[Any]]:
         # Not used at present
         self._writeCmd(f"rdu {UUID(uuid)} {startHnd:X} {endHnd:X}\n")
         return self._getResp(["rd"])
 
     # keep this with connect()
     def _connect(
-        self, addr: str, addrType=ADDR_TYPE_PUBLIC, iface="", timeout=BTLE_TIMEOUT
+        self, addr: str, addrType=ADDR_TYPE_PUBLIC, iface=None, timeout=BTLE_TIMEOUT
     ) -> None:
         max_retries = 5
         if len(addr.split(":")) != 6:
             raise ValueError(f"(btle.py) Expected MAC address, got {repr(addr)}")
         if addrType not in (ADDR_TYPE_PUBLIC, ADDR_TYPE_RANDOM):
             raise ValueError(f"(btle.py) Expected address type public or random, got {addrType}")
         self.retries = max_retries
         while self.retries > 0:
             self._startHelper(iface)
             self.addr = addr
             self.addrType = addrType
             self.iface = iface
-            if iface:
+            if iface is not None:
                 self._writeCmd(f"conn {addr} {addrType} hci{str(iface)}\n")
             else:
                 self._writeCmd(f"conn {addr} {addrType}\n")
             rsp: dict[str, list[Any]] = self._getResp(["stat"], timeout)
             _timeout_exception = BTLEConnectTimeout(
                 f"Timed out while trying to connect to peripheral {addr}, "
                 f"addr type: {addrType}, interface {iface}, timeout={timeout}",
@@ -705,20 +705,21 @@
             while rsp and rsp["state"][0] == "tryconn":
                 rsp = self._getResp(["stat"], timeout)
             if rsp and rsp["state"][0] == "conn":
                 DBG("    -btle- Succesfully connected.")
                 # successful
                 self.retries = 0
             if not rsp or rsp["state"][0] != "conn":
-                self._stopHelper()
+                self._stopHelper()  # todo: should this be disconnect() ?
                 if not rsp:
                     raise _timeout_exception
-                DBG(f"*** -btle-  Failed to connect. ({self.retries})")
+                DBG(f"*** -btle-  Failed to connect. ({self.retries})\n")
                 time.sleep(0.5 * (max_retries - self.retries))
                 if self.retries <= 1:
+                    # TODO: disconnect here to prevent stale connections
                     raise BTLEConnectError(
                         f"Failed to connect to peripheral {addr}, "
                         f"addr type: {addrType}, interface {iface}, timeout={timeout}",
                         rsp,
                     )
             self.retries -= 1
 
@@ -1067,15 +1068,15 @@
 
     my_device_address: str = sys.argv[1]
     if len(sys.argv) == 3:
         my_address_type: str = sys.argv[2]
     else:
         my_address_type = ADDR_TYPE_PUBLIC
     print(f"Connecting to: {my_device_address}, address type: {my_address_type}")
-    conn = Peripheral(my_device_address, my_address_type)
+    conn = Peripheral(my_device_address)
     try:
         for service in conn.services:
             print(f"{str(service)}:")
             for ch in service.getCharacteristics():
                 print(f"    {ch}, hnd={hex(ch.handle)}, supports {ch.propertiesToString()}")
                 chName = AssignedNumbers.getCommonName(ch.uuid)
                 if ch.supportsRead():
```

### Comparing `bluepy3-2.8.1/bluepy3/get_services.py` & `bluepy3-2.8.3/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/helpermaker.py` & `bluepy3-2.8.3/bluepy3/helpermaker.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/uuids.json` & `bluepy3-2.8.3/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.47.h` & `bluepy3-2.8.3/bluepy3/config/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.50.h` & `bluepy3-2.8.3/bluepy3/config/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.60.h` & `bluepy3-2.8.3/bluepy3/config/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.66.h` & `bluepy3-2.8.3/bluepy3/config/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.68.h` & `bluepy3-2.8.3/bluepy3/config/config.5.68.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.70.h` & `bluepy3-2.8.3/bluepy3/config/config.5.70.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.71.h` & `bluepy3-2.8.3/bluepy3/config/config.5.71.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.72.h` & `bluepy3-2.8.3/bluepy3/config/config.5.72.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.73.h` & `bluepy3-2.8.3/bluepy3/config/config.5.73.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.75.h` & `bluepy3-2.8.3/bluepy3/config/config.5.75.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/bluepy3/config/config.5.76.h` & `bluepy3-2.8.3/bluepy3/config/config.5.76.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/.gitignore` & `bluepy3-2.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/LICENSE` & `bluepy3-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/README.md` & `bluepy3-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-2.8.1/pyproject.toml` & `bluepy3-2.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bluepy3"
-version = "2.8.1"  # latest/current distribution version
+version = "2.8.3"  # latest/current distribution version
 # version = "2.7.5"  # latest test version
 description = "A Python3 module for interfacing with Bluetooth LE devices on Linux."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 # license-files = { paths = ["LICENSE"] }
 authors = [
```

### Comparing `bluepy3-2.8.1/PKG-INFO` & `bluepy3-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bluepy3
-Version: 2.8.1
+Version: 2.8.3
 Summary: A Python3 module for interfacing with Bluetooth LE devices on Linux.
 Project-URL: Homepage, https://github.com/Mausy5043/bluepy3
 Project-URL: Bug Tracker, https://github.com/Mausy5043/bluepy3/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Keywords: BLE,Bluetooth,Bluetooth Low Energy,Bluetooth Smart,Raspberry Pi
```

