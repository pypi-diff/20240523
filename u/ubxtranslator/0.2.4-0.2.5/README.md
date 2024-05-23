# Comparing `tmp/ubxtranslator-0.2.4.tar.gz` & `tmp/ubxtranslator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubxtranslator-0.2.4.tar", last modified: Wed Jan 25 10:08:32 2023, max compression
+gzip compressed data, was "ubxtranslator-0.2.5.tar", last modified: Thu May 23 18:58:19 2024, max compression
```

## Comparing `ubxtranslator-0.2.4.tar` & `ubxtranslator-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-01-25 10:08:32.321497 ubxtranslator-0.2.4/
--rw-r--r--   0 alex       (501) staff       (20)    35149 2019-06-01 21:23:18.000000 ubxtranslator-0.2.4/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       34 2019-06-05 10:41:29.000000 ubxtranslator-0.2.4/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     3533 2023-01-25 10:08:32.321303 ubxtranslator-0.2.4/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2997 2021-03-06 01:58:55.000000 ubxtranslator-0.2.4/README.md
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-01-25 10:08:32.321554 ubxtranslator-0.2.4/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      836 2023-01-25 09:58:50.000000 ubxtranslator-0.2.4/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-01-25 10:08:32.320448 ubxtranslator-0.2.4/ubxtranslator/
--rw-r--r--   0 alex       (501) staff       (20)      159 2019-06-08 04:19:08.000000 ubxtranslator-0.2.4/ubxtranslator/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    16879 2023-01-25 09:52:05.000000 ubxtranslator-0.2.4/ubxtranslator/core.py
--rw-r--r--   0 alex       (501) staff       (20)    17020 2023-01-25 09:52:05.000000 ubxtranslator-0.2.4/ubxtranslator/predefined.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-01-25 10:08:32.321037 ubxtranslator-0.2.4/ubxtranslator.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     3533 2023-01-25 10:08:32.000000 ubxtranslator-0.2.4/ubxtranslator.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      298 2023-01-25 10:08:32.000000 ubxtranslator-0.2.4/ubxtranslator.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-01-25 10:08:32.000000 ubxtranslator-0.2.4/ubxtranslator.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2019-06-05 10:47:26.000000 ubxtranslator-0.2.4/ubxtranslator.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       14 2023-01-25 10:08:32.000000 ubxtranslator-0.2.4/ubxtranslator.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-23 18:58:19.413703 ubxtranslator-0.2.5/
+-rw-r--r--   0 alex       (501) staff       (20)    35149 2019-06-01 21:23:18.000000 ubxtranslator-0.2.5/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       34 2019-06-05 10:41:29.000000 ubxtranslator-0.2.5/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     3481 2024-05-23 18:58:19.413469 ubxtranslator-0.2.5/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2965 2024-05-23 18:57:19.000000 ubxtranslator-0.2.5/README.md
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-23 18:58:19.413743 ubxtranslator-0.2.5/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      836 2024-05-23 18:58:12.000000 ubxtranslator-0.2.5/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-23 18:58:19.412389 ubxtranslator-0.2.5/ubxtranslator/
+-rw-r--r--   0 alex       (501) staff       (20)      159 2019-06-08 04:19:08.000000 ubxtranslator-0.2.5/ubxtranslator/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    16879 2023-01-25 09:52:05.000000 ubxtranslator-0.2.5/ubxtranslator/core.py
+-rw-r--r--   0 alex       (501) staff       (20)    19072 2024-05-23 18:57:19.000000 ubxtranslator-0.2.5/ubxtranslator/predefined.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-23 18:58:19.413275 ubxtranslator-0.2.5/ubxtranslator.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3481 2024-05-23 18:58:19.000000 ubxtranslator-0.2.5/ubxtranslator.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      298 2024-05-23 18:58:19.000000 ubxtranslator-0.2.5/ubxtranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-23 18:58:19.000000 ubxtranslator-0.2.5/ubxtranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2019-06-05 10:47:26.000000 ubxtranslator-0.2.5/ubxtranslator.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       14 2024-05-23 18:58:19.000000 ubxtranslator-0.2.5/ubxtranslator.egg-info/top_level.txt
```

### Comparing `ubxtranslator-0.2.4/LICENSE` & `ubxtranslator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ubxtranslator-0.2.4/PKG-INFO` & `ubxtranslator-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ubxtranslator
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight python library for translating UBX packets
 Home-page: http://github.com/dalymople/ubxtranslator
 Author: Dalymople
 Author-email: dalymople@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ubxtranslator [![Build Status](https://travis-ci.org/dalymople/ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/ubxtranslator)
+# ubxtranslator ![Build Status](https://github.com/dalymople/ubxtranslator/actions/workflows/Tests.yml/badge.svg)
 
 ## Overview
 This module provides a simple way to decode messages from uBlox GPS devices in the UBX format. 
 Like the high accuracy NEO-M8U module that I have created, 
 <a href="https://www.tindie.com/products/dalymople/gps-dead-reckoning-board-neo-m8u-compact/">click here for more info.</a><br>
 <br>
 This package has no dependencies! This is written in pure python using only the standard lib and supports any
@@ -80,9 +79,7 @@
 Want to contribute? Please feel free to submit issues or pull requests. 
 Nothing in this package is very complicated, please have a crack and help me to improve this.
 
 - Add the ability to pack messages into packets for two way communications
 - Add more and better tests
 - Add Field type RU1_3
 - Add async support
-
-
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: ubxtranslator Version: 0.2.4 Summary: A lightweight
+Metadata-Version: 2.1 Name: ubxtranslator Version: 0.2.5 Summary: A lightweight
 python library for translating UBX packets Home-page: http://github.com/
 dalymople/ubxtranslator Author: Dalymople Author-email: dalymople@gmail.com
-License: GNU GPL v3 Platform: UNKNOWN Classifier: Development Status :: 3 -
-Alpha Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-Communications Description-Content-Type: text/markdown License-File: LICENSE #
-ubxtranslator [![Build Status](https://travis-ci.org/dalymople/
-ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/
-ubxtranslator) ## Overview This module provides a simple way to decode messages
-from uBlox GPS devices in the UBX format. Like the high accuracy NEO-M8U module
-that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
+License: GNU GPL v3 Classifier: Development Status :: 3 - Alpha Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Communications
+Description-Content-Type: text/markdown License-File: LICENSE # ubxtranslator !
+[Build Status](https://github.com/dalymople/ubxtranslator/actions/workflows/
+Tests.yml/badge.svg) ## Overview This module provides a simple way to decode
+messages from uBlox GPS devices in the UBX format. Like the high accuracy NEO-
+M8U module that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
 
 This package has no dependencies! This is written in pure python using only the
 standard lib and supports any standard byte stream. The predefined messages are
 not added to the parser by default, this allows you to have tight control over
 what messages can be parsed. Is this the fastest implementation of a UBX
 parser? Probably not. If speed is critical then you probably need to go write
 something in C. If you want something that is fast enough and easy to use, you
```

### Comparing `ubxtranslator-0.2.4/README.md` & `ubxtranslator-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ubxtranslator [![Build Status](https://travis-ci.org/dalymople/ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/ubxtranslator)
+# ubxtranslator ![Build Status](https://github.com/dalymople/ubxtranslator/actions/workflows/Tests.yml/badge.svg)
 
 ## Overview
 This module provides a simple way to decode messages from uBlox GPS devices in the UBX format. 
 Like the high accuracy NEO-M8U module that I have created, 
 <a href="https://www.tindie.com/products/dalymople/gps-dead-reckoning-board-neo-m8u-compact/">click here for more info.</a><br>
 <br>
 This package has no dependencies! This is written in pure python using only the standard lib and supports any
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-# ubxtranslator [![Build Status](https://travis-ci.org/dalymople/
-ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/
-ubxtranslator) ## Overview This module provides a simple way to decode messages
-from uBlox GPS devices in the UBX format. Like the high accuracy NEO-M8U module
-that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
+# ubxtranslator ![Build Status](https://github.com/dalymople/ubxtranslator/
+actions/workflows/Tests.yml/badge.svg) ## Overview This module provides a
+simple way to decode messages from uBlox GPS devices in the UBX format. Like
+the high accuracy NEO-M8U module that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
 
 This package has no dependencies! This is written in pure python using only the
 standard lib and supports any standard byte stream. The predefined messages are
 not added to the parser by default, this allows you to have tight control over
 what messages can be parsed. Is this the fastest implementation of a UBX
 parser? Probably not. If speed is critical then you probably need to go write
 something in C. If you want something that is fast enough and easy to use, you
```

### Comparing `ubxtranslator-0.2.4/setup.py` & `ubxtranslator-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='ubxtranslator',
-      version='0.2.4',
+      version='0.2.5',
       description='A lightweight python library for translating UBX packets',
       long_description=readme(),
       long_description_content_type="text/markdown",
       classifiers=[
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
           'Programming Language :: Python :: 3',
```

### Comparing `ubxtranslator-0.2.4/ubxtranslator/core.py` & `ubxtranslator-0.2.5/ubxtranslator/core.py`

 * *Files identical despite different names*

### Comparing `ubxtranslator-0.2.4/ubxtranslator/predefined.py` & `ubxtranslator-0.2.5/ubxtranslator/predefined.py`

 * *Files 4% similar despite different names*

```diff
@@ -424,24 +424,46 @@
         core.Field('velD', 'I4'),
         core.Field('speed', 'U4'),
         core.Field('gSpeed', 'U4'),
         core.Field('heading', 'I4'),
         core.Field('sAcc', 'U4'),
         core.Field('cAcc', 'U4'),
     ]),
+    core.Message(0x62, 'PL', [
+        core.Field('msgVersion', 'U1'),
+        core.Field('tmirCoeff', 'U1'),
+        core.Field('tmirExp', 'I1'),
+        core.Field('plPosValid', 'U1'),
+        core.Field('plPosFrame', 'U1'),
+        core.Field('plVelValid', 'U1'),
+        core.Field('plVelFrame', 'U1'),
+        core.Field('plTimeValid', 'U1'),
+        core.PadByte(repeat=3),
+        core.Field('iTow', 'U4'),
+        core.Field('plPos1', 'U4'),
+        core.Field('plPos2', 'U4'),
+        core.Field('plPos3', 'U4'),
+        core.Field('plVel1', 'U4'),
+        core.Field('plVel2', 'U4'),
+        core.Field('plVel3', 'U4'),
+        core.Field('plPosHorizOrient', 'U2'),
+        core.Field('plVelHorizOrient', 'U2'),
+        core.Field('plTime', 'U4'),
+        core.PadByte(repeat=3),
+    ])
 ])
 
 RXM_CLS = core.Cls(0x02, 'RXM', [
     core.Message(0x13, 'SFRBX', [
         core.Field('gnssId', 'U1'),
         core.Field('svId', 'U1'),
-        core.PadByte(),
+        core.Field('sigId', 'U1'),
         core.Field('freqId', 'U1'),
         core.Field('numWords', 'U1'),
-        core.PadByte(),
+        core.Field('chn', 'U1'),
         core.Field('version', 'U1'),
         core.PadByte(),
         core.RepeatedBlock('RB', [
             core.Field('dwrd', 'U4'),
         ]),
     ]),
     core.Message(0x15, 'RAWX', [
@@ -470,40 +492,85 @@
             ]),
             core.BitField('cpStdev', 'X1', [
                 core.Flag('cpStd', 0, 4),
             ]),
             core.BitField('doStdev', 'X1', [
                 core.Flag('doStd', 0, 4),
             ]),
-            core.BitField('rtkStat', 'X1', [
+            core.BitField('trkStat', 'X1', [
                 core.Flag('prValid', 0, 1),
                 core.Flag('cpValid', 1, 2),
                 core.Flag('halfCyc', 2, 3),
                 core.Flag('subHalfCyc', 3, 4),
             ]),
             core.PadByte()
         ])
+    ])
+])
+
+
+MON_CLS = core.Cls(0x0A, 'MON', [
+    core.Message(0x09, 'HW', [
+        core.Field('pinSel', 'U4'),
+        core.Field('pinBank', 'U4'),
+        core.Field('pinDir', 'U4'),
+        core.Field('pinVal', 'U4'),
+        core.Field('noisePerMS', 'U2'),
+        core.Field('agcCnt', 'U2'),
+        core.Field('aStatus', 'U1'),
+        core.Field('aPower', 'U1'),
+        core.Field('flags', 'U1'),
+        core.PadByte(),
+        core.Field('usedMask', 'U4'),
+        core.RepeatedBlock('RB', [
+            core.Field('VP', 'U1'),
+        ]),
+        core.Field('jamInd', 'U1'),
+        core.PadByte(repeat=1),
+        core.Field('pinIrq', 'U4'),
+        core.Field('pullH', 'U4'),
+        core.Field('pullL', 'U4')
+    ])
+])
+
+
+ESF_CLS = core.Cls(0x10, 'ESF', [
+    core.Message(0x02, 'MEAS', [
+        core.Field('time_tag', 'U4'),
+        core.BitField('flags', 'X2', [
+            core.Flag('timeMarkSent', 0, 2),
+            core.Flag('timeMarkEdge', 2, 3),
+            core.Flag('calibTtagValid', 3, 4),
+            core.Flag('numMeas', 11, 16)
+        ]),
+        core.Field('id', 'U2'),
+        core.RepeatedBlock('RB', [
+            core.BitField('data', 'X4', [
+                core.Flag('dataField', 0, 24),
+                core.Flag('dataType', 24, 30)
+            ]),
+        ]),
+        core.Field('calib_tag', 'U4')
+    ]),
+    core.Message(0x03, 'RAW', [
+        core.Field('msss', 'U4'),
+        core.RepeatedBlock('RB', [
+            core.BitField('data', 'X4', [
+                core.Flag('dataField', 0, 24),
+                core.Flag('dataType', 24, 30)
+            ]),
+            core.Field('sensor_time_tag', 'U4')
+        ])
     ]),
-    core.Message(0x62, 'PL', [
-        core.Field('msgVersion', 'U1'),
-        core.Field('tmirCoeff', 'U1'),
-        core.Field('tmirExp', 'I1'),
-        core.Field('plPosValid', 'U1'),
-        core.Field('plPosFrame', 'U1'),
-        core.Field('plVelValid', 'U1'),
-        core.Field('plVelFrame', 'U1'),
-        core.Field('plTimeValid', 'U1'),
-        core.PadByte(repeat=3),
-        core.Field('iTow', 'U4'),
-        core.Field('plPos1', 'U4'),
-        core.Field('plPos2', 'U4'),
-        core.Field('plPos3', 'U4'),
-        core.Field('plVel1', 'U4'),
-        core.Field('plVel2', 'U4'),
-        core.Field('plVel3', 'U4'),
-        core.Field('plPosHorizOrient', 'U2'),
-        core.Field('plVelHorizOrient', 'U2'),
-        core.Field('plTime', 'U4'),
+    core.Message(0x15, 'INS', [
+        core.Field('bitfield0', 'U4'),
         core.PadByte(repeat=3),
+        core.Field('i_tow', 'U4'),
+        core.Field('x_ang_rate', 'I4'),
+        core.Field('y_ang_rate', 'I4'),
+        core.Field('z_ang_rate', 'I4'),
+        core.Field('x_accel', 'I4'),
+        core.Field('y_accel', 'I4'),
+        core.Field('z_accel', 'I4')
     ])
 ])
```

### Comparing `ubxtranslator-0.2.4/ubxtranslator.egg-info/PKG-INFO` & `ubxtranslator-0.2.5/ubxtranslator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ubxtranslator
-Version: 0.2.4
+Version: 0.2.5
 Summary: A lightweight python library for translating UBX packets
 Home-page: http://github.com/dalymople/ubxtranslator
 Author: Dalymople
 Author-email: dalymople@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ubxtranslator [![Build Status](https://travis-ci.org/dalymople/ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/ubxtranslator)
+# ubxtranslator ![Build Status](https://github.com/dalymople/ubxtranslator/actions/workflows/Tests.yml/badge.svg)
 
 ## Overview
 This module provides a simple way to decode messages from uBlox GPS devices in the UBX format. 
 Like the high accuracy NEO-M8U module that I have created, 
 <a href="https://www.tindie.com/products/dalymople/gps-dead-reckoning-board-neo-m8u-compact/">click here for more info.</a><br>
 <br>
 This package has no dependencies! This is written in pure python using only the standard lib and supports any
@@ -80,9 +79,7 @@
 Want to contribute? Please feel free to submit issues or pull requests. 
 Nothing in this package is very complicated, please have a crack and help me to improve this.
 
 - Add the ability to pack messages into packets for two way communications
 - Add more and better tests
 - Add Field type RU1_3
 - Add async support
-
-
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: ubxtranslator Version: 0.2.4 Summary: A lightweight
+Metadata-Version: 2.1 Name: ubxtranslator Version: 0.2.5 Summary: A lightweight
 python library for translating UBX packets Home-page: http://github.com/
 dalymople/ubxtranslator Author: Dalymople Author-email: dalymople@gmail.com
-License: GNU GPL v3 Platform: UNKNOWN Classifier: Development Status :: 3 -
-Alpha Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-Communications Description-Content-Type: text/markdown License-File: LICENSE #
-ubxtranslator [![Build Status](https://travis-ci.org/dalymople/
-ubxtranslator.svg?branch=master)](https://travis-ci.org/dalymople/
-ubxtranslator) ## Overview This module provides a simple way to decode messages
-from uBlox GPS devices in the UBX format. Like the high accuracy NEO-M8U module
-that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
+License: GNU GPL v3 Classifier: Development Status :: 3 - Alpha Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Communications
+Description-Content-Type: text/markdown License-File: LICENSE # ubxtranslator !
+[Build Status](https://github.com/dalymople/ubxtranslator/actions/workflows/
+Tests.yml/badge.svg) ## Overview This module provides a simple way to decode
+messages from uBlox GPS devices in the UBX format. Like the high accuracy NEO-
+M8U module that I have created, _c_l_i_c_k_ _h_e_r_e_ _f_o_r_ _m_o_r_e_ _i_n_f_o_.
 
 This package has no dependencies! This is written in pure python using only the
 standard lib and supports any standard byte stream. The predefined messages are
 not added to the parser by default, this allows you to have tight control over
 what messages can be parsed. Is this the fastest implementation of a UBX
 parser? Probably not. If speed is critical then you probably need to go write
 something in C. If you want something that is fast enough and easy to use, you
```

