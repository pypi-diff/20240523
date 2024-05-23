# Comparing `tmp/brightify-0.1.1.tar.gz` & `tmp/brightify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightify-0.1.1.tar", last modified: Mon May 20 23:30:08 2024, max compression
+gzip compressed data, was "brightify-0.1.2.tar", last modified: Thu May 23 18:37:13 2024, max compression
```

## Comparing `brightify-0.1.1.tar` & `brightify-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/Brightify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 23:30:08.000000 brightify-0.1.1/Brightify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 23:30:04.000000 brightify-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-20 23:30:08.841576 brightify-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-20 23:30:04.000000 brightify-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/BaseApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/Brightylog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/SensorComm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/UIConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/log_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorDDCCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/MonitorUSB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/monitors/m27q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/res/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/res/icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/res/icon_light.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/sensor_firmware/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/sensor_firmware/platformio.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/sensor_firmware/src/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/sensor_firmware/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:30:08.841576 brightify-0.1.1/brightify/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/WindowsApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/add_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 23:30:04.000000 brightify-0.1.1/brightify/windows/remove_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-20 23:30:04.000000 brightify-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:30:08.841576 brightify-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/Brightify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 18:37:08.000000 brightify-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-23 18:37:13.515554 brightify-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 18:37:08.000000 brightify-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/BaseApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/Brightylog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/SensorComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/UIConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/linux/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/log_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorDDCCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorUSB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/m27q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/res/icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/res/icon_light.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/sensor_firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/sensor_firmware/platformio.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/sensor_firmware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/sensor_firmware/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/brightify/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/WindowsApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/add_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/remove_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-23 18:37:08.000000 brightify-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:37:13.515554 brightify-0.1.2/setup.cfg
```

### Comparing `brightify-0.1.1/Brightify.egg-info/PKG-INFO` & `brightify-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: Brightify
-Version: 0.1.1
-Summary: The Brightify application allows users to adjust the brightness of their monitors.
-Author-email: "Robin S." <brightify@rs-web.net>
-Keywords: brightness,monitor,screen,control,tool
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Requires-Dist: platformio
-Requires-Dist: pyserial
-Requires-Dist: libusb1
-Requires-Dist: PyQt6
-Requires-Dist: monitorcontrol
-Requires-Dist: pywin32; platform_system == "Windows"
-Requires-Dist: winshell; platform_system == "Windows"
-
 # Brightify
 This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
 It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
 You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
 The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
 
 ## Getting started
```

### Comparing `brightify-0.1.1/Brightify.egg-info/SOURCES.txt` & `brightify-0.1.2/Brightify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 brightify/BaseApp.py
 brightify/Brightylog.py
 brightify/SensorComm.py
 brightify/UIConfig.py
 brightify/__init__.py
 brightify/__main__.py
 brightify/log_config.toml
+brightify/linux/helpers.py
 brightify/monitors/MonitorBase.py
 brightify/monitors/MonitorDDCCI.py
 brightify/monitors/MonitorGeneric.py
 brightify/monitors/MonitorUSB.py
 brightify/monitors/m27q.py
 brightify/res/icon_dark.ico
 brightify/res/icon_light.ico
```

### Comparing `brightify-0.1.1/PKG-INFO` & `brightify-0.1.2/Brightify.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.1
-Summary: The Brightify application allows users to adjust the brightness of their monitors.
+Version: 0.1.2
+Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
 Requires-Dist: libusb1
