# Comparing `tmp/abeewayconfig-0.2.2.2.tar.gz` & `tmp/abeewayconfig-0.2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.2.2.tar", last modified: Mon May 20 13:57:13 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.2.8.tar", last modified: Thu May 23 03:01:29 2024, max compression
```

## Comparing `abeewayconfig-0.2.2.2.tar` & `abeewayconfig-0.2.2.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:57:13.978246 abeewayconfig-0.2.2.2/
--rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2.2/LICENSE
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1439 2024-05-20 13:57:13.978246 abeewayconfig-0.2.2.2/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1051 2024-05-16 14:51:58.000000 abeewayconfig-0.2.2.2/README.md
--rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-20 13:57:13.978246 abeewayconfig-0.2.2.2/setup.cfg
--rw-r--r--   0 lucas     (1001) lucas     (1001)      783 2024-05-20 13:56:35.000000 abeewayconfig-0.2.2.2/setup.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:57:13.974913 abeewayconfig-0.2.2.2/src/
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:57:13.974913 abeewayconfig-0.2.2.2/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2248 2024-05-20 13:12:46.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2263 2024-05-20 13:43:18.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4788 2024-05-20 13:14:44.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:57:13.974913 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1439 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      434 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-20 13:57:13.000000 abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)    35149 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/LICENSE
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1695 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1307 2024-05-23 03:01:08.000000 abeewayconfig-0.2.2.8/README.md
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/setup.cfg
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      851 2024-05-23 02:53:17.000000 abeewayconfig-0.2.2.8/setup.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.176905 abeewayconfig-0.2.2.8/src/
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.176905 abeewayconfig-0.2.2.8/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4758 2024-05-23 02:51:28.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/CSVFile.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     3430 2024-05-23 00:22:55.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2807 2024-05-23 00:22:55.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       32 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     6138 2024-05-23 02:27:42.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4026 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1695 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      463 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      121 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       12 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       14 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.2.2/LICENSE` & `abeewayconfig-0.2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.2/PKG-INFO` & `abeewayconfig-0.2.2.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2.2
+Version: 0.2.2.8
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -12,45 +12,55 @@
 Requires-Dist: pyserial
 Requires-Dist: tk
 
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
+
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
 
 ## Installation
 
 To install I recommend you use the package installer for Python - **pip**
 
 ```bash
   pip install abeewayconfig
 ```
 
-Run the package using
+## Usage
 
 ```bash
   abeewayconfig
 ```
 
+Run this command to open the GUI related to device configuring.
+
+```bash
+ abeewayupload
+```
+
+Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
+
 ## Compatibility
 
 ### Operating Systems
 - Linux
   - Arch
 - Windows
   - W11
 
 ### Devices
 - Abeeway Smart Badge
   - A310
   - U310
 
 ### Firmware Version
-- 2.4.1
+- Smart Badge U310/A310
+  - 2.4.1
 
 ## Known issues
 - GUI doesn't stall user action when talking to devices properly, making it able to break communication with serial ports by forcing multiple calls to same serial port
   - (as far as I've looked, this doesn't kill the already established communication)
 
 ## Future goals
 - [ ] Support for multiple firmware versions
```

### Comparing `abeewayconfig-0.2.2.2/README.md` & `abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,66 @@
+Metadata-Version: 2.1
+Name: AbeewayConfig
+Version: 0.2.2.8
+Summary: Abeeway configuration tool
+Home-page: https://github.com/jlabbude/AbeewayConfig
+Author: João Lucas
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyserial
+Requires-Dist: tk
+
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
+
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
 
 ## Installation
 
 To install I recommend you use the package installer for Python - **pip**
 
 ```bash
   pip install abeewayconfig
 ```
 
-Run the package using
+## Usage
 
 ```bash
   abeewayconfig
 ```
 
+Run this command to open the GUI related to device configuring.
+
+```bash
+ abeewayupload
+```
+
+Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
+
 ## Compatibility
 
 ### Operating Systems
 - Linux
   - Arch
 - Windows
   - W11
 
 ### Devices
 - Abeeway Smart Badge
   - A310
   - U310
 
 ### Firmware Version
