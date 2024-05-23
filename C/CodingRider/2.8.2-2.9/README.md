# Comparing `tmp/codingrider-2.8.2.tar.gz` & `tmp/codingrider-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingrider-2.8.2.tar", last modified: Mon May 20 06:34:58 2024, max compression
+gzip compressed data, was "codingrider-2.9.tar", last modified: Thu May 23 01:22:05 2024, max compression
```

## Comparing `codingrider-2.8.2.tar` & `codingrider-2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:58.841629 codingrider-2.8.2/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:58.831656 codingrider-2.8.2/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-05-14 03:59:45.000000 codingrider-2.8.2/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2024-05-14 03:59:45.000000 codingrider-2.8.2/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2024-05-14 03:59:45.000000 codingrider-2.8.2/CodingRider/crc.py
--rw-rw-rw-   0        0        0    41310 2024-05-20 06:32:15.000000 codingrider-2.8.2/CodingRider/drone.py
--rw-rw-rw-   0        0        0    61222 2024-05-20 06:31:08.000000 codingrider-2.8.2/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2024-05-14 03:59:45.000000 codingrider-2.8.2/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1696 2024-05-16 06:55:33.000000 codingrider-2.8.2/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10845 2024-05-20 06:32:55.000000 codingrider-2.8.2/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:58.840629 codingrider-2.8.2/CodingRider/tools/
--rw-rw-rw-   0        0        0       48 2024-05-14 06:50:08.000000 codingrider-2.8.2/CodingRider/tools/__init__.py
--rw-rw-rw-   0        0        0    29709 2024-05-20 02:35:31.000000 codingrider-2.8.2/CodingRider/tools/parser.py
--rw-rw-rw-   0        0        0     9495 2024-05-14 06:53:10.000000 codingrider-2.8.2/CodingRider/tools/update.py
--rw-rw-rw-   0        0        0     9515 2024-05-14 03:59:45.000000 codingrider-2.8.2/CodingRider/update.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:58.840629 codingrider-2.8.2/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      720 2024-05-20 06:34:58.000000 codingrider-2.8.2/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-05-20 06:34:58.000000 codingrider-2.8.2/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:34:58.000000 codingrider-2.8.2/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-20 06:34:58.000000 codingrider-2.8.2/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 06:34:58.000000 codingrider-2.8.2/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.8.2/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0      720 2024-05-20 06:34:58.841629 codingrider-2.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.8.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 06:34:58.841629 codingrider-2.8.2/setup.cfg
--rw-rw-rw-   0        0        0      774 2024-05-20 06:34:35.000000 codingrider-2.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:22:05.751402 codingrider-2.9/
+drwxrwxrwx   0        0        0        0 2024-05-23 01:22:05.732734 codingrider-2.9/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-05-14 03:59:45.000000 codingrider-2.9/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-14 03:59:45.000000 codingrider-2.9/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-14 03:59:45.000000 codingrider-2.9/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    37365 2024-05-23 00:47:17.000000 codingrider-2.9/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    60312 2024-05-23 01:05:17.000000 codingrider-2.9/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2024-05-14 03:59:45.000000 codingrider-2.9/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1696 2024-05-16 06:55:33.000000 codingrider-2.9/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10845 2024-05-20 06:32:55.000000 codingrider-2.9/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:22:05.750395 codingrider-2.9/CodingRider/tools/
+-rw-rw-rw-   0        0        0       48 2024-05-14 06:50:08.000000 codingrider-2.9/CodingRider/tools/__init__.py
+-rw-rw-rw-   0        0        0    28833 2024-05-23 01:12:51.000000 codingrider-2.9/CodingRider/tools/parser.py
+-rw-rw-rw-   0        0        0     9495 2024-05-14 06:53:10.000000 codingrider-2.9/CodingRider/tools/update.py
+-rw-rw-rw-   0        0        0     9515 2024-05-14 03:59:45.000000 codingrider-2.9/CodingRider/update.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:22:05.751402 codingrider-2.9/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-23 01:22:05.000000 codingrider-2.9/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-05-23 01:22:05.000000 codingrider-2.9/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:22:05.000000 codingrider-2.9/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-23 01:22:05.000000 codingrider-2.9/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 01:22:05.000000 codingrider-2.9/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.9/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      718 2024-05-23 01:22:05.751402 codingrider-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:22:05.753618 codingrider-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-23 01:21:44.000000 codingrider-2.9/setup.py
```

### Comparing `codingrider-2.8.2/CodingRider/crc.py` & `codingrider-2.9/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider/drone.py` & `codingrider-2.9/CodingRider/drone.py`

 * *Files 4% similar despite different names*

```diff
@@ -839,31 +839,14 @@
         data.yaw        = yaw
         data.throttle   = throttle
 
         return self.transfer(header, data)
 
 
 
-    def sendWeight(self, weight):
-        
-        header = Header()
-        
-        header.dataType = DataType.Weight
-        header.length   = Weight.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Drone
-
-        data = Weight()
-
-        data.weight     = weight
-
-        return self.transfer(header, data)
-
-
-
     def sendLostConnection(self, timeNeutral, timeLanding, timeStop):
         
         header = Header()
         
         header.dataType = DataType.LostConnection
         header.length   = LostConnection.getSize()
         header.from_    = DeviceType.Base
