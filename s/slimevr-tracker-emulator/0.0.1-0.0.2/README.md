# Comparing `tmp/slimevr_tracker_emulator-0.0.1.tar.gz` & `tmp/slimevr_tracker_emulator-0.0.2.tar.gz`

## Comparing `slimevr_tracker_emulator-0.0.1.tar` & `slimevr_tracker_emulator-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/svr.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/__init__.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/async_tracker_emulator.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/tracker_packet.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/tracker_types.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/LICENSE
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/README.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/svr.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/__init__.py
+-rw-r--r--   0        0        0     8195 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/async_tracker_emulator.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/tracker_packet.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/tracker_types.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/LICENSE
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/README.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 slimevr_tracker_emulator-0.0.2/PKG-INFO
```

### Comparing `slimevr_tracker_emulator-0.0.1/.github/workflows/publish-to-pypi.yml` & `slimevr_tracker_emulator-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/async_tracker_emulator.py` & `slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/async_tracker_emulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import asyncio
 from socket import AF_INET, SOCK_DGRAM, socket
 import numpy as np
 
-from src.slimevr_tracker_emulator.tracker_packet import DatagramPacket
-from src.slimevr_tracker_emulator.tracker_types import Helper, ImuType, PacketType, SensorAcceleration, SensorData, SensorPosition, SensorRotationQuat, SensorState
+from slimevr_tracker_emulator.tracker_packet import DatagramPacket
+from slimevr_tracker_emulator.tracker_types import Helper, ImuType, PacketType, SensorAcceleration, SensorData, SensorPosition, SensorRotationQuat, SensorState
 
 
 class SlimeVRTrackerEmulatorAsync():
 
     _packet_number: int
     _packet_number_lock: asyncio.Lock
```

### Comparing `slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/tracker_packet.py` & `slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/tracker_packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import struct
-from src.slimevr_tracker_emulator.tracker_types import BoardType, HardwareMcuType, ImuType, PacketType, SensorData
+from slimevr_tracker_emulator.tracker_types import BoardType, HardwareMcuType, ImuType, PacketType, SensorData
 
 
 class DatagramPacket:
     buf: bytearray
     offset: int
 
     def __init__(self, buf=None):
```

### Comparing `slimevr_tracker_emulator-0.0.1/src/slimevr_tracker_emulator/tracker_types.py` & `slimevr_tracker_emulator-0.0.2/src/slimevr_tracker_emulator/tracker_types.py`

 * *Files identical despite different names*

### Comparing `slimevr_tracker_emulator-0.0.1/LICENSE` & `slimevr_tracker_emulator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slimevr_tracker_emulator-0.0.1/pyproject.toml` & `slimevr_tracker_emulator-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "slimevr_tracker_emulator"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ameharu", email="me@ameha.ru" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `slimevr_tracker_emulator-0.0.1/PKG-INFO` & `slimevr_tracker_emulator-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.3
 Name: slimevr_tracker_emulator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Project-URL: Homepage, https://github.com/ameharoo/PythonSlimeVRTracker
 Project-URL: Issues, https://github.com/ameharoo/PythonSlimeVRTracker/issues
 Author-email: Ameharu <me@ameha.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
+[![PyPI - latest](https://img.shields.io/pypi/v/slimevr-tracker-emulator?label=latest&logo=pypi)](https://pypi.org/project/slimevr-tracker-emulator/)
+[![PyPI - Python](https://img.shields.io/pypi/pyversions/slimevr-tracker-emulator?logo=pypi)](https://pypi.org/project/slimevr-tracker-emulator/)
+
 # SlimeVR Tracker Emulator
 
-Simple **async lib** for [SlimeVR](https://github.com/SlimeVR) tracker emulation
+Simple **async lib** for [SlimeVR](https://github.com/SlimeVR) tracker emulation
+
+> See [srv.py](https://github.com/ameharoo/PythonSlimeVRTracker/blob/master/srv.py) for examples
```