```

### Comparing `brightify-0.1.1/README.md` & `brightify-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: Brightify
+Version: 0.1.2
+Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
+Author-email: "Robin S." <brightify@rs-web.net>
+Keywords: brightness,monitor,screen,control,tool
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Requires-Dist: platformio
+Requires-Dist: pyserial
+Requires-Dist: libusb1
+Requires-Dist: PyQt6
+Requires-Dist: monitorcontrol
+Requires-Dist: pywin32; platform_system == "Windows"
+Requires-Dist: winshell; platform_system == "Windows"
+
 # Brightify
 This app allows you to set the brightness of your monitor(s). It is essentially a wrapper around the [DDC/CI](https://en.wikipedia.org/wiki/Display_Data_Channel#DDC/CI) protocol, which is supported by most monitors.
 It also supports adding custom communication protocols to control the brightness of USB monitors. For this, you most likely need to reverse engineer the communication protocol of the monitor. In my experience, this provides a more stable experience than using the DDC/CI protocol.
 You can find an example implementation for the [Gigabyte M27Q](https://www.gigabyte.com/Monitor/M27Q) in [here](brightify/monitors/m27q.py).
 The app is designed to be run in the background and can be controlled via a taskbar icon. It also supports a brightness sensor that can automatically adjust the brightness based on the ambient light.
 
 ## Getting started
```

### Comparing `brightify-0.1.1/brightify/BaseApp.py` & `brightify-0.1.2/brightify/BaseApp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import threading
-from typing import List, Tuple, Type, Callable, Generator, Optional, Literal, Dict
+from typing import List, Tuple, Type, Callable, Generator, Optional, Literal, Dict, Any
 
 from PyQt6 import QtCore
 from PyQt6.QtCore import QPoint, Qt, QRect, QPropertyAnimation, QTimer, QThread
 from PyQt6.QtGui import QFocusEvent, QCursor, QRegion, QPainterPath
 from PyQt6.QtWidgets import QMainWindow, QWidget, QVBoxLayout
 
 from brightify import app_name, root_dir
@@ -99,15 +99,15 @@
         self.rows: QVBoxLayout = QVBoxLayout()
         self.central_widget = QWidget(self)
         self.central_widget.setLayout(self.rows)
         self.setCentralWidget(self.central_widget)
 
         self.__anim_lock: threading.Lock = threading.Lock()
         # Store the top left corner given by the OS
-        self.top_left: QPoint | None = None
+        self.__top_left: QPoint | None = None
         self.__get_theme = theme_cb
         self.__ui_config: UIConfig = UIConfig()
         self.__sensor_comm = SensorComm()
 
         # Start timer that reads sensor data every 500ms
         self.__sensor_thread = QThread()
         self.__sensor_comm.moveToThread(self.__sensor_thread)
@@ -121,14 +121,27 @@
         self.fade_up_animation.finished.connect(self.__anim_lock.release)
         self.fade_up_animation.finished.connect(self.activateWindow)
         self.fade_up_animation.finished.connect(self.setFocus)
 
         self.fade_down_animation = QPropertyAnimation(self, b"geometry")
         self.fade_down_animation.finished.connect(self.__anim_lock.release)
         self.fade_down_animation.finished.connect(self.clearFocus)
+        self.fade_down_animation.finished.connect(self.hide)
+
+    @property
+    def top_left(self) -> QPoint | None:
+        return self.__top_left
+
+    @top_left.setter
+    def top_left(self, value: QPoint | Tuple[int, int] | Any):
+        if isinstance(value, tuple):
+            value = QPoint(*value)
+        elif not isinstance(value, QPoint):
+            raise TypeError(f"Expected QPoint or Tuple[int, int], got {type(value)}")
+        self.__top_left = value
 
     @property
     def ui_config(self) -> UIConfig:
         return self.__ui_config
 
     def __config_layout(self):
         self.setWindowTitle(app_name)
```

### Comparing `brightify-0.1.1/brightify/Brightylog.py` & `brightify-0.1.2/brightify/Brightylog.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/SensorComm.py` & `brightify-0.1.2/brightify/SensorComm.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/UIConfig.py` & `brightify-0.1.2/brightify/UIConfig.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/__main__.py` & `brightify-0.1.2/brightify/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,25 @@
     threading.Thread(target=win32gui.PumpMessages, daemon=True).start()
     base_app.show()
     ret_code = app.exec()
     logger.info(f"Exiting with code {ret_code}")
     exit(ret_code)
 
 
-def main_linux():
-    raise NotImplementedError("Linux not supported yet")
-
+def main_linux(app):
+    # from brightify.linux.LinuxApp import LinuxApp
+    from brightify.linux.helpers import get_theme
+    base_app = BaseApp(get_theme)
+    logger.critical("Linux not supported yet, this will most likely crash")
+    base_app.top_left = (0, 0)
+    base_app.redraw()
+    base_app.show()
+    ret_code = app.exec()
+    logger.info(f"Exiting with code {ret_code}")
+    exit(ret_code)
 
 def main_darwin():
     raise NotImplementedError("MacOS not supported yet")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=app_name)
@@ -83,15 +91,15 @@
         app = QApplication(sys.argv)
         match host_os:
             case "Windows":
                 logger.debug("Running on Windows")
                 main_win(app)
             case "Linux":
                 logger.debug("Running on Linux")
-                main_linux()
+                main_linux(app)
             case "Darwin":
                 logger.debug("Running on MacOS")
                 main_darwin()
             case _:
                 logger.error(f"Unsupported OS: {host_os}")
                 exit(1)
     except KeyboardInterrupt:
```

### Comparing `brightify-0.1.1/brightify/log_config.toml` & `brightify-0.1.2/brightify/log_config.toml`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/monitors/MonitorBase.py` & `brightify-0.1.2/brightify/monitors/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/monitors/MonitorDDCCI.py` & `brightify-0.1.2/brightify/monitors/MonitorDDCCI.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/monitors/MonitorGeneric.py` & `brightify-0.1.2/brightify/monitors/MonitorGeneric.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/monitors/MonitorUSB.py` & `brightify-0.1.2/brightify/monitors/MonitorUSB.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/monitors/m27q.py` & `brightify-0.1.2/brightify/monitors/m27q.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/res/icon_dark.ico` & `brightify-0.1.2/brightify/res/icon_dark.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/res/icon_light.ico` & `brightify-0.1.2/brightify/res/icon_light.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/windows/WindowsApp.py` & `brightify-0.1.2/brightify/windows/WindowsApp.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/windows/actions.py` & `brightify-0.1.2/brightify/windows/actions.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/windows/add_startup_task.py` & `brightify-0.1.2/brightify/windows/add_startup_task.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.1/brightify/windows/helpers.py` & `brightify-0.1.2/brightify/windows/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from typing import Literal
 
 from brightify import host_os
 from brightify.UIConfig import Theme
-from brightify.monitors.MonitorBase import MonitorBase
 
 if host_os != "Windows":
     raise RuntimeError("This code is designed to run on Windows only")
 try:
     import win32con, win32api, win32gui, win32ui, winerror, winreg
 except ModuleNotFoundError:
     raise RuntimeError("This code is designed to run with pywin32")
```

### Comparing `brightify-0.1.1/brightify/windows/remove_startup_task.py` & `brightify-0.1.2/brightify/windows/remove_startup_task.py`

 * *Files identical despite different names*

