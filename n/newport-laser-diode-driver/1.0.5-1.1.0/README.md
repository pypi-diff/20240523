# Comparing `tmp/newport_laser_diode_driver-1.0.5.tar.gz` & `tmp/newport_laser_diode_driver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport_laser_diode_driver-1.0.5.tar", last modified: Tue May 21 20:09:58 2024, max compression
+gzip compressed data, was "newport_laser_diode_driver-1.1.0.tar", last modified: Thu May 23 20:24:04 2024, max compression
```

## Comparing `newport_laser_diode_driver-1.0.5.tar` & `newport_laser_diode_driver-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 20:09:58.814911 newport_laser_diode_driver-1.0.5/
--rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.0.5/LICENSE.txt
--rw-r--r--   0 next       (501) staff       (20)     2763 2024-05-21 20:09:58.814605 newport_laser_diode_driver-1.0.5/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)     2275 2024-05-21 20:03:19.000000 newport_laser_diode_driver-1.0.5/README.md
--rw-r--r--   0 next       (501) staff       (20)       38 2024-05-21 20:09:58.814982 newport_laser_diode_driver-1.0.5/setup.cfg
--rw-r--r--   0 next       (501) staff       (20)      849 2024-05-21 20:09:45.000000 newport_laser_diode_driver-1.0.5/setup.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 20:09:58.811287 newport_laser_diode_driver-1.0.5/src/
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 20:09:58.812612 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver/
--rw-r--r--   0 next       (501) staff       (20)       63 2024-05-21 17:39:51.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver/__init__.py
--rw-r--r--   0 next       (501) staff       (20)    15089 2024-05-21 19:58:50.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver/newport_laser_diode_driver.py
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 20:09:58.813742 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/
--rw-r--r--   0 next       (501) staff       (20)     2763 2024-05-21 20:09:58.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/PKG-INFO
--rw-r--r--   0 next       (501) staff       (20)      428 2024-05-21 20:09:58.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/SOURCES.txt
--rw-r--r--   0 next       (501) staff       (20)        1 2024-05-21 20:09:58.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/dependency_links.txt
--rw-r--r--   0 next       (501) staff       (20)       26 2024-05-21 20:09:58.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/requires.txt
--rw-r--r--   0 next       (501) staff       (20)       27 2024-05-21 20:09:58.000000 newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/top_level.txt
-drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-21 20:09:58.813935 newport_laser_diode_driver-1.0.5/tests/
--rw-r--r--   0 next       (501) staff       (20)     1787 2024-05-21 19:59:17.000000 newport_laser_diode_driver-1.0.5/tests/test_model_535b.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-23 20:24:04.582528 newport_laser_diode_driver-1.1.0/
+-rw-r--r--   0 next       (501) staff       (20)     1093 2024-05-21 16:56:31.000000 newport_laser_diode_driver-1.1.0/LICENSE.txt
+-rw-r--r--   0 next       (501) staff       (20)     3038 2024-05-23 20:24:04.582231 newport_laser_diode_driver-1.1.0/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)     2550 2024-05-23 20:22:06.000000 newport_laser_diode_driver-1.1.0/README.md
+-rw-r--r--   0 next       (501) staff       (20)       38 2024-05-23 20:24:04.582589 newport_laser_diode_driver-1.1.0/setup.cfg
+-rw-r--r--   0 next       (501) staff       (20)      849 2024-05-23 20:22:33.000000 newport_laser_diode_driver-1.1.0/setup.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-23 20:24:04.579468 newport_laser_diode_driver-1.1.0/src/
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-23 20:24:04.580547 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver/
+-rw-r--r--   0 next       (501) staff       (20)       63 2024-05-21 17:39:51.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver/__init__.py
+-rw-r--r--   0 next       (501) staff       (20)    15163 2024-05-23 20:06:54.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver/newport_laser_diode_driver.py
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-23 20:24:04.581484 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/
+-rw-r--r--   0 next       (501) staff       (20)     3038 2024-05-23 20:24:04.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/PKG-INFO
+-rw-r--r--   0 next       (501) staff       (20)      428 2024-05-23 20:24:04.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 next       (501) staff       (20)        1 2024-05-23 20:24:04.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 next       (501) staff       (20)       26 2024-05-23 20:24:04.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/requires.txt
+-rw-r--r--   0 next       (501) staff       (20)       27 2024-05-23 20:24:04.000000 newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/top_level.txt
+drwxr-xr-x   0 next       (501) staff       (20)        0 2024-05-23 20:24:04.581637 newport_laser_diode_driver-1.1.0/tests/
+-rw-r--r--   0 next       (501) staff       (20)     1787 2024-05-23 20:06:21.000000 newport_laser_diode_driver-1.1.0/tests/test_model_535b.py
```

### Comparing `newport_laser_diode_driver-1.0.5/LICENSE.txt` & `newport_laser_diode_driver-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newport_laser_diode_driver-1.0.5/PKG-INFO` & `newport_laser_diode_driver-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newport_laser_diode_driver
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python library for interfacing with Newport Model 300-500B Series Laser Diode Driver
 Home-page: https://github.com/NextZtepS/newport_laser_diode_driver
 Author: NextZtepS
 Author-email: natdanaiongarjvaja@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -21,41 +21,44 @@
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 
 
 ## Set-up
 
