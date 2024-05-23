# Comparing `tmp/godice-0.1.0.tar.gz` & `tmp/godice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godice-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "godice-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `godice-0.1.0.tar` & `godice-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      813 2023-09-27 11:37:45.196668 godice-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2023-09-27 11:37:45.196668 godice-0.1.0/.gitignore
--rw-r--r--   0        0        0     8258 2023-09-27 11:37:45.196668 godice-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     2314 2023-09-27 11:37:45.196668 godice-0.1.0/README.md
--rw-r--r--   0        0        0      254 2023-09-27 11:37:45.196668 godice-0.1.0/godice/__init__.py
--rw-r--r--   0        0        0     2861 2023-09-27 11:37:45.196668 godice-0.1.0/godice/demo.py
--rw-r--r--   0        0        0     5484 2023-09-27 11:37:45.196668 godice-0.1.0/godice/dice.py
--rw-r--r--   0        0        0     1366 2023-09-27 11:37:45.196668 godice-0.1.0/godice/factory.py
--rw-r--r--   0        0        0     4945 2023-09-27 11:37:45.196668 godice-0.1.0/godice/xyzinterpret.py
--rw-r--r--   0        0        0      659 2023-09-27 11:37:45.196668 godice-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 godice-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      893 2024-05-23 14:50:26.665313 godice-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2024-05-23 14:50:26.665313 godice-0.1.2/.gitignore
+-rw-r--r--   0        0        0     8258 2024-05-23 14:50:26.665313 godice-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     2307 2024-05-23 14:50:26.665313 godice-0.1.2/README.md
+-rw-r--r--   0        0        0      254 2024-05-23 14:50:26.665313 godice-0.1.2/godice/__init__.py
+-rw-r--r--   0        0        0     2842 2024-05-23 14:50:26.665313 godice-0.1.2/godice/demo.py
+-rw-r--r--   0        0        0     5506 2024-05-23 14:50:26.665313 godice-0.1.2/godice/dice.py
+-rw-r--r--   0        0        0     1492 2024-05-23 14:50:26.665313 godice-0.1.2/godice/factory.py
+-rw-r--r--   0        0        0     4945 2024-05-23 14:50:26.665313 godice-0.1.2/godice/xyzinterpret.py
+-rw-r--r--   0        0        0      684 2024-05-23 14:50:26.665313 godice-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 godice-0.1.2/PKG-INFO
```

### Comparing `godice-0.1.0/.github/workflows/publish.yml` & `godice-0.1.2/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -19,12 +19,16 @@
           with:
             python-version: 3.9
             
         - name: Install Flit
           run: |
               python -m pip install flit
 
+        - name: Build Flit
+          run: |
+              python -m flit build
+
         - name: Publish
           env:
             FLIT_USERNAME: __token__
             FLIT_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           run: python -m flit publish
```

### Comparing `godice-0.1.0/.gitignore` & `godice-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `godice-0.1.0/LICENSE.md` & `godice-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `godice-0.1.0/README.md` & `godice-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # GoDice Python API
 
 ## Overview
 
 Use the GoDice Python API to integrate GoDice functionality into your own Python applications
 
