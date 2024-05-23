# Comparing `tmp/oresat_star_tracker-0.2.0.tar.gz` & `tmp/oresat_star_tracker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_star_tracker-0.2.0.tar", last modified: Sun Apr 28 23:53:40 2024, max compression
+gzip compressed data, was "oresat_star_tracker-0.2.1.tar", last modified: Thu May 23 03:46:50 2024, max compression
```

## Comparing `oresat_star_tracker-0.2.0.tar` & `oresat_star_tracker-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.713847 oresat_star_tracker-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.705846 oresat_star_tracker-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.705846 oresat_star_tracker-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-28 23:53:40.713847 oresat_star_tracker-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.705846 oresat_star_tracker-0.2.0/oresat_star_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/star_tracker_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.709846 oresat_star_tracker-0.2.0/oresat_star_tracker/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/oresat_star_tracker/templates/star_tracker.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.713847 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-28 23:53:40.000000 oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 23:53:40.713847 oresat_star_tracker-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.709846 oresat_star_tracker-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:53:40.709846 oresat_star_tracker-0.2.0/tests/images/
--rw-r--r--   0 runner    (1001) docker     (127)  1929648 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/tests/images/capture-2022-09-25-09-40-25.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-28 23:53:35.000000 oresat_star_tracker-0.2.0/tests/test_lost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/oresat_star_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/star_tracker_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/oresat_star_tracker/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/templates/star_tracker.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  1929648 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/images/capture-2022-09-25-09-40-25.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/test_lost.py
```

### Comparing `oresat_star_tracker-0.2.0/.github/workflows/pypi.yaml` & `oresat_star_tracker-0.2.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/.github/workflows/tests.yaml` & `oresat_star_tracker-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/.gitignore` & `oresat_star_tracker-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/LICENSE` & `oresat_star_tracker-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/PKG-INFO` & `oresat_star_tracker-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-star-tracker
-Version: 0.2.0
+Version: 0.2.1
 Summary: OreSat Star Tracker OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_star_tracker-0.2.0/README.md` & `oresat_star_tracker-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker/__main__.py` & `oresat_star_tracker-0.2.1/oresat_star_tracker/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker/camera.py` & `oresat_star_tracker-0.2.1/oresat_star_tracker/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, mock: bool = False):
         self._mock = mock
 
         if self._mock:
             self._capture_path = f"{dirname(abspath(__file__))}/data/mock.bmp"
         else:
             self._capture_path = "/dev/prucam"
-            self.image_size = self.read_image_size()
+            self.image_size = (-1, -1)
 
     def read_image_size(self):
         """Read dimensions of image from the camera"""
         x_size = self.read_context_setting("x_size")
         y_size = self.read_context_setting("y_size")
         return (y_size, x_size)
 
@@ -58,14 +58,17 @@
 
         Returns
         -------
         numpy.ndarray
             image data in numpy array
         """
 
+        if self.image_size == (-1, -1):
+            self.image_size = self.read_image_size()
+
         if self._mock:
             img = cv2.imread(self._capture_path, cv2.IMREAD_COLOR)
         else:
             # Read raw data
             fd = os.open(self._capture_path, os.O_RDWR)
             fio = io.FileIO(fd, closefd=False)
             imgbuf = bytearray(self.image_size[0] * self.image_size[1])
```

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker/star_tracker_service.py` & `oresat_star_tracker-0.2.1/oresat_star_tracker/star_tracker_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Star Tracker service"""
 
 from enum import IntEnum
 from io import BytesIO
-from time import time
+from time import monotonic, time
 
 import canopen
 import cv2
 import lost
 import numpy as np
 import tifffile as tiff
 from olaf import Service, logger, new_oresat_file  # , set_cpufreq_gov
@@ -99,15 +99,15 @@
         self._upper_percentage_obj = image_filter_rec["upper_percentage"]
 
         self.node.add_sdo_callbacks("status", None, self.on_read_status, self.on_write_status)
         self.node.add_sdo_callbacks(
             "capture", "last_display_image", self._on_read_last_display_image, None
         )
 
-        self._state = State.STANDBY
+        self._state = State.BOOT
 
     def on_stop(self):
         """When service stops clear star tracking data."""
 
         self._right_ascension_obj.value = 0
         self._declination_obj.value = 0
         self._orientation_obj.value = 0
@@ -244,15 +244,17 @@
         if img_count == 0:
             logger.info("no images taken, check camera mode settings and filter")
 
         logger.info(f"changing status: {self._state.name} -> {State.STANDBY.name}")
         self._state = State.STANDBY
 
     def on_loop(self):
-        if self._state == State.STAR_TRACK:
+        if self._state == State.BOOT and monotonic() > 70:
+            self._state = State.STANDBY
+        elif self._state == State.STAR_TRACK:
             self._star_track()
         elif self._state == State.CAPTURE_ONLY:
             self._capture_only_mode()
         else:
             self.sleep(0.1)
 
     def on_loop_error(self, error: Exception):
@@ -279,14 +281,18 @@
         except ValueError:
             logger.error(f"invalid state: {value}")
             return
 
         if new_status == self._state:
             return  # nothing to change
 
+        if self._state == State.BOOT:
+            logger.error("cannot transfer out of BOOT state by command")
+            return
+
         if new_status not in STATE_TRANSISTIONS[self._state]:
             logger.error(f"invalid status change: {self._state.name} -> {new_status.name}")
             return
 
         # When entering low power status, turn on low power mode
         # if new_status == State.LOW_POWER and self._state != State.LOW_POWER:
         #    set_cpufreq_gov('powersave')
```

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker/templates/star_tracker.html` & `oresat_star_tracker-0.2.1/oresat_star_tracker/templates/star_tracker.html`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/PKG-INFO` & `oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-star-tracker
-Version: 0.2.0
+Version: 0.2.1
 Summary: OreSat Star Tracker OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_star_tracker-0.2.0/oresat_star_tracker.egg-info/SOURCES.txt` & `oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/pyproject.toml` & `oresat_star_tracker-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/tests/images/capture-2022-09-25-09-40-25.png` & `oresat_star_tracker-0.2.1/tests/images/capture-2022-09-25-09-40-25.png`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.0/tests/test_lost.py` & `oresat_star_tracker-0.2.1/tests/test_lost.py`

 * *Files identical despite different names*