-### Allow the Newport Laser Diode Driver USB device to be managed by Python [ref](https://stackoverflow.com/questions/31992058/how-can-i-comunicate-with-this-device-using-pyusb/31994168#31994168)
+### Allow the Newport Laser Diode Driver USB device to be managed by Python
 
 Run the Run the following shell command:
 
 ```shell
 usb-devices  # this allows us to see the idVendor and idProduct of all USB devices 
 ```
 
-Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values.
-
+Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values. 
+The process below grants permission for our package to manage the specified Newport USB device.
 
 Run the following shell command:
 
 ```shell
-cd /lib/udev/rules.d/ ;
-sudo touch 50-Newport_Laser_Diode_Driver.rules ;
-sudo vim 50-Newport_Laser_Diode_Driver.rules ;
+cd /etc/udev/rules.d/ ;
+sudo touch 99-usb-permissions.rules ;
+sudo vim 99-usb-permissions.rules ;  # you can use other text editor of your choosing
 ```
 
-Copy & paste the following line into the file: `ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="660", GROUP="plugdev"`
+Copy & paste the following line into the file: 
+```
+# Newport Model 300-500B Series Laser Diode Driver
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="0666"
+```
 
-Then, type `:wq` and press `ENTER` to save the changes
+Then, type `:wq` and press `ENTER` to save the changes and close the file
 
 Run the following shell command:
 
 ```shell
-sudo adduser USERNAME plugdev ;  # don't forget to change the USERNAME
 sudo udevadm control --reload ;
 sudo udevadm trigger ;
 ```
 
 ## Usage
 
 In your desired Python environment, run the following shell command:
@@ -75,11 +78,16 @@
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
+## Compatibility and Testing
+
+I have tested this package with the Newport Model 500B Series devices that I have accessed including 505B and 535B. On paper,
+this package should work with Model 300B Series as well; however, I have no access to the devices to test them out.
+
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
-is not found, try connecting the USB cable from the device to your PC first and then restart the device.
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport 
+device is not found, try connecting the USB cable from the device to your PC first and then restart the Newport device.
```

### Comparing `newport_laser_diode_driver-1.0.5/README.md` & `newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,64 @@
+Metadata-Version: 2.1
+Name: newport-laser-diode-driver
+Version: 1.1.0
+Summary: Python library for interfacing with Newport Model 300-500B Series Laser Diode Driver
+Home-page: https://github.com/NextZtepS/newport_laser_diode_driver
+Author: NextZtepS
+Author-email: natdanaiongarjvaja@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pyusb
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 # Newport Model 300-500B Series Laser Diode Driver Python USB Package (for Linux)
 
 This package is developed within the advisory of the Gallicchio Research Group, Harvey Mudd College.
 
 ## Pre-requisites
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 
 
 ## Set-up
 
-### Allow the Newport Laser Diode Driver USB device to be managed by Python [ref](https://stackoverflow.com/questions/31992058/how-can-i-comunicate-with-this-device-using-pyusb/31994168#31994168)
+### Allow the Newport Laser Diode Driver USB device to be managed by Python
 
 Run the Run the following shell command:
 
 ```shell
 usb-devices  # this allows us to see the idVendor and idProduct of all USB devices 
 ```
 
-Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values.
-
+Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values. 
+The process below grants permission for our package to manage the specified Newport USB device.
 
 Run the following shell command:
 
 ```shell
-cd /lib/udev/rules.d/ ;
-sudo touch 50-Newport_Laser_Diode_Driver.rules ;
-sudo vim 50-Newport_Laser_Diode_Driver.rules ;
+cd /etc/udev/rules.d/ ;
+sudo touch 99-usb-permissions.rules ;
+sudo vim 99-usb-permissions.rules ;  # you can use other text editor of your choosing
 ```
 
-Copy & paste the following line into the file: `ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="660", GROUP="plugdev"`
+Copy & paste the following line into the file: 
+```
+# Newport Model 300-500B Series Laser Diode Driver
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="0666"
+```
 
-Then, type `:wq` and press `ENTER` to save the changes
+Then, type `:wq` and press `ENTER` to save the changes and close the file
 
 Run the following shell command:
 
 ```shell
-sudo adduser USERNAME plugdev ;  # don't forget to change the USERNAME
 sudo udevadm control --reload ;
 sudo udevadm trigger ;
 ```
 
 ## Usage
 
 In your desired Python environment, run the following shell command:
