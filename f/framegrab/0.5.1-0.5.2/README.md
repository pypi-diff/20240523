# Comparing `tmp/framegrab-0.5.1.tar.gz` & `tmp/framegrab-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.5.1.tar", max compression
+gzip compressed data, was "framegrab-0.5.2.tar", max compression
```

## Comparing `framegrab-0.5.1.tar` & `framegrab-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2024-05-16 19:05:28.745376 framegrab-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     9217 2024-05-16 19:05:28.745376 framegrab-0.5.1/README.md
--rw-r--r--   0        0        0      732 2024-05-16 19:05:28.745376 framegrab-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      512 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/__init__.py
--rw-r--r--   0        0        0     1600 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/autodiscover.py
--rw-r--r--   0        0        0     2102 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/clitools.py
--rwxr-xr-x   0        0        0      297 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/main.py
--rw-r--r--   0        0        0     1843 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/preview.py
--rw-r--r--   0        0        0    42610 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2533 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/motion.py
--rw-r--r--   0        0        0      698 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/unavailable_module.py
--rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 framegrab-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-23 18:34:30.508812 framegrab-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     9217 2024-05-23 18:34:30.508812 framegrab-0.5.2/README.md
+-rw-r--r--   0        0        0      732 2024-05-23 18:34:30.508812 framegrab-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-05-23 18:34:30.508812 framegrab-0.5.2/src/framegrab/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:34:30.508812 framegrab-0.5.2/src/framegrab/cli/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-23 18:34:30.508812 framegrab-0.5.2/src/framegrab/cli/autodiscover.py
+-rw-r--r--   0        0        0     2102 2024-05-23 18:34:30.508812 framegrab-0.5.2/src/framegrab/cli/clitools.py
+-rwxr-xr-x   0        0        0      297 2024-05-23 18:34:30.512812 framegrab-0.5.2/src/framegrab/cli/main.py
+-rw-r--r--   0        0        0     1843 2024-05-23 18:34:30.512812 framegrab-0.5.2/src/framegrab/cli/preview.py
+-rw-r--r--   0        0        0    44950 2024-05-23 18:34:30.512812 framegrab-0.5.2/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2533 2024-05-23 18:34:30.512812 framegrab-0.5.2/src/framegrab/motion.py
+-rw-r--r--   0        0        0      698 2024-05-23 18:34:30.512812 framegrab-0.5.2/src/framegrab/unavailable_module.py
+-rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 framegrab-0.5.2/PKG-INFO
```

### Comparing `framegrab-0.5.1/LICENSE.txt` & `framegrab-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/README.md` & `framegrab-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/pyproject.toml` & `framegrab-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "framegrab"
-version = "0.5.1"
+version = "0.5.2"
 description = "Easily grab frames from cameras or streams"
 authors = ["Groundlight <info@groundlight.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.groundlight.ai/"
 repository = "https://github.com/groundlight/framegrab"
```

### Comparing `framegrab-0.5.1/src/framegrab/__init__.py` & `framegrab-0.5.2/src/framegrab/__init__.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/src/framegrab/cli/autodiscover.py` & `framegrab-0.5.2/src/framegrab/cli/autodiscover.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/src/framegrab/cli/clitools.py` & `framegrab-0.5.2/src/framegrab/cli/clitools.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/src/framegrab/cli/preview.py` & `framegrab-0.5.2/src/framegrab/cli/preview.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/src/framegrab/grabber.py` & `framegrab-0.5.2/src/framegrab/grabber.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import platform
 import re
 import subprocess
 import time
 from abc import ABC, abstractmethod
 from threading import Lock, Thread
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 from urllib.parse import urlparse
 
 import cv2
 import numpy as np
 import yaml
 
 from .unavailable_module import UnavailableModule
@@ -508,44 +508,44 @@
         if OPERATING_SYSTEM == "Linux":
             found_cams = GenericUSBFrameGrabber._find_cameras()
         else:
             found_cams = {}
 
         # Assign camera based on serial number if 1) serial_number was provided and 2) we know the
         # serial numbers of plugged in devices
-        if serial_number and found_cams:
+        if found_cams:
+            logger.debug(f"Found {len(found_cams)} USB cameras with Linux commands. Assigning camera by serial number.")
             for found_cam in found_cams:
-                if serial_number != found_cam["serial_number"]:
+                if serial_number and serial_number != found_cam["serial_number"]:
                     continue
 
                 idx = found_cam["idx"]
                 if idx in GenericUSBFrameGrabber.indices_in_use:
-                    raise ValueError(
-                        f"USB camera index {idx} already in use. "
-                        f"Did you use the same serial number ({serial_number}) for two different cameras?"
-                    )
+                    continue
 
-                capture = cv2.VideoCapture(idx)
-                if capture.isOpened():
-                    break  # Found a valid capture, no need to look any further
+                capture = self._connect_and_validate_capture(found_cam)
+                if capture is not None:
+                    break  # Found a valid capture
 
             else:
                 raise ValueError(
                     f"Unable to find USB camera with the specified serial_number: {serial_number}. "
-                    "Please ensure that the serial number is correct and that the camera is plugged in."
+                    "Please ensure that the serial number is correct, that the camera is plugged in, and that the camera is not already in use."
                 )
-        # If no serial number was provided, just assign the next available camera by index
+        # If we don't know the serial numbers of the cameras, just assign the next available camera by index
         else:
+            logger.debug("No USB cameras found with Linux commands. Assigning camera by index.")
             for idx in range(20):  # an arbitrarily high number to make sure we check for enough cams
                 if idx in GenericUSBFrameGrabber.indices_in_use:
                     continue  # Camera is already in use, moving on
 
                 capture = cv2.VideoCapture(idx)
                 if capture.isOpened():
-                    break  # Found a valid capture, no need to look any further
+                    break  # Found a valid capture
+
             else:
                 raise ValueError("Unable to connect to USB camera by index. Is your camera plugged in?")
 
         # If a serial_number wasn't provided by the user, attempt to find it and add it to the config
         if not serial_number:
             for found_cam in found_cams:
                 if idx == found_cam["idx"]:
@@ -555,15 +555,68 @@
         # A valid capture has been found, saving it for later
         self.capture = capture
 
         # Log the current camera index as 'in use' to prevent other GenericUSBFrameGrabbers from stepping on it
         self.idx = idx
         GenericUSBFrameGrabber.indices_in_use.add(idx)
 
+    def _has_ir_camera(self, camera_name: str) -> bool:
+        """Check if the device contains an IR camera.
+
+        Cameras such as the Logitech Brio contain an infrared camera for unlocking the computer with features
+        such as Windows Hello. These cameras are not suitable for use in the context of most applications, so we will
+        exclude them.
+        """
+        cameras_with_ir = ["logitech brio"]  # we can add to this list as we discover more cameras with IR
+        for i in cameras_with_ir:
+            if i in camera_name.lower():
+                return True
+        return False
+
+    def _connect_and_validate_capture(self, camera_details: Dict[str, str]) -> Union[cv2.VideoCapture, None]:
+        """Connect to the camera, check that it is open and not an IR camera.
+
+        Return the camera if it is valid, otherwise return None.
+        """
+        idx = camera_details["idx"]
+        camera_name = camera_details["camera_name"]
+        device_path = camera_details["device_path"]
+
+        capture = cv2.VideoCapture(idx)
+        if not capture.isOpened():
+            logger.warning(f"Could not open camera with index {idx}")
+            return None
+
+        has_ir_camera = self._has_ir_camera(camera_name)
+        if has_ir_camera:
+            ret, frame = capture.read()
+            if not ret:
+                logger.warning(f"Could not read frame from {device_path}")
+                return None
+            elif self._is_grayscale(frame):
+                logger.info(
+                    f"This device ({device_path}) is grayscale and therefore likely an IR camera. Skipping this camera."
+                )
+                capture.release()
+                return None
+            else:
+                return capture
+        else:
+            return capture
+
+    def _is_grayscale(self, frame: np.ndarray) -> bool:
+        """Check if the provided frame is grayscale."""
+        b, g, r = cv2.split(frame)
+
+        return np.array_equal(b, g) and np.array_equal(g, r)
+
     def _grab_implementation(self) -> np.ndarray:
+        if not self.capture.isOpened():
+            self.capture.open(self.idx)
+
         # OpenCV VideoCapture buffers frames by default. It's usually not possible to turn buffering off.
         # Buffer can be set as low as 1, but even still, if we simply read once, we will get the buffered (stale) frame.
         # Assuming buffer size of 1, we need to read twice to get the current frame.
         for _ in range(2):
             _, frame = self.capture.read()
 
         return frame
@@ -575,61 +628,67 @@
     def _apply_camera_specific_options(self, options: dict) -> None:
         self._set_cv2_resolution()
 
         # set the buffer size to 1 to always get the most recent frame
         self.capture.set(cv2.CAP_PROP_BUFFERSIZE, 1)
 
     @staticmethod
+    def _run_system_command(command: str) -> str:
+        """Runs a Linux system command and returns the stdout as a string."""
+        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        stdout, _ = process.communicate()
+        return stdout.decode("utf-8").strip()
+
+    @staticmethod
     def _find_cameras() -> list:
         """Attempts to finds all USB cameras and returns a list dictionaries, each dictionary containing
         information about a camera, including: serial_number, device name, index, etc.
         This is useful for connecting the dots between user provided configurations
         and actual plugged in devices.
 
         This function only works on Linux, and was specifically tested on an Nvidia Jetson.
         """
 
         # ls /dev/video* returns device paths for all detected cameras
         command = "ls /dev/video*"
-        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-        stdout, _ = process.communicate()
+        output = GenericUSBFrameGrabber._run_system_command(command)
 
-        if len(stdout) == 0:  # len is zero when no cameras are plugged in
+        if len(output) == 0:  # len is zero when no cameras are plugged in
             device_paths = []
         else:
-            output = stdout.decode("utf-8")
-            device_paths = output.strip().split("\n")
+            device_paths = output.split("\n")
 
         found_cams = []
         for device_path in device_paths:
             # ls -l /sys/class/video4linux/video0/device returns a path that points back into the /sys/bus/usb/devices/
             # directory where we can determine the serial number.
             # e.g. /sys/bus/usb/devices/2-3.2:1.0 -> /sys/bus/usb/devices/<bus>-<port>.<subport>:<config>.<interface>
             devname = device_path.split("/")[-1]
             command = f"ls -l /sys/class/video4linux/{devname}/device"
-            process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-            stdout, _ = process.communicate()
-            output = stdout.decode("utf-8")
+            output = GenericUSBFrameGrabber._run_system_command(command)
             bus_port_subport = output.split("/")[-1].split(":")[0]
 
             # find the serial number
             command = f"cat /sys/bus/usb/devices/{bus_port_subport}/serial"
-            process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-            stdout, _ = process.communicate()
-            serial_number = stdout.decode("utf-8").strip()
+            serial_number = GenericUSBFrameGrabber._run_system_command(command)
+
+            # find the camera name (e.g. Logitech Brio)
+            command = f"cat /sys/class/video4linux/{devname}/name"
+            camera_name = GenericUSBFrameGrabber._run_system_command(command)
 
             # find the index
             idx = int(re.findall(r"\d+", devname)[-1])
 
             if serial_number:
                 found_cams.append(
                     {
                         "serial_number": serial_number,
                         "device_path": device_path,
                         "idx": idx,
+                        "camera_name": camera_name,
                     }
                 )
 
         return found_cams
 
 
 class RTSPFrameGrabber(FrameGrabber):
```

### Comparing `framegrab-0.5.1/src/framegrab/motion.py` & `framegrab-0.5.2/src/framegrab/motion.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/src/framegrab/unavailable_module.py` & `framegrab-0.5.2/src/framegrab/unavailable_module.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.1/PKG-INFO` & `framegrab-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easily grab frames from cameras or streams
 Home-page: https://www.groundlight.ai/
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

