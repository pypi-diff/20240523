# Comparing `tmp/createbme-1.2.0.tar.gz` & `tmp/createbme-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createbme-1.2.0.tar", last modified: Mon May 13 11:45:44 2024, max compression
+gzip compressed data, was "createbme-1.2.1.tar", last modified: Thu May 23 12:50:38 2024, max compression
```

## Comparing `createbme-1.2.0.tar` & `createbme-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.451104 createbme-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 11:45:39.000000 createbme-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-13 11:45:44.451104 createbme-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-13 11:45:39.000000 createbme-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 11:45:39.000000 createbme-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:45:44.451104 createbme-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 11:45:39.000000 createbme-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.447105 createbme-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.447105 createbme-1.2.0/src/CreaTeBME/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/ImuSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/SensorEmulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/SensorManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 11:45:39.000000 createbme-1.2.0/src/CreaTeBME/uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:45:44.451104 createbme-1.2.0/src/CreaTeBME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 11:45:44.000000 createbme-1.2.0/src/CreaTeBME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 12:50:29.000000 createbme-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 12:50:38.293784 createbme-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-23 12:50:29.000000 createbme-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 12:50:29.000000 createbme-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:50:38.293784 createbme-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-23 12:50:29.000000 createbme-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.289784 createbme-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/src/CreaTeBME/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/ImuSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/SensorEmulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/SensorManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/src/CreaTeBME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/top_level.txt
```

### Comparing `createbme-1.2.0/LICENSE` & `createbme-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `createbme-1.2.0/PKG-INFO` & `createbme-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -25,15 +25,15 @@
 To install the latest stable version simply run this in your terminal.
 If you are using PyCharm then you can open the terminal on the bottom left of the screen.
 ```shell
 pip install CreaTeBME
 ```
 
 # Example
-A simple example to connect to a sensor and read and print the data for 10 seconds.
+A simple example to connect to a sensor and read and print the data indefinitely.
 The package automatically connects to the device, so you do not have to connect to it manually.
 ```python
 from CreaTeBME import SensorManager
 
 # Create a sensor manager for the given sensor names using the given callback
 manager = SensorManager(['0BE6'])
 
@@ -81,14 +81,15 @@
 - **[0:2]** = x,y,z of accelerometer in (g).
 - **[3:5]** = x,y,z of gyroscope in (deg/s).
 
 Finally, make sure to also call the `stop` method when exiting your program.
 ```python
 manager.stop()
 ```
+
 ## Manual Connection
 ⚠️**Understanding of** asyncio **required**⚠️
 
 Another way of connecting IMU sensors is to manually create `ImuSensor` objects.
 This can be done by specifying the BLE device that should be connected as a sensor.
 ```python
 from CreaTeBME import ImuSensor
```

### Comparing `createbme-1.2.0/README.md` & `createbme-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 To install the latest stable version simply run this in your terminal.
 If you are using PyCharm then you can open the terminal on the bottom left of the screen.
 ```shell
 pip install CreaTeBME
 ```
 
 # Example
-A simple example to connect to a sensor and read and print the data for 10 seconds.
+A simple example to connect to a sensor and read and print the data indefinitely.
 The package automatically connects to the device, so you do not have to connect to it manually.
 ```python
 from CreaTeBME import SensorManager
 
 # Create a sensor manager for the given sensor names using the given callback
 manager = SensorManager(['0BE6'])
 
@@ -65,14 +65,15 @@
 - **[0:2]** = x,y,z of accelerometer in (g).
 - **[3:5]** = x,y,z of gyroscope in (deg/s).
 
 Finally, make sure to also call the `stop` method when exiting your program.
 ```python
 manager.stop()
 ```
+
 ## Manual Connection
 ⚠️**Understanding of** asyncio **required**⚠️
 
 Another way of connecting IMU sensors is to manually create `ImuSensor` objects.
 This can be done by specifying the BLE device that should be connected as a sensor.
 ```python
 from CreaTeBME import ImuSensor
```

### Comparing `createbme-1.2.0/setup.py` & `createbme-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='CreaTeBME',
-    version='1.2.0',
+    version='1.2.1',
     author='Jonathan Matarazzi',
     author_email='git@jonathanm.nl',
     description='Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CreaTe-M8-BME/CreaTeBME',
     project_urls={
```

### Comparing `createbme-1.2.0/src/CreaTeBME/ImuSensor.py` & `createbme-1.2.1/src/CreaTeBME/ImuSensor.py`

 * *Files identical despite different names*

### Comparing `createbme-1.2.0/src/CreaTeBME/SensorEmulator.py` & `createbme-1.2.1/src/CreaTeBME/SensorEmulator.py`

 * *Files identical despite different names*

### Comparing `createbme-1.2.0/src/CreaTeBME/SensorManager.py` & `createbme-1.2.1/src/CreaTeBME/SensorManager.py`

 * *Files identical despite different names*

### Comparing `createbme-1.2.0/src/CreaTeBME/connect.py` & `createbme-1.2.1/src/CreaTeBME/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Find the specified sensors and create ImuSensor objects for them.
 
     :param sensor_names: The names of the sensors to connect to
     :return: A list of ImuSensor objects
     """
     devices = await BleakScanner.discover(return_adv=True)
     imus = list(filter(lambda x: IMU_SERVICE_UUID in x[1][1].service_uuids, devices.items()))
-    chosen_imus = list(filter(lambda x: x[1][1].local_name[-4:] in sensor_names, imus))
+    chosen_imus = list(filter(lambda x: x[1][1].local_name and x[1][1].local_name[-4:] in sensor_names, imus))
     sensors = []
     connected_names = []
     for device in chosen_imus:
         sensor = ImuSensor(device[1][0])
         sensors.append(sensor)
         connected_names.append(device[1][1].local_name[-4:])
     for name in sensor_names:
```

### Comparing `createbme-1.2.0/src/CreaTeBME.egg-info/PKG-INFO` & `createbme-1.2.1/src/CreaTeBME.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -25,15 +25,15 @@
 To install the latest stable version simply run this in your terminal.
 If you are using PyCharm then you can open the terminal on the bottom left of the screen.
 ```shell
 pip install CreaTeBME
 ```
 
 # Example
-A simple example to connect to a sensor and read and print the data for 10 seconds.
+A simple example to connect to a sensor and read and print the data indefinitely.
 The package automatically connects to the device, so you do not have to connect to it manually.
 ```python
 from CreaTeBME import SensorManager
 
 # Create a sensor manager for the given sensor names using the given callback
 manager = SensorManager(['0BE6'])
 
@@ -81,14 +81,15 @@
 - **[0:2]** = x,y,z of accelerometer in (g).
 - **[3:5]** = x,y,z of gyroscope in (deg/s).
 
 Finally, make sure to also call the `stop` method when exiting your program.
 ```python
 manager.stop()
 ```
+
 ## Manual Connection
 ⚠️**Understanding of** asyncio **required**⚠️
 
 Another way of connecting IMU sensors is to manually create `ImuSensor` objects.
 This can be done by specifying the BLE device that should be connected as a sensor.
 ```python
 from CreaTeBME import ImuSensor
```