-- 2.4.1
+- Smart Badge U310/A310
+  - 2.4.1
 
 ## Known issues
 - GUI doesn't stall user action when talking to devices properly, making it able to break communication with serial ports by forcing multiple calls to same serial port
   - (as far as I've looked, this doesn't kill the already established communication)
 
 ## Future goals
 - [ ] Support for multiple firmware versions
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abeewayconfig-0.2.2.2/setup.py` & `abeewayconfig-0.2.2.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.2.2",
+    version="0.2.2.8",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
         "tk",
     ],
     entry_points={
         "console_scripts": [
             "abeewayconfig = AbeewayConfig.abeewayconfig:main",
+            "abeewayupload = AbeewayConfig.abeewayconfig:nw_sv_gui"
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     python_requires='>=3.0',
```

### Comparing `abeewayconfig-0.2.2.2/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.2.8/src/AbeewayConfig/Device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import re
 import os
-from serial import Serial
+import re
 from time import sleep
 
+from serial import Serial
+
 
 class Device:
     def reset_dev(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'system reset\r')
             ser.close()
@@ -15,29 +16,37 @@
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'system skip\r')
             sleep(6)
             ser.write(b'system log off\r')
             ser.close()
 
-    def get_deveui(serial_port: str, br: int) -> int:
+    def get_deveui(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'123\r')
             ser.write(b'lora info\r')
             output = ser.read(1000).decode('utf-8')
             p = re.compile(r"DevEUI: (.*)")
             deveui = p.search(output)
+            # TODO: make creator for deveui.txt
             if deveui is not None:
-                return deveui.group(1)
+                deveui_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils", "deveui.txt")
+                deveui = deveui.group(1).strip()
+                with open(deveui_file, 'r') as deveui_log:
+                    deveui_log_content = deveui_log.read().splitlines()
+                if deveui not in deveui_log_content:
+                    with open(deveui_file, 'a') as deveui_log:
+                        deveui_log.write(deveui + "\n")
+                return deveui
 
     def set_config_on_device(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
-            config_file = os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)), "config"), "config.cfg")
+            config_file = os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils"), "config.cfg")
             with open(config_file, 'rb') as config:
                 for line in config:
                     ser.write(line.strip())
                     ser.write(b'\r')
             ser.write(b'config save\r')
             ser.write(b'system buzzer 6\r')
             ser.close()
@@ -49,11 +58,12 @@
             match_line = re.search(r".*\s+%s\s*=\s*(-?\d+)" % parameter, config_name)
             if match_line is not None:
                 return int(match_line.group(1))
 
     def config_show_at_device(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
+            ser.write(b'system log off\r')
             ser.write(b'config show\r')
             output = ser.read(16000)
             ser.close()
             return output.decode('utf-8')
```

### Comparing `abeewayconfig-0.2.2.2/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.2.8/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.2/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.2.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,52 @@
-Metadata-Version: 2.1
-Name: AbeewayConfig
-Version: 0.2.2.2
-Summary: Abeeway configuration tool
-Home-page: https://github.com/jlabbude/AbeewayConfig
-Author: João Lucas
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyserial
-Requires-Dist: tk
-
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
+
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
 
 ## Installation
 
 To install I recommend you use the package installer for Python - **pip**
 
 ```bash
   pip install abeewayconfig
 ```
 
-Run the package using
+## Usage
 
 ```bash
   abeewayconfig
 ```
 
+Run this command to open the GUI related to device configuring.
+
+```bash
+ abeewayupload
+```
+
+Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
+
 ## Compatibility
 
 ### Operating Systems
 - Linux
   - Arch
 - Windows
   - W11
 
 ### Devices
 - Abeeway Smart Badge
   - A310
   - U310
 
 ### Firmware Version
-- 2.4.1
+- Smart Badge U310/A310
+  - 2.4.1
 
 ## Known issues
 - GUI doesn't stall user action when talking to devices properly, making it able to break communication with serial ports by forcing multiple calls to same serial port
   - (as far as I've looked, this doesn't kill the already established communication)
 
 ## Future goals
 - [ ] Support for multiple firmware versions
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