-![PyPI - Version](https://img.shields.io/pypi/v/godice)
+[![PyPI version](https://badge.fury.io/py/godice.svg)](https://pypi.org/project/godice)
 
 **Supported features:**
 
 * Turn ON/OFF GoDice RGB LEDs
 * Read color (dots color)
 * Read battery level
 * Get notifications regarding the die state (Rolling or Stable and get the outcome number)
@@ -38,20 +38,19 @@
 import asyncio
 import bleak
 import godice
 
 
 async def main():
     mac = "00:00:00:00:00:00"
-    client = bleak.BleakClient(mac, timeout=15)
 
     # Python context manager (async with) is used for convenient connection handling
     # Device stays connected during `async with` block execution and auto-disconnected on block finish
     # Otherwise, dice.connect/dice.disconnect can be used instead 
-    async with godice.create(client, godice.Shell.D6) as dice:
+    async with godice.create(mac, godice.Shell.D6, timeout=30) as dice:
 		print("Connected")
         blue_rgb = (0, 0, 255)
         yellow_rgb = (255, 255, 0)
         off_rgb = (0, 0, 0)
         await dice.set_led(blue_rgb, yellow_rgb)
 
         color = await dice.get_color()
```

### Comparing `godice-0.1.0/godice/demo.py` & `godice-0.1.2/godice/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 import bleak
 import godice
 
 
 async def main():
     print("Discovering GoDice devices...")
     discovery_res = await bleak.BleakScanner.discover(timeout=10, return_adv=True)
-    dev_advdata_tuples = discovery_res.values()
-    dev_advdata_tuples = filter_godice_devices(dev_advdata_tuples)
+    device_advdata_tuples = discovery_res.values()
+    device_advdata_tuples = filter_godice_devices(device_advdata_tuples)
 
     print("Discovered devices...")
-    print_device_info(dev_advdata_tuples)
+    print_device_info(device_advdata_tuples)
 
     print("Connecting to a closest device...")
-    dev, _adv_data = select_closest_device(dev_advdata_tuples)
-    client = bleak.BleakClient(dev, timeout=15)
+    device, _adv_data = select_closest_device(device_advdata_tuples)
 
     # Python context manager (async with) is used for convenient connection handling
     # Device stays connected during `async with` block execution and auto-disconnected on block finish
     # Otherwise, dice.connect/dice.disconnect can be used instead 
-    async with godice.create(client, godice.Shell.D6) as dice:
-        print(f"Connected to {dev.name}")
+    async with godice.create(device.address, godice.Shell.D6) as dice:
+        print(f"Connected to {device.name}")
 
         blue_rgb = (0, 0, 255)
         yellow_rgb = (255, 255, 0)
         off_rgb = (0, 0, 0)
         await dice.set_led(blue_rgb, yellow_rgb)
 
         color = await dice.get_color()
```

### Comparing `godice-0.1.0/godice/dice.py` & `godice-0.1.2/godice/dice.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,17 @@
         self._client = ble_client
         self._rx_char = None
         self._tx_char = None
         self._color = None
         self._color_upd_q = asyncio.Queue()
         self._battery_lvl_upd_q = asyncio.Queue()
         self._xyz_interpret_fn = None
-        self._nop_cb = lambda _: None
-        self._position_upd_cb = self._nop_cb
+        async def _noop_cb(_num, _stab_descr):
+            pass
+        self._position_upd_cb = _noop_cb
 
     async def connect(self):
         await self._client.connect()
         self._tx_char = self._client.services.get_characteristic(
             "6e400002-b5a3-f393-e0a9-e50e24dcca9e"
         )
         self._rx_char = self._client.services.get_characteristic(
```

### Comparing `godice-0.1.0/godice/factory.py` & `godice-0.1.2/godice/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     Shell.D20: xyzinterpret.get_rolled_number_d20,
     Shell.D4: xyzinterpret.get_rolled_number_d4,
     Shell.D8: xyzinterpret.get_rolled_number_d8,
     Shell.D12: xyzinterpret.get_rolled_number_d12,
 }
 
 
-def create(ble_client: bleak.BleakClient, dice_shell: Shell):
+def create(ble_address: str, dice_shell: Shell, timeout: int=15, disconnect_cb=None):
     """
     Creates Dice API object representing the specified type of a dice
     :param ble_client: BleakClient
     :param dice_shell: Shell
     """
+    ble_client = bleak.BleakClient(ble_address, timeout=timeout, disconnected_callback=disconnect_cb)
     _dice = dice.Dice(ble_client)
     set_shell(_dice, dice_shell)
     return _dice
 
 
 def set_shell(_dice: dice.Dice, dice_shell: Shell):
     """
```

### Comparing `godice-0.1.0/godice/xyzinterpret.py` & `godice-0.1.2/godice/xyzinterpret.py`

 * *Files identical despite different names*

### Comparing `godice-0.1.0/pyproject.toml` & `godice-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "godice"
+version = "0.1.2"
+description = "A Python API for GoDice"
 authors = [
-    {name = "Guy Levi", email = "todo_update@it.com"},
+    {name = "Guy Levi", email = "guyguylevi60@gmail.com"},
     {name = "Anton Ptashnik", email = "iavtomator@gmail.com"},
 ]
 license = {file = "LICENSE.md"}
 classifiers = [
     "Framework :: AsyncIO",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
 ]
 readme = "README.md"
-dynamic = ["version", "description"]
 dependencies = [
     "bleak >=0.20.2",
 ]
 requires-python = ">=3.6"
 
 [project.urls]
 Home = "https://github.com/ParticulaCode/GoDicePythonAPI"
```

### Comparing `godice-0.1.0/PKG-INFO` & `godice-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: godice
-Version: 0.1.0
-Summary: Use the GoDice Python API to integrate GoDice functionality into your own Python applications
-Author-email: Guy Levi <todo_update@it.com>, Anton Ptashnik <iavtomator@gmail.com>
+Version: 0.1.2
+Summary: A Python API for GoDice
+Author-email: Guy Levi <guyguylevi60@gmail.com>, Anton Ptashnik <iavtomator@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Dist: bleak >=0.20.2
@@ -15,15 +15,15 @@
 
 # GoDice Python API
 
 ## Overview
 
 Use the GoDice Python API to integrate GoDice functionality into your own Python applications
 
-![PyPI - Version](https://img.shields.io/pypi/v/godice)
+[![PyPI version](https://badge.fury.io/py/godice.svg)](https://pypi.org/project/godice)
 
 **Supported features:**
 
 * Turn ON/OFF GoDice RGB LEDs
 * Read color (dots color)
 * Read battery level
 * Get notifications regarding the die state (Rolling or Stable and get the outcome number)
@@ -52,20 +52,19 @@
 import asyncio
 import bleak
 import godice
 
 
 async def main():
     mac = "00:00:00:00:00:00"
-    client = bleak.BleakClient(mac, timeout=15)
 
     # Python context manager (async with) is used for convenient connection handling
     # Device stays connected during `async with` block execution and auto-disconnected on block finish
     # Otherwise, dice.connect/dice.disconnect can be used instead 
-    async with godice.create(client, godice.Shell.D6) as dice:
+    async with godice.create(mac, godice.Shell.D6, timeout=30) as dice:
 		print("Connected")
         blue_rgb = (0, 0, 255)
         yellow_rgb = (255, 255, 0)
         off_rgb = (0, 0, 0)
         await dice.set_led(blue_rgb, yellow_rgb)
 
         color = await dice.get_color()
```