@@ -953,34 +936,14 @@
         data.commandType    = CommandType.SetDefault
         data.option         = 0
 
         return self.transfer(header, data)
 
 
 
-    def sendBacklight(self, flagPower):
-        
-        if  ( (not isinstance(flagPower, bool)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.Command
-        header.length   = Command.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-
-        data = Command()
-
-        data.commandType    = CommandType.Backlight
-        data.option         = int(flagPower)
-
-        return self.transfer(header, data)
-
-
 
     def sendSetSwarm(self):
 
         header = Header()
         
         header.dataType = DataType.Command
         header.length   = Command.getSize()
@@ -1029,36 +992,14 @@
 
         data.motor[3].rotation  = Rotation.Counterclockwise
         data.motor[3].value     = motor3
 
         return self.transfer(header, data)
 
 
-    def sendMotorSingle(self, target, rotation, value):
-        
-        if  ((not isinstance(target, int)) or
-            (not isinstance(rotation, Rotation)) or
-            (not isinstance(value, int))):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.MotorSingle
-        header.length   = MotorSingle.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Drone
-
-        data = MotorSingle()
-
-        data.target     = target
-        data.rotation   = rotation
-        data.value      = value
-
-        return self.transfer(header, data)
-
 
 # Device End
 
 
 
 # Light Start
 
@@ -1217,50 +1158,14 @@
         data.event.repeat   = repeat
 
         data.colors         = colors
 
         return self.transfer(header, data)
 
 
-
-    def sendLightDefaultColor(self, lightMode, interval, r, g, b):
-        
-        if  (((not isinstance(lightMode, LightModeDrone)) and (not isinstance(lightMode, LightModeController))) or
-            (not isinstance(interval, int)) or
-            (not isinstance(r, int)) or
-            (not isinstance(g, int)) or
-            (not isinstance(b, int))):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.LightDefault
-        header.length   = LightModeColor.getSize()
-        header.from_    = DeviceType.Base
-
-        if      isinstance(lightMode, LightModeDrone):
-            header.to_  = DeviceType.Drone
-        elif    isinstance(lightMode, LightModeController):
-            header.to_  = DeviceType.Controller
-        else:
-            return None
-
-        data = LightModeColor()
-
-        data.mode.mode      = lightMode.value
-        data.mode.interval  = interval
-
-        data.color.r        = r
-        data.color.g        = g
-        data.color.b        = b
-
-        return self.transfer(header, data)
-
-
-
 # Light End
 
 
 
 # Buzzer Start
 
 
@@ -1296,15 +1201,15 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.Mute
+        data.mode       = BuzzerMode.MuteInstantly
         data.value      = BuzzerScale.Mute.value
         data.time       = time
 
         return self.transfer(header, data)
 
 
 
@@ -1318,15 +1223,15 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.MuteReserve
+        data.mode       = BuzzerMode.MuteContinually
         data.value      = BuzzerScale.Mute.value
         data.time       = time
 
         return self.transfer(header, data)
 
 
 
@@ -1340,15 +1245,15 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.Scale
+        data.mode       = BuzzerMode.ScaleInstantly
         data.value      = scale.value
         data.time       = time
 
         return self.transfer(header, data)
 
 
 
@@ -1362,15 +1267,15 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.ScaleReserve
+        data.mode       = BuzzerMode.ScaleContinually
         data.value      = scale.value
         data.time       = time
 
         return self.transfer(header, data)
 
 
 
@@ -1384,15 +1289,15 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.Hz
+        data.mode       = BuzzerMode.HzInstantly
         data.value      = hz
         data.time       = time
 
         return self.transfer(header, data)
 
 
 
@@ -1406,76 +1311,23 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Controller
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.HzReserve
+        data.mode       = BuzzerMode.HzContinually
         data.value      = hz
         data.time       = time
 
         return self.transfer(header, data)
 
 
 # Buzzer End
 
 
-
-# Vibrator Start
-
-
-    def sendVibrator(self, on, off, total):
-        
-        if ( (not isinstance(on, int)) or (not isinstance(off, int)) or (not isinstance(total, int)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.Vibrator
-        header.length   = Vibrator.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = Vibrator()
-
-        data.mode       = VibratorMode.Instantally
-        data.on         = on
-        data.off        = off
-        data.total      = total
-
-        return self.transfer(header, data)
-
-
-
-    def sendVibratorReserve(self, on, off, total):
-        
-        if ( (not isinstance(on, int)) or (not isinstance(off, int)) or (not isinstance(total, int)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.Vibrator
-        header.length   = Vibrator.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = Vibrator()
-
-        data.mode       = VibratorMode.Continually
-        data.on         = on
-        data.off        = off
-        data.total      = total
-
-        return self.transfer(header, data)
-
-
-# Vibrator End
-
-
-
 # Update Start
 
 
 
 
 # Update End
```

### Comparing `codingrider-2.8.2/CodingRider/protocol.py` & `codingrider-2.9/CodingRider/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     def toArray(self):
         return pack('<BI', self.dataType.value, self.option)
 
 
     @classmethod
     def parse(cls, dataArray):
-        data = Request()
+        data = RequestOption()
         
         if len(dataArray) != cls.getSize():
             return None
         
         data.dataType, data.option = unpack('<BI', dataArray)
         data.dataType = DataType(data.dataType)
 
@@ -710,22 +710,22 @@
         dataArray.extend(self.event.toArray())
         dataArray.extend(pack('<B', self.colors.value))
         return dataArray
 
 
     @classmethod
     def parse(cls, dataArray):
-        data = Command()
+        data = CommandLightEventColors()
         
         if len(dataArray) != cls.getSize():
             return None
         
         indexStart = 0;        indexEnd = Command.getSize();       data.command    = Command.parse(dataArray[indexStart:indexEnd])
         indexStart = indexEnd; indexEnd += LightEvent.getSize();   data.event      = LightEvent.parse(dataArray[indexStart:indexEnd])
-        indexStart = indexEnd; indexEnd += 1;                      data.colors,    = unpack('<B', dataArray[indexStart:indexEnd])
+        indexStart = indexEnd; indexEnd += 1;                      data.colors    = unpack('<B', dataArray[indexStart:indexEnd])
 
         data.colors     = Colors(data.colors)
 
         return data
 
 
 # Common End
@@ -1493,65 +1493,14 @@
 
         return data
 
 
 # Buzzer End
 
 
-
-# Vibrator Start
-
-
-class VibratorMode(Enum):
-
-    Stop                = 0     # 정지
-
-    Instantally         = 1     # 즉시 적용
-    Continually         = 2     # 예약
-
-    EndOfType           = 3
-
-
-
-class Vibrator(ISerializable):
-
-    def __init__(self):
-        self.mode       = VibratorMode.Stop
-        self.on         = 0
-        self.off        = 0
-        self.total      = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 7
-
-
-    def toArray(self):
-        return pack('<BHHH', self.mode.value, self.on, self.off, self.total)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Vibrator()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.mode, data.on, data.off, data.total = unpack('<BHHH', dataArray)
-
-        data.mode = VibratorMode(data.mode)
-
-        return data
-
-
-# Vibrator End
-
-
-
 # Button Start
 
 
 class ButtonFlagController(Enum):
 
     None_   			= 0x0000
```

### Comparing `codingrider-2.8.2/CodingRider/receiver.py` & `codingrider-2.9/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider/storage.py` & `codingrider-2.9/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider/system.py` & `codingrider-2.9/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider/tools/parser.py` & `codingrider-2.9/CodingRider/tools/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         #drone = Drone(True, True, True, True, True)
         drone = Drone()
         if drone.open() == False:
             print(Fore.RED + "* Error : Unable to open serial port." + Style.RESET_ALL)
             sys.exit(1)
 
         # 데이터 요청
-        drone.sendCommand(commandType, option);
+        drone.sendCommand(commandType, option)
 
 
     def control(self, roll, pitch, yaw, throttle, timeMs):
 
         #drone = Drone(True, True, True, True, True)
         drone = Drone()
         if drone.open() == False:
@@ -343,51 +343,22 @@
         header.dataType = DataType.Buzzer
         header.length   = Buzzer.getSize()
         header.from_    = DeviceType.Base
         header.to_      = target
         
         data = Buzzer()
 
-        data.mode       = BuzzerMode.Hz
+        data.mode       = BuzzerMode.HzInstantly
         data.value      = hz
         data.time       = time
 
         drone.transfer(header, data)
         sleep(time / 1000)
 
 
-    def vibrator(self, target, on, off, total):
-
-        #drone = Drone(True, True, True, True, True)
-        drone = Drone()
-        if drone.open() == False:
-            print(Fore.RED + "* Error : Unable to open serial port." + Style.RESET_ALL)
-            sys.exit(1)
-        
-        if ( (not isinstance(on, int)) or (not isinstance(off, int)) or (not isinstance(total, int)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.Vibrator
-        header.length   = Vibrator.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = target
-        
-        data = Vibrator()
-
-        data.mode       = VibratorMode.Instantally
-        data.on         = on
-        data.off        = off
-        data.total      = total
-
-        drone.transfer(header, data)
-        sleep(total / 1000)
-
-
     def help(self):
 
         print("")
         print(Fore.YELLOW + "* Command List " + Style.RESET_ALL)
 
         print("")
         print(Fore.CYAN + "  - Firmware Upgrade" + Style.RESET_ALL)
```

### Comparing `codingrider-2.8.2/CodingRider/tools/update.py` & `codingrider-2.9/CodingRider/tools/update.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider/update.py` & `codingrider-2.9/CodingRider/update.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.8.2/CodingRider.egg-info/PKG-INFO` & `codingrider-2.9/CodingRider.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.8.2
+Version: 2.9
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.8.2/PKG-INFO` & `codingrider-2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.8.2
+Version: 2.9
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.8.2/setup.py` & `codingrider-2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.8.2",
+    version = "2.9",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```