@@ -60,11 +78,16 @@
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
+## Compatibility and Testing
+
+I have tested this package with the Newport Model 500B Series devices that I have accessed including 505B and 535B. On paper,
+this package should work with Model 300B Series as well; however, I have no access to the devices to test them out.
+
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
-is not found, try connecting the USB cable from the device to your PC first and then restart the device.
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport 
+device is not found, try connecting the USB cable from the device to your PC first and then restart the Newport device.
```

### Comparing `newport_laser_diode_driver-1.0.5/setup.py` & `newport_laser_diode_driver-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="newport_laser_diode_driver",
     description="Python library for interfacing with Newport Model 300-500B Series Laser Diode Driver",
-    version="1.0.5",
+    version="1.1.0",
     author="NextZtepS",
     author_email="natdanaiongarjvaja@gmail.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires=[
         "pyusb",
     ],
```

### Comparing `newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver/newport_laser_diode_driver.py` & `newport_laser_diode_driver-1.1.0/src/newport_laser_diode_driver/newport_laser_diode_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             ValueError: No Device that matches the parameters found
         """
         self._dev = usb.core.find(idVendor=idVendor, idProduct=idProduct) # type: ignore
         if self._dev is None:
             raise ValueError('Device not found')
         else:
             print(f"Connected to {self._dev.manufacturer} {self._dev.product}")
-            self._dev.set_configuration()
+            # self._dev.set_configuration()  # This is not necessary for this device and will lead to timeout error
 
     def send_helper(self, cmd_str: str):
         """
         Helper function to send a command to the device. This device uses port 0x04 for sending commands.
 
         Args:
             cmd_str (str): string command to send
```

### Comparing `newport_laser_diode_driver-1.0.5/src/newport_laser_diode_driver.egg-info/PKG-INFO` & `newport_laser_diode_driver-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,49 @@
-Metadata-Version: 2.1
-Name: newport-laser-diode-driver
-Version: 1.0.5
-Summary: Python library for interfacing with Newport Model 300-500B Series Laser Diode Driver
-Home-page: https://github.com/NextZtepS/newport_laser_diode_driver
-Author: NextZtepS
-Author-email: natdanaiongarjvaja@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pyusb
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
 # Newport Model 300-500B Series Laser Diode Driver Python USB Package (for Linux)
 
 This package is developed within the advisory of the Gallicchio Research Group, Harvey Mudd College.
 
 ## Pre-requisites
 
 - Permission to connect to the Newport Laser Diode Driver USB device
 - Python version >= 3
 
 
 ## Set-up
 
-### Allow the Newport Laser Diode Driver USB device to be managed by Python [ref](https://stackoverflow.com/questions/31992058/how-can-i-comunicate-with-this-device-using-pyusb/31994168#31994168)
+### Allow the Newport Laser Diode Driver USB device to be managed by Python
 
 Run the Run the following shell command:
 
 ```shell
 usb-devices  # this allows us to see the idVendor and idProduct of all USB devices 
 ```
 
-Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values.
-
+Ensure that the idVendor and idProduct match the example below unless change the idVendor and idProduct to the appropriate values. 
+The process below grants permission for our package to manage the specified Newport USB device.
 
 Run the following shell command:
 
 ```shell
-cd /lib/udev/rules.d/ ;
-sudo touch 50-Newport_Laser_Diode_Driver.rules ;
-sudo vim 50-Newport_Laser_Diode_Driver.rules ;
+cd /etc/udev/rules.d/ ;
+sudo touch 99-usb-permissions.rules ;
+sudo vim 99-usb-permissions.rules ;  # you can use other text editor of your choosing
 ```
 
-Copy & paste the following line into the file: `ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="660", GROUP="plugdev"`
+Copy & paste the following line into the file: 
+```
+# Newport Model 300-500B Series Laser Diode Driver
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="104d", ATTRS{idProduct}=="1001", MODE="0666"
+```
 
-Then, type `:wq` and press `ENTER` to save the changes
+Then, type `:wq` and press `ENTER` to save the changes and close the file
 
 Run the following shell command:
 
 ```shell
-sudo adduser USERNAME plugdev ;  # don't forget to change the USERNAME
 sudo udevadm control --reload ;
 sudo udevadm trigger ;
 ```
 
 ## Usage
 
 In your desired Python environment, run the following shell command:
@@ -75,11 +63,16 @@
 
 model_535B.set_current_set_point(10.0)  # set current set point to be 10.0 mA
 current = model_535B.get_current_set_point()  # get the current set point
 print(current)  # 10.0
 model_535B.enable_laser_output()  # enable laser output
 ```
 
+## Compatibility and Testing
+
+I have tested this package with the Newport Model 500B Series devices that I have accessed including 505B and 535B. On paper,
+this package should work with Model 300B Series as well; however, I have no access to the devices to test them out.
+
 ## Troubleshooting
 
-To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport device 
-is not found, try connecting the USB cable from the device to your PC first and then restart the device.
+To check if the device is recognized by the PC, run `usb-devices` to list all USB devices connected to your PC. If the Newport 
+device is not found, try connecting the USB cable from the device to your PC first and then restart the Newport device.
```

### Comparing `newport_laser_diode_driver-1.0.5/tests/test_model_535b.py` & `newport_laser_diode_driver-1.1.0/tests/test_model_535b.py`

 * *Files identical despite different names*

